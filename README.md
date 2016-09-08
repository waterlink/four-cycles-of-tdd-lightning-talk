# 4 Cycles of Test-Driven Development

Pivotal Labs Berlin. 8 Sep 2016

*(lightning version)*



## Test-Driven Development

Is it only about 3 laws and Red-Green-Refactor?

There is more to it.



## Nano Cycle

(seconds)

Three laws of TDD:

1. __First__ write failing test.
2. Write __just enough__ of a test to fail.
3. Write __just enough__ of a production code to pass it.

*(not compiling or parsing failures are failures)*



## Micro Cycle

(minutes)

Red-Green-Refactor:

1. **RED**: Write a failing test
2. **GREEN**: Write production code to make it pass
3. **REFACTOR**: Clean up tests __and__ production code\*

\* - Step back for a few seconds to see if there is anything to clean up. And if so, do so.



## Milli Cycle

(every ~ ten minutes)

> As the tests get __more specific__, the code gets __more generic__.

Add a specific failing test. Write a general code that passes the whole class of such tests. Triangulation technique and Transformation Priority Premise helps.



## Primary Cycle

(hourly)

Step back, look at the overall system, and see which architectural boundaries we are crossing.

*(these boundaries are hard to see in other cycles)*

We make some informed decisions and steer our next nano-, micro- and milli- cycles. Until next primary cycle.



## Thanks

- Blog: [tddfellow.com](http://tddfellow.com)
- Twitter: [twitter.com/waterlink000](https://twitter.com/waterlink000)
- Github: [github.com/waterlink](https://github.com/waterlink)
- Build Testing Framework:

  [bit.ly/build-testing-framework](http://bit.ly/build-testing-framework)

- TDD Screencasts: [bit.ly/tdd-screencasts](http://bit.ly/tdd-screencasts)
