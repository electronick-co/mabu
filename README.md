# mabu
Python library for controlling the robotic head of Mabu, a robot by Catalia Health

To get more detaied documentation, go here: https://electronick-co.github.io/hacking_mabu2/

# Usage

Connect a usb to serial adapter, or use in a raspberry pi.

On the tops


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
