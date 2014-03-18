#Gimmie for Unity
=================
Add Gimmie in
-------------
Extract the plugin and drop the files into Assets/Plugins.
Create a binding class, you can use a basic one here: [GimmieBinding.cs](https://raw.github.com/kakadadroid/GimmieDocs/master/Unity%20Example/GimmieBinding.cs).
Modify/create your AndroidManifest.xml to include all the Gimmie declarations. See [example here](https://raw.github.com/kakadadroid/GimmieDocs/blob/master/Unity%20Example/AndroidManifest.xml).

The structure should look like this:
```
Assets
    Plugins
        Android
    	    AndroidManifest.xml
            gimmie_Android_SDK_Unity
    	GimmieBinding.cs
```


Initialize
-----------
Call the following to bind Gimmie to each new context, for example in Start():
```
	void Start(){
		GimmieBinding.initGimmie();
	}
```

Call Gimmie!
------------
Show rewards:
```
	GimmieBinding.ShowGimmieRewardsCatalogue();
```
Trigger event named "test_event":
```
	GimmieBinding.TriggerGimmieEvent("test_event");
```
