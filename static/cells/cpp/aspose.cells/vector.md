##Aspose::Cells::Vector class
'Aspose::Cells::Vector class. Vector template class. The elements are stored contiguously in C++.'
## Vector class
[Vector](./) template class. The elements are stored contiguously.
```cpp
template<typenameT>class Vector
```
| Parameter | Description |
| --- | --- |
| T |  |
## Methods
| Method | Description |
| --- | --- |
| [GetData()](./getdata/) const | Gets the address of the element array in this vector. |
| [GetLength()](./getlength/) const | Gets the length of the elements in this [Vector](./). |
| [IsNull()](./isnull/) const | Checks whether the element array is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator [bool()](./vector/) |
| [operator=(const Vector\& src)](./operator_asm/) | operator= |
| [operator[](int32_t index)](./operator[]/) const | Array subscript operator. |
| [Vector()](./vector/) | Default constructor. Constructs an empty [Vector](./). |
| [Vector(int32_t len, const T\& default_value)](./vector/) | Constructs an element [Vector](./) of the specified length. |
| [Vector(const T* data, int32_t len)](./vector/) | Constructs from an element array. All elements will be copied. |
| [Vector(std::initializer_list\<T\> init)](./vector/) | Constructs using initialization list. |
| [Vector(const Vector\& src)](./vector/) | Copy constructor. |
| [~Vector()](./~vector/) | Destructor. |
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
