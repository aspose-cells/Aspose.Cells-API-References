##Aspose::Cells::ExternalLinkCollection class
'Aspose::Cells::ExternalLinkCollection class. Represents external links collection in a workbook in C++.'
## ExternalLinkCollection class
Represents external links collection in a workbook.
```cpp
class ExternalLinkCollection
```
## Methods
| Method | Description |
| --- | --- |
| [Add(const U16String\& fileName, const Vector \<U16String\>\& sheetNames)](./add/) | Adds an external link. |
| [Add(const char16_t* fileName, const Vector \<U16String\>\& sheetNames)](./add/) | Adds an external link. |
| [Add(DirectoryType directoryType, const U16String\& fileName, const Vector \<U16String\>\& sheetNames)](./add/) | Add an external link . |
| [Add(DirectoryType directoryType, const char16_t* fileName, const Vector \<U16String\>\& sheetNames)](./add/) | Add an external link . |
| [Clear()](./clear/) | Removes all external links. |
| [Clear(bool updateReferencesAsLocal)](./clear/) | Removes all external links. |
| [ExternalLinkCollection(ExternalLinkCollection_Impl* impl)](./externallinkcollection/) | Constructs from an implementation object. |
| [ExternalLinkCollection(const ExternalLinkCollection\& src)](./externallinkcollection/) | Copy constructor. |
| [Get(int32_t index)](./get/) | Gets the [ExternalLink](../externallink/) element at the specified index. |
| [GetCount()](./getcount/) | Gets the number of elements actually contained in the collection. |
| [GetEnumerator()](./getenumerator/) | Get an enumerator that iterates through this collection. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ExternalLinkCollection\& src)](./operator_asm/) | operator= |
| [RemoveAt(int32_t index)](./removeat/) | Removes the specified external link from the workbook. |
| [RemoveAt(int32_t index, bool updateReferencesAsLocal)](./removeat/) | Removes the specified external link from the workbook. |
| [~ExternalLinkCollection()](./~externallinkcollection/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
//Open a file with external links
Workbook workbook(u"book1.xls");
//Change external link data source
workbook.GetWorksheets().GetExternalLinks().Get(0).SetDataSource(u"d:\\link.xls");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
