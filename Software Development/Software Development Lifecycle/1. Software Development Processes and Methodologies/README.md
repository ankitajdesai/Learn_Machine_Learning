<h1>Week 1: Software development processes : Part 1</h1>



<h2>Introduction</h2>

Why should anybody learn about software development process and methodology? Well, that is the big question. Software Engineering is one of our most complex things that humans have ever done, and that includes all other types of engineering. Civil Engineering is hard. Civil Engineering in software is harder. Think about building the Hoover Dam. It is an incredible thing. It is an incredible amount of work. But if they got half way through building it, and they saw a huge crack in the concrete, they would be able to identify and fix that. And if it was completely done and water were flowing straight through the middle, people would know it is not working. The thing about software is that, it is intangible. We cannot see it, we cannot see when we have made mistakes; and it is hard to see for sure that it is not working right, especially at the grand scale. And just to make it a little bit harder. Anything we do to help us see that it is working right, could be wrong itself. If the program is wrong and the tests are wrong, we do not even know there is a problem. That is what makes following engineering process so important. We have a lot of what I call codified common sense. Of course I would do that. It makes sense, it is almost obvious. But even if you know you should do something, when you are dealing with such a massive endeavor, you could still miss things. Not due to carelessness or negligence but just because it is impossible to keep everything in your cognitive model when dealing with something this complex. And that is why it is so important to learn about the process and follow it. It gives you the roadmap to success. You will not use everything we teach you every time. You may not follow any of the software development life cycles as we present them, ever. What you as a software engineer will do, is take these templates, these plans, these processes, and make engineering decisions necessary to adapt them to your needs, to your project's constraints.

<h3>What software development Looks Like?</h3>

When you're building a software, similar to building a house, you're looking at requirements or you're looking at what exactly you need to build. And during that time, you will do analysis of different options or you might do a prototype and show it to your customer, and just say, "Is this what you're looking for?" But at the end of this phase, you have exactly what you're looking to build. Then comes the architects and the software developers. They're going to design the system, they're going to architect the system, and say, what are the different components that they need to build? And how they're going to work together? Once the design is done, they're going to start coding, and start doing unit testing. So, each of the sub-teams are going to start building their components and test it. Once all the components are ready, they're going to bring all of these components together, and do integration testing or card verification. And, they will do functional testing. And when the software is ready from the developer point of view, then they're going to invite the user, and they will do a testing called, UAT, User Acceptance Testing, in which a user says, "Yup, this is what I was looking for." or "No, this is not what I was looking for." And then, once everything is done, then the software goes into production, which means the user is going to start using, and they might ask for some changes, or you may have to fix some defects, and so on. So, that's called the operation and maintenance. So, as you can see, it's quite similar to building a house. The model that we just reviewed is called, a waterfall method, where you go from phase to phase to phase. Requirements, design, implementation.

As industries started to use this method, they ran into several issues. For example, they found that it's very difficult to predict the requirements one year or two a year ahead, as the market changes, or sometimes it's just really difficult to predict what a user will like or not like. And, since the cycle is a year or two year, it is possible that the developers or the architects misinterpreted the requirements. And so, that misinterpretation will go undetected all the way to design, implementation, and the verification. And similarly, the integration issues between the different components, go undetected for a year while the software is being developed. So, as these issues were coming up, other variants for waterfall started to evolve. Like a V-model, which focuses a lot on testing. Or Sashimi model or RUP model, that focuses a lot on overlapping different phases. And then, the incremental model, where you do the requirements in one shot, but then you do the design testing and deployment in increments. And then, there is the Spiral model, which is a very risk-driven approach.

<img src="../1. Software Development Processes and Methodologies/images/variants_of_waterfall.png">

As all of these variants were coming along, there was another thought process that were evolving in the software industry, called Agile. So, Agile is not a model. It's a mindset. There were a lot of top leaders in software industry, that were building the software very successfully. And so, they came together and said, "What is it that we are doing that is making us successful?" And they articulated what we call now the Agile Manifesto and principles. And, as this manifesto and principles were crafted, there were models like Scrum, and Kanban, and XP, that helped implement this mindset, that promote this mindset. And so, you can see it's not just these three, but many other models came into be. The basic idea behind all of this model, was that instead of building this whole one year cycle, you build in short cycles. So, you define little, you build, you test, and you learn. And then again, you just keep doing this. That way you can adjust to the market quickly. And then, you are learning from your users quickly.

