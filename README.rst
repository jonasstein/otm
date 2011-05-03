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
- final PCB should use a AVR
- use IRQ
- to measure 100 km/h with resolution of +/- 1 km/h
  with 1 m sensordistance we need timeresolution of at least
  1m /(100 km/h ) - 1m /(101 km/h ) = 0.35 ms 
  it takes 3.6 seconds to go 1m at 1 km/h 
- need to count more then 1..12000 (> 8 Bit)
- perhaps external counter with parallel -> serial converter will help to 
  count fast and precise.
- wich photodiod to use? (BPW 82 is fast)
- wich LASER to use? IR-Laserdiods are cheaper and invisible
- how to adjust lower threshold for the photodiods?
- should we use a pulsed light barrier and IR-filter? 
