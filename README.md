# flutter_note


To select an entire widget in Flutter while using Android Studio on macOS, you can use the shortcut ``` Option + Up Arrow (⌥ + ↑). ```

```
SchedulerBinding.instance.addPostFrameCallback((_) {
  print("This runs after the current frame.");
});
```

```
WidgetsBinding.instance.addPostFrameCallback((_) {
  // Your UI update or async task
});
```


# Add Flutter

``` export PATH="/Users/thawdezin/Flutter/flutter/bin:$PATH" ```

## Upgrade Flutter
``` flutter pub upgrade --major-versions ```


### စာသားအစိမ်းလိုင်း Spelling မှား ဖျောက်ဖို့
``` Android 4.1.1: File -> Preferences -> Editor -> Inspections -> Proofreading -> Typo ```


### To clear all iOS related things

```
flutter clean
rm pubspec.lock
rm -rf ./ios/.symlinks
rm -rf ./ios/Pods
rm ./ios/Podfile.lock
flutter pub get
cd ios ; pod repo update ; pod update ; cd ..
flutter run
```


To fix an individual diagnostic, run one of:
  ```dart fix --apply --code=avoid_function_literals_in_foreach_calls ```
  ```dart fix --apply --code=duplicate_import ```
  ```dart fix --apply --code=unnecessary_string_interpolations ```
  ```dart fix --apply --code=unused_import ```

To fix all diagnostics, run:
  ```dart fix --apply```  
  
## Get CLI
``` dart pub global deactivate get_cli ```<br/>
``` dart pub global activate -s git https://github.com/knottx/get_cli.git ```<br/>
``` flutter pub global activate get_cli 1.8.0 ```<br/>  
