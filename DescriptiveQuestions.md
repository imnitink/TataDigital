First Question - All you need to do is replace Row with Wrap.Normally when you want to layout multiple widgets horizontally or vertically you can use a row or column.But if there is not enough room the content gets clipped and you get the yellow and black overflow warning.To fix that you can use a Wrap widget instead of a Row.


Second Question - It blocks your app because counting to ten billion is a computationally expensive task, even for a computer.Dart code runs inside its own area of memory called an isolate — also known as memory thread. Each isolate has its own memory heap, which ensures that no isolate can access any other isolate's state.The solution is to run it on a different isolate


Third Question - When using the var keyword, the Data type is inferred and its value can change.With final and const, you can’t reassign a new value after the initial assignment. final values are assigned once at runtime and a const variable value has to be either known at compile time, set, or hard coded before you run your app.

The third line will compile. You’re not reassigning the list2 list itself, but changing the value of an item in the third index position

The fourth line will not compile because the value of list1 isn’t assigned until runtime. 
