# yard_bot
GPS-RTK based autonomous lawn mower

The idea is to use the NEO-M8P-2 GPS-RTK module from uBlox to control a lawn mower.  This device is spec'd to 25mm accuracy.  You need one at a known location as the base station, the other one goes on the rover (mower).  
So we need a base station, probably a RaspberyPI to allow easy wireless access from a computer for config and debugging.  A LoRA conection from the base station to the rover.  A processor (Arduino) on the rover to manage the GPS, LoRA and driving the mower from waypoint to waypoint.
Mower hardware should be a battery powered mower, Ryobi's 40V line looks cost effective.  Add two BLDC drills that can be indpendantly controlled from the Arduino and we have the ability to steer.
