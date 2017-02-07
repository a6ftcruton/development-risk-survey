# Development Risk Survey
####Before any implementation, consider...
- User Perspective
  - how might these changes be confusing?
  - does the user get appropriate feedback/guidance from the app to understand the new feature?
- Existing Code
  - will you just be adding new code or will existing code require updates?
  - is the existing code reusable for your purpose?
  - what parts of the app could be impacted/broken by changes?
  - what are potential bugs these changes could introduce?
  - what regression testing is prudent?
- Performance
  - are you querying huge tables?
  - class-level performance: is there a way to be smarter, in loops/iterators?
  - what is the state of the data you are relying on (or creating?)
- Scalability
  - what happens to this code if we add 2 million users?
  - what happens to this code if we add 10 million db records to related tables?
- Scope
  - is this project dependent on features in other applications?
  - will this require migrations and/or backfilling data?
  - what is the potential for scope creep?

