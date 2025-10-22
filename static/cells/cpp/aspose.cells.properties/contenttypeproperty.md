##Aspose::Cells::Properties::ContentTypeProperty class
'Aspose::Cells::Properties::ContentTypeProperty class. Represents identifier information in C++.'
## ContentTypeProperty class
Represents identifier information.
```cpp
class ContentTypeProperty
```
## Methods
| Method | Description |
| --- | --- |
| [ContentTypeProperty(ContentTypeProperty_Impl* impl)](./contenttypeproperty/) | Constructs from an implementation object. |
| [ContentTypeProperty(const ContentTypeProperty\& src)](./contenttypeproperty/) | Copy constructor. |
| [GetName()](./getname/) | Returns or sets the name of the object. |
| [GetType()](./gettype/) | Gets and sets the type of the property. |
| [GetValue()](./getvalue/) | Returns or sets the value of the content type property. |
| [IsNillable()](./isnillable/) | Indicates whether the value could be empty. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ContentTypeProperty\& src)](./operator_asm/) | operator= |
| [SetIsNillable(bool value)](./setisnillable/) | Indicates whether the value could be empty. |
| [SetName(const U16String\& value)](./setname/) | Returns or sets the name of the object. |
| [SetName(const char16_t* value)](./setname/) | Returns or sets the name of the object. |
| [SetType(const U16String\& value)](./settype/) | Gets and sets the type of the property. |
| [SetType(const char16_t* value)](./settype/) | Gets and sets the type of the property. |
| [SetValue(const U16String\& value)](./setvalue/) | Returns or sets the value of the content type property. |
| [SetValue(const char16_t* value)](./setvalue/) | Returns or sets the value of the content type property. |
| [~ContentTypeProperty()](./~contenttypeproperty/) | Destructor. |
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
