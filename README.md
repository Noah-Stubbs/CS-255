# CS-255


Briefly summarize the DriverPass project. Who was the client? What type of system did they want you to design?
  
  The DriverPass project was designing a system for a client to offer driver's education, including both online and in-person resources. This platform allows anyone with a modern browser and internet connection to schedule driving lessons with an instructor and/or take practice exams derived from current DMV regulation. 



What did you do particularly well?

  I believe I stood out most in my diagrams. I noticed many students submitted plain black-and-white versions that were harder to follow. I found myself getting lost in a "sea of white", while my diagrams used color for both organization and visual clarity. I also went beyond the minimum BRD requirements by including sections tailored to different audiences—for example, a BLUF at the beginning for quick context, a five-paragraph order for veterans, and quick index's for specifics like the role-based index view, system behavior quick reference, and regulatory cross-reference table.


  
If you could choose one part of your work on these documents to revise, what would you pick? How would you improve it?
 
  If I had additional time for revisions, and had to fix something already in place, I would reevaluate the actors in the system. In my BRD, I had IT and Admin as separate classes. In the System Design Document, IT was just absorbed by Admin. I don't think either method is inherently bad, the permissions for both user roles could be booleans under one class, or IT could be a sub-class of Admin so they have Admin permissions and the additional IT. I don't think that specific is critical, but it does feel like a piece of the puzzle that I haven't figured out in which way it fits yet. 
  If I could not change existing sections, I’d add something. Specifically, I’d include a simple UI sketch to help contextualize the system. While the BRD and diagrams define structure and logic well, a rough homepage mockup would provide a visual anchor. This would help others follow along without needing strong abstract thinking skills. Even for me, who first vividly visualizes everything in my head, a simple sketch serves as a massive head start. 


  
How did you interpret the user’s needs and implement them into your system design? Why is it so important to consider the user’s needs when designing?
  
  An easy trap in software design is forcing a fancy technology or method into the project just for the sake of using it, in short; creating a solution in search of a problem. I avoided this by starting with the initial interview, identifying clear constraints, and asking myself: “If I were the user trying to [task], what’s the best way to do that without breaking any rules?”
  Considering the user’s needs is essential because they are the system’s reason for existing. You can build the fastest, cleanest, easiest-to-maintain system imaginable, but if users find it too complicated or confusing, they won’t use it. For DriverPass, that would mean no customers. In other settings, it might mean the client hires a different development team.


  
How do you approach designing software? What techniques or strategies would you use in the future to analyze and design a system?
 
  I design software by focusing on the core problem it’s meant to solve. I start with the broad concept, then gradually peel layers back, deconstructing each step before going deeper. I don’t usually go all the way to function-level design in the beginning. Instead, I like to identify the core functions or modules the system will need. For school projects, that means starting with a driver class and creating placeholder methods. These usually just print statements showing what would happen. Once the logic flow feels right, I start filling in the actual functionality. Outside of class, I mostly write procedural code. I follow the same structure: scaffold the logic with placeholder prints, then convert prints into full functions once I’m confident in the structure. In the future, I plan to use more iterative development and more diagrams from the start. I’ve seen this naturally evolve in my greenhouse and Pod Racer projects. Originally, both had centralized head units making the high-level decisions and sending the commands to microcontrollers to accomplish the task with precision. That worked for the Pod Racer, and I don't expect it to change. However, for the greenhouse, I’m now considering the same head unit but running a CAN BUS. In this rough draft, the head unit was running one small driving loop with one update(); function. What happened when that function executed depends on what class object it's performing the action on, meaning I created a more OOP design. Iterative development and diagrams, even the "quick and dirty" drafts, are essential. The best solution rarely shows up on day one, and clear visuals help guide and improve the process.