And so, the change became a norm, because after every cycle you may have a change. And, software industry also has to learn how to respond to this change quickly and confidently. And, the idea of continuous integration, where a developer who is building the code, as soon as he commits a code or has soon as he finishes the code, it's integrated with all the other components of that software. And then, all the tests that verifies whether the system is running. They're called, the automated testing. So, as soon as you commit a code, all of the test is tested, to make sure nothing else is broken in the system. And, all of this deployment is automated. So, as soon as the code is committed, it's deployed automatically so that there is no manual errors, as well as it reduces the effort to deploy a code. And not only just these three, many other practices evolved. And so, the safety net of automated testing, and this automation, help developers respond quickly and confidently to the changes. This also led to a new partnership between the developers and the operations. They march towards a common goal. And, that led to a culture of DevOps.


<h2>Requirements</h2>

<h3>Why do we need requirements?</h3>

Well, what is a requirements. Well, it's really two different things. First, it's a process. The process by which we create our shared understanding of both the problem that exists and eventually the needs of our supposed solution which we want to build that will solve that problem. We create high level descriptions of all the concerns we hoped to address by our work with a primary goal of developing a document which can clearly describe the details of what the system will do versus what it won't do. Additionally, it's very important that we capture the what and not the how. We hope to determine what the behavior of the solution will be without making any premature decisions that might affect our ability to design the solution. The design solution will be decided but not at this stage. On the other hand, the requirement specification is also the product of that process. The requirement specification is the documentation that we produce from that process. This can be an informal understanding, it could be a statement of work, it could even be a formal software requirement specification, an SRS document. IEEE is an international organization that has a computer society that has developed a template SRS which we're going to post. You can take a look at what a formal document might look like. There are many reasons why this requirement specification process is important but the most widely cited reasons fall into two categories, engineering and economic. The engineering argument is pretty simple. Spending time up front saves time later. We make fewer mistakes, mistakes which often have far ranging impact. When we spend a significant percentage of our work time line on this planning stage, we do much better. Don't plan anything, your schedule and budget explodes.

<h3>Requirements vs Specification</h3>

There are two ways to document functionality in a software requirement specification document (SRS). The reason there are two ways to write these statements of what the system will do is that there are two audiences for that information. The first audience is the user or the client, depending on whether or not they're the same person. In many cases, the user isn't technical. And so we'd have a very difficult time talking with you about what they want the software to do. They don't know the potential of what they can do. But we still need to provide some sort information that explains what the system will do, so that the user is relatively assured that they get at the end what the client is paid for and it actually does what the user or client wanted them to do. The second audience is the developing team. We also need to provide enough detail to allow the people making the solution, making the code. Know what the system should and shouldn't do. Now, this is where things tend to get tricky. We use natural language, primarily because it allows for an easy communication protocol with our users. Know or very little, technical jargon should hopefully avoid some miscommunications.

User requirements are exactly what the user wants the solution to do in the user’s language. Users do not want to log in though, we want them to. They want the system to be secured to only allow them to say, post to Facebook on their behalf. Logging in is the systems specification. The required action of the system solution were developing. System spec is the usually more precise or constraining statement of how the system will meet the user requirements. This is still with the solution we'll do not how, but it's how the system will meet the requirement. Software design then takes this requirement specification and details that how, which modules be constructed will it be oriented toward design and development. How do we make it happen?

Requirements and Specifications are closely related concepts in defining your solution. Requirements are for the user and Specifications are for the developer. Write your requirements in the user language and write your specifications in the system language. Be sure that your specifications meet the requirements.

<h3>Non-functional Requirements</h3>

Non-functional requirements, requirements which don't specify what the system will do, but rather how the system will perform the behaviors. There many, many non-functional requirements for a system. Many of them revolve around process or quality attributes you're seeking to instill in a project. Process requirements may be things like mandating a particular case system, that is, a computer-assisted software engineering tool like Microsoft Project or Ajira, a bug-tracking software. Or it might have to do with the programming language the team will be using or the development method. These are often design constraints.

