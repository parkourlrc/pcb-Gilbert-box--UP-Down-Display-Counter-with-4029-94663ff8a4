# UP-DOWN-Counter-with-single-7-segment-display


This a simple project Up/Down binary counter circuit using the CD4029BE (Binary/Decade Counter) and a 74LS47 BCD-to-7-Segment Decoder/Driver to display count values on a 7-segment common anode display.
The circuit also includes LED indicators for binary output and control logic for manual counting, reset, and direction (Up/Down) selection.

# Features

  - Up/Down counting mode using a toggle switch
  - Manual clock input via push button
  - Reset control for restarting count sequence
  - Binary LED indicators for visualizing Q outputs
  - BCD to 7-segment display via 74LS47 decoder
  - Suitable for educational and hobby projects

# How It Works

1. Clock Pulse(SW1) - Generate HIGH input to the clock pin of CD4029BE and led indicator (D6)
2. Reset (SW2) - Clears counter to 0000
3. Up/Down Switch(SW3) - Select counting mode (UP/DOWN) with led indicator (D5)
    - Led ON = UP
    - Led OFF = DOWN
5. Output Display
    - LEDs show binary output (Q0–Q3)
    - 7-segment display shows decimal equivalent (0–9)
    
# Notes & Tips

- Use SPST switches instead of DPDT for smaller PCB.
- For clean input, consider using debouncing on push buttons.
- Modify the counter mode (binary/decade) by changing pin 9 on CD4029.
- For continuous counting, replace the push button with a clock generator (555 timer or square wave source).
