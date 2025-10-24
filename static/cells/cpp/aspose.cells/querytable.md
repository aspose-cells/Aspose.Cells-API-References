##Aspose::Cells::QueryTable class
'Aspose::Cells::QueryTable class. Represents QueryTable information in C++.'
## QueryTable class
Represents [QueryTable](./) information.
```cpp
class QueryTable
```
## Methods
| Method | Description |
| --- | --- |
| [GetAdjustColumnWidth()](./getadjustcolumnwidth/) | Returns or sets the AdjustColumnWidth of the object. |
| [GetConnectionId()](./getconnectionid/) | Gets the connection id of the query table. |
| [GetExternalConnection()](./getexternalconnection/) | Gets the relate external connection. |
| [GetName()](./getname/) | Gets the name of querytable. |
| [GetPreserveFormatting()](./getpreserveformatting/) | Returns or sets the PreserveFormatting of the object. |
| [GetResultRange()](./getresultrange/) | Gets the range of the result. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const QueryTable\& src)](./operator_asm/) | operator= |
| [QueryTable(QueryTable_Impl* impl)](./querytable/) | Constructs from an implementation object. |
| [QueryTable(const QueryTable\& src)](./querytable/) | Copy constructor. |
| [SetAdjustColumnWidth(bool value)](./setadjustcolumnwidth/) | Returns or sets the AdjustColumnWidth of the object. |
| [SetPreserveFormatting(bool value)](./setpreserveformatting/) | Returns or sets the PreserveFormatting of the object. |
| [~QueryTable()](./~querytable/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
//Instantiating a Workbook object
Workbook workbook(u"example.xlsx");
//Obtaining the reference of the first worksheet
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//Getting the first query table in the worksheet if exists
QueryTableCollection qts = worksheet.GetQueryTables();
if(!qts.IsNull() && qts.GetCount() != 0)
{
QueryTable qt = worksheet.GetQueryTables().Get(0);
//Getting display address of the query table.
U16String address = qt.GetResultRange().GetAddress();
}
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
