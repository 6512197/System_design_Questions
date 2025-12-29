# System_design_Questions 
Leetcode gets your foot in the door.
System Design gets you the keys to the corner office

simulacro para mejorar tu entrevista en SD 

# Interviewer :



Interviewer :
Let us begin simply. Imagine you are tasked with designing a URL shortener service—something like bit.ly.
At Stage 1 (1 user), our only concern is functional correctness.
What are the core functional requirements of this service?
Sketch out a minimal API design that supports shortening a URL and later retrieving it.


Interviewer :
What if Scenario (Stage 1 Challenge):
Suppose your single server restarts and your database gets wiped (say it was in-memory only). Suddenly, all shortened links are gone.
What would you change in your design to ensure persistence and durability of links, even in this simplest architecture?




Interviewer :
Let us escalate.
Now we enter Stage 2 (Scaling to ~10,000 users). With this small traffic spike, our single server/database may slow down.
How would you evolve your schema and architecture to handle higher traffic especially repeated reads of popular short links?


Interviewer:
Now, let’s push forward to Stage 3 (Scaling to ~1M users).
Now Imagine your database starts becoming a bottleneck for writes. Some short links get extremely hot (millions of clicks/hour), and some partitions of your database are overloaded.
What would you do to scale your database beyond a single instance?


Interviewer:

traffic keeps growing , one short link becomes globally viral 
even with caching  DB  node can handle writes and metadata 
growth 
how would your partition (shard your database)  ?
explain your shard key and how to avoid hot partitions?
