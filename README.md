# **Flutter Camp " DNA Turkey"**

***

## <u>Flutter #01</u>

1- StatefulWidget

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(const MyApp());
}

class MyApp extends StatefulWidget {
  const MyApp({Key? key}) : super(key: key);

  @override
  _MyAppState createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  @override
  Widget build(BuildContext context) {
    return Container();
  }
}
```

***

2- StatelessWidget

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(const MyApp());
}

class MyApp extends StatelessWidget {
  const MyApp({Key? key}) : super(key: key);

  @override
  Widget build(BuildContext context) {
    return Container();
  }
}
```

***

3- Scaffold

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: MyApp(),));
}

class MyApp extends StatefulWidget {
  const MyApp({Key? key}) : super(key: key);

  @override
  _MyAppState createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  @override
  Widget build(BuildContext context) {
    return Scaffold();
  }
}
```


<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p1.png" alt="p1.png">
</p>


***

4- Change Background Color 

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: MyApp(),));
}

class MyApp extends StatefulWidget {
  const MyApp({Key? key}) : super(key: key);

  @override
  _MyAppState createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.deepPurpleAccent,
    );
  }
}
```


<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p2.png" alt="p2.png">
</p>


***

5- App Bar

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: MyApp(),));
}

class MyApp extends StatefulWidget {
  const MyApp({Key? key}) : super(key: key);

  @override
  _MyAppState createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.white,
      appBar: AppBar(backgroundColor: Colors.black,title: Text("DNA SCHOLARSHIP"),),
    );
  }
}
```

<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p3.png" alt="p3.png">
</p>

***

6- Body and Text

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: MyApp(),));
}

class MyApp extends StatefulWidget {
  const MyApp({Key? key}) : super(key: key);

  @override
  _MyAppState createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.white,
      appBar: AppBar(backgroundColor: Colors.black,title: Text("DNA SCHOLARSHIP"),),
      body: Text("Test Text",style: TextStyle(fontSize: 20,color: Colors.deepPurpleAccent),),
    );
  }
}
```


<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p4.png" alt="p4.png">
</p>

***

7- Center

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: MyApp(),));
}

class MyApp extends StatefulWidget {
  const MyApp({Key? key}) : super(key: key);

  @override
  _MyAppState createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.white,
      appBar: AppBar(backgroundColor: Colors.black,title: Text("DNA SCHOLARSHIP"),),
      body: Center(
        child: Text("Test Text",style: TextStyle(fontSize: 20,color: Colors.deepPurpleAccent),),
      )
    );
  }
}
```


<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p5.png" alt="p5.png">
</p>

***

8- Container

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: MyApp(),));
}

class MyApp extends StatefulWidget {
  const MyApp({Key? key}) : super(key: key);

  @override
  _MyAppState createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.white,
      appBar: AppBar(backgroundColor: Colors.black,title: Text("DNA SCHOLARSHIP"),),
      body: Center(
        child: Container(
          height: 200,
          width: 200,
          color: Colors.amberAccent,
        )
      )
    );
  }
}
```


<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p6.png" alt="p6.png">
</p>

***

9- Container with Border Radius

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: MyApp(),));
}

class MyApp extends StatefulWidget {
  const MyApp({Key? key}) : super(key: key);

  @override
  _MyAppState createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.white,
      appBar: AppBar(backgroundColor: Colors.black,title: Text("DNA SCHOLARSHIP"),),
      body: Center(
        child: ClipRRect(
          borderRadius: BorderRadius.all(Radius.circular(50)),
          child: Container(
            height: 200,
            width: 200,
            color: Colors.amberAccent,
          ),
        )
      )
    );
  }
}
```

<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p7.png" alt="p7.png">
</p>

***

10- Child

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: MyApp(),));
}

class MyApp extends StatefulWidget {
  const MyApp({Key? key}) : super(key: key);

  @override
  _MyAppState createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.white,
      appBar: AppBar(backgroundColor: Colors.black,title: Text("DNA SCHOLARSHIP"),),
      body: Center(
        child: ClipRRect(
          borderRadius: BorderRadius.all(Radius.circular(50)),
          child: Container(
            height: 200,
            width: 200,
            color: Colors.amberAccent,
            child: Center(
              child: Text("HELLO",style: TextStyle(fontSize: 20,color: Colors.blue),),
            )
          ),
        )
      )
    );
  }
}
```

<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p8.png" alt="p8.png">
</p>

***

