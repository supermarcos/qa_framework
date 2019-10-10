---


---

<h1 id="implementation-plan">IMPLEMENTATION PLAN</h1>
<p>Changing methodologies in a company or team very often means changing culture, acquiring new workflows, habits and ditching others.<br>
This is acceptable and very much is the entire reason of the shift.<br>
By no means changing culture means changing the way the team interact with each other or communicates if such areas are not limping because issues, but more often than not, when the moment and need for Agile implementation comes to a company or team, usually it means some issues have already been surfaced and need to be tackled.</p>
<h1 id="phase-1---communication-as-a-goal">Phase #1 - Communication as a goal</h1>
<p>In our particular case, due our team’s early days and size, it makes a lot of sense to establish the right channels of communication, name the tools and set the workflows.<br>
The absolute end goal of this implementation phase will be the communication.</p>
<h2 id="benefits-of-better-communication">Benefits of better communication</h2>
<p>Improving communication not only means getting information to flow from one side to the other across the team not matter their background or set of tasks, it will also result in a greater sense of team as a group where responsibility is shared and issues are tackled together instead of parcelling them within unrealistic areas of action such backend, frontend, devops, engineering or developing fronts.</p>
<h2 id="challenges">Challenges</h2>
<p>The challenges we are trying to beat are those where a piece of information apparently seems to be under a particular area and, as such, it gets owned by one part of the team that naturally works on said area as their area of expertise.<br>
However, frequently, this a subjective evaluation and the implications as well as the responsibility may be biased.</p>
<p>A server scheduled to be down may look like it’s only devOps responsibility and communication with providers may be good enough to keep it under control. But our servers host APIs, websites, geoServers, modelling tools and even authentication proxies.</p>
<h4 id="real-example">Real example</h4>
<p>In a recent real life event, a set of NCI boxes were scheduled to be migrated from one network to another. This information was given to devOps long before it happened, but such information wasn’t shared to the rest of the team. A preliminary overview would look like the implications were not much important as current customers’ servers in production seemed lightly affected by only a few hours SOMEGAS not being able to be performed, however, the day in question came and adfs server was down, cutting down access to Azure services and impeding deployments, database servers for development of new generations of NCOS were down, front end developers, architects and backend developers were affected.</p>
<p>A better communication would’ve brought the issue to the light and many eyes on it would have started questioning and researching how other stakeholders may have been affected, resulting in a much exhaustive and through-out assessment of the situation.</p>
<p>Issues can’t be brought to zero. They will happen whether there is a brilliant communication workflow in place or not. But having good communication channels will mitigate the effects of them, spread information across and help to share responsibilities by being proactive instead of reactive.</p>
<p>In this line of thoughts, it’s easy to get to the conclusion that better communication will facilitate better decision-making, better assessments of situations and will mitigate the impact that could filter down to our customers.<br>
A poorly assessed situation could result in a server not able to communicate with another and not getting modelling results back to the user interface, completely voiding the service agreement we are bound to and potentially costing customers, and ultimately us, hundreds of thousands of dollars.</p>
<h3 id="share-responsibility">Share responsibility</h3>
<p>Sharing information across the team helps to share responsibility and works in favor of a better work-life balance for everyone, mitigating situations where some members of the team may need to spend hours of frustrating work trying to bring together a critical service in the middle of the night.</p>
<h3 id="documenting-issues-its-also-communication">Documenting issues it’s also communication</h3>
<p>Every issue that happens on our systems, as irrelevant as it may look, should be documented.<br>
The good practice of documenting everything is an art that will pay off great deal the time invested.</p>
<ul>
<li>New members of the team can have an overview of the state of the services and be aware of risks and common issues</li>
<li>An issue is likely to happen again. Documentation will help act in consequence faster and faster, improving the final service given to our customers</li>
<li>Documenting and tagging / indexing issues will help reporting systems to look at the big picture and find out architecture flows, identify bugs, performance issues and assess service quality</li>
<li>Data mining over issue documentation will bring to light hidden expenses, time leaks, workforce lacks and help planning future iterations, sprints and investment</li>
</ul>
<h2 id="tools">Tools</h2>
<ul>
<li><strong>Project boards:</strong> kanban boards seem to be the preferred project representation within the team, however, Trello as we use it, lacks of discipline and hardly ever gives a full introspective analysis of time leaks, effort needs or road blockers we may face. In addition, we are not really iterating nor sprinting at all. We are waterfalling all the way, pushing for a final product instead of partial MVPs fully self contained and deliverable where the customer sees progress and craves for more</li>
<li><strong>Communication broadcasters:</strong> our favourite two ways of communication seem to be email and skype. Both of them lack forum-like approach. Skype won’t store very well conversations you can search across again trying to find a conversation where somebody suggested a good idea now we forgot. Emails pollutes our inboxes with very little meaning, broadcasting information that may not be relevant to the members included and making our days disrupted and rough</li>
<li><strong>Common channels:</strong> our common channels of communication should be forum-oriented. These kind of channels encourage information flow, endorse back-search, don’t pollute nor disrupt normal workflow and they allow users to achieve instant or delayed communication depending on the urgency of such information posted there. Let’s think about tools like Slack or Ms Teams. Different (literally) channels can be created with different topics where the conversations and information posted there has a common denominator. Using the example given before: a channel called NCI incidences or similar would have been the perfect place where this information would have been posted so everyone would have seen it, even if it wasn’t brought to a SCRUM meeting or members owning it are not physically present in the office. Immediately, everyone subscribed to the channel would have been notified about the situation and research would have started in a natural way from different perspectives.</li>
</ul>
<h3 id="a-bit-of-fanciness-about-modern-tools">A bit of fanciness about modern tools</h3>
<p>Most of the modern tools Slack-like (also Teams) allow plugins and apps to be connected, meaning you easily can integrate CD/CI, performance monitors or load-balancers into them.<br>
A new version deployed to the server could post a change log message with a link in a channel and everyone, sales, front and back end, would be immediately aware of it, acting in consequence as needed.<br>
A failed critical model or workflow could be monitored on another channel where performance and issues are tracked. Messages coming across anyone subscribed would help people take control of the situation and save money in rudimentary systems such sms’. These apps are most of them available for free.</p>
<h3 id="agile-by-scrum">Agile by SCRUM</h3>
<p>The ultimate mean of communication is, of course, talking to each other. This doesn’t mean it’s the best mean in the long run (what it’s being spoken out loud can’t be researched afterwards in a month time) nor it’s the most efficient (sometimes getting a notifications is good enough to know something has happened, where getting the same information by somebody telling it on a SCRUM meeting may be irrelevant for some members of the team).</p>
<p>However, SCRUM is the easiest first step towards a fully Agile environment integration.</p>
<ul>
<li>Facilitates a simple channel of communication where everyone is at the same level</li>
<li>A well driven SCRUM shouldn’t be more than a few minutes, say one or two per person</li>
<li>Independently of role, everyone in the SCRUM meeting is a the same level. The SCRUM master it’s a mediator, but not necessarily has a voice in the round. Take it as a referee.</li>
<li>The rules are set, are very clear, and everyone is entitled to invoke them at any necessary point during the SCRUM session</li>
<li>The SCRUM master is a facilitator as well as a referee. Anything that deserves to be talked deeper should be wrote down and followed up offline. This role will take care neither segway conversations nor solution-finding exchange of ideas happen. SCRUM is not the place for that.</li>
<li>The SCRUM master HAS to be always present</li>
<li>The SCRUM session HAS a very restrictive and firm time to start and very well controlled environment. Everyone has to be ready at the moment it is scheduled as the session won’t wait for anyone</li>
<li>Regular SCRUM sessions allow the team getting in a culture of gathering together and sharing information, as well as encourages openness and caring. Everyone, because we are aware of somebody else’s work load, will be more conscious of their needs, limitations, level of stress and will encourage collaboration to achieve common goals</li>
<li>Ideally SCRUM sessions would have also a visible board easy to manipulate that doesn’t generate delays in the fluency of the session itself. If it does, it’s better to ditch the board altogether</li>
<li>After SCRUM is well implemented and a natural part of the team’s culture, implementing new phases of Agile will feel natural such: iterations or sprints, estimations, backlog cleaning sessions, planning sessions, delivery planning, cut-off and deployment days, regular testing, measurable achievements and retrospective sessions where both, managing positions and team mates can evaluate iterations, find out bumps in the workflow and work out solutions testing them over and over again, iterating on the process as the product gets its own iterations</li>
</ul>