Software quality is also something that takes on importance at the very beginning. Security, performance, usability. These are things that every system needs. It can't be completely slow or completely unusable or horribly insecure. Some baseline amount of each of these things is necessary and usually cheap to make happen. But some of these are going to be judged as more important than the others, and a conflict is always there.

Let's take a closer look at three classifications of non-functional requirements. Product, organization and external:
- Product requirements which are non-functional talk about specific behavior. This is often in the form of protocol requirements, encodings, or encryption requirements, that sort of thing. They are requirements on the product itself.

- Organizational requirements are those that are defined by the company. Company standards, your development team's code style requirements, even the development process itself like using SCRAM could be defined as something like this.

- External constraints are a big factor, especially in regulated industries. When the FAA says you have to use this development process or meet these code coverage testing metrics, that's all there is to it. You have to. And if they change, you have to change. This is the kind of control we're talking about, being impacted by external entities. That's something you want to document early on in the process.

<h3>WRSPM</h3>

WRSPM reference model, something we call the world machine model. It's all about capturing the right thing. Requirements are always in the problem domain. It's all about what the user wants to do in order to solve some problem that they have. Our job is then to take those requirements, capture them and then determine what software specifications we need in order to constrain the solution in the solution domain. What we're going to do with our computer, our system in order to solve the problem. And there are several layers of abstraction that exist between, what we call requirements the user's goals and the software specifications, what the system's goals are in order to supposedly meet those user goals or requirements. The WRSPM model is one way of looking at this system in order to determine what the requirements specifications might be. So this is the very formal model in the way of looking at how we separate these. So, you will see here that we have environment and a system. So the environment is all the user visible elements of everything in the world, which includes some part of the system where that overlaps and that overlap is called the interface. So, our system interface is usually a user interface or UI or you may have heard of a GUI, a graphical user interface. That's what we mean by that interface. It's the location of meeting between what the user can do and what the system can do or display to the user in order to capture input and provide output. So, we then have the WRSPM model.

<img src="../1. Software Development Processes and Methodologies/images/wrspm.png">

We have five different elements in this model.
- W is the world. These are all the world assumptions, these are things that we know are true. Now, it doesn't get so complex as to say that gravity works. Of course, that's a world assumption but we are more specific about the world assumptions that have an impact on our system and on our problem domain. There are things that everyone takes for granted and they're one of the more difficult parts to capture.
- R then is the requirements. This is the user's language understanding of what the user wants from the solution. Users, for example, want to withdraw money. That's what they want to do. They go and find an ATM to do that. The ATM is the solution.
- S is the specification. The specification lies in that interface area. It's the interface between how the system will meet those requirements. So it's still written in system language that is from a user or natural language perspective. So it says in natural language, just plain English, what the system will do. So it'll say things like, in order to withdraw money from the ATM you have to insert your card. You have to insert your PIN number. You have to select from checking or savings, you have to enter using a numerical pad, the amount to draw and it has to be in 20 increments for most ATM. Those are all things the user does not care about. The user wants to get money. The specification is how they do that, how the system meets that requirement.
- P then is the program and you'll notice that that's outside of the environment in the system. So all the way over the other side of the line. That program is what the software developers will write, the program that will meet the specifications to provide the user goal for the requirements. The program has all the code, underlying frameworks, anything like that that we would use from a software perspective, which leaves M all the way on the side.
- The M is the machine. It's the hardware specification, so it includes the roller for distributing money, the lockbox to make sure that one of the business requirements is that you don't just walk up and take all the money. It's the hardware behind the system. So you have this world understanding, the requirements which sit within the environment that deal with the user requirements, the specification that defines how the two will meet, the program that meets that specification in order to meet the requirements, and the machine that it all runs on.

