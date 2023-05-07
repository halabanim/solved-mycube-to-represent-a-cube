Download Link: https://assignmentchef.com/product/solved-mycube-to-represent-a-cube
<br>
java Design a class named MyCube to represent a cube. A cube is a three-dimensional solid object bounded by six square faces. Implement the MyCube class using composition. The MyCube class contains the following:

<ul>

 <li>A <strong>private</strong> instance variable named base (of type MySquare2D) that specifies the base square of a cube with default top left corner at (0, 0) and 10 for side length.</li>

 <li>A no-arg default constructor that creates a cube with default values.</li>

 <li>An overloaded constructor that creates a cube with the specified side length.</li>

 <li>An overloaded constructor that creates a cube with the specified top left corner coordinates (of type Point).</li>

 <li>An overloaded constructor that creates a cube with the specified top left corner (of type Point) and side length.</li>

 <li>An overloaded constructor that creates a cube with the specified x, y coordinates and side length.</li>

 <li>An overloaded constructor that creates a cube with the specified base (of type MySquare2D).</li>

 <li>The toString() method that returns a string describing the object as shown in the examples below. Note: the toString() of the MySquare2D class returns “MySquare2D:(x, y), side=d”.</li>

</ul>

Write the MyCube class in the answer box below assuming that the <strong>MySquare2D</strong> class is given.

Composition: A cube has 6 squares faces.

For example:

<table>

 <thead>

  <tr>

   <th scope="col">Test</th>

   <th scope="col">Result</th>

  </tr>

 </thead>

 <tbody>

  <tr>

   <td><pre>MyCube c1 = new MyCube(5);System.out.println(c1);MyCube c2 = new MyCube(10,20,5);System.out.println(c2);MyCube c3 = new MyCube(new Point(10,20));System.out.println(c3);MyCube c4 = new MyCube(new Point(10,20), 20);System.out.println(c4);MyCube c5 = new MyCube();System.out.println(c5);</pre></td>

   <td><pre>MyCube: MySquare2D:(0, 0), side=5MyCube: MySquare2D:(10, 20), side=5MyCube: MySquare2D:(10, 20), side=10MyCube: MySquare2D:(10, 20), side=20MyCube: MySquare2D:(0, 0), side=10</pre></td>

  </tr>

 </tbody>

</table>

add the following methods to your MyCube class to extend its functionality:

<ul>

 <li>The accessor and mutator methods for the base.</li>

 <li>The getVolume() method that returns the volume of a MyCube object.</li>

 <li>The getSurfaceArea() method that returns the surface area of a MyCube object. The surface area of a Mycube object is: 6 * base area.</li>

 <li>The getBase() method that returns the base of a MyCube object.</li>

</ul>

Write the entire MyCube class in the answer box below assuming that the MySquare class is given.

For example:

<table>

 <thead>

  <tr>

   <th scope="col">Test</th>

   <th scope="col">Result</th>

  </tr>

 </thead>

 <tbody>

  <tr>

   <td><pre>MyCube c1 = new MyCube(15);System.out.println(c1.getBase());System.out.printf("volume=%d
", c1.getVolume());System.out.printf("surface area=%d
", c1.getSurfaceArea());</pre></td>

   <td><pre>MySquare2D:(0, 0), side=15volume=3375surface area=1350</pre></td>

  </tr>

  <tr>

   <td><pre>MyCube c1 = new MyCube (10, 20, 30);System.out.println(c1.getBase());System.out.printf("volume=%d
", c1.getVolume());System.out.printf("surface area=%d
", c1.getSurfaceArea());</pre></td>

   <td><pre>MySquare2D:(10, 20), side=30volume=27000surface area=5400</pre></td>

  </tr>

  <tr>

   <td><pre>MySquare2D s1 = new MySquare2D(12, 23, 8);MyCube c1 = new MyCube(s1);System.out.printf("volume=%d
", c1.getVolume());System.out.printf("surface area=%d
", c1.getSurfaceArea());MySquare2D base = c1.getBase();System.out.println(base);</pre></td>

   <td><pre>volume=512surface area=384MySquare2D:(12, 23), side=8</pre></td>

  </tr>

 </tbody>

</table>