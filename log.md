# Simulation log
### Settings : 2 actuators and 2 sensors
### The output simulation corresponds to about 5 beacon intervals
### The data value is always collected after a beacon period due the way the code is structured, thus they will be sent during the following beacon
### All the output is copy-pasted directly from the respective source in the same order they've been produced

# CONFIGURATION : SLOT SIZE 500 ms due to high network delays -> slightly longer beacon interval [13.000ms]


# Coordinator Output - [Node-Red] [Verbose]
Processing association message for mote : 10656748-ACT1
{
  number_of_nodes: 4,
  '10656748-ACT2': {
    association_timestamp: 1688410426935,
    association_id: 1,
    mote_type: 'actuator'
  },
  '10656748-SENS1': {
    association_timestamp: 1688410431680,
    association_id: 2,
    mote_type: 'sensor'
  },
  '10656748-SENS2': {
    association_timestamp: 1688410431703,
    association_id: 4,
    mote_type: 'sensor'
  },
  '10656748-ACT1': {
    association_timestamp: 1688410432001,
    association_id: 8,
    mote_type: 'actuator'
  }
}

Sending beacon message - [2023-07-03 20:53:58] -  seq : [10]

Sending beacon message - [2023-07-03 20:54:11] -  seq : [11]

Sending beacon message - [2023-07-03 20:54:24] -  seq : [12]

Sending beacon message - [2023-07-03 20:54:37] -  seq : [13]

Sending beacon message - [2023-07-03 20:54:50] -  seq : [14]

Sending beacon message - [2023-07-03 20:55:03] -  seq : [15]
PAN coord. received an uplink data message from mote 4 - seq : [0] - dest [8]
PAN coord. received an uplink data message from mote 2 - seq : [0] - dest [8]
# only 1 message per beacon
Relaying downlink message [0] to mote #8 
Mote #8 acknowledged message #0
# acked in the same slot
Sending beacon message - [2023-07-03 20:55:16] -  seq : [16]
PAN coord. received an uplink data message from mote 4 - seq : [1] - dest [1]
PAN coord. received an uplink data message from mote 2 - seq : [1] - dest [8]

Relaying downlink message [1] to mote #1
Relaying downlink message [0] to mote #8
Mote #1 acknowledged message #1
Mote #8 acknowledged message #0

Sending beacon message - [2023-07-03 20:55:29] -  seq : [17]

PAN coord. received an uplink data message from mote 4 - seq : [2] - dest [1]
PAN coord. received an uplink data message from mote 2 - seq : [2] - dest [8]
Relaying downlink message [2] to mote #1
Relaying downlink message [1] to mote #8
Mote #1 acknowledged message #2
Mote #8 acknowledged message #1

Sending beacon message - [2023-07-03 20:55:42] -  seq : [18]

PAN coord. received an uplink data message from mote 4 - seq : [3] - dest [1]
PAN coord. received an uplink data message from mote 2 - seq : [3] - dest [8]
Relaying downlink message [3] to mote #1
Relaying downlink message [2] to mote #8
Mote #1 acknowledged message #3
Mote #8 acknowledged message #2

3 Jul 20:55:49 - [info] Stopping flows
3 Jul 20:55:49 - [info] Stopped flows



## Actuator Mote 1 Output [Verbose] - 10656748-ACT1