Within this then, we care about four variables. EH, EV, SV and SH. EH are the elements of the environment that are hidden from the system. So there very well may be things that we care about outside of the system that we still have to care about. It's the parts of the environment that the user wants. For example, the card. The card that they insert is something that is typically outside of the system. You can't really read the card. What we want to make sure is that the user using the ATM has a card. We prove that by making them insert a card, reading the magnetic stripe and requiring the user to enter their PIN. The EV, the parts that are visible to the system in the environment are the data that generated when you read a mag strip on the card and the entered PIN number. The PIN number exists and is hidden from the system until it's entered in the system. The data that the user enters then is the visible part of the environment in that case. So the pin, once it's entered, would be environment information that's now visible to the system using the interface. The SV is the system elements that are visible in the environment. This includes things like the buttons, the information on the screen, the prompts asking them to enter the card, the prompt asking them to enter their PIN number, the stars that show up when you enter in the values that you end up getting for asterisks so that no one looking over your shoulder can read your pin. Those are all system elements that are visible to the user and you'll see that, again, it sits within that interface intersection. It's something that's in the interface. That all the system data that is hidden from the environment is all the other data and elements of our system. So the roller behind the scenes inside the machinery that the user can't actually see, they can maybe hear it and that may or may not make it visible to the user depending on your definition, but it's typically understood as it's hidden from the user. It's hidden behind the machine, it's hidden in the code, it's hidden in the data in the system. For example, making sure that it gets an approval number from the actual bank before distributing money. That's all hidden from the user, though it does happen and it is important that it happens because the users hope that no one else can get their money.

The WRSPM model is a reference model for how we understand problems in the real world and it helps us to identify the difference between a requirement, the user domain information and the specification. The system domain, how we're going to solve that problem. And you've got to be really careful to separate the two and understand the two because there is a big difference between writing down or capturing the requirements and then making specifications that really do meet those requirements. Just because a system can do it, doesn't mean that it necessarily meets the requirements and having a good understanding of the entire WRSPM model helps you make sure that your specifications do in fact meet the requirements.


<h2>Architecture</h2>

<h3>Software Architecture: Definition</h3>

There's a lot of parallels between software architecture and what most people think of architecture when it comes to building buildings. Architects, no matter which field it is, are that interface between the customer, what they want, and a contractor or the implementer, the person building the thing.

And it's always too across all architecture that bad architectural design can't be rescued by good construction. A bad design can't be fixed when you're building that design, it's unbelievably rare. And there's also parallels in how architects actually work. There are specialist types of projects that require certain architect expertise. If you can imagine it's very different building skyscrapers than it is to build, say, a dam. Or a nuclear reactor or anything else that might need to be architected in a specific way. So, there are specialist types of projects within each field of architect. And in all those fields, schools of thought and styles of architecture have already emerged and continue to emerge as we work through the life cycle of all architectural projects.

Below is three separate definitions, two of them from very popular, well-respected architecture text books that are used in the field. And as well as one from one of the premier international computing bodies, IEEE.

<img src="../1. Software Development Processes and Methodologies/images/software_architecture.png">

In software architecture what we really care about is partitioning large systems into smaller ones. And these smaller systems still individually and independently have business value. And that they can, supposedly, if they're linked properly, be integrated with one another and other existing systems very easily. Now there's a number of reasons why this partitioning is a key component. One of the things that we talk about in terms of software architecture is a decision, for example, buy versus build. You need to decide whether or not the overall project you're going to build should be built by an internal team or you should go out and find an existing product, piece of software off of the Internet, off the shelf. And merely customize it to your specific needs.

Software architectures are about a lot of different things, okay? A big part of it is funding. One of the reasons why we decompose systems into these components that are independent is so that we can talk about parallelization.

<h3>Software Architecture: Models</h3>

So there's a variety of models that have become essentially go-to best practice models for a number of different common problems. So these models are effectively best practiced solutions for commonly occurring problems at the enterprise level, for example:

- __Pipe and Filter__: This pattern can be used to structure systems which produce and process a stream of data. Each processing step is enclosed within a filter component. Data to be processed is passed through pipes. These pipes can be used for buffering or for synchronization purposes.

    Usage:
    - Compilers. The consecutive filters perform lexical analysis, parsing, semantic analysis, and code generation.
    - Workflows in bioinformatics.

<img src="../1. Software Development Processes and Methodologies/images/pipers_and_filter.png">

- __Blackboard__: This pattern is useful for problems for which no deterministic solution strategies are known. The blackboard pattern consists of 3 main components.

    - _blackboard_ — a structured global memory containing objects from the solution space
    - _knowledge source_ — specialized modules with their own representation
    - _control component_ — selects, configures and executes modules.

    All the components have access to the blackboard. Components may produce new data objects that are added to the blackboard. Components look for particular kinds of data on the blackboard, and may find these by pattern matching with the existing knowledge source.

    Usage:
    - Speech recognition.
    - Vehicle identification and tracking.
    - Protein structure identification.
    - Sonar signals interpretation.

