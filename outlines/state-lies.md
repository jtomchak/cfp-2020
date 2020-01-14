# Your State is Lying to You


# Abstract (600 char, what they will learn from your talk and why they care about it)
We've got global state, component state, state in a store, app-level state, state in context, its a very delicate balance of what is true now, what has happened, and what’s possible in the future. State can notably be the most complex, difficult part of any application. I am here to break the difficult news to you that your state has been lying to you this whole time. Now, these are not full outrageous lies, no. They are dozens and dozens of little white lies, sometimes just an omission of the truth. Of what is actually going on in your program. 
There is a path to reform, for even the most misbehaved state. I’ll expose how your state has been fudging the truth, making you and your team’s life more difficult. Once we know exactly what’s going on, we’ll explore some ideas to keep state on the straight and narrow. 

Your state has been lying to you this entire time. Letting isLoading, isSuccess, and isError all exist simultaneously leaving it up to you to constantly juggle which ones are true and false and when. But it doesn't have to be. We can model our state to be explicitly in one and only one state at at any given time. This removes any possibility that our app could be both loading and already successful. 


# Details (more detailed information about how your talk will go down)
The core of the is talk is to introduce the audience to finite state machines, using one of the problems we've all experience in our React code, getting into an impossible state. The most notable example is the never ending list of Boolean flags such as isLoading, isFetching, isCollapsed, or isAMillionOtherOptions. Suddenly our app is fetching, error'd, and rendering content all at the same time.  

# Pitch (yourself pitch yourself as the the person capable of making this talk awesome. Why does this talk need to happen? Why are you excited about it?)

State machines offer compelling solution to keeping the every growing state of an application manageable. Explicitly defining each and every possible state and most importantly their connection to one an other, there is added confidence that the logic of our application is correct. 
Looking for more trust in my code I've explored static type systems, transpilers, linters, extensions, unit tests, but none of them have given me as much confidence as even the simplest finite state machine. 
