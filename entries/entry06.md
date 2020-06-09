# Entry 6
##### 6/1/20

## Summary

Throughout the months of March and April, Jagger and I created a functional prototype of our product within [**Unity**](https://unity.com "Unity").

## The Engineering Design Process (EDP)

In our previous blog entry, Jagger and I only created a movement C# script for our character object. Now, we improved upon that movement C# script and created many more scripts for our character and other game objects, finally completing our **prototype** phase of the Engineering Design Process. Based on our current [**github repository**](https://github.com/yahiae6643/FreedomProject_RPG_Product/tree/master/Assets/Scripts "Repository"), we created C# scripts ranging from camera detection to a turn-based battle system. Despite this, I still believe that our prototype still needs some improvements, such as adding more types of enemies and adding a shop NPC for the user to buy weapons to defeat these new monsters. As a result, we are now within the **improving** stage of our Engineering Design Process (if time is on our side).

*Update (6/8/20)*: Completed the **improving** stage. Scripts that were improved upon include `enemyGenerator.cs` `ButtonFunctions.cs`, `Enemy.cs`, and `Player.cs`. Scripts that were added include `Restart.cs` and `shopBehavior.cs`.

*Scripts that need explaining*

- `enemyGenerator.cs` is a script that opens up the battle GUI when it detects that the user's sprite made a certain amount of movement.
- `ButtonFunctions.cs` is a script that assigns certain functions to the buttons on the battle GUI. For example, the **Attack** button on the battle GUI is assigned a function that deals a certain amount of damage to the enemy on the screen.
- `shopBehavior.cs` is a script that allows the player to purchase or sell weapons on the shop GUI.

<br />

<p align="center">
<a href="https://gyazo.com/05dd9a83cb038285de06ec17a14ad9d4"><img src="https://i.gyazo.com/05dd9a83cb038285de06ec17a14ad9d4.gif" alt="Image from Gyazo" width="400"/></a>
</p>
<h6 align="center">Visual demonstration of ButtonFunctions script</h6>

<br />

<p align="center">
<a href="https://gyazo.com/d0748a9f56a5608c259408d4c089ed64"><img src="https://i.gyazo.com/d0748a9f56a5608c259408d4c089ed64.gif" alt="Image from Gyazo" width="400"/></a>
</p>
<h6 align="center">Visual demonstration of ButtonFunctions script</h6>

<br />

<p align="center">
<a href="https://gyazo.com/f0233809f45c893dfee324c07c3a4ea6"><img src="https://i.gyazo.com/f0233809f45c893dfee324c07c3a4ea6.gif" alt="Image from Gyazo" width="400"/></a>
</p>
<h6 align="center">Visual demonstration of shopBehavior script</h6>

## Skills

Probably the #1 skills we had to use was organization and collabation. Jagger and I constantly shared our results about the prototype and discussed new ideas to implement. Also, our google documents and github repository helped keep us on track in terms of easy file placement and checking off our list of ideas that we successfully implemented. Without these skills, we wouldn't have been able to complete our MVP.

*I need to thank Jagger for all of the help he has provided. His innovative approach to ideas really helped me to add the essential mechanics our RPG game needed.*

## Knowledge

Again, my basic knowledge on Java and the great similarity between Java and C# allowed to quickly read and understand C# documentation. There were many C# methods I needed to use in order to implement certain features, such as adding a delay to when the enemy attacks the player. Here is a small list of methods I found useful.

- [`yield return new WaitForSeconds(N)`](https://docs.unity3d.com/ScriptReference/WaitForSeconds.html "Delay"):  Adds a **N** seconds of delay to the methods below the return statement
- [`SetActive(boolean)`](https://docs.unity3d.com/ScriptReference/GameObject.SetActive.html "Visibility"): Makes game objects appear or disappear from the screen (true: visible, false: invisible)
- [`Mathf.Clamp(Object.x, x1, x2)`](https://docs.unity3d.com/ScriptReference/Mathf.Clamp.html "Restrict"): Restricts the x or y coordinate of a game object between two values

## Final Words

Despite finishing our MVP, I still believe we need to add a few more mechanics in order for our game to be like we envisioned. It was a fun ride to create this game and I hope we can continue updating it in the future.


[Previous](entry05.md) | [Next](entry07.md)

[Home](../README.md)