<img src="../1. Software Development Processes and Methodologies/images/blackboard.png">


- __Layered__ : This pattern can be used to structure programs that can be decomposed into groups of subtasks, each of which is at a particular level of abstraction. Each layer provides services to the next higher layer.

    The most commonly found 4 layers of a general information system are as follows.
    - _Presentation layer_ (also known as UI layer)
    - _Application layer_ (also known as service layer)
    - _Business logic layer_ (also known as domain layer)
    - _Data access layer_ (also known as persistence layer)

    Usage:
    - General desktop applications.
    - E commerce web applications.

<img src="../1. Software Development Processes and Methodologies/images/layer.png">

- __Client Server__: This pattern consists of two parties; a server and multiple clients. The server component will provide services to multiple client components. Clients request services from the server and the server provides relevant services to those clients. Furthermore, the server continues to listen to client requests.

    Usage:
    - Online applications such as email, document sharing and banking.

<img src="../1. Software Development Processes and Methodologies/images/client_server.png">

- __Event Based__: This pattern primarily deals with events and has 4 major components; _event source_, _event listener_, _channel_ and _event bus_. Sources publish messages to particular channels on an event bus. Listeners subscribe to particular channels. Listeners are notified of messages that are published to a channel to which they have subscribed before.

    Usage:
    - Android development
    - Notification services

<img width="60%" src="../1. Software Development Processes and Methodologies/images/event_based.png">

Below is a summary of the model advantages and disadvantages.

<img src="../1. Software Development Processes and Methodologies/images/model_summary.png">

<h3>Software Architecture: Process</h3>

There's three major concerns when we start talking about design process.

1. __System Structuring__: refers to how the system is decomposed into these several principal subsystems and communications between those subsystems are then identified. We're keying in particularly on things like the interfaces. As soon as we start to decompose or separate elements or components, large scale subsystems of our overall system, we have to start worrying about how they're going to continue to communicate now that we've separated them. This is particularly important when you're going to then parallelize the development work once you split them out giving one component to one development team, another component to another development team and yet more to further development teams. Having that interface as an agreed-upon contract is a very key component to making sure that it all works once it comes back together and the system structuring is part of that.

2. __Control Modeling__:  is how architectures create a model of the control relationships between the different parts of the system that's established. This is particularly true when we have these separate components dealing with the flow of control, not just the interfaces but the flow of control in communicating with each other, but how the software will work once it's running.

3. __Modular decomposition__: is how we identify those subsystem partitions. We are particularly looking at things like simplicity. We're looking for things like maintainability, reliability, security, all those kinds of quality attributes but also, we're worried about things like resource management, who needs to go where and what teams are best suited to handle what kind of responsibilities.

So, when we talk about _subsystem_ versus _modules_, it's important here to note the distinction. Subsystems are still an independent system which could hold business value. It's not our full product but it's still some part of that product that, by itself, has business value and it can run completely independently, or, at the very least, can be developed entirely independently. That's really what we're looking for when it comes to a subsystem and that's the primary goal for architecture. That's versus modules. Module design's what we consider software design. That's a individual component of a subsystem which can't function as a standalone system or a standalone piece of the overall product. It doesn't, by itself, have business value. You have to gather and integrate multiple modules to make up a subsystem.

Another thing we care about at the architectural level is software quality attributes.
- Performance
- Reliability
- Testability
- Security
- Usability

Each of these tends to be something that's associated with architecture. It doesn't mean that it can't be associated with other stages in the process like requirements, design, or even implementation but it's something that we particularly focus on at the architectural stage.

Software architecture process concerns itself primarily with those three things.
- Estimation; estimating the work and total, deciding how much it's going to take, how long it's going to take, who's going to do it.
- Focusing on quality; how do we ensure things like reliability and performance especially at this architectural level since those are primarily hardware and developer-focused concerns.
- And then partitioning; actually dividing the work into subsystems or modules that can then be passed off on to the design stage because then, design stage goes into the actual building of the individual modules.



