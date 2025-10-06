### Group Design Activity: Modeling a Real-Time Notification System for a Community Event App

*Activity Overview*  
In this 2-hour in-class group activity, you'll work in teams of 3 to model and design a simple software system. This builds on last week's lesson where we explored what modeling is and how design patterns (like Singleton) solve real problems—remember how we researched Prisma and issues without Singleton? Today, we're concluding Unit 2 by letting you try designing a system yourselves. You haven't learned all the technical design details yet, but that's the point: use online research, AI tools (like ChatGPT, Grok, or GitHub Copilot), and group discussion to figure it out. The goal is to think creatively about design patterns, concurrency (handling multiple things at once), and real-time features (like instant updates). There's no single "right" answer—focus on communicating your ideas clearly through simple sketches or diagrams. We'll use lightweight tools like Draw.io (free online) for modeling. At the end, each group will share a quick 2-minute summary, and I'll do a brief class walkthrough of some basic technical modeling tips.

*Why This Activity?*  
- It encourages you to research and apply design patterns without me teaching them all first (we can't cover every pattern anyway!).  
- You'll think about how to handle concurrency (e.g., multiple users doing things at the same time) and real-time elements (e.g., live updates).  
- Using AI will show how it can help brainstorm ideas, but you'll need to discuss and adapt them as a group.  
- Keep it simple: Aim for clear, basic models—don't overcomplicate for perfection.  

*System to Design: A Real-Time Notification System for a Community Event App*  
Imagine you're building a simple mobile/web app for a local community center that hosts events like workshops, sports games, or meetings. Users (community members) can sign up for events, and the app needs to handle real-time updates so everyone stays informed instantly. The system should:  
- Allow multiple users to browse and register for events at the same time (e.g., 50-100 users online).  
- Collect registrations and send instant notifications (e.g., "Event is full!" or "Your spot is confirmed!") to users' devices without delays.  
- Use a basic AI feature to suggest similar events based on what users like (e.g., if someone signs up for a yoga class, suggest nearby fitness events).  
- Log all activities for admins to review later, handling things like if two users try to register for the last spot at the exact same moment.  

This system is straightforward but will make you think about:  
- How to structure parts of the app (e.g., events, users, notifications) using patterns like factories (to create different types of notifications) or observers (to "watch" for changes and alert users).  
- Concurrency: What happens if many users act at once? How to avoid issues like double-booking?  
- Real-time: How to make updates happen live, like using events or messages?  

*Step-by-Step Guidance for Your Group (2 Hours Total)*  
Use the time wisely—divide tasks among your group of 3 (e.g., one researches patterns, one handles diagrams, one focuses on concurrency). Collaborate and discuss every step. You can use AI prompts like "Suggest design patterns for real-time notifications in an app" or "How to model concurrency for user registrations." Research online for examples, but adapt them to this system. No coding needed—just models and explanations.  

1. *Brainstorm and Research (20-30 minutes)*:  
   - As a group, discuss the system's main parts: What are the key components (e.g., Event Manager, User Registry, Notification Sender, AI Suggester)?  
   - Research design patterns: Search for "common design patterns for apps with notifications" or "problems without using patterns in real-time systems." Think back to Singleton—could something like that help here (e.g., for a single event list everyone shares)? Explore 2-3 patterns that might fit, like Factory (for creating notifications) or Observer (for watching changes). Use AI to ask: "What patterns handle multiple users registering at once?" Note any problems that could arise without patterns (e.g., confusion if notifications aren't coordinated).  
   - Look into concurrency: Search "what is concurrency in software" and "simple ways to handle multiple users at once." Think about real-world issues, like "What if two people grab the last event spot simultaneously?"  
   - Explore real-time: Research "real-time features in apps" or "event-driven designs." AI prompt: "How to model instant updates in a community app?"  

2. *Model the Static Structure (30-40 minutes)*:  
   - Create a simple diagram showing the system's "building blocks" (e.g., a class diagram in Draw.io). Include components like classes for Events, Users, Notifications, and AI Suggester.  
   - Apply patterns: Show how a pattern (e.g., Observer) connects things—e.g., how users "subscribe" to event updates. Keep it basic: Use boxes for classes, arrows for relationships.  
   - Add concurrency thoughts: Note in your diagram or text where multiple things happen at once (e.g., a note saying "Use threads or queues here to handle simultaneous registrations").  

3. *Model the Dynamic Behavior (30-40 minutes)*:  
   - Make another simple diagram for how the system works over time (e.g., a sequence diagram in Draw.io). Show steps like: A user registers → AI suggests events → Notification sends instantly → System checks for conflicts.  
   - Incorporate real-time and concurrency: Illustrate how live updates flow (e.g., an event fills up, and all waiting users get alerted right away). Think about "what if" scenarios, like handling delays or multiple actions.  
   - Use AI to help: Prompt "Generate a simple sequence diagram for real-time notifications" and tweak it for your ideas.  

4. *Reflect and Document Tradeoffs (20-30 minutes)*:  
   - In 1-2 paragraphs, explain your choices: Why did you pick those patterns? What tradeoffs (e.g., simpler design vs. handling more users)? Any basic ethical ideas (e.g., privacy for user data)?  
   - Note how AI/research helped: "AI suggested Observer, which we adapted because..."  
   - Prepare a quick share: One diagram slide or doc with your models and reflection.  

*Tools and Tips*  
- Diagrams: Use Draw.io (or paper sketches if needed)—export as images or PDFs.  
- AI/Research: Free tools like ChatGPT or Google searches. Be specific in prompts to get useful ideas.  
- Keep it Simple: Aim for 1-2 diagrams total, no more than 1 page of text. Focus on clarity over complexity—most students are new to this!  
- Group Roles: Assign one for research/AI, one for diagrams, one for writing/reflection, but discuss everything together.  

*Submission and Sharing*  
By the end of class, upload your group's work (diagrams + reflection) to the class shared folder. Each group shares for 2 minutes: "Here's our model and why we chose it." After, I'll quickly demo some technical basics like UML for patterns or concurrency (10 minutes). Great job experimenting— this is how real designers learn!
