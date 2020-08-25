# Programmer Time Estimates

(from: https://coding.abel.nu/2012/06/programmer-time-translation-table/)

An experienced project manager I used to work with claimed that he took the programmers’ time estimates, multiplied by pi and converted to the next time 
magnitude to get the true number. 1 day converts to 3.14 weeks.  To get a more precise conversion, I’ve created a translation table for programmers’ 
time estimations, trying to narrow down where things go wrong.

| Estimate | The Programmer Thinks | What the Programmer Forgot | Actual Time |
| -------- | --------------------- | -------------------------- | ----------- |
| 30 sec   | There’s just a small change to the code to be done. I know exactly what to type and where. It takes 30 seconds to type. | Time for starting the computer, the development environment and getting the right source. The time to build, test, check in and document the fix | 1 hour |
| 5 min    | It’s a minor thing, I just have to look up the exact syntax on google and fix it. | It’s quite rare to find exactly the right information on the first try. Even if it is found, it probably needs some adjustments before it works. Add time for building, testing etc. | 2 hours |
| 1 hour   | I know how to do it, but it’s some code to write so it will take some time. | 1 hour is too tight to have any margin for unforeseen problems. Something always fails. | 2 hours |
| 4 hours  | 	It’s some code to write, but I roughly know the step. I know the Wizzabanga module of our standard framework can do it, but I have to check the documentation on exactly how to call it. | This is probably the only realistic estimation. It is large enough to have some margin for unexpected problems, while the task is still small enough to grasp. | 4 hours |
| 8 hours  | I first have to refactor the Balunga class into two, then I’ll add a call to the Wizzabanga code and finally add the new fields to the GUI | There’s a lot of dependencies on the Balunga class from different parts of the system. About 40 different files have to be adjusted. The newly added field in the GUI has to be added in the database as well. 8 hours is too large to grasp completely. There will be more steps than the programmer thought of when estimating. | 12 - 16 hours |
| 2 days   | It’s really quite a lot to code. I have to add some new tables to the database, a GUI for those and then the logic to read and write data to the tables. | 2 days of work is too large to overview for most developers. There will surely be things that are missed. Not just small things, but entire major pieces of functionality required will be forgotten during the estimation. | 5 days |
| 1 week   | 	Ouch… that’s a HUGE task. I don’t have a clue on how to do it, but I can’t say I don’t know. One week should be enough, I hope, I really hope, but I can’t ask for more or they’ll think I’m not competent enough. | The task is way too large to get an understanding of for most programmers. It has to be sent back to an architect that can help splitting it in smaller parts and provide some direction how it should be solved. The architect might find a simple way to do it – or find that there’s a lot more work than expected. | 2 - 20 days |


Time estimation is hard. Every programmer has an interval where the estimations are realistic. Going below that interval means that the overhead (building, testing checking in code) was overlooked. Going above that interval means that the task is too large to overview.

For junior developers, the interval might even be non existing. They overlook the overhead while on the same time any non-trivial task is too large for them to overview. I’d say that an experienced developer should get anything between 0.5 hours and 24 hours right. Above 24 hours a breakdown is needed. It can be done in the head and then summed to 60 hours by the developer – but even someone experienced need to have manageable chunks to think of.

It is also important to understand that experience in programming is not the same as experience in estimation. A developer that’s not involved in the estimation process won’t get good at estimation. Also if actual time spent is never measured and compared to the estimates, there is no feedback to learn from.

Eventually, every programmer will have use for estimation skills. To prepare for that, decide when things are done for each task you take on. Then estimate the task before starting. Finally count the time spent and compare that to the estimate. Also compare what you actually had to do to your own definition of done. That way you’ll improve both your understanding of all the details involved in a task, as well as improve your estimation skills.
