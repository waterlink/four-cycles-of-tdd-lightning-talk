# 4 Cycles of Test-Driven Development

Codemotion Warsaw 2016. 16 Sep 2016

*(quick version)*

Note:
Hello everyone. Thank you for coming. Today you will learn about well-known cycles of TDD, such as 3 Laws of TDD and RGR cycle. And other 2 not so well-known cycles of TDD, that address issues that the first 2 have.



<img src="../my-presentation-template/me.jpeg" class="photo-me">

## Oleksii Fedorov

Software Craftsperson

Software Engineer  
@ Pivotal Labs

[@waterlink000](https://twitter.com/waterlink000)

Note:
My name is Oleksii Fedorov. I am a Software Craftsperson and I work as a Software Engineer at Pivotal Labs. I encourage you to ask any questions and raise any concerns that you have about TDD, I will try my best to address them. Shall we get started?



## Test-Driven Development


### Main benefits

- No fear while changing & releasing the code
- Ruthless refactoring
- Ability to change design & structure (as a result)
- I trust my tests as a parachute when jumping out of the plane
- QA & Deploy process: `$ ./ship_it.sh`


### Side benefits

- Living documentation
- Near to no bugs
- Forget all your debugger shortcuts



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


### [bit.ly/triangulation-tdd](http://bit.ly/triangulation-tdd)

(blog by TDD Fellow)

##### -

### [bit.ly/transformation-priority-premise](http://bit.ly/transformation-priority-premise)

(blog by Uncle Bob)



## Primary Cycle

(hourly)

Step back, look at the overall system, and see which architectural boundaries we are crossing.

*(these boundaries are hard to see in other cycles)*

We make some informed decisions and steer our next nano-, micro- and milli- cycles. Until next primary cycle.



## Thanks

- Blog: [tddfellow.com](http://tddfellow.com)
- Twitter: [twitter.com/waterlink000](https://twitter.com/waterlink000)
- Github: [github.com/waterlink](https://github.com/waterlink)
- Build Testing Framework series:

  [bit.ly/build-testing-framework](http://bit.ly/build-testing-framework)

- Stuck with TDD? series:

  [bit.ly/stuck-with-tdd](http://bit.ly/stuck-with-tdd)

- TDD Screencasts: [bit.ly/tdd-screencasts](http://bit.ly/tdd-screencasts)



## -



## FAQ


### Q: Uncertain what will the first test look like?

### A: TDD is a Tool. Use another tool: SPIKE


### Q: Don't know how to test it without first having coded it?

### A: TDD is an API design tool. Start from the ASSERTION.

and go backwards.
