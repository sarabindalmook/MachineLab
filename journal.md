## Homework 1

This homework includes three history versions of the code ([link to homework](homework1_jan29)):

1. **Original code** – the starter example from the Adafruit Multitasking Tutorial (FILE CREATED)
2. **Button version** – modified so the servo stops sweeping when the button is not pressed (FIRST UPDATE)
3. **Potentiometer version** – extended to control the sweep speed using a potentiometer (SECOND UPDATE)

## Challenges & Debugging

During this process, I spent a lot of time debugging both the code and the wiring because the circuit was not behaving the way I expected. The main issue ended up not being the code at all, but the pushbutton on my breadboard. I initially assumed there was a logic or wiring mistake, but after checking different parts of the circuit, I replaced the physical button with another one and everything immediately worked. This taught me to consider hardware issues as well, not just software errors (something that also happened last week).

Another issue was completely my own mistake. The second servo was not moving at all, even though the code was correct. After some debugging, I realized that I had connected the servo to pin 6 instead of pin 9 because I was reading the pin numbers backwards. Once I fixed the pin connection to match the code, the servo worked normally.

To debug these issues, I changed one thing at a time and tested the circuit after each change. When something did not make sense, I simplified the setup and checked individual components, such as testing the button and servos separately. Through this process, I also learned that the speed of the servo sweep is controlled by a time interval rather than a delay. The potentiometer value is read and mapped to an interval, which determines how often the servo position is updated. When the interval is smaller, the updates happen more frequently and the servo sweeps faster, and when the interval is larger, the updates happen less frequently and the sweep is slower.

