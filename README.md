# flutter_bs_porter

A new Flutter project.

## App features
This is simple Flutter app that when it's opened it will show a screen with a counter that it's incremented every second. The interesting thing is that the counter never stops counting. No matter if you remove the app from recent apps or Android system kills the process to reclaim more memory. The app always recovers from any situation and keeps counting. Just uninstall the app if you want to stop it.

These are the techniques used by this project to keep Flutter running:

Use of ==moveTaskToBack== to survive when back button is pressed.
Creation of a foreground service to increase process priority.
Start and stop a new Isolate to run Dart background code when FlutterActivity is destroyed.

## How to run the project
- Follow Get Started tutorial and install Flutter
- Start and Android emulator
- Run the app from ==terminal== with flutter ==run==