<h1>Week 2: Software Development Processes: Part 2</h1>



<h2>Design</h2>

<h3>Software Design: Introduction</h3>

In the V-model of software development, design comes into the process at the fourth stage, after architecture and before implementation. It sits between the enterprise level decisions in the subsystem designing and the development effort.

<img src="../1. Software Development Processes and Methodologies/images/v_model.png">

I want to know here that this is not the only way to represent this. In fact, you are going to see architecture and design phases shown here bunched together in various places. The combined stage could be called architectural design or it could even just be called architecture or design alone even though it contains both sets of tasks. We split them so that we can be more specific and provide insight into each of the responsibilities separately.

So, what is software design? Software design is what we call the deliverable, design, the noun, and what we call the process to make that design. Design, the verb, is the creative process of transforming the problem into a solution. In our case, transforming a requirement specification into a detailed description of the software that's code-ready. The noun then is the documented description of that solution and the constraints and explanations used to arrive at it. We develop the software design.

We'll cover architecture separately but as a brief overview, architecture is primarily focused on overarching, cross-cutting concerns for our system especially in the context of the entire enterprise. Large scale decisions like, should we build or buy the software from another company? How is security going to be handled, by the server or by the application? Lots of enterprise and management focused decisions go into this two like apportioning resources and personnel, deciding if the current staff and hardware can handle the project itself, and what is it going to cost to get us there. Securing the internal funding for such endeavors is often looked at as an architectural concern.

<img src="../1. Software Development Processes and Methodologies/images/stages_of_design.png">

The first thing we do is get a good problem understanding when it comes to design. Most of this should come from your requirements and specification documents. If you are unlucky enough not to have these or maybe at least not have them as written documents, it becomes even more important that you get a full grasp of the problem domain before starting to develop your own design solution.

Do not be tunnel-visioned into any large-scale solution as always the only way to go about solving the problem. There is almost always another way to reach the same singular goal, so consider multiple alternatives before deciding definitively which one to pursue. When we say solution abstractions, we essentially mean any documentation of the solution that is not technological. Mostly, that means anything that's not code or hardware. Graphical including mock-ups or wireframes, formal descriptions including unified modeling language or UML diagrams like class diagrams and sequence diagrams, and other descriptive notations should be used to capture your description of the solution that you intend to build or have built for you. What you are going to do is repeat for all abstractions, subsystem components etc. under the entire design and until the entire design is expressed in primitive terms. Now, primitive terms is a bit subjective. What I want you to imagine is this, keep abstracting and designing until you are convinced that you can hand this design off to a developer team that you do not know and you are confident they will come back with a solution that's right. And you do all this without being technology-specific. You let the developers, those coding in C Sharp or Java or Python decide what kind of collection to use at the code level. Let them decide exactly how to sort. Those things are very language-specific and should be left to the developers. Those decisions do not need to be made at the design level. You should still be focused on what makes the overall solution work correctly, leaving all the language-specific optimization to the developer team. They follow your design. They work out the optimizations at the language level.

<img src="../1. Software Development Processes and Methodologies/images/stages_of_design_formal.png">

In architecture and design, we follow these six stages. The first three are architectural. The last three, design. After we decide on a system architecture, separate behavior responsibility into components, and determine how those components will interact through their interfaces, we set out to design the individual components. Each component is designed in isolation, the benefit of encapsulation and reliance on those interfaces we design. Once each component is fully designed in isolation, any data structures which are inherently complex, important, or shared between the classes, or even shared between components, are then designed for efficiency. The same goes for algorithms. When the algorithm is particularly complex, novel, or important to the successful fulfillment of the components' required behavior, you might see software designers rather, than the developers, writing pseudo code to ensure that the algorithm is properly built.

Software design takes abstract requirements and then you build the detail and until you are satisfied that you can hand it off and it will be developed properly. So, you are going to decide things like classes, methods, data types, that kind of thing but not the individual language-specific optimizations that will go into the eventual code. So, you are going to provide detail, which is implementation-ready but it does not include implementation detail.

Software design is all about designing a solution, creating the deliverables and documentation necessary to allow the developing team to build something that meets the needs of the user or the client. The best people to do that is the designing team. This is a crucial step that moves from our natural language understanding to code-ready solutions.

