# Android snippets

I love find and store information for future use. This repo is used to store all expirience and might of android. Here I do experiments, ideas, and so more.

## Code snippets description

### Menu in android
Menu in android can be created many diff. Using drawable:
1. Create Custom ```android.app.Fragment``` classes and xml-layouts for this.
2. ```MainActivity@onNavigationItemSelected``` store following code
```
    @SuppressLint("CommitTransaction") FragmentTransaction ft = getFragmentManager().beginTransaction();
```
and on click for items
```
ft.replace(R.id.container, fragmentImport);
```
after all clicks menus init
```ft.commit();```