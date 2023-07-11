!!! important !!!
the tabs in which wokwi is running should always be stand-alone (1 browser window per tab like in the image in the .zip file) and in 
the foreground if possible or wokwi will pause the simulation. It's not a big deal if it happens as no 
messages will be lost, however to see a "real" simulation of a PAN network this should be avoided. 

0) Configuration misc
    a) version info (i haven't used the course VM but the same modules that are on there)
    [info] Node-RED version: v3.0.2
    [info] Node.js  version: v18.13.0
    [info] Linux 6.2.0-24-generic x64 LE
    [OS version] Ubuntu 23.04 lunar

1) How to start the simulation to minimize the chances of wokwi messing up something
    a) start the motes in wokwi (the order is irrelevant, the sensors will wait for the actuators before sending messages
    which will be buffered until that point) and wait until they're all ready (waiting for beacon).
    a.1) set the slider to the desired probability value in the sensors 
    (slide at the top = 1 message produced per beacon)
    b) boot node-red
        b.1) when the motes will be associated correctly the onboard led #2 (blue one) will turn on

2) Useful info
    a) The motes can be "hot" restarted, they will reassociate to the network anyways if the 
    coordinator is running.
    b) The coordinator CANNOT be, if it is restarted while motes are associated they
    will detect it (different PAN id unless of a 1 in a billion collision), restart and
    reassociate, this is done to keep things clean
    c) From node-red's ui it is possible to send messages to the actuators even when
    no sensors are online, to allow this the actuators won't check if the source of the 
    message belongs to the network, they will just use the value and destination field.
    The value sent to the motes will be the result of form_value % 101 


2) Known issues
    a) for some reason wokwi might randomly disconnect the wifi module
        The motes are able to detect it as i inserted a snippet that keeps trying
        to reconnect to the wifi, but it doesn't always work unfortunately, it must be
        something going wrong in their backend. The only solution is to reload the 
        page and restart the mote.

3) Simulation results
    a) the sim has been run with 4 motes for about 12-hours without any issues.
    b) in principle up to 16 (sizeof(short)*8) motes are supported by the coordinator,
    however the sensor will only send values to the first and second actuators as their names are hardcoded. 
    c) the output of a simulation ran for 5 beacon interval is included in the log.md file 

4) (If the project is ran in windows) .wokwi files are normal text files 

5) The report might seem a bit too long but it's mostly figures, it'd be equivalent to 4-5 pages without them and the indices.