11- Icon

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: MyApp(),));
}

class MyApp extends StatefulWidget {
  const MyApp({Key? key}) : super(key: key);

  @override
  _MyAppState createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.white,
      appBar: AppBar(backgroundColor: Colors.black,title: Text("DNA SCHOLARSHIP"),),
      body: Center(
        child: ClipRRect(
          borderRadius: BorderRadius.all(Radius.circular(50)),
          child: Container(
            height: 200,
            width: 200,
            color: Colors.amberAccent,
            child: Center(
              child: Icon(Icons.add,size: 50,color: Colors.blue,)
            )
          ),
        )
      )
    );
  }
}
```

<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p9.png" alt="p9.png">
</p>

***

12- Image by Direct Link

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: MyApp(),));
}

class MyApp extends StatefulWidget {
  const MyApp({Key? key}) : super(key: key);

  @override
  _MyAppState createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.white,
      appBar: AppBar(backgroundColor: Colors.black,title: Text("DNA SCHOLARSHIP"),),
      body: Center(
        child: ClipRRect(
          borderRadius: BorderRadius.all(Radius.circular(50)),
          child: Container(
            height: 200,
            width: 200,
            color: Colors.amberAccent,
            child: Center(
              child: Image.network("https://w7.pngwing.com/pngs/340/946/png-transparent-avatar-user-computer-icons-software-developer-avatar-child-face-heroes.png")
            )
          ),
        )
      )
    );
  }
}
```


<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p10.png" alt="p10.png">
</p>


***

13- Image from File


<p align="center" width="100%">
    <img width="100%" src="Flutter Camp\p-11.jpg" alt="p-11.jpg">
</p>


<p align="center" width="100%">
    <img width="100%" src="Flutter Camp\p-12.jpg" alt="p-12.jpg">
</p>

***

14- Column

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: MyApp(),));
}

class MyApp extends StatefulWidget {
  const MyApp({Key? key}) : super(key: key);

  @override
  _MyAppState createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.white,
      appBar: AppBar(backgroundColor: Colors.black,title: Text("DNA SCHOLARSHIP"),),
      body: Column(
        children: [
          
          Container(
            height: 100,
            color: Colors.blue,
          ),

          Container(
            height: 100,
            color: Colors.amberAccent,
          ),

          Container(
            height: 100,
            color: Colors.deepPurpleAccent,
          ),

          Container(
            height: 100,
            color: Colors.deepOrange,
          ),

        ],
      )
    );
  }
}
```


<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p-13.png" alt="p-13.png">
</p>

***

16- Row

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: MyApp(),));
}

class MyApp extends StatefulWidget {
  const MyApp({Key? key}) : super(key: key);

  @override
  _MyAppState createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.white,
      appBar: AppBar(backgroundColor: Colors.black,title: Text("DNA SCHOLARSHIP"),),
      body: Row(
        children: [

          Container(
            width: 50,
            color: Colors.blue,
          ),

          Container(
            width: 50,
            color: Colors.amberAccent,
          ),

          Container(
            width: 50,
            color: Colors.deepPurpleAccent,
          ),

          Container(
            width: 50,
            color: Colors.deepOrange,
          ),

        ],
      )
    );
  }
}
```


<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p-14.png" alt="p-14.png">
</p>

***

17- Stack

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: MyApp(),));
}

class MyApp extends StatefulWidget {
  const MyApp({Key? key}) : super(key: key);

