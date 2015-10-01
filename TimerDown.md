# Introduction #

TimerDown is an object class which can be instanciated by user as many time as needed to create time counters which are decremented from x to 0 on a time basis.

time base and start value can be set during object declaration or inside program. Once the counter as reach the 0 value, it will keep it unitl the user change it. possibility to pause/resume.

# Details #

**TimerDown.h**

this file defines the TimerDown class and corresponding methods.

class **TimerDown**

this object can be instanciated by the user program. contains only static method and 3 variables (1 long + 1 int + 1 bool).

_declaration examples:_

TimerDown countMs;

TimerDown count10sec(10,1000);

_usage example:_

if (countMs==0) countMs=1000;

if (count10sec==0) { count10sec=10; }

countMs.pause();

countMs.resume();

if (countMS.paused()) { ... }

countMs.set(100);

countMs.reset();

countMs.init(1000,1);