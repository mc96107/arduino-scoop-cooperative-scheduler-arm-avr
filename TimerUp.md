# Introduction #

TimerUp is an object class which can be instanciated by user as many time as needed to create time-counters which are incremented from 0 to x on a time basis.

time base and roll over value can be set during object declaration or within program.
roll over can be monitored by the program in order to trigger periodic activities.


# Details #

**TimerUp.h**

this file defines the TimerUp class and corresponding methods.

class **TimerUp**

this object can be instanciated by the user program. contains only static method and 5 variables (3 long + 2 boolean).

declaration examples:

TimerUp countup;        // count from 0 to 1 billion every milli second

TimerUp countup(100);   // count from 0 to 99 continuously every milli seconds

TimerUp countup(3600,1000);   // count from 0 to 3599 continuously every seconds

utilisation example

loop() {
> if (countup > 100) { countup=0; }

> countup.pause();

> if (countup.paused()) countup.resume();

> countup.set(10);

> countup.reset();

> countup.setRollOver(100);

> if (countup.rollOver()) { .. }