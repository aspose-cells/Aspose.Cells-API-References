##Aspose::Cells::Properties::DocumentPropertyCollection class
'Aspose::Cells::Properties::DocumentPropertyCollection class. Base class for BuiltInDocumentPropertyCollection and CustomDocumentPropertyCollection collections in C++.'
## DocumentPropertyCollection class
Base class for [BuiltInDocumentPropertyCollection](../builtindocumentpropertycollection/) and [CustomDocumentPropertyCollection](../customdocumentpropertycollection/) collections.
```cpp
class DocumentPropertyCollection
```
## Methods
| Method | Description |
| --- | --- |
| [Contains(const U16String\& name)](./contains/) | Returns true if a property with the specified name exists in the collection. |
| [Contains(const char16_t* name)](./contains/) | Returns true if a property with the specified name exists in the collection. |
| [DocumentPropertyCollection(DocumentPropertyCollection_Impl* impl)](./documentpropertycollection/) | Constructs from an implementation object. |
| [DocumentPropertyCollection(const DocumentPropertyCollection\& src)](./documentpropertycollection/) | Copy constructor. |
| [Get(int32_t index)](./get/) | Returns a [DocumentProperty](../documentproperty/) object by index. |
| [Get(const U16String\& name)](./get/) | Returns a [DocumentProperty](../documentproperty/) object by the name of the property. |
| [Get(const char16_t* name)](./get/) | Returns a [DocumentProperty](../documentproperty/) object by the name of the property. |
| [GetCount()](./getcount/) |  |
| [IndexOf(const U16String\& name)](./indexof/) | Gets the index of a property by name. |
| [IndexOf(const char16_t* name)](./indexof/) | Gets the index of a property by name. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const DocumentPropertyCollection\& src)](./operator_asm/) | operator= |
| [Remove(const U16String\& name)](./remove/) | Removes a property with the specified name from the collection. |
| [Remove(const char16_t* name)](./remove/) | Removes a property with the specified name from the collection. |
| [RemoveAt(int32_t index)](./removeat/) | Removes a property at the specified index. |
| [~DocumentPropertyCollection()](./~documentpropertycollection/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
//Instantiate a Workbook object by calling its empty constructor
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
