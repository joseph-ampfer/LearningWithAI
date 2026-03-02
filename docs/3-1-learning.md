I chatted with ai to learn about latency compensation and different ways to combat it. One way is to use client side prediction, and the server sends an event and time it went off, and client can start the same event, and fast forward the delay it has from the server.

I also learned about spawning and despawning network objects. Spawning them makes a duplicated copy on every client, and any code you have on them will run sepearately on each client. Also that Despawning them can trigger a callback that you can react to, like to play explosion vfx.

I learned about network variables and how they sync across clients/server. You can attach functions to the listener so that each time it is changed, you can run as many functions as you want to react to that.