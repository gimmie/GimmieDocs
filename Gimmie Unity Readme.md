#Gimmie for Unity
=================
Add Gimmie in
-------------
Extract the plugin and drop the files into Assets/Plugins.
The structure should look like this:
Assets
└── Plugins
    ├── Android
    │   ├── AndroidManifest.xml
    │   ├── gimmie_Android_SDK_Unity
    │   └──...
    └── GimmieBinding.cs


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