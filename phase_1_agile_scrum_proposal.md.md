---


---

<h1 id="agile--scrum-proposal">AGILE / SCRUM proposal</h1>
<h3 id="proposal-for-phase-1">Proposal for phase #1</h3>
<p>Due the very raw Agile culture in the company, it may seem natural to go slowly testing and acquiring different aspects of the Agile methodology.<br>
However, implementing only some parts of the full Agile workflow may be risky.</p>
<p>Agile is not a textbook methodology with only one way of implementation and the Agile Manifesto it’s nothing but a collection of suggestions adaptable to different situations and company cultures.</p>
<h3 id="common-rules">Common Rules</h3>
<p>Basic SCRUM rules may be: (they are applicable to every participant)</p>
<ul>
<li>Allow every member in the SCRUM 1 or 2 minutes to answer: What did you do yesterday? What will you do today? Do you have any blockers?</li>
<li>Do not jump into problem-solving situations nor offtrack conversations</li>
<li>Be always on time</li>
<li>Be concise, brief and precise in your information</li>
<li>Take notes when something deserves, in your opinion, further discussion and take it offline with whoever you think opportune</li>
<li>Call out any rule is broken, speak freely and left outside your team role, here everyone is the same</li>
<li>Listen to your colleagues when they’re speaking. Do not bring any device into the meeting unless you need to follow a board with a laptop</li>
<li>Designate a referee or SCRUM master. This can be rotated as agreed every week, every month, every time. This delegate could be the person in charge for the meeting in particular, to take notes, follow up action points or questions and update board when needed. It makes sense the member is familiarised with the boards in particular so there is no time wasted.</li>
</ul>
<h3 id="common-tools">Common Tools</h3>
<p>Tools facilitate our jobs when well used and understood. Make some time to agree in the tools your team is going to use. Some suggestions could be:</p>
<ul>
<li>For spoken communication it’s quite clear we’re using Skype</li>
<li>For written communication it seems like emails get lost quite often and they are hard to follow, create a conversation or include the right members (sometimes are more than needed or less than advised). Avoid emails if there is an alternative, some people get their inboxes flooded with emails from many different origins.</li>
<li>Pick a common channel with both features: live communication such a individual private chat and forum-like nature where a message can be left for the rest of the channel members to read, evaluate and engage in discussions. Slack or Ms Teams do this very well and they allow the creation of different channels, private messages, attachments and text formatting as well as tool linking using add-ons (you could, for instance, link Trello and get notifications of movements in your board directly in a Slack channel instead of your mail)</li>
<li>Pick a tool to follow your project progress that suits your needs.
<ul>
<li>Ad-hoc tasks and support usually don’t fit very well in an Agile methodology, they are more suited for an “eternal” Kanban board where tickets or cards are popping up in the TODO column and they progress across the different status until they’re done.</li>
<li>Continuous development of big projects are very well suitable to be governed by a full blown Agile methodology oriented tool. It is clear Trello is not quite there for these purposes and keeping track of story points, user stories and sprints is almost impossible.</li>
<li>Jira seems to be a good candidate to replace Trello in these cases where sprints and iterations are needed. Jira empowers the project manager to take control of all the backlog, tasks, sprint evolution, status (or columns) and retrospectively allows us look into capacity sprint by sprint.</li>
<li>When using Agile and sprints:
<ul>
<li>Create a general backlog with wish-lists and tasks business members and customers are requesting.</li>
<li>Don’t make them all urgent. When everything is urgent, nothing is urgent.</li>
<li>Create templates for the description of each request. Take the time to think about the user story behind it. Describe them as much as you can, take screenshots, videos, document them as much as possible.</li>
<li>Define your status columns and define what it is meant by DONE.</li>
<li>Schedule a clean-up session every sprint and prioritise what should be allocated into the next sprint.</li>
<li>Schedule a planning session. Bring those weed-out tasks to the sprint backlog. One by one explain their meaning, document them if needed any further and clarify their acceptance criteria. Feel free to use parts of the task_guidelines document defined in the QA framework</li>
<li>Assign resources and story points to tasks</li>
<li>Define length of your sprint. Usually in software development 2 weeks sprint works quite well.</li>
<li>Calculate how many tasks by their story points will fit your sprint. This is usually something that it’s learnt as the team gets several sprints done, then retrospectively looking at the amount of points and how off they were estimated gives you an idea of how much capacity is there in the team</li>
<li>Define a cutoff day and delivery date. After this date, anything is not ready for testing, won’t be in this release.</li>
<li>Define release expectations, what’s this sprint meaning and goals</li>
<li>Use some kind of template to document internally and externally the change-log. Internally helps developers and technical staff to understand changes and technical tasks. External helps business members and customers to understand what’s expected in the new release.</li>
<li>Allow some days for staging / testing state and test throughout each requirement and task included in the release expected when the sprint was defined. Be constructively critical and agnostic, try to find problems, bugs, flaws and issues. Document them as ‘defects’ unless they are new, outside the sprint’s tasks, which in that case are ‘bugs’ (they may be ‘regressions’ too). Feel free to use parts or the totality of the bugs_guidelines template to document them. Tag and index them with colours or codes so they can be classified easily, think if they belong to a particular user story, usually defects raised about a non-compliant sprint task will go side by side or under such task within the same user story. Bugs may be different. Jira allows creating epics, user stories, tasks, sub-tasks, defects, bugs, blockers and different workflows for different project types such Kanban or Agile boards with multiple backlogs and sprints.</li>
<li>Define a retrospective meeting to follow up process, difficulties, what when well, what didn’t go as expected and what can be improved and how. Learn from these meetings and refine next sprints. Keep on reiterating in the process, learning and enhancing it.</li>
</ul>
</li>
</ul>
</li>
</ul>
<h3 id="the-step-by-step-approach">The step by step approach</h3>
<p>Since the communication seems to be the most urgent of the problems to solve within the team, I would suggest the first part to implement should be some kind of regular meetings or SCRUMs where different parts of the team are collaborating together in an open and light discussion.<br>
In a previous meeting, different context of these SCRUMs where identified and enumerated as:</p>
<ul>
<li>SCRUM of team members within the same project and area of expertise.</li>
<li>SCRUM of team members within the same project or not involving teammates independently of their areas of expertise</li>
<li>SCRUM of team members from all the different areas of the business. Special mention to business members who have a global overview, direct contact with customers and the full picture.</li>
</ul>
<h4 id="same-project-and-area-of-expertise">Same project and area of expertise</h4>
<p>These SCRUM sessions are already happening in a way, i.e. MA front end development is bringing together different front end developers in order to understand, every day, where is the project going, its health, find out blockers, communicate effectively of changes, progress and new ideas…<br>
How is it done:</p>
<ul>
<li>Find a time that suits everyone in the team</li>
<li>These sessions need to happen very often, the best way is every day</li>
<li>Find out a way to track your progress, store your wish-lists, backlog, user stories and tasks.</li>
<li>Over the board, each member will explain what was done the day before, what it is planned to do today and briefly mention if there are any blockers</li>
<li>Set the rules of SCRUM / stand up meeting to make it very concise, precise and short:
<ul>
<li>Do not jump out of the three questions (yesterday, today, blockers)</li>
<li>Do not go offtrack the meeting goal</li>
<li>Be always on time for the meeting</li>
<li>Do not bring anything to the meeting, except whatever the mean you have to follow your project’s progress (kanban board, sprint board, white board, sticky notes or spreadsheet in the case)</li>
<li>Do not try to find a solutions. This is not the meeting for that. If there is a discussion that goes sideways, it will be taken offline</li>
<li>Invest 1 or 2 minutes only per member</li>
<li>Speak freely and call out for time excess, offtrack discussions or any broken rule</li>
<li>Everyone in this meeting has the same role. Everyone collaborates to enhance communication as its ultimate goal</li>
</ul>
</li>
</ul>
<h4 id="same-project-or-different-project-but-different-areas-of-expertise">Same project or different project, but different areas of expertise</h4>
<p>Every project requires different areas of expertise. So there is no reason for a front end to exist if there is not a back end and a good set of models in our case make sense of its existence.</p>
<p>The front end will be affected by decisions taken in the back end and vice-versa, so when there is a field that it’s going to change its name in the DTO definition on the back end, such decision should filter beyond the back end limits and get to the front end developers.</p>
<p>Same it is applicable for front end in the other direction. If there is a compromise to make on the structure of the data sent to the server, the back end developers need to have their expectations met for the system to work.</p>
<p>In another level where both the back end and front end are affected is the devOps. If a server has to be configured in a particular way, both the front end and back end may be affected, therefore many times the details of these decisions will make sense to be shared across different layers of the technology stack.</p>
<ul>
<li>Pick a bunch of representative individuals for different projects and different disciplines. Not everyone has to be involved.</li>
<li>This SCRUM / stand up meeting should follow same rules as the previous one, except here the board may be less significant and there may no be a common ground to follow up different layers</li>
<li>This sessions don’t need to happen as often, maybe twice a week such Tuesday and Thursday or Tuesday and Friday. Usually Mondays are very little relevant unless an extraordinary event happened during the weekend.</li>
<li>Feel free to call out an extraordinary meeting to inform about something or post the urgent information somewhere available for everyone. Maybe not everyone has something to share, but they will appreciate you sharing the information from the extraordinary event.</li>
<li>Pick a channel of communication for events, action points and follow ups.
<ul>
<li>Ensure it is streamlined, followed by every stakeholder with interest</li>
<li>Be concise and specific in the information. Avoid technicalities unless talking privately with somebody within your area of expertise. Long discussions or technical diminish the value of the information and wear communication quality.</li>
</ul>
</li>
</ul>
<h4 id="the-all-together">The all-together</h4>
<p>These meetings have a double goal:</p>
<ol>
<li>Communication to flow from the business representatives to the technical team and vice-versa</li>
<li>Steer and define priorities regarding urgency, events, sales, extraordinary events as well as know the health of the different team areas and projects</li>
</ol>
<p>In a way, we are already doing this, however, we tend to jump into solutions and the meeting usually gets long and technical. We should keep it clean and quick, a fast check list over different areas and projects, communicate changes that are relevant in a very quick way and take offline to each area or project the details of such needs, changes or questions.</p>
<ul>
<li>Define a delegate for each project or area</li>
<li>Follow same routine than in previous points: clean, concise, short… 1 or 2 minutes per delegate, quickly move around or write down follow ups and move on so nobody waits for too long unnecessarily.</li>
<li>This meeting may only make sense once a week as we’re already doing</li>
<li>Business delegates should act as a team themselves, bringing their ideas, needs, requests and issues as a checklist altogether without getting into too much detail. When over-steering is needed in a project, team or task, this should be risen, highlighted, mentioned, but taken offline with the project, team or task members in particular.</li>
<li>Use a general overview system of the whole team, define milestones, goals and objectives and move along the progress as indicated. Usually it’s best practice to have a catch up with different teams before this meeting so those needles are already moved to its right positions.</li>
<li>A possible approach:
<ul>
<li>Find a few minutes before this meeting and catch up with different teams or areas, projects of tasks you need to follow up about</li>
<li>Move along project progress</li>
<li>Write down in tasks to follow up blockers and issues that may involve deeper understanding or other team members / areas</li>
<li>Be sceptical about the context of bugs, downtime, errors… write them down and bring them to light in the this multidisciplinary session quickly. Every team or project should take in consideration such pointer and follow up offline scheduling a more technical and deeper meeting offline, if required.</li>
</ul>
</li>
<li>An alternative to the “in-person” pre-meetings: (the idea is to speed up the system and avoid spend more time that necessary on the phone)
<ul>
<li>Formulate a template with questions and progress quadrants for each team / project</li>
<li>Request them before the all-hands meeting, catch up with the members and teams when necessary to clarify points reported</li>
<li>Highlight only items that are relevant for this all-hands meeting</li>
</ul>
</li>
</ul>

