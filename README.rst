Open Traffic Control
====================

Open Traffic Control (OTC) is a open hardware and 
open source project to analyse traffic on roads.

Goals of OTC:

- counting vehicles
- measure speed of vehicles
- measure length of vehicles
- measure noise of vehicles
- write logfiles that are easy to evaluate (csv?)
- use inexpensive hardware (ready to use < 200 EUR)


Citizens claims about traffic situation are very subjective. 
There are driving "too many vehicles too fast and too loud".
Citizens' action committee can use OTC to collect data and 
use it to establish constructive actions based on facts.

OTC will never substitute a official survey but it can provide
a good estimation in a pilot survey.

Brainstorming
-------------

- 3 Laserdiodes and photodiods make 3 light barriers (a,b,c)
- the barrier that is crossed first is called 'a'
- the time a-b is called 'tab' 
- the time b-c is called 'tbc' 
- the distance 'sab=sbc' between a-b-c should be equal (1 metre?)
- a display for the current measurement would be nice
- use a Seeduino (Arduino) as base-system
- final PCB should be a Seeduino-Shield
