# C# Class

### 1. Accessibility
* internal: within program
* protected internal: within program and containing class

### 2. Base Class Inheritence
* public class Point3D: Point

### 3. Constant Field
* const int defaultCapacity = 4;

### 4. Property
* a wrapped variable field(sometimes)
* simplify getter and setter

### 5. Indexer
* getter and setter for array

### 6. Operator
```sh
   public static bool operator ==(List a, List b) {

      return Equals(a, b);

   }

   public static bool operator !=(List a, List b) {

      return !Equals(a, b);

   }
```

### 7. Virtual, Overide and New
* Method inheritance is different from Java
    * Method default is not virtual
    * Using virtual, then it's inherited and can be overide with "overide"
    * Or without virtual, using "new" to hide base class method

