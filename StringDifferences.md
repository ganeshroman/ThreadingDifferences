

# String, StringBuffer & StringBuilder Differences


## String
Since String is ***immutable*** in Java, whenever we do String manipulation like concatenation, substring, etc. it generates a new String and discards the older String for garbage collection.

## StringBuffer & StringBuilder
StringBuffer and StringBuilder are ***mutable*** objects in Java. They provide append(), insert(), delete(), and substring() methods for String manipulation.


| StringBuffer |  StringBuilder |
|----------|:---------:|
| StringBuffer is ***synchronized i.e. thread safe.*** It means two threads can't call the methods of StringBuffer simultaneously. | StringBuilder is ***non-synchronized i.e. not thread safe.*** It means two threads can call the methods of StringBuilder simultaneously.|
| StringBuffer is less efficient than StringBuilder. |StringBuilder is more efficient than StringBuffer.  |
| StringBuffer was introduced in Java 1.0	 |StringBuilder was introduced in Java 1.5  |





