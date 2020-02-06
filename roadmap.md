

# IMPLEMENTATION STRATEGY



## **Stage 1: Name those Pain Points**

How much can we implement, given the resources and the workload we handle?
The first stage on any QA Framework implementation is to identify the pain points inthe context of the company, the available resources (the team, the timeframe, the funding) and the knowledge of the team in the testing arena.


## **Stage 2: Definition of QA Framework and dev guidelines**

This is precisely this documentation and the proposal.
What we try to do here is to analyse the testing needs, procedures and capabilities that we can progresively implement whereas they make sense in our context.
For that we should write guidelines, documentation and help-docs about the different stages of the QA Framework, what are the risks of not implementing it and quantify when possible the resources needed for its implementation along a well defined roadmap.
We will talk about code style, development paradigms and approaches, management methodologies, version control, different kind of testing procedures and workflows.
We all talk a lot about User Experience and we take good care of that, but we talk very little about Developer Experience and a good development experience has its reflexion on the final product and the productivity itself: this is development guidelines, documentation, agreement on code style...

**Specs, features and bug commenting guidelines**
We need to agree in the way we are going to document specs and features when they are requested as well as bugs and defects when they are found on the application.
 - You can find our Specs Style Guide / Template here
 - You can find our Ticket / task Style Guide here
 - You can find our Bug / Defect Style Guide here

## **Stage 3: Code Style, Code Documentation and Unit Testing**

One of the easiest and simpliest stages to implement when talking about testing is actually having a solid set of good practices well defined. 
These good practices usually start with the code style itself, the quality of the different algorithms from different points of view, the documentation, unit testing, etc...
 - Code Styles: picking an existing code style suite can go a long way when implementing good practices. There are many different code styles already defined by third party software oriented companies, such the example with ReactJs code style written by AirBnB. Whereas quite restrictive, it can be tweaked further in order to adjust it to our needs and skills making its adoption easier, but the main part being already largely accepted by the community. Code style is not only a topic about taste, but about maintanability and consistency. When two pieces of software has been written following the same style guidelines, any developer can jump on and off those pieces of software  seamessly making transitions and hand-overs extremely easy since the developer feels like in home at any time. Code styles enforce knowledge and resource share.
	 - You can find our Javascript Code Style ***here***.
	 - You can find our CSS Code Style ***here***.
	 - You can find C# Code Style ***here***.
 - Commenting Code: closely to the code style topic, commenting code is a good practice nobody argues, however the way of doing it sometimes differ a lot from some developers to others. Having a good definition of what has to be commented and how (such templates) will help everyone to stick to the rules and always comment what makes sense to be commented and avoid both under and over commenting. Also, sticking to a particular way of commenting would help to run automatic tools that can generate developers documentation out of such comments.
	 - You can find our Code Commenting Style Guide ***here*** to make use of autodocumenting tools (*define the autocomenting tool here...*).
 - How-to's guides and documentation for developers: another important part when talking about best practices is commenting not only the code, but creating guidelines and how-to's, simple websites that can be published, README files on repositories with some simple examples of use...
 - Unit testing: we all know we have to test our code, writting unit tests for each of the pieces of code (that are actually testable and it makes sense to do so) is a must and we should try to make it part of the minimum requirements when pushing code to our repositories to be approved and merged into the main branches.

## **Stage 4: GitFlow, Code Review and SemVer**

### **Adopting GitFlow**
GitFlow is not everyone's favourite branching model nor a silver bullet to solve every issue that may arise when a particular repository is receiving code from multiple developers working in different (or the same) area, features, bugs... however, in my humble personal experience with and without it, I definitely see its relevance specially important when talking about scattered team members working from different places.
Having a proper branching model in place helps communicating changes, review them, avoid merging conflicts and keep a consistent code quality across the repository and the different team members.
Probably everyone knows gitflow or some similar branching model. We should get to the agreement of using a consistent and homogeneous branching model across different teams and repositories so that way it is easier to jump from team to team or project to project and keep the same workflow with minimum hiccups and very flat adapting curve.
Let's talk about the GitFlow strategy to implement [here](gitflow.md).

