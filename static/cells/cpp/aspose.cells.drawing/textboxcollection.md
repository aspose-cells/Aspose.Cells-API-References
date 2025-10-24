##Aspose::Cells::Drawing::TextBoxCollection class
'Aspose::Cells::Drawing::TextBoxCollection class. Encapsulates a collection of TextBox objects in C++.'
## TextBoxCollection class
Encapsulates a collection of [TextBox](../textbox/) objects.
```cpp
class TextBoxCollection
```
## Methods
| Method | Description |
| --- | --- |
| [Add(int32_t upperLeftRow, int32_t upperLeftColumn, int32_t height, int32_t width)](./add/) | Adds a textbox to the collection. |
| [Clear()](./clear/) | Clear all text boxes. |
| [Get(int32_t index)](./get/) | Gets the [TextBox](../textbox/) element at the specified index. |
| [Get(const U16String\& name)](./get/) | Gets the [TextBox](../textbox/) element by the name. |
| [Get(const char16_t* name)](./get/) | Gets the [TextBox](../textbox/) element by the name. |
| [GetCount()](./getcount/) |  |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const TextBoxCollection\& src)](./operator_asm/) | operator= |
| [RemoveAt(int32_t index)](./removeat/) | Remove a text box from the file. |
| [TextBoxCollection(TextBoxCollection_Impl* impl)](./textboxcollection/) | Constructs from an implementation object. |
| [TextBoxCollection(const TextBoxCollection\& src)](./textboxcollection/) | Copy constructor. |
| [~TextBoxCollection()](./~textboxcollection/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
//Instantiating a Workbook object
Workbook workbook;
//get collection object
TextBoxCollection textBoxCollection = workbook.GetWorksheets().Get(0).GetTextBoxes();
//add a textbox
textBoxCollection.Add(1, 1, 50, 100);
for (int i = 0; i < textBoxCollection.GetCount(); ++i)
{
TextBox tbox = textBoxCollection.Get(i);
//do what you want
}
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells::Drawing](../)
* Library [Aspose.Cells for C++](../../)
