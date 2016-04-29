# DestructibleComponent Issues

This repository is a project that reliably reproduces two DestructibleComponent issues for Unreal Engine 4.11.2:

 1. An "Ensure condition failed" showing some messages about NaNs shows up in the log. Note that this only happens the first time the Destructible Component is destroyed (right after opening the editor). In subsequent Plays, this message no longer appears.
 2. OnComponentFracture is called yet again many times, I'm guessing once per chunk that disappears.

To reproduce them, simply play the map and walk the character into the house to his left.
