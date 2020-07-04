# Actor-Based-Model-in-Concurrent-and-Distributed-systems
Implementation of the Actor Based Model in Concurrent and Distributed systems using Python Thespian Library

The actor model is used in concurrent computing in which the actor is considered as the primitive for concurrent computing. The actor is considered as an example of combining distribution and multithreading. It can perform a wide range of functions such as transmit a limited no. of messages to similar actors, create a more limited number of similar actors, specify actions for incoming messages.
Actor model implementation follows the following steps - First, using a configuration file to specify the host process on which the actors will execute as well as the port that can be used to receive the messages. Secondly, to provide the ability to create actors in remote processes. Third, provide logical names to identify remote actors. And finally serializing the messages transmitted among actors.

In this project, we have created an actor that responds to the request by creating/generating the other actors dynamically. Actors are the independent of process, they do not copy the data instead they directly send data to the other process.

The actor does the following things:
a)	Changes the internal state.
b)	Create other actors.
c)	Communicate with other actors using the addresses of other targeted actors by described protocols.
d)	The life cycle of Actor in existing system:
e)	Actor is created by using the function createActor(), address is assigned by the actorSystem.
f)	The actor is called by using function ask().
g)	Actorsystem.ask() calls another actor.
h)	Actor passes the message to the other targeted actor using function tell.
