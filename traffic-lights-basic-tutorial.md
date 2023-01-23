### @activities true
### @explicitHints true

# ERPS STEM WEEK :: Traffic Lights - Basic Tutorial

## Introduction
### Introduction Step @unplugged
In this tutorial, you will start by getting all of the lights to come on!
![All lights lit up](https://raw.githubusercontent.com/niaxotim/erps-stem-week-2023/master/assets/traffic_lights_basic.png)


### Assembly
The traffic light has 3 different LED bulbs, each of which can be controlled individually.
But we are going to start nice and simple! Can you make all 3 lights come on
at the same time?  First, make sure your micro:bit is connected to your lights.

## Traffic Lights
### Step 1

First we need to add some input. We will create code to turn all the lights on and off with buttons presses.  
Add ``||input:on Button A||``.

#### ~ tutorialhint
```blocks
input.onButtonPressed(Button.A, function () {
	
})
```

### Step 2

From the STOP:bit blocks, add into the ``||input:on Button A||`` block 3 x ``||Kitronik_STOPbit.Turn Traffic Light On||`` blocks.

#### ~ tutorialhint
```blocks
input.onButtonPressed(Button.A, function () {
    Kitronik_STOPbit.trafficLightLED(Kitronik_STOPbit.LightColours.Red, Kitronik_STOPbit.DisplayLights.On)
    Kitronik_STOPbit.trafficLightLED(Kitronik_STOPbit.LightColours.Red, Kitronik_STOPbit.DisplayLights.On)
    Kitronik_STOPbit.trafficLightLED(Kitronik_STOPbit.LightColours.Red, Kitronik_STOPbit.DisplayLights.On)
})
```
