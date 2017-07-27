# Automatic-Room-Light-Controller-with-a-Visitor-Counter

## Automatic Room Light Control
When we enter a room, as a habitual tendency, we often search for a switch to turn the light on, and if we are new to the room, we often find it difficult to locate the switch. Most of the times, many of us forget to switch off the lights while leaving the room in which we stay most of the time. This results in unnecessary power wastage. Therefore, an automatic room-light controller automatically turns on the lights when a person enters into a room, and turns off the lights when the person leaves the room. This automatic room controller can be implemented by using a simple microcontroller(here we are using arduino uno) and wireless IR technologies.

### Automatic Room Light Controller with a Visitor Counter
This system is designed by using two sets of IR transmitters and receivers. These IR sensors are placed in such a way that they detect a person entering and leaving the room to turn the home appliances. In this optimun energy management system, a microcontroller is the central processing unit of this project which is arduino uno. This system facilitates a bidirectional visitor counter for displaying the number of persons inside the room.
This is how IR sensor works:![409px-ir_sensor_principles](https://user-images.githubusercontent.com/25952213/28656115-ad8e2f6c-72bd-11e7-9b8e-cca3a0d3370c.png)

When a person enters into the room, an IR beam is obstructed between the IR transmitter and the receiver. This IR obstruction from the sensor-1 gives the corresponding signal to the microcontroller. The microcontroller is programmed in such a way that by the reception of the signal from the sensor-1 it turns on the fans and lights inside the room. Thus, the microcontroller gives command signals to a relay driver which turns the relays such that all these appliances turn on.

When the person leaves from this room, another set of IR sensors enable and give control signals to the microcontroller. Furthermore, similar to the above process, this system turns off the appliances like fans and lights. Apart from this, the system also takes account of the number of persons inside the room so that this control operation is varied depending on the persons’ availability in the room.

For every person entering and leaving the room, the microcontroller reads the digital input from two receivers, and calculates the number of persons inside the room, and then displays it on the LCD. When the persons’ count is greater than one, the microcontroller turns on the room light and when the persons’ count is zero, it turns off all the lights and fans.(here in this project, I have not connected fan to it ...but it can be done in similar way of light connection )

