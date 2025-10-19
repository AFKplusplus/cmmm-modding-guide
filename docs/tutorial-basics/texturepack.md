---
sidebar_position: 5
title: Adding a built-in texturepack
description: Programmer Art
---

# Adding your own built-in texturepack

First, you need some textures for your texturepack. So, go to the `Assets` folder, then enter the `texturepacks` folder. 

Here, you will see a folder named `Default`. This folder *should* have all the textures of the cells you've made (if there isn't, refer back to [Adding A Texture](../adding-cell/texture).)
Copy the folder and rename it to whatever you like, such as `Programmer Art`.

Then, go inside of the newly created folder, and open the `pack.json` file.
The code inside should look like this:
```json
{
    "title": "Default",
    "desc": "Mystic Mod's default texturepack."
}
```
Change the title and description of the texturepack to your liking.

After that's finished, you can change the textures of the cells in the texturepack.

### Making the cells change textures

Currently, if you start the game and select your texturepack, the game wont change the textures of the cells **you've** created.
This is because you have to add the cells you've made onto the TextureLoader script.

First, open your project in Unity. If you don't have a project, please visit [Introduction](../intro).

In the file explorer at the bottom, open the `Scenes` folder. Here, double-click the `MainMenu` scene.
Next, open the `TextureLoader` object. Expand `Texturables` if it is collapsed, and increase the size by the amount of cells you've made.
In the file explorer at the bottom, located the `Assets` folder and open `Cells`. Drag the textures of your created cells to the bottom of the Texturables tab, replacing duplicate BGDefault.

Now you are done with your built-in texturepack! Run the `MainMenu` scene, and click on the `Textures` button. Select your newly created texturepack and try it out!