  @override
  _MyAppState createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.white,
      appBar: AppBar(backgroundColor: Colors.black,title: Text("DNA SCHOLARSHIP"),),
      body: Center(
        child: Stack(
          children: [

            Container(
              height: 200,
              width: 200,
              color: Colors.blue,
            ),

            Container(
              height: 150,
              width: 150,
              color: Colors.amberAccent,
            ),

            Container(
              height: 100,
              width: 100,
              color: Colors.deepPurpleAccent,
            ),

            Container(
              height: 50,
              width: 50,
              color: Colors.deepOrange,
            ),

          ],
        ),
      )
    );
  }
}
```


<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p-15.png" alt="p-15.png">
</p>

***

18- Column and Row

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: MyApp(),));
}

class MyApp extends StatefulWidget {
  const MyApp({Key? key}) : super(key: key);

  @override
  _MyAppState createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.white,
      appBar: AppBar(backgroundColor: Colors.black,title: Text("DNA SCHOLARSHIP"),),
      body: Column(
        children: [

          Container(
            height: 100,
            color: Colors.blue,
            child: Row(
              children: [
                Text("row1",style: TextStyle(fontSize: 25),),
                Text("row2",style: TextStyle(fontSize: 25),),
                Text("row3",style: TextStyle(fontSize: 25),)
              ],
            ),
          ),

          Container(
            height: 100,
            color: Colors.amberAccent,
            child: Row(
              children: [
                Text("row1",style: TextStyle(fontSize: 25),),
                Text("row2",style: TextStyle(fontSize: 25),),
                Text("row3",style: TextStyle(fontSize: 25),)
              ],
            ),
          ),

          Container(
            height: 100,
            color: Colors.deepPurpleAccent,
            child: Row(
              children: [
                Text("row1",style: TextStyle(fontSize: 25),),
                Text("row2",style: TextStyle(fontSize: 25),),
                Text("row3",style: TextStyle(fontSize: 25),)
              ],
            ),
          ),

          Container(
            height: 100,
            color: Colors.deepOrange,
            child: Row(
              children: [
                Text("row1",style: TextStyle(fontSize: 25),),
                Text("row2",style: TextStyle(fontSize: 25),),
                Text("row3",style: TextStyle(fontSize: 25),)
              ],
            ),
          ),

        ],
      )
    );
  }
}
```


<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p-16.png" alt="p-16.png">
</p>


***

19- Size Box

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: MyApp(),));
}

class MyApp extends StatefulWidget {
  const MyApp({Key? key}) : super(key: key);

  @override
  _MyAppState createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.white,
      appBar: AppBar(backgroundColor: Colors.black,title: Text("DNA SCHOLARSHIP"),),
      body: Column(
        children: [

          Container(
            height: 100,
            color: Colors.blue,
            child: Row(
              children: [
                Text("row1",style: TextStyle(fontSize: 25),),
                SizedBox(width: 20,),
                Text("row2",style: TextStyle(fontSize: 25),),
                SizedBox(width: 20,),
                Text("row3",style: TextStyle(fontSize: 25),)
              ],
            ),
          ),

          SizedBox(height: 50,),
          Container(
            height: 100,
            color: Colors.amberAccent,
            child: Row(
              children: [
                Text("row1",style: TextStyle(fontSize: 25),),
                SizedBox(width: 20,),
                Text("row2",style: TextStyle(fontSize: 25),),
                SizedBox(width: 20,),
                Text("row3",style: TextStyle(fontSize: 25),)
              ],
            ),
          ),
          SizedBox(height: 50,),
          Container(
            height: 100,
            color: Colors.deepPurpleAccent,
            child: Row(
              children: [
                Text("row1",style: TextStyle(fontSize: 25),),
                SizedBox(width: 20,),
                Text("row2",style: TextStyle(fontSize: 25),),
                SizedBox(width: 20,),
                Text("row3",style: TextStyle(fontSize: 25),)
              ],
            ),
          ),
          SizedBox(height: 50,),
          Container(
            height: 100,
            color: Colors.deepOrange,
            child: Row(
              children: [
                Text("row1",style: TextStyle(fontSize: 25),),
                SizedBox(width: 20,),
                Text("row2",style: TextStyle(fontSize: 25),),
                SizedBox(width: 20,),
                Text("row3",style: TextStyle(fontSize: 25),)
              ],
            ),
          ),

        ],
      )
    );
  }
}
```


<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p-17.png" alt="p-17.png">
</p>


***

20- Cross Axis & Main Axis

```dart
import 'package:flutter/cupertino.dart';
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: Page1(),));
}

class Page1 extends StatefulWidget {
  const Page1({Key? key}) : super(key: key);
  @override
  _Page1State createState() => _Page1State();
}

class _Page1State extends State<Page1> {

