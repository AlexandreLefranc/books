# Preface

> **Tip 1 - Care About Your Craft**

> **Tip 2 - Think! About Your Work**
> - Turn off autopilot



# Chapitre 1 - A Pragmatic Philosophy

## Topic 1 - It's Your Life

Don't stay passive. Be proactive. 

> **Tip 3 - You Have Agency**

## Topic 2 - The Cat Ate My Source Code

- Admit your ignorances or mistakes.
- This way, your team can trust you and you can trust your team
- If you accept a responsability, you are accountable for it
- If things don't go as expected, provide solutions, not excuses

> **Tip 4 - Provide Options, Don't Make Lame Excuses**

## Topic 3 - Software Entropy

- Software Entropy = Software rot = Technical Debt
- Many factors but the most important is the **broken window**
  - Once there is a broken window (bad designs, wrong decisions, poor code), things get worse very quickly
 
> **Tip 5 - Don't Live With Broken Windows**

- Even under pressure, we should not break windows

## Topic 4 - Stone Soup and Boiled Frogs

- Use manipulative techniques to get what you want.
- 'It's easier to ask forgiveness than it is to get permission' Dr. Grace Hopper

> **Tip 6 - Be a Catalyst for Change**

- Projects drift little by little without noticing it
- You might be the manipulated one

> **Tip 7 - Remember the Big Picture**


## Topic 5 - Good-Enough Software

- We cannot produce perfect software
- Good-Enough does not mean sloppy !
- Good-enough for the user, future maintainers and your-self
- User should decide when the software is good enough

> **Tip 8 - Make Quality a Requirements Issue**

- Great software today is often preferable to perfect software tomorrow
- Don't overembellish or overefine your program

## Topic 6 - Your Knowledge Portfolio

- Knowledge assets are expiring over time
- To keep your knowledge portfolio up to date, you have to:
  - Invest regularly: Keep learning
  - Diversify: New technologies, soft skills...
  - Manage risk: Some knowledge might never be in demand, some may become very popular
  - Review and rebalance regularly

> **Tip 9 - Invest Regularly in Your Knowledge Portfolio**

You can learn new language, read technical and non-technical books, read articles, meet others, try different tools.

> **Tip 10 - Critically Analyze What You Read And Hear**

Find root cause, find who does this benefit, consider context and use cases

## Topic 7 - Communicate!

> **Tip 11 - English is Just Another Programming Language**

- Consider the audience to convey your idea as effectively as possible
- Plan what you want to say, and how
- Choose good moment
- Get back to people

> **Tip 12 - It's Both What You Say and Way You Say It**

- Documentation is a kind of communcation. It is in the code.

> **Tip 13 - Build Documentation In, Don't Bolt It On**

# Chapter 2 - A Programtic Approach

## Topic 8 - The Essence of Good Design

> **Tip 14 - Good Design is Easier to Change Than Bad Design**

- ETC principle: Easier To Change
- This is the god principle. All designs are meant to make things easier to change.

## Topic 9 - DRY - The Evils of Duplication

- Do not duplicate **knowledge**, **intent** !

> **Tip 15 - DRY -- Don't Repeat Yourself**

- If a specification change, it should only be changed once in the codebase
- Not all duplication is knowledge duplication. Two different knowledges can have the same rules, so the same code, but this is still 2 knowledge. Ex: 2 fields having the same validation rules.
- Don't duplicate intent in comments where intent is already in code.
- Often, communicating with an API leads to a DRY violation: endpoints, schemas, etc... are defined both in API client and server. This is inevitable but:
  - In case of internal API, you can use shared modules
  - In case of external API, you can use formal documentation (OpenAPI)

> **Tip 16 - Make It Easy to Reuse**

- Another form of DRY violation is knoweldge implemented by two developers independently. You need to communicate and make it easy to reuse by another developer.

## Topic 10 - Orthogonality

- Two or more things are orthogonal is changes in one do not affect any of the others. 

> **Tip 17 - Eliminate Effects Between Unrelated Things**

- Gain productivity: localized changes, reusable
- Reduce risk: problems are isolated
- In code: write shy code, avoid globals, avoid similar functions
- In a orthogonal system, modules should be easy to test

## Topic 11 - Reversibility

- Critical decisions are not easily reversible and for some reason, they will be changed

> **Tip 18 - There Are No Final Decision**

- Databases should be abstracted to make it easy to change
- Hide third-party behind abstraction layers

> **Tip 19 - Stop Following Trends**

## Topic 12 - Tracer Bullets

- Tracer bullet development = development with immediate feedback under actual conditions with a moving goal

> **Tip 20 - Use Tracer Bullets to Find the Target**

