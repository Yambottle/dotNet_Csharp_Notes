# C# Generics

### 1. Better Code/Algorithm Reusability

### 2. Better Performance
* Skip boxing and unboxing while parsing from object to value

### 3. Better Type Safety
* Type Constraint ("where")
    * T : class | reference type : class, interface, delegate, array(but not System.Array)
    * T : struct | value type
    * T : unmanaged | non-reference type : not in Heap?
    * T : base class name/interface name | easy
    * T : new() | contain none-parameter constructor, must put at last among multi-constraints
    * Combo constraints: ordered
    * T : U | T is a base class of U, <T, U>
    * two generics: T, U
        * where T:class
        * where U:class
