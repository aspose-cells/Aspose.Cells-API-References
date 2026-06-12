---
title: Aspose::Cells::QueryTable class
linktitle: QueryTable
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::QueryTable class. Represents QueryTable information in C++.'
type: docs
weight: 12300
url: /sv/cpp/aspose.cells/querytable/
---
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
//Instansierar ett Workbook‑objekt
Workbook workbook(u"example.xlsx");

//Hämtar referensen till det första kalkylbladet
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//Hämtar den första frågetabellen i kalkylbladet om den finns
QueryTableCollection qts = worksheet.GetQueryTables();
if(!qts.IsNull() && qts.GetCount() != 0)
{
    QueryTable qt = worksheet.GetQueryTables().Get(0);
    //Hämtar visningsadressen för frågetabellen.
    U16String address = qt.GetResultRange().GetAddress();
}

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
