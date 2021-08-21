## Using submodules with GitHub Pages Pro
### You can use submodules with GitHub Pages to include custom assets that you cant do normally!

### Setting up and other crap
Your gonna need to install `gitmodules`. Simple go to the `commandline` and type in `gitlib install module:2.6.2`.
Now go to `assets/preload/data` and create a `gitmodule` file, Ex:  `tagname.gitmodule`, Then Head over to `source/substates`

### Types of SubStates

- **Snd:** This SubState Allows you to make a 1-5 seccond video anywhere on your site!
- **SndTV:** This Substate Allows you to add videos no matter the duration! **MUST BE ADDED VIA ASSETS**
- **TType**: This Substate Allows you to create linkable text anywhere on your site!
- **TWar**: This Substate Allows you to have a Watermark on your page!

### Adding SubStates

Choose what kind of Substate you want to add and put it on the list at `Line 17` Make Sute to write it like this: (PS: MAKE SURE THE NAME IS THE SAME AS THE `.gitmodule` FILE YOU CREATED EARLIER) `var <name> = <type of substate>;`  
```
@:publicFields
class TweenV {
	static var GUID = 0;
	var uid 		= 0;
	
	var tagname = TType;
```

Now On Line 32 You have to list the `gitmodule` file. Like This:
```
	public inline function new (
		parent:Snd	 ,
	    n:Float		 ,
	    ln:Float	 ,
		varType:TVVar,
	    speed:Float	 ,
	    from:Float	 ,
	    to:Float	 ,
	    type:h2d.Tweenie.TType ,
	    plays		 ,
	    onUpdate	 ,
	    onEnd		 
	) {
		this.tagname = gitmodule;
	}
```

Now Go to Line 120, and scroll down until you see the `class` statement with the submodule you created! Now Add a new like this:
```
	public function() {
		gitmodule=data;

		x.pos = <position>
		y.pos = <position>

		new dataScript() {
			
		}
	}
```

In `<positions>` replace it with the position where your subModule is going to be! to add a z cord just do `z.pos(new) = <positions>` and in data script is where you write all the scripts for the subModule. To Begin First Make a new line in `dataScript` like this `newStringType = textDisplay("<text>")` Then Underneath write `string.linkUrl('<url>')`, Then underneath that line type `save(gitmodule(tagname))`, now build your site and your done!

If You want to change your Link Url Color for the subModule just do `linkCrl = new('#(<colorCodeName>)')`. You can use this [link]() to find color codes!

We Have A Full Guide On How dataScript(s) work for each class! in this guide we will go over TTType! but here are the guides!
- [TWar]()
- [Snd]()

### More Docementations on the [Homepage](https://kadedevteam.github.io/Documentations/)
