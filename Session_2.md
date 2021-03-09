# Session 2
[Back to workshop](https://github.com/Bleeck/UE_Workshop)

---
* (Inputs 2.0 and spawning actors)[https://github.com/Bleeck/UE_Workshop/blob/master/Session_2.md#inputs-20-and-spawning-actors]
* Switch projectile logic to raycast
* Change Hud to fix aiming offset
* Particle systems -> Add hit effects
---
### [Inputs 2.0 and spawning actors](https://github.com/Bleeck/UE_Workshop/blob/main/Session_2.md)

    Inputs need a layer of abstraction in order to accommodate different input devices
    and allow the player to remap them during runtime.

    This layer of abstraction is managed through axis and action mappings.

    Navigate to Project Settings->Input.

    Add an Action Mapping by clicking the plus Icon.

    Name it "SpawnInput".

    You can click on the keyboard icon and press a key in order to record it as
    the input for the SpawnInput action mapping.

  <details>
  <summary>click to expand </summary>

  ![](./Assets/Session2/Inputs/1.jpg)
  </details>   

###

    Create a new blueprint (derived from Actor).
    Name it "Props".
    Add a Static Mesh component to the actor and set the mesh to "1M_Cube".

###

  <details>
  <summary>click to expand </summary>

  ![](./Assets/Session2/Inputs/2.jpg)
  ![](./Assets/Session2/Inputs/3.jpg)
  </details>   

###

    In the "MyActor" blueprint we can now replace the "X" keyboard event with an
    Input Action SpawnInput.

###

  <details>
  <summary>click to expand </summary>

  ![](./Assets/Session2/Inputs/4.jpg)
  </details>   

###


---
[Back to workshop](https://github.com/Bleeck/UE_Workshop)
