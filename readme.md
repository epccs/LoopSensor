# Loop Sensor

From <https://github.com/epccs/LoopSensor/>

This is a collection of current loop sensor circuit boards. 

Current loop devices are normally operated over a pair of wires. They take power from the voltage and current and transmit information by controlling the current flow. I have a number of circuits that transmit two states (3mA or 10mA) depending on the output of a 555 timer. The change of state is a timing event. It is transmitted through the loop and can be remotely measured. The events can be used to tell if the 555 timing capacitance (or the current source feeding it) has changed  and how much. The current loop works over a CAT5 pair (a well-known 100 Ohm transmission line) that provides superior noise immunity. 

Note: a typical 4-20mA loop will work over phone line wire which has a higher characteristic impedance when compared with a CAT5 pair, these sensors may work over a small distance with a phone line pair, but need CAT5 for runs with more distance.

[Forums](http://rpubus.org/bb/viewforum.php?f=9)

