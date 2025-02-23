HashMap and HashTable are both implementations of the Map interface in Java, but they have some key differences:

1. **Synchronization**:
   - **HashMap**: Not synchronized. This means it is not thread-safe and should be used in a single-threaded environment or explicitly synchronized externally.
   - **HashTable**: Synchronized. It is thread-safe and can be used in a multi-threaded environment without external synchronization.

2. **Null Values**:
   - **HashMap**: Allows one null key and multiple null values.
   - **HashTable**: Does not allow any null key or value.

3. **Performance**:
   - **HashMap**: Generally faster because it is not synchronized. The lack of synchronization overhead leads to better performance in single-threaded applications.
   - **HashTable**: Slower due to synchronization overhead.

4. **Legacy**:
   - **HashMap**: Part of the Java Collections Framework introduced in Java 1.2.
   - **HashTable**: Older class that was part of the original version of Java (JDK 1.0). It is considered a legacy class now.

5. **Iterators**:
   - **HashMap**: Uses fail-fast iterators. If the map is structurally modified after the iterator is created (except through the iterator's own `remove` method), the iterator will throw a `ConcurrentModificationException`.
   - **HashTable**: Uses fail-safe iterators. Modifications to the table after the iterator is created do not affect the iterator and will not throw `ConcurrentModificationException`.

6. **Subclassing**:
   - **HashMap**: Can be subclassed to create custom map implementations.
   - **HashTable**: Less flexible for subclassing due to synchronized methods.

Here's a summary in a table format:

| Feature             | HashMap                      | HashTable                    |
|---------------------|------------------------------|------------------------------|
| Synchronization     | Not synchronized (thread-unsafe) | Synchronized (thread-safe)    |
| Null Keys/Values    | Allows one null key and multiple null values | Does not allow null keys or values |
| Performance         | Generally faster             | Slower due to synchronization overhead |
| Introduced in       | Java 1.2 (part of Collections Framework) | JDK 1.0 (legacy class)         |
| Iterators           | Fail-fast                    | Fail-safe                    |
| Subclassing         | Flexible                     | Less flexible                |

Choosing between the two depends on the specific requirements of the application, particularly regarding thread safety and performance considerations. For modern applications, `ConcurrentHashMap` is often preferred over `Hashtable` for better concurrency performance.