- Implement the minimum to make it work
- Implement features when you need it
- Users are involved early, getting feedback
- Integration is incremental, not a big bang (CI)
- You have something to show and be proud of

## Topic 13 - Prototypes and Post-it Notes

- Prototype = disposable, simplified, focused and minimized version of something
- Prototype something risky to avoid to much commitment

> **Tip 21 - Prototype to Learn**

- To Prototype architecture, you can use post it

## Topic 14 - Domain Languages

- Each programming language has characteristics that will influence how you solve problems

> **Tip 22 - Program Close to the Problem Domain**

- Internal Domain Language = domain is described directly with the implementation language (example: Express.js, bash, Vitest)
- External Domain Language = domain is described using a dedicated language (example: OpenAPI, Ansible, Cucumber)
- Recommand to use external language only if domain has to be described by the users

## Topic 15 - Estimating

> **Tip 23 - Estimate to Avoid Surprise**

- Units used gives how accurate is the estimate. ~130 days is more accurate than ~6 months, even though it is equivalent
- To have good estimates:
  - Favor asking someone who has already done it
  - Understand what is being asked, and its scope
  - Modelize, find parameters and express estimates based on these parameters 
- For large estimates, iterate through it

> **Tip 24 - Iterate the Schedule with the Code**


# Chapter 3 - The Basic Tools

## Topic 16 - The Power of Plain Text

- Source code, designs, tests, etc... should be as independent as possible of external tools => plain text does the job

> **Tip 25 - Keep Knowledge in Plain Text**

- Plain text does not mean unstructured (HTML, HTTP, JSON)

## Topic 17 - Shell Games

- GUI is great for productivity
- CLI is great for productivity if you need custom actions not provided in GUI tools

> **Tip 26 - Use the Power of Command Shells**

- Customize your terminal: alias, function, theme

## Topic 18 - Power Editing

- Editing text file should be intuitive, fluent

> **Tip 27 - Achieve Editor Fluency**

## Topic 19 - Version Control

> **Tip 28 - Always Use Version Control**

- Use branches

## Topic 20 - Debugging

- See debugging has problem solving task

> **Tip 29 - Fix the Problem, Not the Blame**

> **Tip 30 - Don't Panic**

- Fix the cause. Don't fix symptoms 
- Get accurate bug report. This might require to watch the user triggering the bug
- Reproduce and isolate the bug in a test

> **Tip 31 - Failing Test Before Fixing Code**

> **Tip 32 - Read the Damn Error Message**

- Use debugger, use print, explain the problem to a rubber duck
- Resist temptation to say too early 3rd-party or system calls have a bug

> **Tip 33 - "select" Isn't Broken**

> **Tip 34 - Don't Assume It - Prove It**

## Topic 21 - Text Manipulation

> **Tip 35 - Learn a Text Manipulation Language**

## Topic 22 - Engineering Daybooks

- Write down things 

# Chapter 4 - Pragmatic Paranoia

> **Tip 36 - You Can't Write Perfect Software**

## Topic 23 - Design by Contract

- Modules should have contracts:
  - preconditions defining what you have to provide
  - postcondition defining what the module does 

> **Tip 37 - Design With Contracts**

- DBC forces you to think 
- If contract is not honored, a common solution is to crash early

## Topic 24 - Dead Programs Tell No Lies

> **Tip 38 - Crash Early**

- Dead program does less damage then a crippled one

## Topic 25 - Assertive Programming

- If you think something will never happen, check it brutally
- Keep assertions in production to find hard to reproduce bug

> **Tip 39 - Use Assertions to Prevent the Impossible**

## Topic 26 - How to Balance Resources

> **Tip 40 - Finish What You Start**

- Function that allocate/open resources should deallocate/close it

> **Tip 41 - Act Locally**

## Topic 27 - Don't Outrun Your Headlights

> **Tip 42 - Take Small Steps -- Always**

- Rely on feedback to be sure you are in the good direction 
- Because you don't know if what you do will still be revelant in the future, make your code replaceable

> **Tip 43 - Avoid Fortune-Telling**


# Chapter 5 - Bend, or Break

## Topic 28 - Decoupling

- You want your software to be flexible

> **Tip 44 - Decoupled Code Is Easier to Change**

> **Tip 45 - Tell, Don't Ask**

- Don't expose implementation. Access et make action through dedicated methods

> **Tip 46 - Don't Chain Method Calls**

- Law of Demeter: method in a class should not know more than other method of that class, its parameters, methods in objects it creates

> **Tip 47 - Avoid Global Data**

- Global Data = variables, singleton, external resources (db, fs, ...)

> **Tip 48 - If It's Important Enough to Be Global, Wrap It in an API**

- Inheritance adds coupling 