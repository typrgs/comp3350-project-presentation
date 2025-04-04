---
layout: page
title: Post-Mortem
include_in_header: true
---

# Post-Mortem 🏖️

### Successes

One of our biggest strengths was our ability to reprioritize tasks effectively. When refactoring became a more pressing need than new feature development, we adjusted our workflow to address it first. In the third iteration of the project, we made a concentrated effort to focus on increasing our code coverage and addressing grader feedback. This adaptability helped us focus on the parts that mattered and kept us on course throughout the project.

### Setbacks  

However, our biggest challenge was communication and awareness of changes. At times, code modifications were made without the entire team being informed, which led to deficiencies in code quality due to a lack of proper reviews. Being more active in cluing in members about current developments and establishing a more structured review process would have helped prevent these issues better.

### What We Would Have Done Differently

If we had the chance to start over, we not have waited as long as we did to make concrete progress in iteration 1. We also would place a similar emphasis as we did nearing the end of the project, to clearly and frequently announce tasks we are working on to the entire team. The lack of communication in the beginning was the primary source of our problems. We gradually developed habits to correct that as the term progressed, but it would have been better if we got it right from the start. Finally, if we were to restart, we would establish a structured review process such as regular in-meeting reviews to mitigate against problematic code slipping through the cracks.

### What Took the Most Time? The least? Any Surprises?

What took us the most amount of time was getting the architecture right. We were consistently unhappy with some decisions we made early on and it took some time to make it the way we wanted. Examples include how to relate our domain specific objects, and how to structure the layers such that the persistence layer could be independent of Android packages. The things that took the least amount of time were quick things like assigning issues and reviewing the requirements of an iteration. Those tasks could usually be concluded in a single two hour meeting. The group agrees that the most surprising outcome was the sheer amount of difficulties we experienced with miscommunication and dealing with merge conflicts.

### Outstanding Bugs

The only outstanding bugs that we are aware of is the fact that the cover images for exercises are unresponsive to the aspect ratio of the device. The result is that the images will appear cropped or zoomed out on certain screens. A few other issues are due to deliberate decisions to cut down on features in favour of improving the quality of the code. This includes the fact that cover images are not displayed when playing back a workout, as well as the fact that completed sessions are not recorded in the app. The implementation of these features were deferred to the next iteration of the project.

### Revisiting the Iteration 2 Retrospective

In our retrospective from iteration 2, we noted some problems we had during the final moments before the deadline as we merged our branches onto `dev`. We decided that in the following iteration we should avoid making large architectural changes to the project at such a late stage in the iteration.

While we did become more effective working together in iteration 3, we unfortunately ran into eerily similar problems. Nearing the end of the iteration, we merged significant changes to the architecture of the project, hoping to resolve some inappropriate dependencies between the persistence layer and Android packages. This time we were careful about only merging once the team was finished with their tasks. Unfortunately, we did encounter a problem as we tried to merge the `dev` branch onto `main`. Upon investigation we identified the crux of the problem being an older pull request which had mistakenly been merged onto `main` and thereafter reverted. We're not sure why this caused our problems since theoretically the reversion should have returned the branch to a normal state. We made several attempts to resolve it such as emptying the files in the main branch, yielding unsuccessful results. We're still not sure why, but the only successful solution we managed was manual copying of the files to the main branch.

While we did exercise more caution this time around when making large changes, we regret being so optimistic as to expect that there wouldn't be random inconceivable errors in the very tools we were using to manage the project. In hindsight, we see that it should have been obvious to us no matter the measures we took, that making large changes to the code at such a late point in the iteration was overly optimistic and risky. In future iterations, we will remember this experience as a reminder that we cannot prevent random disruptions from occurring and from now on we will make preliminary merge commits onto main well before the due date to validate the merging software and ensure our merges are small.

### Moving Forward

While making this project, we learned that communication is extremely important. It really isn't possible to work together without telling everyone exactly what you're doing. It's important for many reasons, but one notable reason is that decisions made by one person routinely influence the decisions of other team members. This project reinforced this idea to us and, going forward, we'll focus on frequent and clear communication, structured planning, as well as rigorous code review to ensure smoother collaboration and improved code quality.