---
description: The Numbers Within
---

# Variables

**Game Creator** comes with a variables system that allows you to keep track of the game progress and save the state between play sessions.

![](../../../.gitbook/assets/variables-example.jpg)

A **variable** is a value container with information that can be changed during gameplay.

{% hint style="info" %}
For example, in a **Zelda** game, the hearts at the top of the screen would be a variable identified by the name "_hearts_".
{% endhint %}

![\(You can track the Player health creating an integer variable called &quot;hearts&quot;\)](../../../.gitbook/assets/variables-header.jpg)

There are different types of Variables:

* [Global Variables](global-variables.md): Identified by a unique name.
* [Local Variables](local-variables.md): identified by a unique name. Only affect one scene.
* [List Variables](list-variables.md): An array of values accessed by index. Only affect one scene.

{% hint style="info" %}
Variables can also be accessed through code. Head to [Variables Access](../../systems/game-creator-api/variables-access.md) to know more.
{% endhint %}

## Anatomy of a Variable

A **variable** is has a `name` that identifies it \(for example: “shotgun ammo“\) and a `value`. 

A variable can have different types of values, including character **strings**, **numbers**, **booleans** \(on/off\), **Colors**, **Vector3**, and references to **Game** **Objects**.

{% hint style="info" %}
Next to the name there's a checkbox. This allows to save the variable's state between play sessions
{% endhint %}

{% hint style="warning" %}
Not all variable types allow to save its state. For example, **Game Objects** can't be saved because they are a reference type, which Unity doesn't allow to serialize.
{% endhint %}