Wifi ON
Attempting to connect to the wifi...
Connected to MQTT broker
10656748-ACT1 online, waiting for a beacon to connect 
PWM task running on Core 0,waiting for data
First beacon received, associating...
Sending ASSOCIATION MESSAGE to the PAN coordinator
Mote has AID : 8
Received beacon with sequence number : 10
Time until CFP up and down : [4000,6000]
Going to sleep for the inactive part
Received beacon with sequence number : 11
Time until CFP up and down : [4000,6000]
Going to sleep for the inactive part
Received beacon with sequence number : 12
Time until CFP up and down : [4000,6000]
Going to sleep for the inactive part
Received beacon with sequence number : 13
Time until CFP up and down : [4000,6000]
Going to sleep for the inactive part
Received beacon with sequence number : 14
Time until CFP up and down : [4000,6000]
Going to sleep for the inactive part
Received beacon with sequence number : 15
Time until CFP up and down : [4000,6000]
Received downlink DATA message
Semaphore obtained, starting PWM of the LED
Received humidity value from mote 4, value : 75
Sent an ACK to the broker
Going to sleep for the inactive part
Received beacon with sequence number : 16
Time until CFP up and down : [4000,6000]
Received downlink DATA message
Received humidity value from mote 2, value : 75
Sent an ACK to the broker
Going to sleep for the inactive part
Received beacon with sequence number : 17
Time until CFP up and down : [4000,6000]
Received downlink DATA message
Received humidity value from mote 2, value : 75
Sent an ACK to the broker
Going to sleep for the inactive part
Received beacon with sequence number : 18
Time until CFP up and down : [4000,6000]
Received downlink DATA message
Received humidity value from mote 2, value : 75
Sent an ACK to the broker
Going to sleep for the inactive part

## Actuator Mote 2 Output [Verbose] - 10656748-ACT1

Wifi ON
Attempting to connect to the wifi...
Connected to MQTT broker
10656748-ACT2 online, waiting for a beacon to connect 
PWM task running on Core 0,waiting for data
First beacon received, associating...
Sending ASSOCIATION MESSAGE to the PAN coordinator
Mote has AID : 1
Received beacon with sequence number : 9
Time until CFP up and down : [2500,3000]
Going to sleep for the inactive part
Going to sleep for the inactive part
Received beacon with sequence number : 10
Time until CFP up and down : [3500,5500]
Going to sleep for the inactive part
Received beacon with sequence number : 11
Time until CFP up and down : [3500,5500]
Going to sleep for the inactive part
Received beacon with sequence number : 12
Time until CFP up and down : [3500,5500]
Going to sleep for the inactive part
Received beacon with sequence number : 13
Time until CFP up and down : [3500,5500]
Going to sleep for the inactive part
Received beacon with sequence number : 14
Time until CFP up and down : [3500,5500]
Going to sleep for the inactive part
Received beacon with sequence number : 15
Time until CFP up and down : [3500,5500]
Going to sleep for the inactive part
Received beacon with sequence number : 16
Time until CFP up and down : [3500,5500]
Received downlink DATA message
Semaphore obtained, starting PWM of the LED
Received humidity value from mote 4, value : 75
Sent an ACK to the broker
Going to sleep for the inactive part
Received beacon with sequence number : 17
Time until CFP up and down : [3500,5500]
Received downlink DATA message
Received humidity value from mote 4, value : 75
Sent an ACK to the broker
Going to sleep for the inactive part
Received beacon with sequence number : 18
Time until CFP up and down : [3500,5500]
Received downlink DATA message
Received humidity value from mote 4, value : 75
Sent an ACK to the broker
Going to sleep for the inactive part