  @override
  void initState() {
    // TODO: implement initState
    super.initState();
  }
  
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.white,
      appBar: AppBar(backgroundColor: Colors.grey,title: Text("Emaar Co."),),
      body:Column(
        mainAxisAlignment: MainAxisAlignment.center,
        crossAxisAlignment: CrossAxisAlignment.center,
        children: [

          Container(
            height: 100,
            color: Colors.orange,
            child: Row(
              mainAxisAlignment: MainAxisAlignment.center,
              crossAxisAlignment: CrossAxisAlignment.center,
              children: [
                Text("row1",style: TextStyle(fontSize: 25),),
                SizedBox(width: 20,),
                Text("row2",style: TextStyle(fontSize: 25),),
                SizedBox(width: 20,),
                Text("row3",style: TextStyle(fontSize: 25),)
              ],
            ),
          ),

          SizedBox(height: 20,),
          Container(
            height: 100,
            color: Colors.deepPurple,
            child: Row(
              mainAxisAlignment: MainAxisAlignment.center,
              crossAxisAlignment: CrossAxisAlignment.center,
              children: [
                Text("row1",style: TextStyle(fontSize: 25),),
                SizedBox(width: 20,),
                Text("row2",style: TextStyle(fontSize: 25),),
                SizedBox(width: 20,),
                Text("row3",style: TextStyle(fontSize: 25),)
              ],
            ),
          ),

          SizedBox(height: 20,),
          Container(
            height: 100,
            color: Colors.blue,
            child: Row(
              mainAxisAlignment: MainAxisAlignment.center,
              crossAxisAlignment: CrossAxisAlignment.center,
              children: [
                Text("row1",style: TextStyle(fontSize: 25),),
                SizedBox(width: 20,),
                Text("row2",style: TextStyle(fontSize: 25),),
                SizedBox(width: 20,),
                Text("row3",style: TextStyle(fontSize: 25),)
              ],
            ),
          ),

          Container(
            height: 100,
            color: Colors.orange,
            child: Row(
              mainAxisAlignment: MainAxisAlignment.center,
              crossAxisAlignment: CrossAxisAlignment.center,
              children: [
                Text("row1",style: TextStyle(fontSize: 25),),
                SizedBox(width: 20,),
                Text("row2",style: TextStyle(fontSize: 25),),
                SizedBox(width: 20,),
                Text("row3",style: TextStyle(fontSize: 25),)
              ],
            ),
          ),
        ],
      )
    );
  }
}
```

<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p-18.png" alt="p-18.png">
</p>

***

21- Children Icon

```dart
import 'package:flutter/cupertino.dart';
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: Page1(),));
}

class Page1 extends StatefulWidget {
  const Page1({Key? key}) : super(key: key);
  @override
  _Page1State createState() => _Page1State();
}

class _Page1State extends State<Page1> {
  @override
  void initState() {
    // TODO: implement initState
    super.initState();
  }

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.white,
      appBar: AppBar(backgroundColor: Colors.grey,title: Text("Emaar Co."),),
      body:Column(
        mainAxisAlignment: MainAxisAlignment.center,
        crossAxisAlignment: CrossAxisAlignment.center,
        children: [
          Container(
            height: 100,
            color: Colors.orange,
            child: Row(
              mainAxisAlignment: MainAxisAlignment.spaceAround,
              crossAxisAlignment: CrossAxisAlignment.center,
              children: [
                Icon(Icons.call,size: 30,color: Colors.black,),
                Icon(Icons.home,size: 30,color: Colors.black,),
                Icon(Icons.info,size: 30,color: Colors.black,)
              ],
            ),
          ),
        ],
      )
    );
  }
}
```

<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p-19.png" alt="p-19.png">
</p>

***

22-  Margin

```dart
import 'package:flutter/cupertino.dart';
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: Page1(),));
}

class Page1 extends StatefulWidget {
  const Page1({Key? key}) : super(key: key);
  @override
  _Page1State createState() => _Page1State();
}

class _Page1State extends State<Page1> {
  @override
  void initState() {
    // TODO: implement initState
    super.initState();
  }
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.white,
      appBar: AppBar(backgroundColor: Colors.grey,title: Text("Emaar Co."),),
      body:Center(
        child: Container(
          margin: EdgeInsets.only(left: 80),
          height: 50,
          width: 250,
          color: Colors.orange,
          child: Center(
            child: Text(" EdgeInsets.only(left: 80) "),
          )
        ),
      )
    );
  }
}
```

<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p-20.png" alt="p-20.png">
</p>

***

23- Padding

```dart
import 'package:flutter/cupertino.dart';
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: Page1(),));
}

class Page1 extends StatefulWidget {
  const Page1({Key? key}) : super(key: key);
  @override
  _Page1State createState() => _Page1State();
}

