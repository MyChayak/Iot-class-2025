# Exploring MQTT QoS Levels

Experiment with QoS 0, 1, and 2.
Observe how message delivery changes based on QoS settings.

## Publisher_qos.py output

```
client = mqtt.Client()
[16:29:43] DEBUG | Sending CONNECT (u0, p0, wr0, wq0, wf0, c1, k60) client_id=b''
Enter message to publish: [16:29:43] DEBUG | Received CONNACK (0, 0)
hii
Enter QoS level (0, 1, 2): 2
[16:30:07] DEBUG | Sending PUBLISH (d0, q2, r0, m1), 'b'test/qos/6510301013/temperature'', ... (3 bytes)
[16:30:07] PUBLISH REQUESTED | QoS=2 | Message='hii' | msgid=1
Enter message to publish: [16:30:07] DEBUG | Received PUBREC (Mid: 1)
[16:30:07] DEBUG | Sending PUBREL (Mid: 1)
[16:30:07] DEBUG | Received PUBCOMP (Mid: 1)
[16:30:07] PUBLISHED | msgid=1
```

## Subscriber_qos.py Output

```
client = mqtt.Client()
[16:26:01] DEBUG | Sending CONNECT (u0, p0, wr0, wq0, wf0, c1, k60) client_id=b''
[16:26:01] DEBUG | Received CONNACK (0, 0)
[16:26:01] Connected with result code 0
[16:26:01] DEBUG | Sending SUBSCRIBE (d0, m1) [(b'test/qos/6510301013', 2)]
[16:26:01] DEBUG | Received SUBACK
[16:27:01] DEBUG | Sending PINGREQ
[16:27:01] DEBUG | Received PINGRESP
[16:28:02] DEBUG | Sending PINGREQ
[16:28:02] DEBUG | Received PINGRESP
[16:29:02] DEBUG | Sending PINGREQ
[16:29:02] DEBUG | Received PINGRESP
```