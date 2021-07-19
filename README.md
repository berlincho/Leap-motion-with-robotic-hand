# Leap motion with Robotic hand

A project for robotic hands using Leap motion and Arduino.

[Demo video (Chinese ver.)](https://drive.google.com/file/d/0B_9g7tQeWZJLNkxOek5TdGMzTkU/view?resourcekey=0-iGA5vIL-mWacBAOpg4WDDA)

Leap Motion is a computer hardware sensor device that supports hand and finger motions as input, analogous to a mouse, but requires no hand contact or touching.

## Architecture

<img src="https://github.com/berlincho/Leap-motion-with-robotic-hand/blob/master/architecture.png" width="70%">

## Environment

- **Arduino**, **Leap Motion** are required.

- **Servo Motors** 5 per hand (optional)

- Host: **Nodejs** (LeapJS, Johnny-five)

## 3D printing

- `/Gcode` contains the 3D robotic hands gcodes. Use 3D printer to build the hands.
- `/Gcode/number.txt` describes the number of components for each parts.
- To assembly the components of the hand. Refer to http://enablingthefuture.org/upper-limb-prosthetics/raptor-reloaded/.

## Development

- `app.js` describes the connection part of Leap Motion and Arduino. Update the `COM` in line 8.
- `lib/handToHand.js` describes the linear algebra of finger movement.

## Execution

Install the dependencies.

```shell
npm install
```

Run the application.

```shell
npm run start
```

Note: make sure the Arduino and Leap Motion have connected to the computer.
