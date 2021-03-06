LegacyBar is an open source and free ActionBar which works from Android 2.1 and up!

It features:
* A fully customizeable Action Bar
* 4 Built in base themes
* Integrates with current Menus
* Overflow on API 11+ Devices
* Dynamic Action Bar Item Count based on screen resolution
* Bottom Action Bar (beta)

Add it easily to your Layout:

```xml
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout 
  xmlns:android="http://schemas.android.com/apk/res/android"
  android:orientation="vertical"
  android:layout_width="fill_parent"
  android:layout_height="fill_parent">
  
  <legacybar.library.bar.LegacyBar
    android:id="@+id/actionbar"
    style="@style/actionbar" />
	
	<!-- your style definitions here -->
	
</LinearLayout>
```

Interact with it in your Activity and add Actions:

```csharp
// Find it from the resource
LegacyBar = FindViewById<Library.Bar.LegacyBar>(Resource.Id.actionbar);
// Set a home logo
LegacyBar.SetHomeLogo(Resource.Drawable.MyLogo);
// Add an Action
var action = new MenuItemLegacyBarAction(this, Resource.Id.menu_search, Resource.Drawable.ic_action_search, "Search");
LegacyBar.AddAction(action);
```

Fork it on [GitHub!](https://github.com/Cheesebaron/LegacyBar)

Device screenshot made with [breezi's placeit](http://placeit.breezi.com/)