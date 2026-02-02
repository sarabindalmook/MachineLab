# Homework 1 (Jan 29)

This homework includes three history versions of the code ([link to homework](homework1_jan29)):

1. **Original code** – the starter example from the Adafruit Multitasking Tutorial (FILE CREATED)
2. **Button version** – modified so the servo stops sweeping when the button is not pressed (FIRST UPDATE)
3. **Potentiometer version** – extended to control the sweep speed using a potentiometer (SECOND UPDATE)

## Challenges & Debugging

During this process, I spent a lot of time debugging both the code and the wiring because the circuit was not behaving the way I expected. The main issue ended up not being the code at all, but the pushbutton on my breadboard. I initially assumed there was a logic or wiring mistake, but after checking different parts of the circuit, I replaced the physical button with another one and everything immediately worked. This taught me to consider hardware issues as well, not just software errors (something that also happened last week).

Another issue was completely my own mistake. The second servo was not moving at all, even though the code was correct. After some debugging, I realized that I had connected the servo to pin 6 instead of pin 9 because I was reading the pin numbers backwards. Once I fixed the pin connection to match the code, the servo worked normally.

To debug these issues, I changed one thing at a time and tested the circuit after each change. When something did not make sense, I simplified the setup and checked individual components, such as testing the button and servos separately. Through this process, I also learned that the speed of the servo sweep is controlled by a time interval rather than a delay. The potentiometer value is read and mapped to an interval, which determines how often the servo position is updated. When the interval is smaller, the updates happen more frequently and the servo sweeps faster, and when the interval is larger, the updates happen less frequently and the sweep is slower.

# Homework 2 (Feb 3)

## Part 1
This part was postponed due to not having access to the Scene Shop.

## Part 2

![Minecraft Mood Board](MinecraftMoodBoard.png)

An idea that came to mind is using Minecraft as a direct reference to build a physical 3-D world miniature that functions the way the game does. The goal is not to imitate the look only, but to recreate a world that behaves through mechanics that already exist in the game. Rails and minecart logic could act as the main visible motion in the world. A cart endlessly looping through the environment, triggering actions as it passes certain points.

Everything would be built from blocks or cubes to create the environment, with a loose storyline embedded into it. There is a main player who has a house that exists in the world. Around it, mobs such as zombies, spiders, or skeletons are programmed to move or react to triggers. A skeleton might shoot arrows on a loop, a zombie could slowly approach the house, or an explosion effect could reference a creeper moment.

Other references from the game could include hidden piston doors that briefly open and close, trapdoors that drop or reveal spaces below, or underground Redstone paths that are partially exposed like a mined cave. Sound elements inspired by note blocks could activate when certain actions happen, giving feedback similar to the game.

And noticing how in Minecraft there is a clear day and night cycle, the installation could play with that shift as well. When the installation is closed, the world exists in a “nighttime” state. The moment someone presses a button, the world switches to daytime.  
