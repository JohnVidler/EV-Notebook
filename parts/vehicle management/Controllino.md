# Controllino

![A Controllino, Animated](/img/controllino/Controllino-Animated-V2.gif)

[The Controllino Homepage](https://www.controllino.com/)

- Lots of 12-24v tolerant IO
- Arduino-based, so easy enough to program
- Lots of relay outputs for driving lights, etc. directly
- DIN mounted
- Reasonable serial I/O
    - RS485 support natively
    - Isolated ethernet on-board, for debugging, etc.
    - Missing direct CAN bus support, but easy enough to add via a custom expansion board.
        - Note to John: Upload details on the board you designed here!
- Uses a fair amount of current during standby
    - Note to John: Take standby measurements, they're not listed on the Controllino site at all :(