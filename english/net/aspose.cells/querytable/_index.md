---
title: Class QueryTable
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.QueryTable class. Represents QueryTable information
type: docs
url: /net/aspose.cells/querytable/
---
## QueryTable class

Represents QueryTable information.

```csharp
public class QueryTable
```

## Properties

| Name | Description |
| --- | --- |
| [AdjustColumnWidth](../../aspose.cells/querytable/adjustcolumnwidth/) { get; set; } | Returns or sets the AdjustColumnWidth of the object. |
| [ConnectionId](../../aspose.cells/querytable/connectionid/) { get; } | Gets the connection id of the query table. |
| [ExternalConnection](../../aspose.cells/querytable/externalconnection/) { get; } | Gets the relate external connection. |
| [Name](../../aspose.cells/querytable/name/) { get; } | Gets the name of querytable. |
| [PreserveFormatting](../../aspose.cells/querytable/preserveformatting/) { get; set; } | Returns or sets the PreserveFormatting of the object. |
| [ResultRange](../../aspose.cells/querytable/resultrange/) { get; } | Gets the range of the result. |

### Examples

```csharp

[C#]

//Instantiating a Workbook object
Workbook workbook = new Workbook();

//Obtaining the reference of the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
//Getting the first query table in the worksheet if exists
//QueryTable qt = worksheet.QueryTables[0];
//Getting display address of the query table.
//string address = qt.ResultRange.Address;

[VB.NET]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()

'Obtaining the reference of the first worksheet
Dim worksheet As Worksheet = workbook.Worksheets(0)
'Getting the first query table in the worksheet
QueryTable qt = worksheet.QueryTables[0];
'Getting display address of the query table.
string address = qt.ResultRange.Address;
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


