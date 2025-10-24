##Aspose::Cells::Properties::ContentTypePropertyCollection class
'Aspose::Cells::Properties::ContentTypePropertyCollection class. A collection of ContentTypeProperty objects that represent additional information in C++.'
## ContentTypePropertyCollection class
A collection of [ContentTypeProperty](../contenttypeproperty/) objects that represent additional information.
```cpp
class ContentTypePropertyCollection
```
## Methods
| Method | Description |
| --- | --- |
| [Add(const U16String\& name, const U16String\& value)](./add/) | Adds content type property information. |
| [Add(const char16_t* name, const char16_t* value)](./add/) | Adds content type property information. |
| [Add(const U16String\& name, const U16String\& value, const U16String\& type)](./add/) | Adds content type property information. |
| [Add(const char16_t* name, const char16_t* value, const char16_t* type)](./add/) | Adds content type property information. |
| [ContentTypePropertyCollection(ContentTypePropertyCollection_Impl* impl)](./contenttypepropertycollection/) | Constructs from an implementation object. |
| [ContentTypePropertyCollection(const ContentTypePropertyCollection\& src)](./contenttypepropertycollection/) | Copy constructor. |
| [Get(int32_t index)](./get/) | Gets the content type property by the specific index. |
| [Get(const U16String\& name)](./get/) | Gets the content type property by the property name. |
| [Get(const char16_t* name)](./get/) | Gets the content type property by the property name. |
| [GetCount()](./getcount/) |  |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ContentTypePropertyCollection\& src)](./operator_asm/) | operator= |
| [~ContentTypePropertyCollection()](./~contenttypepropertycollection/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
//Instantiating a Workbook object
Workbook workbook;
//Add a new property.
workbook.GetContentTypeProperties().Add(u"Admin", u"Aspose", u"text");
//Save the Excel file
workbook.Save(u"book1.xlsm");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells::Properties](../)
* Library [Aspose.Cells for C++](../../)
