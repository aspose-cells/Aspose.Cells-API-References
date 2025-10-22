##Aspose::Cells::ExternalLink class
'Aspose::Cells::ExternalLink class. Represents an external link in a workbook in C++.'
## ExternalLink class
Represents an external link in a workbook.
```cpp
class ExternalLink
```
## Methods
| Method | Description |
| --- | --- |
| [AddExternalName(const U16String\& text, const U16String\& referTo)](./addexternalname/) | Adds an external name. |
| [AddExternalName(const char16_t* text, const char16_t* referTo)](./addexternalname/) | Adds an external name. |
| [ExternalLink(ExternalLink_Impl* impl)](./externallink/) | Constructs from an implementation object. |
| [ExternalLink(const ExternalLink\& src)](./externallink/) | Copy constructor. |
| [GetDataSource()](./getdatasource/) | Represents data source of the external link. |
| [GetOriginalDataSource()](./getoriginaldatasource/) | Represents stored data source of the external link. |
| [GetPathType()](./getpathtype/) | Get the path type of this external link. |
| [GetType()](./gettype/) | Gets the type of external link. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsReferred()](./isreferred/) | Indicates whether this external link is referenced by others. |
| [IsVisible()](./isvisible/) | Indicates whether this external link is visible in MS Excel. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ExternalLink\& src)](./operator_asm/) | operator= |
| [SetDataSource(const U16String\& value)](./setdatasource/) | Represents data source of the external link. |
| [SetDataSource(const char16_t* value)](./setdatasource/) | Represents data source of the external link. |
| [SetOriginalDataSource(const U16String\& value)](./setoriginaldatasource/) | Represents stored data source of the external link. |
| [SetOriginalDataSource(const char16_t* value)](./setoriginaldatasource/) | Represents stored data source of the external link. |
| [~ExternalLink()](./~externallink/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
//Open a file with external links
Workbook workbook(u"book1.xls");
//Get External Link
ExternalLink externalLink = workbook.GetWorksheets().GetExternalLinks().Get(0);
//Change External Link's Data Source
externalLink.SetDataSource(u"d:\\link.xls");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
