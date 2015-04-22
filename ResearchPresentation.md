# Research Presentation

### Teleporation in Unity

##### Purpose:
The reason I am examining teleportation is because for my project the main focus is the aesthetics of different worlds that are being created. As a result, the main mechanic of the game will come from teleporting between these planets to emphasize the distinction between all of them.

###### Finding the Answer:
It appears there are many different methods for approaching the concept of teleportation in unity. I took a look at some of the examples that can be found on the unity forums and found a few different ways in which teleportation can be implemented.

The first of which was a user named Elicoor inquiring about >"Moving (teleporting) player and camera when they enter a certain area"
[The thread can be found here](http://answers.unity3d.com/questions/11617/moving-teleporting-player-and-camera-when-they-ent.html)

##### How it Works:

The consensus across the board is that the proper approach would be to utilize **Triggers**.

The user would be required to create a new _GameObject_ to represent the teleporation area, whether or be a capsule, platform or whatever you may choose.

Once that has been created, the next move is to check the **"Is Trigger"** button located in the collider component. Uncheck the **Mesh Renderer** component so it becomes invisible.

From this point it is all about creating a destination for going to and from.

To do this, we would utilize a script being added to the teleporter object which would read: "_var destination: transform;
function OnTriggerEnter(other :Collider) {other.transform.position = destination.position;}_"

The purpose for using this is so that objects and players can go through the portal as I am exploring the option of making the game revolve around building a space ship to return home which would require taking pieces from different planets or dimensions. The story will get fleshed out.

By using this, I can make the most out of all the different designs created for my game and really make the player feel as though they are experiencing many different worlds without having to go through the nuisance of slowly traveling between them.
