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

# C# Collections (FCL)

### 1. System.Collections Interface
* IEnumerable<T>{IEnumerator<T>}
* ICollection<T> : IEnumerable<T>,...
* IList<T> : ICollection<T>,...
* IDictionary<TKey, TValue> : ICollection<KeyValuePair<TKey, TValue>>,...

### 2. Collections
* Dictionary<TKey, TValue>: linked array against collision, hash mapping
* SortedDictionary<TKey, TValue>: red-black tree, all O(logN)
* SortedList<TKey, TValue>: array, insert/delete O(N), search O(logN)
* List<T>: unit of 4-element array
* LinkedList<T>: double direction
* HashSet<T>: hash code as key
* SortedSet<T>
* Stack
* Queue

### 3. Thread Safety - System.Collections.Concurrent
* ConcurrentQueue
* ConcurrentStack
* ConcurrentBag: set
* ConcurrentDictionary