class _Page1State extends State<Page1> {
  @override
  void initState() {
    // TODO: implement initState
    super.initState();
  }
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.white,
      appBar: AppBar(backgroundColor: Colors.grey,title: Text("Emaar Co."),),
      body:Center(
        child: Container(
          padding: EdgeInsets.only(left: 80),
          height: 50,
          width: 250,
          color: Colors.orange,
          child: Center(
            child: Text(" EdgeInsets.only(left: 80) "),
          )
        ),
      )
    );
  }
}
```

<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p-21.png" alt="p-21.png">
</p>

***

24- Button

```dart
import 'package:flutter/cupertino.dart';
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: Page1(),));
}

class Page1 extends StatefulWidget {
  const Page1({Key? key}) : super(key: key);
  @override
  _Page1State createState() => _Page1State();
}

class _Page1State extends State<Page1> {
  @override
  void initState() {
    // TODO: implement initState
    super.initState();
  }
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.white,
      appBar: AppBar(backgroundColor: Colors.grey,title: Text("Emaar Co."),),
      body:Center(
        child: ElevatedButton(
          onPressed: () {
          },
          child: Text("Press here"),
        ),
      )
    );
  }
}
```

<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\P-22.png" alt="P-22.png">
</p>

***

25- Button Radius

```dart
import 'package:flutter/cupertino.dart';
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: Page1(),));
}

class Page1 extends StatefulWidget {
  const Page1({Key? key}) : super(key: key);
  @override
  _Page1State createState() => _Page1State();
}

class _Page1State extends State<Page1> {
  @override
  void initState() {
    // TODO: implement initState
    super.initState();
  }

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.white,
      appBar: AppBar(backgroundColor: Colors.grey,title: Text("Emaar Co."),),
      body:Center(
        child: ElevatedButton(
          onPressed: () {
          },
          style: ElevatedButton.styleFrom(shape: new RoundedRectangleBorder(
            borderRadius: new BorderRadius.circular(30.0),
          ),),
          child: Text("Press here"),
        ),
      )
    );
  }
}
```

<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p-23.png" alt="p-23.png">
</p>

***

26- List View & List Title

```dart
import 'package:flutter/cupertino.dart';
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: Page1(),));
}

class Page1 extends StatefulWidget {
  const Page1({Key? key}) : super(key: key);
  @override
  _Page1State createState() => _Page1State();
}

class _Page1State extends State<Page1> {
  @override
  void initState() {
    // TODO: implement initState
    super.initState();
  }
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.white,
      appBar: AppBar(backgroundColor: Colors.grey,title: Text("Emaar Co."),),
      body:ListView.builder(
          itemCount: 5,
          itemBuilder: (BuildContext context,int index){
            return ListTile(
                leading: Icon(Icons.list),
                trailing: Text("GFG",
                  style: TextStyle(
                      color: Colors.green,fontSize: 15),),
                title:Text("List item $index")
            );
          }
      ),
    );
  }
}
```

<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p-24.png" alt="p-24.png">
</p>

***

27- Text Field

```dart
import 'package:flutter/cupertino.dart';
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: Page1(),));
}

class Page1 extends StatefulWidget {
  const Page1({Key? key}) : super(key: key);
  @override
  _Page1State createState() => _Page1State();
}

class _Page1State extends State<Page1> {
  @override
  void initState() {
    // TODO: implement initState
    super.initState();
  }
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.white,
      appBar: AppBar(backgroundColor: Colors.grey,title: Text("Emaar Co."),),
      body:Center(
        child:TextField(
          decoration: InputDecoration(
            border: OutlineInputBorder(),
            labelText: 'Full Name',
          ),
        )),
    );
  }
}
```

<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p-25.png" alt="p-25.png">
</p>

***

28- Text Field Type Password

```dart
import 'package:flutter/cupertino.dart';
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: Page1(),));
}

class Page1 extends StatefulWidget {
  const Page1({Key? key}) : super(key: key);
  @override
  _Page1State createState() => _Page1State();
}

class _Page1State extends State<Page1> {
  @override
  void initState() {
    // TODO: implement initState
    super.initState();
  }
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.white,
      appBar: AppBar(backgroundColor: Colors.grey,title: Text("Emaar Co."),),
      body:Center(
        child:TextField(
          obscureText: true,
          decoration: InputDecoration(
            border: OutlineInputBorder(),
            labelText: 'Password',
          ),
        )),
    );
  }
}
```

<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p-26.png" alt="p-26.png">
</p>

***

29- Radio Check => [Online](https://api.flutter.dev/flutter/material/RadioListTile-class.html)

```dart
import 'package:flutter/material.dart';

void main() => runApp(const MyApp());

