##Aspose::Cells::Enumerator class
'Aspose::Cells::Enumerator class. Enumeration template class, provides a simple way to iterate over a collection in C++.'
## Enumerator class
Enumeration template class, provides a simple way to iterate over a collection.
```cpp
template<typenameT>class Enumerator
```
| Parameter | Description |
| --- | --- |
| T |  |
## Methods
| Method | Description |
| --- | --- |
| [Enumerator(void* impl)](./enumerator/) | Constructs from an implementation object. Internal use. |
| [Enumerator(const Enumerator \<T\>\& src)](./enumerator/) | Copy constructor. |
| [GetCurrent()](./getcurrent/) | Gets the current element in the enumeration. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [MoveNext()](./movenext/) | Advances the enumerator to the next element of the enumeration and returns a boolean indicating whether an element is available. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const Enumerator \<T\>\& src)](./operator_asm/) | operator= |
| [Reset()](./reset/) | Resets the enumerator to the beginning of the enumeration. |
| [~Enumerator()](./~enumerator/) | Destructor. |
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
