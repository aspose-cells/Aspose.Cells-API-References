##Aspose::Cells::Drawing::OleObjectCollection class
'Aspose::Cells::Drawing::OleObjectCollection class. Represents embedded OLE objects in C++.'
## OleObjectCollection class
Represents embedded OLE objects.
```cpp
class OleObjectCollection
```
## Methods
| Method | Description |
| --- | --- |
| [Add(int32_t upperLeftRow, int32_t upperLeftColumn, int32_t height, int32_t width, const Vector \<uint8_t\>\& imageData)](./add/) | Adds an [OleObject](../oleobject/) to the collection. |
| [Add(int32_t upperLeftRow, int32_t upperLeftColumn, int32_t height, int32_t width, const Vector \<uint8_t\>\& imageData, const U16String\& linkedFile)](./add/) | Adds a linked [OleObject](../oleobject/) to the collection. |
| [Add(int32_t upperLeftRow, int32_t upperLeftColumn, int32_t height, int32_t width, const Vector \<uint8_t\>\& imageData, const char16_t* linkedFile)](./add/) | Adds a linked [OleObject](../oleobject/) to the collection. |
| [Clear()](./clear/) | Remove all embedded OLE objects. |
| [Get(int32_t index)](./get/) | Gets the [OleObject](../oleobject/) element at the specified index. |
| [GetCount()](./getcount/) |  |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [OleObjectCollection(OleObjectCollection_Impl* impl)](./oleobjectcollection/) | Constructs from an implementation object. |
| [OleObjectCollection(const OleObjectCollection\& src)](./oleobjectcollection/) | Copy constructor. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const OleObjectCollection\& src)](./operator_asm/) | operator= |
| [RemoveAt(int32_t index)](./removeat/) | Removes the element at the specified index. |
| [~OleObjectCollection()](./~oleobjectcollection/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Namespace [Aspose::Cells::Drawing](../)
* Library [Aspose.Cells for C++](../../)
