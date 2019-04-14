# C# Type

### 1. Pre-defined Type:
* object
* dynamic
* string: string can be treated as a value or an object(System.String) because of Operator Overloading
* Simple Type(value define or object define(System.ValueType)):
    * Non-value Type: bool, char('' only)
    * Value Type:
        * Integer Type:
            * 8-bit: sbyte, byte
            * 16-bit: short, ushort
            * 32-bit: int, uint
            * 64-bit: long, ulong
        * Floating Point Type:
            * decimal: 28 digits, e.g 12.30m
            * float: 7 digits, e.g 12.3f
            * double(default if not Ff,Mm hardcode): 15-16 digits(sign or not)

### 2. User-defined Type
* Class
* Struct
* Array
* Enum
* Delegate
* Interface

### 3. Stack and Heap
* Stack: Value type variable, parameter, reference
* Heap(GC): Object data

### 4. Type Convertion(WTH feature)
* X.TryParse() with Exception Handling
* Convert.Toint32 pick even number
* User-defined converter: IConvertible, TypeConverter

### 5. Function Parameter Type Defination
* out: simplify return, init within function, using ref at function defination and function call
* ref: simplify parameter passing(Bye *), init before function call, using ref before and at function defination and function call

### 6. dynamic Type
* throw Runtime Error but Compiled Error
* **Advantages:**
    * reduce using force casting
    * provide dynamic language call(python)
* **Constraints:**
    * Can't be function parameter
    * Must specify type befor implicit cast(in Delegate)
    * Can't call constructor or static function
    * Can't be base class, can't be generic class
* P.S.: var: php is the best programming language?

### 7. Type Safty
* A well-defined type guarantee for compiler
* Eliminate the implicit error like "Colorless green", which has correct grammar, but wrong meaning

### 8. Delegate, Event, vs Interface, Callback
* **Callback:** 
    * Provide a mechanisem for lower layer(API) to call upper layer(Application) methods
    * Java concept Example: Boss(implement Interface) assigned jobs(Interface) to employees. After each employee(call Interface(Boss Class)) finished, one has to notify(While calling employee, specify who the boss is) boss. Employee class is lower layer, and Boss class is upper layer
* Delegate vs Interface: a function pointer set, and a more flexible interface(don't have implement all fuctions)
* Event: Event Publisher(Trigger/Boss), Event Subscriber(Handler/Employee)
* Delegate and Event: Delegate provides a simple way to subscribe(specify Boss) based on Callback mechanism

### 9. array and Array
* array
    * n-D array: int[,] twoDim = new int[3,3];
    * Jagged array: int[][] jagged = new int[3][];(array of vectors)
* Array
    * Multiple CreateInstance() overloading
    * Clone(): Deep copy value type, shadow copy reference type(unless implements IClonable)
    * Copy(): Deep copy
    * Sort(): IComparable
    * Covariant&Contravariant: Base Class<=>Derived Class
    * ArraySegment<T>: window reference
 
### 10. Enum
* default tpye: int, or use ":" define
* default first element = 0, and increasement = 1
* Enum.Parse(): int 1 == doulb 1? or string false == bool false?
    
### 11. Indexer: mark here, talk about it until in Class section



