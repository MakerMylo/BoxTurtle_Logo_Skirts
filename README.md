BoxTurtle Logo Panel front skirt
===
This is an alternative front skirt for the BoxTurtle that includes a logo panel that can be illuminated using the LED Matrix panel provided or printed in your 2 colours to be a static logo.

Printing
===
- Pick a Size, `_5_bay` needs a 510mm Wide frame (I.e. Voron 2.4 350mm), `_4_bay` is standard BoxTurtle sizing.
- Pick an LED Matrix Housing, `_back` & `_front` can be used for individual neopixels, `_blank` can be used for LED Strips (No Front needed on the blank one).
- On the Left/Right & Middle panels set a layer height filament swap at 1.5mm (For the colour of your mesh), set the top/bottom layer of the mesh bodies to 0, tweek your infil for optimal results, mine is 17% Honeycomb at a 90 Degree angle to match the hexes, with 3 Walls for borders.
- Printing the logo plate, you want the base to be clear and the top to be your primary colour, so do a filament change at 2.6mm. I recommend a very light infil and something that doesn't cross over to much, such as triangles.

Design Features
===
 - 17mm Wide, leaving 3mm on the inside of the BoxTurtle.
 - 1mm Thick mesh to allow a height range filament change at 1.5mm.
 - Mesh designed as single Body to allow outer walls to be used.
 - Turtle Logo designed in multiple parts to allow layer changes (Assuming your BT isn't built when this is being printed).
 - Supports are pre-added to all STL's

![Render](./Images/render.png)

Assembly
===
1. Add 2 Heatset inserts to the back of the middle panel.

2. Press in your logo plate.

3. Assemble your LED Matrix and screw this in from behind using 2x M3x6 Screws.

4. Slide it into place on the BoxTurtle

Config
===
![Photo](./Images/photo_led.jpg)
Assuming you have LED Effects installed, add this to the bottom of your `AFC_Hardware.cfg` file to get the rainbow effect behind the logo.
```
[neopixel bt_logo]
pin: AFC: PA2 #Set your own Pin
chain_count: 11
color_order: GRB
initial_RED: 1.0
initial_GREEN: 0.0
initial_BLUE: 0.0
initial_WHITE: 0.0

[led_effect rainbow_turtle]
leds:
    neopixel:bt_logo
autostart:                          true
frame_rate:                         24
layers:
    gradient  0.3  1 add (0.3, 0.0, 0.0),(0.0, 0.3, 0.0),(0.0, 0.0, 0.3)
```

Bill of Materials
===
Every link in the Bill of Materials is an affiliate link, This costs you nothing to use but helps buy me some filament and trinkets to make this kind of mod.

 - [2x M3x5x4 Heatset Inserts](https://s.click.aliexpress.com/e/_DdHrjjj)
 - [2x M3x6 Screws (Not FHCS)](https://s.click.aliexpress.com/e/_DEccKQd)
 - [11x Neopixel LEDs](https://s.click.aliexpress.com/e/_DCKnF41)
 - [1m 26AWG Wire](https://s.click.aliexpress.com/e/_Dcg8I5b)
 - [1x JST-XHx3 Connector](https://s.click.aliexpress.com/e/_DE6E8Rn)

Upcoming Changes
===
 - ~~Standard 4 Lane Version~~ - DONE
 - ~~Add Blank LED Matrix for use with LED Strips~~ - DONE
 - Slimmed down (17mm) Side Panels

Thank Me
===
A few ways you can show your appreciation for my work:\
[Buy Me a Coffee](https://buymeacoffee.com/makermylo) | [Subscribe on YouTube](https://www.youtube.com/@makermylo) | [Follow on X](https://x.com/MakerMylo)
