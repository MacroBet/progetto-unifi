# progetto-unifi

# Sensor Reader usage Example
s = Sensor()
s.readLightLevel()

# Beeper usage Example
b = Beeper()
b1 = Beeper()
b2 = Beeper()
b.turnOn("white")
b.makeBeep("red",3)
b.makeBeep("green",3)
b.makeBeep("white",10,.5,.3)

# EventManager usage Example
from led import Beeper
def beep():
    beeper = Beeper()
    beeper.makeBeep("white",3,0.4,.2)
evm = EventManager()
evm.registerButtonListener(beep)