<h3>Software Design: Modularity</h3>

When we talk about modularity, we're primarily talking about these four things:

1. __Coupling__: is the degree of interdependence between software modules; a measure of how closely connected two routines or modules are; the strength of the relationships between modules.

2. __Cohesion__: refers to the degree to which the elements inside a module belong together. In one sense, it is a measure of the strength of relationship between the methods and data of a class and some unifying purpose or concept served by that class. In another sense, it is a measure of the strength of relationship between the class's methods and data themselves. Coupling, cohesion are measures of how well modules work together and how well each individual module meets a certain single well-defined task and they tend to go together.

3. __Information Hiding__: describes our ability to abstract away information and knowledge in a way that allows us to complete complex work in parallel without having to know all the implementation details concerning how the task will be completed eventually.

4. __Data Encapsulation__: refers to the idea that we can contain constructs and concepts within a module, allowing us to much more easily understand and manipulate the concept when we're looking at it in relative isolation.

Software development is complex, attempting to hold the entire concept of a large scale program in your mind all at once is a fool's errand. We have no choice but to break the problem down into smaller parts. Which we might then be able to comprehend. To do that properly, we're going to focus on three concepts or aspects of modularity:

1. _Decomposability_: Essentially it's the ancient possibly Roman concept of divide and conquer. When the problem is too large and complex to get a proper handle on it, breaking it down into smaller parts until you can solve the smaller part is the way to go. Then you just solve all the smaller parts.

2. _Composability_: But then we have to put all those smaller parts back together and that's where composability comes into play. This is often not as simple as one would like.

3. _Ease of Understanding_: So we try to focus on ease of understanding by breaking down the components we hope to provide an ease of understanding, which will then hopefully lead to an ease of communication.

When it comes to _information hiding_, all we want is the ability to use something by understanding what it does but not necessarily how. This tends to work well until the understanding of what it does is strained. Take Rand. What does the function rand do? You might answer that it provides you with a random number but that's not quite right. For most purposes, it generates a random enough value for most uses, but in reality, rand is a pseudo random number generator. It's based off of a seeded value and isn't exactly random. So when you need true randomness, it doesn't quite fit the bill but it does work in many typical situations where true randomness isn't quite necessary.

Because of _data encapsulation_, protecting the data from unauthorized access and maintaining integrity is a key point. The developer of a module has the best idea of how and when the attributes should be modified, and then we try to allow them to maintain as much control as is possible. Nobody else is allowed to mess with that data. If it gets corrupted, it must have been done by the module, that's the intent. And data encapsulation makes designs more robust, by robust here, I mean that chances are that new additions aren't going to break the current design.

So when we talk about modularity, we're really talking about breaking down and reassembling all these components. So when it comes to _coupling, cohesion, information hiding,_ and _data encapsulation_, they are just qualities, different perspectives on what modularity really means.

<h3>Software Design: Coupling</h3>

__Measuring the strength of connection between sub system components:__

One of the key ideas of modularity is 'decomposability', separating complexity. One way we can control the change on a design is to enforce the separation. When the requirements are changed, may be half way through our process, we don't want that change to have massive impact across entirety of our system.

__Loose coupling allow for changes to be unlikely to propagate across components:__

By enforcing low coupling, what we're hoping to accomplish is that changes don't cross the boundaries of our modules. Ideally, when a requirement changes, and it will, the changes in our code should be contained within a single module, the module tasked with completing that function that's changed. When you produce effective low coupling, changes in one module shouldn't affect the other modules, or should do so as minimally as possible. That's our goal. We accomplish that goal by being attentive to the kinds of coupling we are using between our modules.

__Shared variables and control information lead to tight coupling:__

Even though the mantra is low coupling, high cohesion, we talk about the levels of coupling in terms of loose and tight coupling. Those terms make more sense in isolation. The worst, strongest, highest, forms of coupling are listed below.

Tight Coupling:

- _Content coupling_: happens when module _a_ directly relies on the local data members of module _b_, rather than relying on some access or a method.

- _Common coupling_: happens when module _a_ and module _b_ both rely on some global data, or global variable.

