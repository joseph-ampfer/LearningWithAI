I learned about latency in multiplayer games, and strategies to hide it. One way that I found works well with my game is "Action Anticipation". 
This is what some games use when throwing grenades. When the user clicks the button, a sound / animation plays immediately on their screen (before server confirmation).
This gives enough time for the request to go to the server, confirm it, and spawn the grenade object. The animation before hand hides the latency of the Round Trip Time the 
network messages take to get to the server and back.
