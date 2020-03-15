# Entry 5
##### 3/14/20

## Summary

Throughout the middle of Februray to now, Jagger and I attempted to create a basic prototype of our product within [**Unity**](https://unity.com "Unity").

## The Engineering Design Process (EDP)

In our previous blog entry, it was stated that Jagger and I learned more about our simple and intuitive tool, Unity, in order to create our prototype. For about two weeks after our previous blog entry, Jagger and I studied enough about Unity to say that we are now knowledgable in using our tool. With that, we began our **prototype** stage.

We first took out our [**MVP Plan**](https://docs.google.com/document/d/1iS1Bwc5UVCwYeEUM-ebBoWghxekGvK2Fx_ZQv47Lj0Q/edit?usp=sharing "Unity"), the [**C# beginner guide**](http://www.miro.ing.unitn.it/download/Didactics/Misure2/UNITY/Learning%20Csharp%20chapter_1-6.pdf "C#"), and other google documents as a reference to making our prototype. Our goal is to create a sprite that can move around the screen and interact with other game entities either through textboxes or combat. We knew that the interaction system would take a lot of time to create, so we decided on first creating the sprite with movement.

We created a 2D template called "Prototype" and added a sprite object called "Player" within the 2D terrian. We then rendered the sprite object to be a small square for simplicity.

Now that we have the sprite object on the screen, we need to implement the object with a script (A block of code that makes the object attached to it execute a certain function). Our script should make our player object move around the screen through the WASD keys.

In order to create the script, we need utilize four unity C# classes, [`Vector2`](https://docs.unity3d.com/ScriptReference/Vector2.html "Vector2"), [`Time.deltaTime`](https://docs.unity3d.com/ScriptReference/Time-deltaTime.html "Time"), [`Input.GetKey`](https://docs.unity3d.com/ScriptReference/Input.GetKey.html "Input"), and [`transform.Translate`](https://docs.unity3d.com/ScriptReference/Transform.Translate.html "Translate").
* [`Vector2`](https://docs.unity3d.com/ScriptReference/Vector2.html "Vector2") returns the position of our 2D object through X and Y coordinates. It also has the ability to set the object's direction by attaching `.right`,`.left`,`.up`, or `.down` at the end of the class.
* [`Time.deltaTime`](https://docs.unity3d.com/ScriptReference/Time-deltaTime.html "Time") returns the amount of seconds it takes to complete a action since the last frame.
* [`Input.GetKey`](https://docs.unity3d.com/ScriptReference/Input.GetKey.html "Input") checks if a certain key on the keyboard is pressed.
* [`transform.Translate`](https://docs.unity3d.com/ScriptReference/Transform.Translate.html "Translate") simply moves / translates the object

Together, you can create an if statement that translates the object at a certain direction and speed when certain keys are pressed.

```cs
// FORMAT FOR IF STATEMENT

if (Input.GetKey(KeyCode.[PLACE KEY HERE])){
        {
            transform.Translate(Vector2.[PLACE DIRECTION HERE] * [PLACE MOVEMENT SPEED HERE] * Time.deltaTime);
        }
}
```


```cs
// IF STATEMENT WHEN IMPLEMENTED IN SCRIPT

using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class Movement : MonoBehaviour
{
    public int movementspeed = 5;
    // Use this for initialization
    void Start()
    {
    }

    // Update is called once per frame
    void Update()
    {
        if (Input.GetKey(KeyCode.A))
        {
            transform.Translate(Vector2.left * movementspeed * Time.deltaTime);
        }

        if (Input.GetKey(KeyCode.D))
        {
            transform.Translate(Vector2.right * movementspeed * Time.deltaTime);
        }

        if (Input.GetKey(KeyCode.S))
        {
            transform.Translate(Vector2.down * movementspeed * Time.deltaTime);
        }

        if (Input.GetKey(KeyCode.W))
        {
            transform.Translate(Vector2.up * movementspeed * Time.deltaTime);
        }


    }
}
```

<p align="center">
<a href="https://gyazo.com/337326e8529e8a09a94b36eddf7db097"><img src="https://i.gyazo.com/337326e8529e8a09a94b36eddf7db097.gif" alt="Image from Gyazo" width="800"/></a>
</p>



<h6 align="center">Visual demonstration of movement script</h6>

Basically, the script is detecting if any of the WASD keys were pressed. If so, the object will move either left, right, up, or down at a speed of 5 units per second.

Currently, Jagger and I are still trying to figure how to make our player object both detect and interact with another object on the screen. We are both in the middle of our **prototype** stage.

## Skills

Reading documentation was probably the most significant skill Jagger and I had to use. Creating the movement script for our player object required many Unity classes that we were unaware of. As a result, we had to consult the [**Unity Manual**](https://docs.unity3d.com/Manual/UnityManual.html "Manual"). The manual contained important information and tutorials on many Unity classes and functions. However, it also contained many terms and phases that we didn't know about. To fully understand and create our script, we needed to learn how to read the documentation.

## Knowledge

As Jagger and I worked on the first type of our prototype, we found out that both Java and C# has access to many different types of libraries. Similar to [`Java.util.*`](https://www.cs.mun.ca/java-api-1.5/guide/lang/index.html "Java.util.*"), C# has libraries that consist of collections framework, legacy collection classes, event model, and date and time facilities. These libraries allow me to use methods and classes that are essential for creating my Unity scripts, such as `Time.deltaTime`.
* A few examples of C# libraries are  [`System.Collections`](https://docs.microsoft.com/en-us/dotnet/api/system.collections?view=netframework-4.8 "Collection") and [`System.Collections.Generic`](https://docs.microsoft.com/en-us/dotnet/api/system.collections.generic?view=netframework-4.8 "Collection.Generic").

## Final Words

As stated in the previous blog entry, Jagger and I are still far from fully completing our product. Despite creating a working movement script, we still need to create more scripts for the interaction system between the player object and other Unity objects. This requires us to further read into the C# and Unity documentation, utilizing our reading and critical thinking skills.

Until the next blog entry, adios!

[Previous](entry04.md) | [Next](entry06.md)

[Home](../README.md)