- _External coupling_: is a reliance on an externally imposed format, protocol, or interface. In some cases, this can't be avoided. But it does represent tight coupling, which means that changes here could affect a large number of modules, which is probably not ideal.

Medium Coupling:

- _Control coupling_: happens when a module can control the logical flow of another by passing in information on what to do or the order in which to do it, a what to do flag. Changing the process may then necessitate changes to any module which control that part of the process. That's not necessarily good.

- _Data structure_ coupling: occurs when two modules rely on the same composite data structure, especially if the parts the modules rely on are distinct. Changing the data structure could adversely affect the other module even when the parts of the data structure that were changed aren't necessarily those that were relied on by that other module.

__Loose coupling achieved by state decentralization and message passing:__

Loose Coupling:

- _Data couplings_:  is when only parameters are shared. These includes elementary pieces of data like when you pass an integer to a function to compute the square root.

- _Message coupling_: is then the loosest type of coupling. It's primarily achieved through state decentralization and component communications, only accomplished either through parameters or message passing.

- _No coupling_: this is usually the trivial case and isn't really of that much interest to us.

<h3>Software Design: Cohesion</h3>

__Measures how well a module's components fit together:__

__Implements a single logical entity or function:__

__Represents a desirable design attribute:__

__Divides into various levels of strength:__

Cohesion is really how well everything within a module fits together, how it works towards a singular purpose. Now this is pretty subjective, in that the context in which you consider the singular purpose makes a big difference. For example, imagine you're building a game as a mobile application. Technically, everything you do is cohesive to the idea that you are building a game. Every line of code works towards that singular goal, from advertising to user accounts to micro-transactions to the game and the graphics themselves. But that's a very high level categorization. That's why we typically refer to cohesion using various levels of cohesion to better define what we mean when we say cohesion. So let's start with the weakest forms of cohesion.

Weakest Cohesion:

- _Coincidental cohesion_: is effectively the idea that parts of the module are together just because they are, they are in the same file. If you just throw all the code into one file, technically it's cohesive in that it resides in the exact same file location. It's in the same class, for example, in object-oriented programming. But this is ultimately very, very weak cohesion. Its proximity to other code is the only relationship between it and the other. That's not good.

- _Temporal cohesion_: means that the code is activated at the same time, but that's it. That's really the only connection. Being in a module because you're both called at the start isn't a very OO way of looking at the solution.

- _Procedural cohesion_: is similarly time based and not very strong cohesion. Just because one comes after the other doesn't really tie them together, not necessarily. What if the process flow changes? Again, that's not good. They don't necessarily need to be cohesive in that way.

- _Logical association_: is the idea that components which perform similar functions are grouped. We're getting less weak, but it's still not good enough. The idea here is that at some level the components do similar, but separate or parallel things. That's not a good reason to combine them in a module. They are considered separate, though similar, for a reason. And so we should separate them.

Medium Cohesion:

- _Communicational cohesion_: means that all elements of the component operate on the same input or produce the same output. This is more than just doing a similar function. It's producing identical types of output or working from a singular input.

- _Sequential cohesion_: is the stronger form of procedural cohesion. Instead of merely following the other in time, sequential cohesion is achieved when one part of the component is the input to another part of the component. It's a direct handoff and a cohesive identity.

Strong Cohesion:

- _Object cohesion_: In object cohesion, we see that each operation in a module is provided to allow the object attributes to be modified or inspected. Every single operation in the module. Each part is specifically designed for purpose within the object itself, that's that object cohesion.

- _Functional cohesion_: goes above and beyond sequential cohesion to assure that every part of the component is necessary for a well-defined function or behavior. So it's not just input to output, it's everything together is functionally cohesive.

I also want to make this note. Technically speaking, inheritance weakens cohesion. The idea is being able to have the full understanding of a concept in a single module. When you inherit, you by design don't have all the concepts in a single module when you're viewing the code base. You have to go look at the super class files as well. That does make it harder to find detail and goes against the principle of high cohesion. However, that is usually a very easy tradeoff, given the benefits available to us using inheritance.


<h2>Implementation</h2>



<h2>Testing and Verification</h2>





<h1>Week 3: Software Development Models: Traditional Models</h1>









<h1>Week 4: Software Development Models: Agile and Lean</h1>