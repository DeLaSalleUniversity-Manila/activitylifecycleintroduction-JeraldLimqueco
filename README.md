# activitylifecycleintroduction(with Logcat output)
activitylifecycleintroduction-JeraldLimqueco created by Classroom for GitHub

This assignment illustrates the Android activity lifecycle using Logcat.

## Problem:

Implement an Android application that displays Logs in Logcat when the following methods are called:

1. *onCreate()* - handles the creation of the activity object, and the loading of any static resources like themes, images, layouts, set up menus, and the like.

2. *onStart()* - executes every time the activity begins.

3. *onResume()* - executes when the activity is making a transition from the Paused state and into the Running state again.

4. *onPause()* - called when the activity is still partially visible.

5. *onSaveInstanceState()* - called before the activity gets destroyed, which means you get an opportunity to save any variables you want to retain.

6. *onStop()* - called when the activity is no longer visible on the screen.

7. *onRestart()* - called when activity was stopped but is started again later.

8. *onDestroy()* - called when the entire app is being shut down and unloaded from memory.

## Basig Logging:

```Java
  private static final String LOG_TAG = "MainActivity";
  ...
    @Override
    protected void onStop(){
        super.onStop();
        Log.d(LOG_TAG, "onStop() method was called");
    }
    ...
```

