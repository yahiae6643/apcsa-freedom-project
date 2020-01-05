# Entry 3 (1 / 4 / 2020)



## Summary

Throughout December, my partner, Jagger, and I attempted to learn the coding language C# and outlined our prototype.

## The Engineering Design Process (EDP)

Throughout the time of learning C#, we were **brainstorming** and **planning** different designs and features for our prototype. The process consisted of mostly sketching and typing onto a google document.

During our **brainstorming stage** We sketched designs for how our prototype would look like. Since the prototype is going to be an RPG (role-playing game), we made sure to include essential RPG elements within our sketches. This includes:

- Meters and numbers that measure the player's resources (Health, Mana)

<img src="https://cdn.designbyhumans.com/product_images/p/104514.f56.652b5S7ay1Cm2MjUAAA-650x650-b-p.jpg"
     alt="Health & Mana Meter"
     style="margin-left: 250px; width: 400px" />

- Boxes that appear when the user interacts with a character or item within the game

<img src="http://i.imgur.com/Nj7OcbX.jpg"
     alt="Chat"
     style="margin-left: 250px; width: 400px" />

- Possible terrains that the user can encounter and explore

<img src="http://i.imgur.com/Q2BQ8zj.png"
     alt="Terrian"
     style="margin-left: 250px; width: 400px" />


Once we completed our final sketch, we start our **planning** stage. Jagger and I created a google document where we created C# variables that would be needed to implement our sketch onto Unity. Different elements of our sketch required different C# variables, so we decided on using:

- Integer variables for the health, mana, and everything else that is countable
 ```
 int HP = 100;
 int MP = 100;
 ```
- String variables for chatboxes and item descriptions
```
string message = "Hero! We need help!";
string descOfSword = "A sharp iron sword. Does 30 dmg";
```
- Boolean variables for checking if the user is interacting in any way (fighting, talking, etc)
```
bool isInBattle = true;
bool isSpeaking = false;
```

We are still currently planning out our C# variables in our [**document**](https://docs.google.com/document/d/18f9qcz2JyZ-BGMIxdP59HZ8n27FTovv30-qeWeXPChY/edit?usp=sharing "document"). Once completed, we'll quickly onto **creating** our prototype since we'll have a reference and some code to start with.

## Skills


Jagger and I have used our skills of **collaboration** and **time-management** while approaching our project.

A majority of our time in class was utilized to fix a persistent issue with [**Unity**](https://unity.com "Unity"). The school computers weren't able to install the software. Our attempts to fix the installation issue failed, and after one week of constant debugging, Jagger and I finally decided to focus our energy on blueprinting our prototype and learning C#.

During the rest of December, we used our class-time and some time outside of class to develop a solid understanding of C#. We went through [**w3schools**](https://www.w3schools.com/cs/ "w3schools") and many other resources about the coding language. Our lessons on C# ranged from syntax to classes. After finishing our lessons, we discussed what we learned and asked questions to fill in any knowledge gaps.

While developing a solid understanding of C#, we also discussed possible designs and features that should be added into our prototype (Go the EDP section above to see more about our brainstorming and planning).


## Knowledge

As stated in our previous entry, we noticed that Java and C# are very similar. This comes from the fact that both are  [**object-oriented languages**](https://www.upwork.com/hiring/development/object-oriented-programming/ "object-oriented languages"). Both coding languages function through the use of `classes` and `methods`, which is very important when creating a game. However, the main factor that differentiates C# from Java is that it is also a [**managed language**](https://docs.microsoft.com/en-us/dotnet/standard/managed-code "managed language"). This means C# has strong memory backup, which prevents memory leakage problems and other memory issues from occurring. These type of problems often happen when using Java and may lead to our software to shutdown when testing our game prototype, so C# is the ideal coding language for Jagger and me to use.

## Final Words

Jagger and I still have a long way to go from creating a proper RPG. By the time we reach the next entry, our goal is to implement our drafted ideas onto Unity. However, this will require us to learn the mechanics of the software. Also, we will be required to learn the C# methods and classes that Unity often uses.


[Previous](entry02.md) | [Next](entry04.md)

[Home](../README.md)