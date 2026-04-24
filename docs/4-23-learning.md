I learned about synchronous scene loading with Unity NGO NetworkManager.Singleton.SceneManager.  The server can use this to switch scenes, and all connected clients will switch as well.

I ran into a problem that one client would take 15 seconds+ to load the scene. Then I learned about a callback OnSceneLoadedAll where it fires when all connected clients finish
loading the scene. I can use that to wait to start the game until everyone has finished loading the game.
