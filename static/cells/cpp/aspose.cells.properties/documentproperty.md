##Aspose::Cells::Properties::DocumentProperty class
'Aspose::Cells::Properties::DocumentProperty class. Represents a custom or built-in document property in C++.'
## DocumentProperty class
Represents a custom or built-in document property.
```cpp
class DocumentProperty
```
## Methods
| Method | Description |
| --- | --- |
| [DocumentProperty(DocumentProperty_Impl* impl)](./documentproperty/) | Constructs from an implementation object. |
| [DocumentProperty(const DocumentProperty\& src)](./documentproperty/) | Copy constructor. |
| [GetName()](./getname/) | Returns the name of the property. |
| [GetSource()](./getsource/) | The linked content source. |
| [GetType()](./gettype/) | Gets the data type of the property. |
| [GetValue()](./getvalue/) | Gets or sets the value of the property. |
| [IsGeneratedName()](./isgeneratedname/) | Returns true if this property does not have a name in the OLE2 storage and a unique name was generated only for the public API. |
| [IsLinkedToContent()](./islinkedtocontent/) | Indicates whether this property is linked to content. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const DocumentProperty\& src)](./operator_asm/) | operator= |
| [SetValue(const Aspose::Cells::Object\& value)](./setvalue/) | Gets or sets the value of the property. |
| [ToBool()](./tobool/) | Returns the property value as bool. |
| [ToDateTime()](./todatetime/) | Returns the property value as DateTime in local timezone. |
| [ToDouble()](./todouble/) | Returns the property value as double. |
| [ToInt()](./toint/) | Returns the property value as integer. |
| [ToString()](./tostring/) | Returns the property value as a string. |
| [~DocumentProperty()](./~documentproperty/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
//Instantiate a Workbook object
Workbook workbook(u"book1.xls");
//Retrieve a list of all custom document properties of the Excel file
DocumentPropertyCollection customProperties = workbook.GetWorksheets().GetCustomDocumentProperties();
//Accessng a custom document property by using the property index
DocumentProperty customProperty1 = customProperties.Get(3);
//Accessng a custom document property by using the property name
DocumentProperty customProperty2 = customProperties.Get(u"Owner");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells::Properties](../)
* Library [Aspose.Cells for C++](../../)
