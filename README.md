# mabu
Python library for controlling the robotic head of Mabu, a robot by Catalia Health

To get more detaied documentation, go here: https://electronick-co.github.io/hacking_mabu2/

# Usage

Connect a usb to serial adapter, or use in a raspberry pi.

On the top board, disconnect the serial cable that comes from the tablet (black, white, and red), and solder the pins for connecting to the serial converter or the Raspberry Pi.

![WhatsApp Image 2025-03-05 at 9 02 30 PM](https://github.com/user-attachments/assets/74f8dfa5-caef-4444-aa3e-a178850016dc)

![WhatsApp Image 2025-03-05 at 9 01 57 PM](https://github.com/user-attachments/assets/c1007bb4-5c55-4116-97a3-f26234f11e7d)


`py -m pip install mabu`

``` python
from mabu import Mabu
mabu = Mabu("COM3")
mabu.on()

mabu.center_all() # move all part to the center (50)

mabu.mover_robot_part("LDR",0) # movement goes from 0 to 100


```

## Mabu parts:

LDL = left eyelid

LDR = right eyelid

ELR = eyes up and down

EUD = eyes left and right

NE = head up and down

NR = head left and right

NT - tilt head left and right