class MyApp extends StatelessWidget {
  const MyApp({Key? key}) : super(key: key);
  static const String _title = 'Flutter Code Sample';

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: _title,
      home: Scaffold(
        appBar: AppBar(title: const Text(_title)),
        body: const MyStatefulWidget(),
      ),
    );
  }
}
enum SingingCharacter { lafayette, jefferson }
class MyStatefulWidget extends StatefulWidget {
  const MyStatefulWidget({Key? key}) : super(key: key);
  @override
  State<MyStatefulWidget> createState() => _MyStatefulWidgetState();
}
class _MyStatefulWidgetState extends State<MyStatefulWidget> {
  SingingCharacter? _character = SingingCharacter.lafayette;
  @override
  Widget build(BuildContext context) {
    return Column(
      children: <Widget>[
        RadioListTile<SingingCharacter>(
          title: const Text('Lafayette'),
          value: SingingCharacter.lafayette,
          groupValue: _character,
          onChanged: (SingingCharacter? value) {
            setState(() {
              _character = value;
            });
          },
        ),
        RadioListTile<SingingCharacter>(
          title: const Text('Thomas Jefferson'),
          value: SingingCharacter.jefferson,
          groupValue: _character,
          onChanged: (SingingCharacter? value) {
            setState(() {
              _character = value;
            });
          },
        ),
      ],
    );
  }
}
```

<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p-27.png" alt="p-27.png">
</p>

***

30- Check Box

```dart
import 'package:flutter/cupertino.dart';
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: GetCheckValue(),));
}

class GetCheckValue extends StatefulWidget {
  @override
  GetCheckValueState createState() {
    return new GetCheckValueState();
  }
}

class GetCheckValueState extends State<GetCheckValue> {
  bool _isChecked = true;
  String _currText = '';

  List<String> text = [ "Flutter.io"];

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text("Get check Value Example"),
      ),
      body: Column(
        children: <Widget>[
          Expanded(
            child: Center(
              child: Text(_currText,
                  style: TextStyle(
                    fontSize: 20.0,
                    fontWeight: FontWeight.bold,
                  )),
            ),
          ),
          Expanded(
              child: Container(
                height: 350.0,
                child: Column(
                  children: text
                      .map((t) => CheckboxListTile(
                    title: Text(t),
                    value: _isChecked,
                    onChanged: (val) {
                      setState(() {
                        _isChecked = val!;
                        if (val == true) {
                          _currText = t;
                        }
                      });
                    },
                  ))
                      .toList(),
                ),
              )),
        ],
      ),
    );
  }
}
```

<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p-28.png" alt="p-28.png">
</p>

***

31- Option List

```dart
import 'package:flutter/material.dart';

void main() => runApp(const MyApp());

class MyApp extends StatelessWidget {
  const MyApp({Key? key}) : super(key: key);

  static const String _title = 'Flutter Code Sample';

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: _title,
      home: Scaffold(
        appBar: AppBar(title: const Text(_title)),
        body: const Center(
          child: MyStatefulWidget(),
        ),
      ),
    );
  }
}

class MyStatefulWidget extends StatefulWidget {
  const MyStatefulWidget({Key? key}) : super(key: key);

  @override
  State<MyStatefulWidget> createState() => _MyStatefulWidgetState();
}

class _MyStatefulWidgetState extends State<MyStatefulWidget> {
  String dropdownValue = 'One';

  @override
  Widget build(BuildContext context) {
    return DropdownButton<String>(
      value: dropdownValue,
      icon: const Icon(Icons.arrow_downward),
      elevation: 16,
      style: const TextStyle(color: Colors.deepPurple),
      underline: Container(
        height: 2,
        color: Colors.deepPurpleAccent,
      ),
      onChanged: (String? newValue) {
        setState(() {
          dropdownValue = newValue!;
        });
      },
      items: <String>['One', 'Two', 'Free', 'Four']
          .map<DropdownMenuItem<String>>((String value) {
        return DropdownMenuItem<String>(
          value: value,
          child: Text(value),
        );
      }).toList(),
    );
  }
}
```

<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p-29.png" alt="p-29.png">
</p>

***

32- Card

```dart
import 'package:flutter/cupertino.dart';
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: Page1(),));
}

class Page1 extends StatefulWidget {
  const Page1({Key? key}) : super(key: key);
  @override
  _Page1State createState() => _Page1State();
}

