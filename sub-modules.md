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

Choose what kind of Substate you want to add and put it on the list at `Line 17` Make Sute to write it like this: (PS: MAKE SURE THE NAME IS THE SAME AS THE `.gitmodule` FILE YOU CREATED EARLIER)`var <name> = <type of substate>`  
```

```