### **Code Review Strategy**
One of the best advantages of having a proper branching strategy in place is the posibility of identify events in the workflow where Code Review practices can implemented.
You can find references to the Code Review Strategy in the [GitFlow](gitflow.md) section.

### **Facilitating Semantinc Versioning**
The final step in this stage is implementing a proper semantic versioning strategy when releasing new revisions of a particular component or application. Having a good branching model helps to match up the roadmap, the workload and the different versions released with the needed changelog documentation in place.
This is particularly important when releasing revisions of components that are being used across different projects by multiple teams.
The release strategy is also documented in the [GitFlow](gitflow.md) section.

## **Stage 5: Environments and CD/CI**

When a solid branching model and versioning system are in place and working, it is time to think about automating deployments.
We need to discuss about the system to implement so we all (or at least the people responsible for deployments) can be familiar with it. A system we can use in different environments either if those are in our own hosting system or in a PaaS whatever it is.
It is important to try and think about vendor-locking here, if we configure this deployment system only for a particular PaaS or hosting type, we may not be able to reuse it for other platforms.

**GEO Server**: currently we are overriding and backing up files manually every time we want some changes, but actually many customers are sharing the same configuration, styles, etc for different entities. There has been some issues when changing some styles and introducing breaking changes for other ports or features.
Every client using GeoServer should have their own configuration and styles. The ones that are shared should be transparent and very well known so anyone introducing changes can test in different places before making their way into production environments. Environments are also an issue, currently we don't have dev, test and prod environments so every change is being made directly on production, which is very dangerous. The final issue is about how GeoServer stores files, configurations and styles: some seem to be on folders as json or xml files, some are somewhere else, maybe in a database... We have to find out a method to version and sandbox by environments (and customers) the different configurations, shapefiles and styles so it is safe to develop, test and deploy changes.

**Http Server**: same issues that with the GeoServer is more or less happening for the Web Server.

## Stage 6: RACI Matrix and Comunication

At this stage we should already have a set of good practices implemented, a solid branching model that results in good versioning and our deployments are being automated, now we need to start thinking about developing a responsibility assigment matrix.
Identifying in each stage of a new release (however small it could be) responsibilities. 
In the past I adopted a RACI matrix as such:
Responsible: the people that completes the tasks. In our case, generally developers.
Accountable: the person with authority to say yes or no to a particular deployment. This participant needs to be informed prior to any release with the technical details and how those changes affect functionality, features and final users. Usually it would be a team leader or project owner position (or above).
Consulted: the people that needs to be consulted, they don't hold the final decision, but they can influence whether it is a good time or set of features or the specs are met accordingly. Many times are technical consultants or even account manager if the deployment is very particular to an unique customer.
Informed: everyone that should know about the new features being shiped in the new release with what, why, when and how. They can be from technical members of the team working in parts related with some to be released to customer assistants, support teams, sales, marketing... almost anyone.
This matrix helps pinpointing and addressing the right players in every release. It is like a checklist that helps the deployment manager to go through the right path when a new release is scheduled and ready to happen. Then is when the communication channels are in stake.
We have to find the right way to communicate actively the people involved and those people involved have the responsibility of replying and make the questions they may have in a timely manner and very well comunicated to the accountable player so comunication can go both ways fluently.
We have to identify, in each project or task, who are the different people and their roles as well as a reliable communication mean that can fluently work both ways in a timely manner.

## Stage 7: Implementing different software testing techniques

At this stage we know what we can get done in regards to our resources.
Here is when we start talking about integrating in the workflow different testing techniques more advanced than the ones so far implemented. We start thinking more about testing than code here.

Have a look af the diferent types of testing phases we could implement [here](testing_phases.md).

