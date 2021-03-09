# Session 1
[Back to workshop](https://github.com/Bleeck/UE_Workshop)

---

* [Creating a new project](https://github.com/Bleeck/UE_Workshop/blob/main/Session_1.md#creating-a-new-project)
* [Editor Basics](https://github.com/Bleeck/UE_Workshop/blob/main/Session_1.md#editor-basics)
* [Play In Editor](https://github.com/Bleeck/UE_Workshop/blob/main/Session_1.md#play-in-editor)
* [Editor Settings](https://github.com/Bleeck/UE_Workshop/blob/main/Session_1.md#editor-settings)
* [Blueprint Basics](https://github.com/Bleeck/UE_Workshop/blob/master/Session_1.md#blueprint-basics)
* [Printing to the screen and Detecting inputs](https://github.com/Bleeck/UE_Workshop/blob/master/Session_1.md#printing-to-the-screen-and-detecting-inputs)
---

### [Creating a new project](https://github.com/Bleeck/UE_Workshop/blob/main/Session_1.md)
  - 1: <span style ="color:pink"> Launch the "Epic Games Launcher".</span>
  - 2: <span style ="color:pink"> Navigate to Unreal Engine->Library</span>
  - 3: <span style ="color:pink"> Click on launch on version 4.26.1 (or whatever 4.26.X version you have installed)</span>
  <details>
  <summary>click to expand </summary>

  ![](./Assets/ProjectStartAssets/new_project_1.jpg)
  </details>  

###

    After a few seconds the editor should start and you will be presented with
    the Unreal Project Browser.

    Note: You might be asked to install additional features. Allow
    the editor to install what it needs (like dotnet 3.5 etc).

  - 4:  <span style ="color:pink"> Select Games. Click Next.</span>
  - 5:  <span style ="color:pink"> Select First Person. Click Next".</span>
  - 6:  <span style ="color:pink"> Leave settings to default and set a project location and name. Click Create Project.</span>


  <details>
  <summary>click to expand </summary>

  ![](./Assets/ProjectStartAssets/SelectGames.jpg)
  ![](./Assets/ProjectStartAssets/SelectFirstPerson.jpg)
  ![](./Assets/ProjectStartAssets/ProjectName.jpg)
  </details>  

###

    The Unreal Project Browser allows you to open an existing project or create
    a new one.
    When creating a new project there are two main aspects to consider:
      - the template project to start from
      - blueprint or C++ project

    While you don't need to start from a template project, as you can rebuild
    everything yourself, it's not recommended as the template projects are
    often good starting points (at least for learning purposes).

    Selecting C++ will generate a .sln file that needs to be opened with Visual
    Studio. C++ falls outside the scope of this workshop. We will be sticking
    with Blueprints because they are:
      - easier to understand
      - sufficient for building a complete game (that doesn't heavily deviate
      from the standard systems already implemented in unreal)

  [Where C++ is more or less mandatory](https://forums.unrealengine.com/community/general-discussion/121087-blueprints-vs-c-programming-which-one-to-use?148076-Blueprints-Vs-C-Programming-Which-one-to-use=&viewfull=1#post1013378)

---

### [Editor Basics](https://github.com/Bleeck/UE_Workshop/blob/main/Session_1.md)

<details>
<summary>click to expand </summary>

![](./Assets/Session1/Editor.jpg)
</details>   

    * Actor placement browser : this usually doesn't get used that much. Mostly
    used to place lights and volumes
    * ToolBar : Quick access to commonly used commands and menus
    * Content Browser : the asset library of the project
    * World Outliner : lists all of the actors placed in a level
    * Details : shows the properties of the selected level object

---

### [Play In Editor](https://github.com/Bleeck/UE_Workshop/blob/main/Session_1.md)

<details>
<summary>click to expand </summary>

![](./Assets/Session1/PIE.jpg)
![](./Assets/Session1/Eject.jpg)
</details>   

    PIE. By clicking on the play button (or pressing alt + P) the
    editor enters Play in Editor mode. In this mode, the game is running in the
    viewport. To exit PIE press the escape key.

    When PIE starts, LMB clicking in the viewport will lock the mouse cursor to
    that viewport. To release the cursor either press Escape to stop PIE or press
    Shift + F1 to regain control. After regaining control, if you click back
    in the viewport, you will again lose control. In order to select and
    manipulate objects during PIE, click on the Eject Button (or press F8).



<span style = "color:red">WARNING</span>: All changes done in the level during play in     editor are LOST when exiting PIE.

---

### [Editor Settings](https://github.com/Bleeck/UE_Workshop/blob/main/Session_1.md)
  <details>
  <summary> Open Editor Preferences </summary>

  ![](./Assets/Session1/Editor_Preferences.jpg)
  </details>

  <details>
  <summary> Type in "Search Details" textbox to filter settings </summary>

  ![](./Assets/Session1/filter_settings.jpg)
  </details>


  <details>
  <summary> Disable Autosave </summary>

  ![](./Assets/Session1/disable_autosave.jpg)
  </details>

      I personally never rely on autosave.

  <details>
  <summary> Disable Game Sound </summary>

  ![](./Assets/Session1/disable_game_sounds.jpg)
  </details>

      If you don't need game sounds, it's easier to just disable them in the
      editor.


  <details>
  <summary> Disable Use Camera Location From Play In Viewport </summary>

  ![](./Assets/Session1/camera_location.jpg)
  </details>

    This setting will cause the viewport camera to return to where it was before
    the PIE session started. Useful if you're editing a mission and don't want
    to have to keep navigating to the mission start location.


  <details>
  <summary> Enable Blueprint Save On Successful Compile </summary>

  ![](./Assets/Session1/save_on_compile.jpg)
  </details>

      This setting will cause the editor to automatically save your blueprint
      when it successfully compiles. I've found that it is extremely rare that
      you don't also click the save button after compiling (and it's usually because
      you forget to save)
  [ ]()
  [ ]()

#### Mouse Cursor Icon :
     The default mouse cursor behavior makes the cursor difficult to see in the
     editor viewport. The editor uses the windows "Precision" cursor while the mouse
     is over the viewport. In order to change it perform the following steps:

  <details>
  <summary> 1: Search and open "mouse settings" in start menu </summary>

  ![](./Assets/Session1/mouse_settings.jpg)
  </details>   

  <details>
  <summary> 2: Click on "Additional Mouse Options" </summary>

  ![](./Assets/Session1/Additional_Mouse_Options.jpg)
  </details>   

  <details>
  <summary> 3: Go to "Pointers" -> select "Precision Cursor" -> Click on browser </summary>

  ![](./Assets/Session1/Precision_Select.jpg)
  </details>   

  <details>
  <summary> 4: Navigate to "C:/Windows/Cursors" and select "aero_arrow.cur". Click on "Open" </summary>

  ![](./Assets/Session1/Cursors.jpg)
  </details>   

  <details>
  <summary> 5: Click OK to close the window</summary>

  ![](./Assets/Session1/OkMouse.jpg)
  </details>   

---

### [Blueprint Basics](https://github.com/Bleeck/UE_Workshop/blob/main/Session_1.md)

    Create a folder by RMB click in the content browser and selecting
    "New Folder". Name it "Work".

  <details>
  <summary>click to expand </summary>

  ![](./Assets/Session1/blueprint/1.jpg)
  </details>   

###

    Inside that folder, let's create our first blueprint. Right click in the content browser
    and select Blueprints-> Blueprint Class.

  <details>
  <summary>click to expand </summary>

  ![](./Assets/Session1/blueprint/2.jpg)
  </details>   

###

    Select Actor as the parent class. Name the blueprint "MyActor"

  <details>
  <summary>click to expand </summary>

  ![](./Assets/Session1/blueprint/3.jpg)
  </details>   

###

    Note: An asterisk next to an asset in the content browser means that
    the asset has unsaved modifications. You can save by RMB clicking on the asset
    and selecting "Save", selecting the asset and pressing CTRL+S or by
    pressing "CTRL + SHIFT + S" which saves everything.

  <details>
  <summary>click to expand </summary>

  ![](./Assets/Session1/blueprint/4.jpg)
  </details>   

###

    Double click on the actor to open the blueprint editor.

    The Blueprint Editor contains the following elements:
      - components panel: this is where you can add or remove components on your actor
      - my blueprint: this is where you declare your functions, variables, events etc
      - toolbar: this is were you can find the main debugging controls
      - Details panel

  <details>
  <summary>click to expand </summary>

  ![](./Assets/Session1/blueprint/5.jpg)
  </details>   

###

    The Blueprint Editor also has 2 extra panels that are hidden behind the viewport
    panel. Those are:
    - the construction script : useful for level design automation
    - the event graph : the place where you actually do your blueprint
    scripting

  <details>
  <summary>click to expand </summary>

  ![](./Assets/Session1/blueprint/6.jpg)
  </details>   

###
---

### [Printing to the screen and Detecting inputs](https://github.com/Bleeck/UE_Workshop/blob/main/Session_1.md)
    To directly get an input (the quick, dirty and incorrect way), we can add a Keyboard Event
    node in the event graph.

    Right click and type "Keyboard Events X" and press enter.

###

  <details>
  <summary>click to expand </summary>

  ![](./Assets/Session1/Inputs/1.jpg)
  </details>   

###

    To print something to the screen we need to add a
    "Print String" node.

###

  <details>
  <summary>click to expand </summary>

  ![](./Assets/Session1/Inputs/2.jpg)
  </details>   

###

    By connecting the "Pressed" execution pin from the Keyboard Event to the execution pin of
    the "Print String", we will print the string to the screen every time the X key is pressed.

###

  <details>
  <summary>click to expand </summary>

  ![](./Assets/Session1/Inputs/3.jpg)
  </details>   

###


    Placing an instance of "MyActor" in the level will not run the input event. That is because
    we must first configure the actor to actually receive inputs.
    Select the actor, in details find Input->Auto Receive Input and select "Player 0".

###

  <details>
  <summary>click to expand </summary>

  ![](./Assets/Session1/Inputs/4.jpg)
  </details>   

###


    Now if we press Play and press "X" we get the print string "Pressed X".

###

  <details>
  <summary>click to expand </summary>

  ![](./Assets/Session1/Inputs/5.jpg)
  </details>   

###

---

### [Variables](https://github.com/Bleeck/UE_Workshop/blob/main/Session_1.md)

---
[Back to workshop](https://github.com/Bleeck/UE_Workshop)
