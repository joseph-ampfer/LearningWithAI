I learned about state machines by talking to ai. I had a Lobby with multiple states to show the correct panel and right buttons. The state machine helped manage the complexity.

The version I learned about with ai involved a ILobbyState that had enter() and exit() functions.
For each state (default, PublicSearch, Lobby, PrivateMatch) I made a class that implemented the ILobbyState interface.
The state machine class would create an object for each of those classes, and add it to it's own states list (to check against when some component wants to transition).
The state machine had a transitionTo(ILobbyState) method, that checks if it is a valid state, calls exit() on the current state and enter() on the next state.

That tied this together was a UIController class that created a context bag that has refs to all the ui elements and buttons, so it can pass this context to each state that needed it.

Even though there were more files at the end of this learning, it helped keep everything organized and easy to add new elements.
