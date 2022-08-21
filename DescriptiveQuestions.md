First Question - Yes, we can nest a scaffold.That’s the beauty of Flutter. You control the entire UI. It is just a widget, so you can put it anywhere a widget might go. By nesting a Scaffold, you can layer drawers, snack bars and bottom sheets.

Second Question - You can create a custom widget by combining other widgets like container,text,Rows,column ,button etc, you can also draw it on a canvas that Flutter provides. You do this using CustomPainter.If you want to go really low level, it’s also possible to make widgets the same way that the Flutter framework does it by using RenderObjects.

Third Question - Platform channels can be used to access platform specific code from flutter. Two types of Platform channels are Method channels and Event Channels.

Method Channel- Data is serialized on the Dart side and then sent to the native side. You can write native code to interact with the platform before sending a serialized message back. That message might be written in Java or Kotlin on Android or Objective-C or Swift on iOS.

Event Channel - It use to send a stream of data from the native platform back to Flutter. This is useful for monitoring sensor data.

Fourth Question - BuildContext is, like it's name is implying, the context in which a specific widget is built. BuildContext is really useful when you want to pass data downward without having to manually assign it to every widgets' configurations for example ; you'll want to access them everywhere. But you don't want to pass it on every single constructor.
