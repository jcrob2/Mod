# I'm still alive
Hello and welcome back! There has been a pivot in how the bat add-on is being handled. To fascilitate better control over which worlds and saves have access to this add-on, I've chosen to implement the feature as a datapack, which can be added to select worlds. If you're unsure how a datapack works, a quick google search will answer most questions, but I'll answer a few here.

# Features
This datapack is designed to be used in version `1.20.1`. Here's the list of features added to this version of the add-on:
- Player is 40% the size of a normal character
- Player is able to utilize Elytra gliding even without an Elytra
- Player is able to see in the dark to some degree
- Player is able to "flap their wings" and be launched upwards 6ish blocks every 1.5 seconds(ish)
- Player becomes exhausted faster when flying

# FAQ

_Q: What do I need to use the datapack?_

At a bare minimum you need the [Fabric API](https://www.curseforge.com/minecraft/mc-mods/fabric-api), [Fabric launcher](https://fabricmc.net/use/installer/), the [Origins](https://github.com/apace100/origins-fabric) mod, [Pehkui](https://github.com/Virtuoel/Pehkui), and maybe [ExtraOrigins](https://github.com/MoriyaShiine/extra-origins) (I use this one but theoretically you don't need it). These mods need to be located in your `.minecraft/.mods` folder within your mincraft installation.

_Q: Why datapacks?_

Datapacks allow for more fine-grained control over what saves have access to what features. For example, if I had implemented this as a mod, every world you create would have access to it, which isn't always a good thing. Additionally, you are able to reload datapacks within the game without having to save and exit by entering `/reload` into the chat bar. This will reload all datapacks within the datapack directory (I'm getting there), allowing for new features to be added/removed on the fly.

_Q: How do I use datapacks?_

This is the meat of this long instructions, and what you really care about. I'll make this as easy as I can:
1. download the .zip file for the datapack you care about (in this case it's located at `/Mod/datapacks/data`)
2. copy or move this .zip file into the particular datapack directory for the save you want to have access to it. For example, if I previously created the world `Testing`, my datapack directory for this world is located at `%AppData$/Roaming/.minecraft/.saves/.Testing/datapacks`. Your specific file location may be different depending on where you installed your minecraft installation. If you're unsure how to access this, you can also go to the world selection screen, select your world, click `edit`, and select `open world folder`. This will open up the directory for the save/world and will contain the `datapacks` folder you care about.
3. if you're not in the world yet, enter the world
4. type `/reload`
5. that's it!

If there are features that would be nice to have/are necessary that I missed, feel free to let me know and I might get back to it in another year!
