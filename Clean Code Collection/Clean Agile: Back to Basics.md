 # Clean Agile

Book by Robert CeC.cil Martin
- [Chapter 1: Introduction to Agile](#chapter-1-introduction-to-agile)
- [Chapter 2: The Reasons For Agile](#chapter-2-the-reasons-for-agile)
- [Chapter 3: Business Practices](#chapter-3-business-practices)
- [Chapter 4: Team Practices](#chapter-4-team-practices)
- [Chapter 5: Technical Practices](#chapter-5-technical-practices)
- [Chapter 6: Becoming Agile](#chapter-6-becoming-agile)
- [Chapter 7: Craftsmanship](#chapter-7-craftsmanship)


## Chapter 1: Introduction to Agile
###  The Agile Manifesto
- Written in February 2001 in Utah by 17 software experts.
- The Preamble of the Agile Manifesto: 
	-  We are uncovering better ways of developing software by doing it and helping others do it.
- The Agile Manifesto:
	- **Individuals and interactions** over processes and tools.
	- **Working software** over comprehensive documentation.
	- **Customer collaboration** over contract negotiation.
	- **Responding to change** over following a plan.

### The Iron Cross
- All projects to obey an unassailable trade-off.
- Good, fast, cheap, done - pick any three you like, you will **not** have the fourth.
- A good manager drives a project to be good enough, fast enough, cheap enough, and done as much as necessary. 
- They do this by making changes to the scope, the schedule, the staff, and the quality:
	1. **Changing Schedule:**
		- The _Date_ is the very first thing everyone knows about a project.
		- Usually, the date was chosen for good business reasons, and those reasons will hold in future. Hence, a delay often means that the business is going to take a significant hit of some kind.
		- Any delay should be communicated as early as possible so any consequences can be avoided.
	2. **Adding Staff:**
		- Adding new staff decreases the productivity of the team before it, hopefully, increases it.
		- The new staff consumes the time and energy of the old staff at the beginning to get familiar with the project.
		- Brooks' law: _Adding manpower to a late project makes it later._ You need enough time and improvement to compensate for the initial loss.
		- Adding staff is expensive, and more often the project budget will not allow it.
	3. **Decreasing Quality:**
		- The only way to go fast, is to go well.
		- No such thing as quick and dirty. Only slow and dirty.
		- If we want to shorten our schedule, the only option is to _increase_ quality.
	4. **Changing Scope:**
		- Some features can be postponed beyond the arranged deadline.
		- Business people will argue to have it all done, and by the deadline. Yet, the programmers have the data. Data always win.
		- if the organization is rational, then the stakeholders eventually bow their heads in acceptance and begin to scrutinize the plan.

### Circle Of Life
TODO: image 
- The outer ring shows the business-facing practices of XP - equivalent to the scrum process.
- The middle ring presents the team-facing practices.
- The innermost ring represents the technical practices - to ensure the highest quality.


## Chapter 2: The Reasons For Agile

### 1. Professionalism
- Why software developers must become more professional?
	1.  Software is everywhere, even where you don’t notice.
	2. Software developers’ work is most prolific, and thus intentionally or unintentionally, we are accountable for a lot of the world around us.
	3.  Given that we are responsible for so much software around us, one day, we may cause a huge disaster that may cause the governments to regulate the entire industry.

### 2. Reasonable Expectations
- Meeting expectations is one of the primary goals of Agile development
- Managers, customers and users should _reasonably_ be able to expect:
	1. **We will not ship shyt:**
		- Provide systems that are high in quality and low in defect.
		- No system should require its users to think like programmers to be able to use it.
		- Agile assures this through Testing, Refactoring, Simple design and Customer feedback.
	2. **Continuous Technical Readiness:**
		- The system should be ready to be _technically_ deployed at the end of every iteration.
		- The actual deployment is a business decision.
	3. **Stable Productivity:**
		- Productivity should be stable over time and software teams are not expected to slow down with time.
		- This is done by continuously keeping the architecture, design and code as clean as possible.
		- Agile supports that through practices of Testing, Pairing, Refactoring, and Simple Design.
	4. **Inexpensive Adaptability**
		- Software - "ware" means product, "soft" means easy to change.
		- Requirements can change often, and this should **not** break the software architecture.
		- Accommodating the change requirements should be relatively inexpensive.
		- Agile practices of TDD, Refactoring, and simple design help in this.
	5. **Continuous Improvement**
		- The most irresponsible attitude is to expect systems to get messier, more brittle and more fragile with time.
		- Steady improvement should be expected and early problems should fade away over time.
	6. **Fearless Competence**
		- It is expected to be competent and confident enough to make any necessary changes in the software to keep it cleaner and clearer.
		- The Agile practice of TDD builds that discipline.
	7. **QA Should Find Nothing**
		- QA job should not be to list issues found in the system. Rather their job should be to say, “Everything looks ok to release.”
		- QA have better places to be positioned than at the back end of the process.
		- This is supported by the Agile practices of Acceptance Tests, TDD, and Continuous Integrations.
	8. **Test Automation**
		- Manual tests are expensive and so are always a target for reduction.
		- Repeatable tests must be automated. 
		- Manual QA should do something that involves human creativity and imagination.
		- No tests should be bypassed because the team ran out of time or money.
	9. **We cover for each other**
		- The team should support each other and step in anytime.
		- The team is not expected to keep knowledge in silos, the knowledge should be shared.
		- The Agile practices of Pair Programming, Whole Team, and Collective Ownership supports these expectations.
	10. **Honest Estimates**
		- “I don’t know” is a much better estimate than “I will try” or estimates based on gut feeling.
		- The Agile practices of the Planning Game and Whole Team supports this expectation.
	11. **You Need to say "NO"**
		- It is important to strive to find solutions to problems, but it is more important to say no when there are no solutions.
	12. **Continuous Aggressive Learning**
		- Learn Learn Learn
		- The industry changes quickly and the developer must be able to change with it.
	13. **Mentoring**
		- Teach to learn and learn to teach

### 3. The Bill of Rights
- There are customer bill of rights and Developer bill of rights. 
- Both are complementary. They create a balance of expectations between the two groups.

## Chapter 3: Business Practices

### 1. Iteration Activities
- This practice tells you how to organize your high-level business requirement into granular features, stories and tasks. 
- It helps you prioritize, estimate, and plan.
- It is crucial to spend a small amount of time choosing the smallest range that remains accurate.
- This deals with accuracy and precision by using a very tight feedback loop that iteratively calibrates and recalibrates estimates against reality.
	- Precision - How close the actual result is to the estimation.
	- Accuracy - Is the estimation true or not?
- **Common Techniques**:
	1. **Trivariate Analysis** three numbers representing confidence
		- The _worst case_ is the amount of time within which you feel **95%** confident the task will be completed
		- The _nominal case_ is the amount of time within which you feel **50%** confident the task will be completed
		- The _best case_ is the amount of time within which you feel **5%** confident the task will be completed
	2. **User Story**
		- is an abbreviated description of a feature of the system, told from the point of view of a user. 
		- Specifications of those details are delayed as long as possible, right up to the point where the story is developed.
		- The temporary lack of details is what makes a story manageable, schedulable and estimable.
		- Stories follow a simple set of guidelines that we remember with the acronym **_INVEST_**.
			-- **Independent**: user stories are independent of each other - this is a soft requirement. 
			-- **Negotiable**: details to be negotiable between developers and the business.
			-- **Valuable**: the story must have clear and quantifiable value to the business. - Refactoring/Architecture/Code cleanup are not stories
			-- **Estimable**: a story must be concrete enough to allow the developers to estimate it.
			-- **Small**: a story should not last more than an iteration.
			-- **Testable**: the business should be able to articulate tests that will prove that the story has been completed.
		-  Estimating stories is done in various ways, but the most popular ones are:
			-- Flying fingers: developers assign points using their fingers all at once. If there is no obvious average they can debate.
			-- Shirt size: small, medium, large
			-- Planning poker: choose points from a deck of value (Fibonacci is often used: ? [don't know] , 0, ½, 1, 2, 3, 5, 8, 13, 20, 40, 100, and ∞ [too much] )
	3. **Story Points**
		- Are a unit of estimated effort, not real time. 
		- They are not even estimated time - they are estimated effort.
	4. **Iteration Planning Meeting (IPM)**
		- Where stories to be implemented in this iteration are decided.
		- Stories are decided based on the number of story points that can be allocated to the team in an iteration -_Velocity_.
		- Should be one-twentieth the duration of the iteration
	5. **Four-Quadrant Game (The Highest Return of Investment)**
		- Stories that are valuable but cheap will be done right away. 
		- Those that are valuable but expensive will be done later. 
		- Those that are neither valuable nor expensive might get done one day. 
		- Those that are not valuable but are expensive will never be done.
	6. **Midpoint Check**
		- The team gathers with stakeholders and they look at the progress.
		- The main purpose of an iteration is to generate data for managers.
	7. **The Demo**
		- The iteration ends with a brief demonstration of the new stories to the stakeholders.
		- 1 or 2 hours long.
		- All acceptance tests and unit tests (including old ones).
		- Show off the newly added features.
		- Let the stakeholders themselves operate the system.
		- The project is over when there are no more stories in the deck worth implementing.
	8. **Yesterday's weather**
		- The best predictor of today's weather is yesterday's weather 
		- The best predictor of the progress of an iteration is the previous iteration.
	9. **Velocity**
		- The last act of the iteration is to update the velocity and burn-down charts.
			- Velocity: how much the development team has gotten done every week.
			- Burn-down chart:  how many points remain until the next major milestone.
		- Velocity is a measurement, not an objective - do not put pressure on the thing you are measuring
		- After a few iterations the slope should be expected to become zero, otherwise:
			- A **rising velocity** 
				-- probably means that the project manager is putting pressure on the team to go faster 
				-- As the pressure builds, the team will unconsciously shift the value of their estimates to make it appear that they are going faster
				-- Inflation happens.
			- A **falling velocity**
				-- the most common cause is the quality of the code
				-- As velocity falls, pressure builds on the team, This causes the points to inflate. That inflation can hide the falling velocity.
		- The Golden Story: is comparing estimates to an original story to see if inflation is occurring.

### 2. Small Releases
- This practice suggests that a development team should release their software as often as possible.
- The new goal is _Continuous Delivery_ - the practice of releasing the code to production after every change.
- The term “release” means that the software is technically ready to be deployed.

### 3. Acceptance Tests
- This practice says that, to the degree practicable, the requirements of the system should be written as automated tests
- **Behaviour Driven Development (BDD)**: the goal is to remove the techie jargon from the tests and make the tests appear more like specifications that businesspeople would appreciate.
-  Business people can give formal and precise requirements translatable to tests by specifying: _Given, When,_ and _Then_
- Business Analysts specify the happy paths
- QA specify the unhappy paths, they need to have the ability to figure out how to break the system.
- The developers integrate those tests into the continuous build - to run them every time any programmer checks in a module.
- Definition of _done_ 
	- establishes the criteria for when a task or feature is considered complete and ensures that everyone on the team is working towards the same goal
	- Usually, it is "acceptance tests pass".
- This is not about going fast. This is about making concrete, measurable progress. This is about reliable data.
- It is far better to get 80% of the stories done than it is to get each story 80% done. Focus on driving the stories to completion.

### 4. Whole Team
- The practice of Whole Team was initially called _On-Site Customer_.
- Believed that the shorter the distance between the users and the programmers, the better the communication, and the faster and more accurate the development.
- When teams are co-located, the business runs much more smoothly.

## Chapter 4: Team Practices

### 1. Metaphor
- Use a language that everyone understands and is familiar to technical people and business stakeholders.
- This allows the team to communicate effectively.

### 2. Sustainable Pace
- You must run at a Sustainable Pace. 
- A software project is not a marathon, not a sprint, or a sequence of sprints.
- It is your job to husband your resources to ensure that you endure the end.
- Working overtime is not a way to show your dedication to your employer. What it shows is that you are a bad planner, that you agree to deadlines to which you shouldn't agree, that you make promises you shouldn't make, and that you are a manipulable laborer and not a professional. - This is not to say that all overtime is bad.
- The most precious ingredient in the life of a programmer is sufficient sleep. Make sure you know how many hours of sleep your body needs and then prioritize those hours. Those hours will more than pay themselves back.

### 3. Collective Ownership
- No one owns the code in an Agile project. The code is owned by the team as a whole.
- As you specialize, you must generalize. -Maintain your ability to work outside of your speciality.

### 4. Continuous Integration
- For ensuring that code is tested and delivered quickly and reliably.
- The continuous build should _never_ break.
- Fail fast, and get feedback faster on where you stand all the time.

### 5. Standup Meetings
- This meeting is optional. Many teams get by just fine without one.
- It can be less often than daily. Pick the schedule that makes sense to you.
- It should take ~10 minutes, even for large teams.
- This meeting follows a simple formula.
- The basic idea is that the team members stand in a circle and answer 3 questions:
	1. What did I do since the last meeting?
	2. What will I do until the next meeting?
	3. What is in my way?
	4. [Optional] Whom do you want to thank?
- No discussion. No Posturing. No deep explanations. No complaints. Everybody gets 30 seconds to answer those 3 questions.

## Chapter 5: Technical Practices
- Technical excellence is critical for creating clean, maintainable, and scalable code. 
- Technical debt is the result of poor technical practices and shortcuts that are taken during software development. It accumulates over time and can lead to significant problems, including slower development times, increased bugs, and higher maintenance costs.

### 1. Test-Driven Development
- This practice involves writing tests before writing code. 
- TDD ensures that code is tested thoroughly and helps to
- The tests are a form of documentation that describe the system being tested
- Every required behavior should be entered twice: once as a test, and then again as production code that makes the test pass.
- Three rules:
	1.  Do not write any production code until you have first written a test that fails due to the lack of that code.
	2.  Do not write more of a test that is sufficient to fail - and failing to compile counts as a failure.
	3.  Do not write more production code that is sufficient to pass the currently failing test.
- The main aim of a test suite of automated tests is to tell us that it is safe to deploy. It also eliminates the fear of changing the code.
- Test coverage is a team metric, not a management metric.

### 2. Refactoring
- This is the process of improving the design of existing code without changing its behavior. 
- It is essential for maintaining clean and scalable code.
- The Red/Green/Refactor cycle:
	1.  We create a test that fails.
	2.  Then we make the test pass.
	3.  Then we clean up the code.
	4.  Return to step 1.
- Writing code that works is different from writing code that is clean.
- We do not reserve time for refactoring. Refactoring is simply part of our minute-by-minute, hour-by-hour approach to writing software.

### 3. Simple Design
- The practice of writing only the code that is required with a structure that keeps it simplest, smallest, and the most expressive.
- Rules of Simple Design: 
	1.  Pass all the tests.
	2.  Reveal the intent - It should be easy to read and self-descriptive.
	3.  Remove duplication.
	4.  Decrease elements - reduce the number of structural elements, such as classes, functions, and variables.
- **Design weight:** is the cognitive load placed on the programmers based on how complex the system design is. The greater the weight of that design, the more time and effort are required for the programmers to understand and manipulate the system.

### 4. Pair Programming
- This is an effective technical practice for sharing knowledge and promoting collaboration among team members.
- It reduces errors and improves design quality.
- Never, ever, ever, ask for permission to pair. Or test. Or refactor. Or... You are the expert. You decide.

## Chapter 6: Becoming Agile
- Becoming Agile requires a cultural shift within the organization. Leaders must be committed to creating a culture of collaboration, communication, and continuous improvement.
- Agile adoption requires a shift in mindset from traditional command-and-control management to servant leadership.

### Agile Values
1. **Courage** - a reasonable degree of risk-taking.
2. **Communication** - value direct and frequent communication that crosses channels. Face-to-face, informal, interpersonal conversations.
3. **Feedback** - Maximize the frequency and quantity of feedback. They determine when things are going wrong early enough to correct them and provide massive education about the consequences of earlier decisions.
4. **Simplicity** - being direct. Passive aggression is indirection. Keep the code simple. Keep the team simpler.

### Coaching
- The coach is not a manager and not a trainer
- The coach acts as the team's conscience, always reminding the team of the promises they made to themselves and the values they agreed to hold. 
- Agile coaches are members of the team whose role is to define the process within the team.
- In Scrum, the coach is called a Scrum Master.
- Every member of an Agile team needs to understand the values and techniques of Agile. Therefore, if one member of the team is trained, all members of the team should be trained.

### Agile Tools
- Teams should establish a pattern of work compatible with their specific context first, and then consider using tools that support their workflow. 
- Define some great aids from software to physical tools.
- Workers use and control tools, tools don't control and use people. 
- Definition of a great tool: 
	- Help people accomplish their objectives
	- Can be learned "well enough" quickly
	- Become transparent to users
	- Allow adaptation and exaptation
	- Are affordable
-  Metrics are essential for measuring progress and identifying areas for improvement. Organizations should track metrics such as team velocity, cycle time, and lead time to monitor the effectiveness of their Agile practices.

#### ALM 
- Agile Lifecycle Management systems
- A software system for managing agile projects.
- Despite being feature-rich and commercially successful, ALM tools utterly fail at being great because:
	- Tends to be complicated, usually demanding up-front training
	- Often requires constant attention
	- Aren't always easily adapted.
	- Usually expensive.
	- Rarely works the way your team does, and often their default mode is at odds with Agile methods.
## Chapter 7: Craftsmanship
- Software development is a craft, and software developers are craftsmen. 
- Craftsmanship is a mindset that involves taking pride in one's work, striving for excellence, and continuously improving one's skills.
- Most companies are still not mature enough to understand that technical problems are in fact business problems.
- Focus on the value, not the practice - Agree first on the goals to be achieved when discussing practices.
- The discussion around practices should be done at the right level and with the right people
- Conversations between developers and businesses should be about why, what and when - not how.
- _Agile_ communities have an emphasis on the people and the process side of the software projects. While _craftsmanship_ communities focus more on the technical side.
- Craftsmanship promotes software development as a profession. 
	- A profession is part of who we are. A job is a thing that we do but is not part of who we are. A profession is something we invest in. It is something we want to get better at. We want to gain more skills and have a long-lasting and fulfilling career.

#### Software Craftsmanship
- As aspiring Software Craftsmen, we are raising the bar for professional software development by practicing it and helping others learn the craft. Through this work we have come to value:
	-   Not only working software, but also well-crafted software.
	-   Not only responding to change, but also steadily adding value.
	-   Not only individuals and interactions, but also a community of professionals.
	-   Not only customer collaboration, but also productive partnership.

- The Software Craftsmanship manifesto describes an ideology, a mindset. It promotes professionalism through different perspectives.
	- **Well-crafted software**  - code that is well-designed and well-tested. It is code that is both flexible and robust.
	- **Steadily adding value**  - no matter what we do, we should always be committed to continuously providing increasing value to our clients and employees.
	- A **community of professionals**  -  expected to share and learn with each other, raising the bar of our industry. We are responsible for preparing the next generation of developers.
	- **Productive partnership**  - we will have a professional relationship with our clients and employers, behaving ethically and respectfully, advising and working with clients and employers in the best way possible, expecting a relationship of mutual respect and professionalism.