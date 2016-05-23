Baby steps...

OK so here we have a more complex network with 4 sites - some of them with redundant connections and some of them without.

Everything should already have IP addresses assigned to the Gigabit interfaces and should also have some loopback addresses.

Here's the tasks:

1. Draw a simple diagram of this network and include all IPs and interface names. This will make everything easier.
2. Create just enough static routes to be able to ping from any router to any other's GigabitEthernet interface. What's the least amount of routes you can do this in?
3. Now make sure you can ping from any router to any other router's loopback address.
4. Ensure that you can shut down any one of the connections between LA, SF, and NY and that everything can still ping everything else.
5. Bring back up all interfaces and configure things so that SF will prefer the link to LA to get to Chicago, but if this link goes down SF will go through NY to get there.

Thinking Questions:

1. How can you source a ping from a specific interface?
2. What in the routing table tells you the priority of a route?
3. Why might you want to use loopback addresses?
4. Can static routes take into account link speeds?
5. How does load balancing work with static routes?
