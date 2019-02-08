# TESTING PHASES

## Types of Software Testing

We are not going to be able to implement every single stage of software testing and many, in fact, wouldn't make sense because of the nature of the projects, the data handled, the type of users or the underlying infrastructure.

Relevant software testing stages for our projects could be defined as follows:

## Functional testing:

 - **Code styling and quality:**
	 - Although it is not usually included as part of the testing process, it is a fundamental corner stone for software quality therefore I include it as part of the QA framework. This is defining a code style, following it and checking regularly that developers are following those rules agreed on it.
 - **Unit testing**
	 - Testing an individual component, module or feature by using automated test runners and definitions.
 - **Integration testing**
	 - Having a good definition of each piece of software's limits and how they interact to each other gives us a good understanding about the moving pieces that need to gear up together to make the software achieve its purpose and work efficently. Integration testing is very interrelated with system testing, but there are differences. In the integration testing there is no need of going across the whole system, but only the pieces related with the software to test at any level.
 - **System testing**
	 - A throughfully test of the whole system involved in a piece of software. Frontend, Backend, Database, Interfacing, Infrastructure... This kind of testing, when a good integration testing is in place, is usually not first need for incremental software versions implementing minor new features or fixing bugs.
 - **Sanity testing**
	 - When a deep QA Framework is in place and there is a lot to test every time, this kind of test is a some sort of preview of the software so, if it crashes immediately or there is major defects detected right away, the testing process is abandoned for the sake of efficiency forcing the development to focus on the defects detected that are blocking the testing process.
 - **Smoke testing**
	 - Having a good definition of what the software is expected to do, how is it expected to look and how the different users are expected to interact with it gives us a good starting point as reference for developing a smoke testing plan. Usually the tester will go through a list of "poking" points searching for simple common points of failure. This is usually one of the more common testing practices and it's performed as one of the first stages. It need a good set of test cases defined and it helps A LOT when identifying if the User Acceptance Criteria is being followed.
 - **Regresion testing**
	 - Documenting bugs and deffects is as important as fixing them. Testers usually write down those bugs detected and tend to poke around the area of the software that caused such bugs in future versions in order to find out if any new implementation has introduced back the bug already solved in previous iterations. The key for this testing suite is having a properly documented process with the bugs that have been solved and how such bugs were reproduced step by step.
 - **Beta/Acceptance testing**
	 - This area of testing is also know sometimes as User Aceptance Testing. It usually includes the final users or, at least, a part of them. They would go through the piece of software finding in everything required has been implemented and if the features are aligned with the original specs. This kind of testing is very useful to find out whether the software is following users requirements before a public release.

## Non-functional testing:

 - **Performance testing**
	 - Quite self-explanatory. Performance testing is meant to identify bottlenecks, performance issues and hickups on the piece of software in question, however still we can talk about tooling, logging and reporting to achieve this tests. Tools are very different when talking about database performance, server performance or front-end performance. Picking the right monitoring tools can help a lot when trying to hunt down performance issues.
 - **Stress testing**
	 - As a sideway of performance testing, stress testing are meant to identify the same kind of issues when the software is under stress being such stress the amount of data stored, the indexing process, the downloaded data or how the server can handle millions of connections at the same time.
 - **Security testing**
	 - Also pretty self-explanatory, this kind of tests are more difficult to implement because good practices are not always the only way to avoid security holes, the way security testing works is a whole different world and it should be performed by profesionals specialized in security. To avoid the most common issues, following best practices is a good start, having a collection of common security vulnerabilities and going through them methodically should help to early identify them.
 - **Recovery testing**
	 - If the piece of software goes down, crashes or fails? What methods are in place to recover where I left? From backups to state management and partial work recovery when the user hasn't saved... etc.
 - **Usability testing**
	 - This is one of the most elocuent tests that can be performed on a piece of software developed for final users who will interact with it by the use of UI interfaces. It is usually performed to determine whether the UX is being addressed correctly and helps to identify flaws and incorrect assumptions. There is three major different approaches to this kind of testing:
	 - Final User Testing: performed by the kind of users that will finally use the piece of software and it assumes some knowledge on the field and sometimes on the software itself, how it is supposed to be used and its purpose. This test sessions help to steer back decisions and assumpsions helping the software to get closer to the user needs and habits of use.
	 - Monkey Testing: usually performed by testers, it assumes nothing and the tests will be ridiculously stupid all around, punching anything at any point. This kind of test is very efficient when finding overflows, stress, interface issues and fool-proofing the software making it more robust.
	 - Grandma Testing: grab a non-technical user on the field with no previous knowledge at all and observe carefully how they go through all the steps and features, let them explore and discover by themselves what the software is for and how to use it. If the user gets stuck frequently, there is lack of help or usability.
	 - *Side note on UX*: when any person is using a piece of software, we tend to start using it without having training nor reading introductory tutorials whatsoever. Therefore the user will get stuck more easily in user interfaces with odd layouts or with non-intuitive  user interfaces, make the user experience frustrating and generating in the user what it is called "ego depletion" which basically means the user feels frustrated, useless, not skilled enough for the application and tends to abandon it quickly saying either "you need to be a rocket scientist to use it" or "it is very hard to use".
 - **Localization testing**
	 - In internationally deployed software, this kind of testing helps a lot identifying weak translations, cultural clashes (sometimes what a color means in western cultures is not the same in oriental ones, being able to comunicate with iconography or colors becomes more of a challenge in this case).

# OUR IMPLEMENTATION STEP BY STEP

## Phase 0
Define and Implement Agile/SCRUM tools and procedures
Implement dev workflow / sprint physionomy

## Phase 1
Implement Specs guidelines
Implement Tasks guidelines
Implement Bug / Defects guidelines

## Phase 2
Implement Code Style and Unit Testing
Implement Branching Model and Code Review
Implement SemVer and Release Strategy

## Phase 3
Implement CD/CI automation systems
Implement Changelog guidelines
Implement RACI matrix and Communication channels

## Phase 4
Implement QA / Testing phases (define here which ones we can start implementing and how to go ahead with more advanced ones).