class _Page1State extends State<Page1> {
  @override
  void initState() {
    // TODO: implement initState
    super.initState();
  }
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.white,
      appBar: AppBar(backgroundColor: Colors.grey,title: Text("Emaar Co."),),
      body:Center(
        child:Card(
          elevation: 2,
          child: Container(
            height:80,
            width: 350,
            child: Center(
              child: Text(
                "Hello i am Card"
              ),
            ),
          ),
        )
      ),
    );
  }
}
```

<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p-30.png" alt="p-30.png">
</p>

***

33- Login Card UI

```dart
import 'package:flutter/material.dart';

void main() => runApp(const MyApp());

class MyApp extends StatelessWidget {
  const MyApp({Key? key}) : super(key: key);

  static const String _title = 'Sample App';

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: _title,
      home: Scaffold(

        body: const MyStatefulWidget(),
      ),
    );
  }
}

class MyStatefulWidget extends StatefulWidget {
  const MyStatefulWidget({Key? key}) : super(key: key);

  @override
  State<MyStatefulWidget> createState() => _MyStatefulWidgetState();
}

class _MyStatefulWidgetState extends State<MyStatefulWidget> {
  TextEditingController nameController = TextEditingController();
  TextEditingController passwordController = TextEditingController();

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      body: Center(
        child: Card(
          elevation: 5,
          child: Container(
            height: 500,
            width: 350,
            decoration: BoxDecoration(
                border: Border.all(color: Colors.blueAccent)
            ),
            child: Padding(
                padding: const EdgeInsets.all(20),
                child: ListView(
                  children: <Widget>[
                    Container(
                        alignment: Alignment.center,
                        padding: const EdgeInsets.all(10),
                        child: const Text(
                          'TutorialKart',
                          style: TextStyle(
                              color: Colors.blue,
                              fontWeight: FontWeight.w500,
                              fontSize: 30),
                        )),
                    Container(
                        alignment: Alignment.center,
                        padding: const EdgeInsets.all(10),
                        child: const Text(
                          'Sign in',
                          style: TextStyle(fontSize: 20),
                        )),
                    Container(
                      padding: const EdgeInsets.all(10),
                      child: TextField(
                        controller: nameController,
                        decoration: const InputDecoration(
                          border: OutlineInputBorder(),
                          labelText: 'User Name',
                        ),
                      ),
                    ),
                    Container(
                      padding: const EdgeInsets.fromLTRB(10, 10, 10, 0),
                      child: TextField(
                        obscureText: true,
                        controller: passwordController,
                        decoration: const InputDecoration(
                          border: OutlineInputBorder(),
                          labelText: 'Password',
                        ),
                      ),
                    ),
                    TextButton(
                      onPressed: () {
                        //forgot password screen
                      },
                      child: const Text('Forgot Password',),
                    ),
                    Container(
                        height: 50,
                        padding: const EdgeInsets.fromLTRB(10, 0, 10, 0),
                        child: ElevatedButton(
                          child: const Text('Login'),
                          onPressed: () {
                            print(nameController.text);
                            print(passwordController.text);
                          },
                        )
                    ),
                    Row(
                      children: <Widget>[
                        const Text('Does not have account?'),
                        TextButton(
                          child: const Text(
                            'Sign in',
                            style: TextStyle(fontSize: 20),
                          ),
                          onPressed: () {
                            //signup screen
                          },
                        )
                      ],
                      mainAxisAlignment: MainAxisAlignment.center,
                    ),
                  ],
                )),
          ),
        ),
      ),
    );
  }
}
```

<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p-31.png" alt="p-31.png">
</p>

***

34- Bottom Navigation Bar

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: MyApp(),));
}

class MyApp extends StatefulWidget {
  const MyApp({Key? key}) : super(key: key);
  @override
  _MyAppState createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.white,
      appBar: AppBar(backgroundColor: Colors.black,title: Text("DNA SCHOLARSHIP"),),
      bottomNavigationBar: BottomNavigationBar(
        items: const <BottomNavigationBarItem>[
          BottomNavigationBarItem(
            icon: Icon(Icons.home),
            label: 'Home',
          ),
          BottomNavigationBarItem(
            icon: Icon(Icons.business),
            label: 'Business',
          ),
          BottomNavigationBarItem(
            icon: Icon(Icons.school),
            label: 'School',
          ),
        ],
        currentIndex: _selectedIndex,
        selectedItemColor: Colors.amber[800],
        onTap: _onItemTapped,
      ),
      body: Text("Test Text",style: TextStyle(fontSize: 20,color: Colors.deepPurpleAccent),),
    );
  }
}
```

