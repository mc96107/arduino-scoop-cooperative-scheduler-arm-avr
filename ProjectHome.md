---> HAPPY NEW YEAR ! SCoop V1.2 RELEASED with lot of optimizations :)

---> Standard Scheduler.h originally made for Arduino DUE now ported on AVR, see downloads (also included in the SCoop pack)

---> New User guide updated V1.2. (also included in SCoop Pack)

project support on Arduino forum :
http://arduino.cc/forum/index.php/topic,137801.0.html



This library provides a comprehensive set of objects for creating multi task multi thread programs with smart support for fifo, timer and event handling.

Task switching is orchestrated by a scheduler fully cooperative, which enables using almost any existing Arduino library without risk of re-entrant code, by calling standard yield() method.

The library is inspired from the Java Thread/Timer libraries and a set of macro simplifies the creation of derived user objects.

In addition, a TimerUp and TimerDown library provides a simple but powerful way of handling un-limited time counters with rollover or "ground zero" stop.

In addition, a IOFilter library provides a simple and very comprehensive way to declare Input and Output by using object and support time filtering and counting possibilities.

in V1.1 a new SCoopFifo object simplifies fifo handling and communication across task or events.

next steps ? well, use it and burn it :)