## Sensor Mote 1 Output [Verbose] - 10656748-SENS1
Wifi ON
Connected to MQTT broker
10656748-SENS1 online, waiting for a beacon to connect 
First beacon received, associating...
Sending ASSOCIATION MESSAGE to the PAN coordinator
Mote has AID : 2
Received beacon with sequence number : 10
Detected Actuator 1 online, AID : 8
Detected Actuator 2 online, AID : 1
Time until CFP up and down : [3000,5000]
Current probability interval : [0,0]
Going to sleep for the inactive part
Received beacon with sequence number : 11
Time until CFP up and down : [3000,5000]
Current probability interval : [0,0]
Going to sleep for the inactive part
Received beacon with sequence number : 12
Time until CFP up and down : [3000,5000]
Current probability interval : [0,0]
Going to sleep for the inactive part
Received beacon with sequence number : 13
Time until CFP up and down : [3000,5000]
Current probability interval : [0,0]
Going to sleep for the inactive part
Received beacon with sequence number : 14
Time until CFP up and down : [3000,5000]
Current probability interval : [0,100]
[DATA COLLECTION] - Buffering measurement,value : 75
Going to sleep for the inactive part
Received beacon with sequence number : 15
Time until CFP up and down : [3000,5000]
Sending measurement to PAN coordinator
Waiting for my CFP uplink slot :3000
Sent a DATA message to the broker
Message [#0] has been acknowledged
Current probability interval : [0,100]
[DATA COLLECTION] - Buffering measurement,value : 75
Going to sleep for the inactive part
Received beacon with sequence number : 16
Time until CFP up and down : [3000,5000]
Sending measurement to PAN coordinator
Waiting for my CFP uplink slot :3000
Sent a DATA message to the broker
Message [#1] has been acknowledged
Current probability interval : [0,100]
[DATA COLLECTION] - Buffering measurement,value : 75
Going to sleep for the inactive part
Received beacon with sequence number : 17
Time until CFP up and down : [3000,5000]
Sending measurement to PAN coordinator
Waiting for my CFP uplink slot :3000
Sent a DATA message to the broker
Message [#2] has been acknowledged
Current probability interval : [0,100]
[DATA COLLECTION] - Buffering measurement,value : 75
Going to sleep for the inactive part
Received beacon with sequence number : 18
Time until CFP up and down : [3000,5000]
Sending measurement to PAN coordinator
Waiting for my CFP uplink slot :3000
Sent a DATA message to the broker
Message [#3] has been acknowledged
Current probability interval : [0,100]
[DATA COLLECTION] - Buffering measurement,value : 75
Going to sleep for the inactive part

## Sensor Mote 2 Output [Verbose] - 10656748-SENS2

Wifi ON
Connected to MQTT broker
10656748-SENS2 online, waiting for a beacon to connect 
First beacon received, associating...
Sending ASSOCIATION MESSAGE to the PAN coordinator
Mote has AID : 4
Received beacon with sequence number : 10
Detected Actuator 1 online, AID : 8
Detected Actuator 2 online, AID : 1
Time until CFP up and down : [2500,4500]
Current probability interval : [0,0]
Going to sleep for the inactive part
Received beacon with sequence number : 11
Time until CFP up and down : [2500,4500]
Current probability interval : [0,0]
Going to sleep for the inactive part
Received beacon with sequence number : 12
Time until CFP up and down : [2500,4500]
Current probability interval : [0,0]
Going to sleep for the inactive part
Received beacon with sequence number : 13
Time until CFP up and down : [2500,4500]
Current probability interval : [0,0]
Going to sleep for the inactive part
Received beacon with sequence number : 14
Time until CFP up and down : [2500,4500]
Current probability interval : [0,100]
[DATA COLLECTION] - Buffering measurement,value : 75
Going to sleep for the inactive part
Received beacon with sequence number : 15
Time until CFP up and down : [2500,4500]
Sending measurement to PAN coordinator
Waiting for my CFP uplink slot :2500
Sent a DATA message to the broker
Message [#0] has been acknowledged
Current probability interval : [0,100]
[DATA COLLECTION] - Buffering measurement,value : 75
Going to sleep for the inactive part
Received beacon with sequence number : 16
Time until CFP up and down : [2500,4500]
Sending measurement to PAN coordinator
Waiting for my CFP uplink slot :2500
Sent a DATA message to the broker
Message [#1] has been acknowledged
Current probability interval : [0,100]
[DATA COLLECTION] - Buffering measurement,value : 75
Going to sleep for the inactive part
Received beacon with sequence number : 17
Time until CFP up and down : [2500,4500]
Sending measurement to PAN coordinator
Waiting for my CFP uplink slot :2500
Sent a DATA message to the broker
Message [#2] has been acknowledged
Current probability interval : [0,100]
[DATA COLLECTION] - Buffering measurement,value : 75
Going to sleep for the inactive part
Received beacon with sequence number : 18
Time until CFP up and down : [2500,4500]
Sending measurement to PAN coordinator
Waiting for my CFP uplink slot :2500
Sent a DATA message to the broker
Message [#3] has been acknowledged
Current probability interval : [0,100]
[DATA COLLECTION] - Buffering measurement,value : 75
Going to sleep for the inactive part