<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p-32.png" alt="p-32.png">
</p>

***

35- Routing or Navigator Between Pages

- Push => Go to new page

```dart
class FirstRoute extends StatelessWidget {
  const FirstRoute({Key? key}) : super(key: key);
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: const Text('First Route'),
      ),
      body: Center(
        child: ElevatedButton(
          child: const Text('Open route'),
          onPressed: () {
            // Navigate to second route when tapped.
          },
        ),
      ),
    );
  }
}

class SecondRoute extends StatelessWidget {
  const SecondRoute({Key? key}) : super(key: key);

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: const Text('Second Route'),
      ),
      body: Center(
        child: ElevatedButton(
          onPressed: () {
            // Navigate back to first route when tapped.
          },
          child: const Text('Go back!'),
        ),
      ),
    );
  }
}
```

- Pop => Get back to last page

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(const MaterialApp(
    title: 'Navigation Basics',
    home: FirstRoute(),
  ));
}

class FirstRoute extends StatelessWidget {
  const FirstRoute({Key? key}) : super(key: key);
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: const Text('First Route'),
      ),
      body: Center(
        child: ElevatedButton(
          child: const Text('Open route'),
          onPressed: () {
            Navigator.push(
              context,
              MaterialPageRoute(builder: (context) => const SecondRoute()),
            );
          },
        ),
      ),
    );
  }
}

class SecondRoute extends StatelessWidget {
  const SecondRoute({Key? key}) : super(key: key);
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: const Text('Second Route'),
      ),
      body: Center(
        child: ElevatedButton(
          onPressed: () {
            Navigator.pop(context);
          },
          child: const Text('Go back!'),
        ),
      ),
    );
  }
}
```

<p align="center" width="1000px">
    <img width="33%" src="Flutter Camp\p-33.png" alt="p-33.png">
</p>

***

36- Passing Data Between Pages

```
- After build all dart pages, We need to create new dart file called like (database.dart |or| data.dart).
- After that, We need to write all Variables and write the values.
- Then, We can use those data in anywhere. By the way, You must use the same variables names.
```

***

37- Add [Alert] Library => [Click Here](https://pub.dev/packages/cool_alert)

***

38- Add [Http] Library => [Click Here](https://pub.dev/packages/http)

***

39- Add [intl] Library => [Click Here](https://pub.dev/packages/intl)

***

40- Add [Flashy] Library => [Click Here](https://pub.dev/packages/flashy_tab_bar2)

***

41- Flutter Flow GUI & Deal With It => [Click Here](https://flutterflow.io/)


<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p-34.png" alt="p-34.png">
</p>

***

42- MySQL => GUI & Deal With It

**<u>Notice:</u>** Should Setup [Mamp] or Any Local Server on Your PC. <u>**[Click To Download MAMP](https://www.mamp.info/en/downloads/)**</u>.

<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p-35.png" alt="p-35.png">
</p>

***

43- MySQL => Insert Query

```mysql
INSERT INTO "table_name"
("column1", "column2", "column3", ...)
VALUES 
('value1', "value2", 'value3', ...); 
```

```mysql
INSERT INTO tb1 
(id, fname, lname, age, birthdate)
VALUES 
(1, 'Ahmed', 'Amer', 22, '1/2/2000');
```

***

44- MySQL => Update Query

```mysql
UPDATE table_name
SET 
column1 = value1, column2 = value2, ...
WHERE condition;
```

```mysql
UPDATE tb1
SET 
fname = 'Dev', lname = 'Mustafa', birthdate = '3/5/2000'
WHERE id = 2;
```

***

45- MySQL => Delete Query

```mysql
DELETE FROM table_name
WHERE 
condition;
```

```mysql
DELETE * FROM tb1
WHERE
id = 2;
```

***

46- MySQL => Select Query

```mysql
SELECT 
column1, column2, ...
FROM 
table_name;
```

```mysql
SELECT * FROM tb1;
```

```mysql
SELECT * FROM tb1
WHERE id = 2;
```

***

47- MySQL => Select Condition Query

```mysql
SELECT column1, column2, ...
FROM table_name
ORDER BY column1, column2, ... ASC|DESC;
```

```mysql
SELECT * FROM `tb1`
ORDER BY points DESC;
```

***

48- [Github](https://github.com/) 

<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p-36.png" alt="p-36.png">
</p>

***

49- End

p-37


