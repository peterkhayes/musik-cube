# Music Cube

A musical Rubik's Cube. Plays generative loop-based music based on the solvedness of a Rubik's Cube.

Will soon combine with Arduinos to make a physical cube with LEDs.

## Installation

### Prerequisites

- [Sonic Pi](http://sonic-pi.net/) to play the audio, along with `sonic-pi-cli`
- [node.js](https://nodejs.org/en/) to run the controller
- [Arduino](https://www.arduino.cc/) or other microcontroller with serial-port communication if you want to build it physically

### Install dependencies

- `yarn && gem install sonic-pi-cli`

## Usage

First make sure Sonic Pi is running. On a Mac, this means opening it as an application.

Then run one of the commands below. If a usage method expects input, send one of the strings listed under *available rotations* below (one per message).

### Launch cube and make random rotations every 2 seconds

`yarn random [-- OVERRIDE_INTERVAL]`

### Launch cube and listen on UDP port 12345 for rotations

`yarn udp [-- OVERRIDE_PORT]`

### Launch cube and listen on serial port for rotations

`yarn serial` (not working for now)

### Available rotations

- `F`: Rotate front face clockwise
- `f`: Rotate front face counterclockwise
- `B`: Rotate back face clockwise
- `b`: Rotate back face counterclockwise
- `U`: Rotate up face clockwise
- `u`: Rotate up face counterclockwise
- `D`: Rotate down face clockwise
- `d`: Rotate down face counterclockwise
- `L`: Rotate left face clockwise
- `l`: Rotate left face counterclockwise
- `R`: Rotate right face clockwise
- `r`: Rotate right face counterclockwise
- `?`: Random rotation