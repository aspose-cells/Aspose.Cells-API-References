##Aspose::Cells::Properties::CustomDocumentPropertyCollection class
'Aspose::Cells::Properties::CustomDocumentPropertyCollection class. A collection of custom document properties in C++.'
## CustomDocumentPropertyCollection class
A collection of custom document properties.
```cpp
class CustomDocumentPropertyCollection : public Aspose::Cells::Properties::DocumentPropertyCollection
```
## Methods
| Method | Description |
| --- | --- |
| [Add(const U16String\& name, const U16String\& value)](./add/) | Creates a new custom document property of the **[PropertyType.String](../propertytype/)** data type. |
| [Add(const char16_t* name, const char16_t* value)](./add/) | Creates a new custom document property of the **[PropertyType.String](../propertytype/)** data type. |
| [Add(const U16String\& name, int32_t value)](./add/) | Creates a new custom document property of the **[PropertyType.Number](../propertytype/)** data type. |
| [Add(const char16_t* name, int32_t value)](./add/) | Creates a new custom document property of the **[PropertyType.Number](../propertytype/)** data type. |
| [Add(const U16String\& name, const Date\& value)](./add/) | Creates a new custom document property of the **[PropertyType.DateTime](../propertytype/)** data type. |
| [Add(const char16_t* name, const Date\& value)](./add/) | Creates a new custom document property of the **[PropertyType.DateTime](../propertytype/)** data type. |
| [Add(const U16String\& name, bool value)](./add/) | Creates a new custom document property of the **[PropertyType.Boolean](../propertytype/)** data type. |
| [Add(const char16_t* name, bool value)](./add/) | Creates a new custom document property of the **[PropertyType.Boolean](../propertytype/)** data type. |
| [Add(const U16String\& name, double value)](./add/) | Creates a new custom document property of the **PropertyType.Float** data type. |
| [Add(const char16_t* name, double value)](./add/) | Creates a new custom document property of the **PropertyType.Float** data type. |
| [AddLinkToContent(const U16String\& name, const U16String\& source)](./addlinktocontent/) | Creates a new custom document property which links to content. |
| [AddLinkToContent(const char16_t* name, const char16_t* source)](./addlinktocontent/) | Creates a new custom document property which links to content. |
| [Contains(const U16String\& name)](../documentpropertycollection/contains/) | Returns true if a property with the specified name exists in the collection. |
| [Contains(const char16_t* name)](../documentpropertycollection/contains/) | Returns true if a property with the specified name exists in the collection. |
| [CustomDocumentPropertyCollection(CustomDocumentPropertyCollection_Impl* impl)](./customdocumentpropertycollection/) | Constructs from an implementation object. |
| [CustomDocumentPropertyCollection(const CustomDocumentPropertyCollection\& src)](./customdocumentpropertycollection/) | Copy constructor. |
| [CustomDocumentPropertyCollection(const DocumentPropertyCollection\& src)](./customdocumentpropertycollection/) | Constructs from a parent object. |
| [DocumentPropertyCollection(DocumentPropertyCollection_Impl* impl)](../documentpropertycollection/documentpropertycollection/) | Constructs from an implementation object. |
| [DocumentPropertyCollection(const DocumentPropertyCollection\& src)](../documentpropertycollection/documentpropertycollection/) | Copy constructor. |
| [Get(int32_t index)](../documentpropertycollection/get/) | Returns a [DocumentProperty](../documentproperty/) object by index. |
| [Get(const U16String\& name)](../documentpropertycollection/get/) | Returns a [DocumentProperty](../documentproperty/) object by the name of the property. |
| [Get(const char16_t* name)](../documentpropertycollection/get/) | Returns a [DocumentProperty](../documentproperty/) object by the name of the property. |
| [GetCount()](../documentpropertycollection/getcount/) |  |
| [IndexOf(const U16String\& name)](../documentpropertycollection/indexof/) | Gets the index of a property by name. |
| [IndexOf(const char16_t* name)](../documentpropertycollection/indexof/) | Gets the index of a property by name. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const CustomDocumentPropertyCollection\& src)](./operator_asm/) | operator= |
| [operator=(const DocumentPropertyCollection\& src)](../documentpropertycollection/operator_asm/) | operator= |
| [Remove(const U16String\& name)](../documentpropertycollection/remove/) | Removes a property with the specified name from the collection. |
| [Remove(const char16_t* name)](../documentpropertycollection/remove/) | Removes a property with the specified name from the collection. |
| [RemoveAt(int32_t index)](../documentpropertycollection/removeat/) | Removes a property at the specified index. |
| [UpdateLinkedPropertyValue()](./updatelinkedpropertyvalue/) | Updates values of all custom properties that are linked to content(use cell value of linked range to update value of custom property). |
| [UpdateLinkedRange()](./updatelinkedrange/) | Updates all ranges that are linked to custom properties(use the value of custom document property to update cell value of linked range). |
| [~CustomDocumentPropertyCollection()](./~customdocumentpropertycollection/) | Destructor. |
| [~DocumentPropertyCollection()](../documentpropertycollection/~documentpropertycollection/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Remarks
Each [DocumentProperty](../documentproperty/) object represents a custom property of a container document.
## Examples
```cpp
Aspose::Cells::Startup();
//Instantiate a Workbook object
Workbook workbook(u"book1.xls");
//Retrieve a list of all custom document properties of the Excel file
CustomDocumentPropertyCollection customProperties = workbook.GetWorksheets().GetCustomDocumentProperties();
Aspose::Cells::Cleanup();
```
## See Also
* Class [DocumentPropertyCollection](../documentpropertycollection/)
* Namespace [Aspose::Cells::Properties](../)
* Library [Aspose.Cells for C++](../../)
