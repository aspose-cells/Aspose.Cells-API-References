---
title: Class RowCollection
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.RowCollection class. Collects the  objects that represent the individual rows in a worksheet
type: docs
url: /net/aspose.cells/rowcollection/
---
## RowCollection class

Collects the  objects that represent the individual rows in a worksheet.

```csharp
public class RowCollection : IEnumerable
```

## Properties

| Name | Description |
| --- | --- |
| [Count](../../aspose.cells/rowcollection/count/) { get; } | Gets the number of rows in this collection. |
| [Item](../../aspose.cells/rowcollection/item/) { get; } | Gets a  object by given row index. The Row object of given row index will be instantiated if it does not exist before. |

## Methods

| Name | Description |
| --- | --- |
| [Clear](../../aspose.cells/rowcollection/clear/)() | Clear all rows and cells. |
| [GetEnumerator](../../aspose.cells/rowcollection/getenumerator/#getenumerator)() | Gets an enumerator that iterates rows through this collection |
| [GetEnumerator](../../aspose.cells/rowcollection/getenumerator/#getenumerator_1)(bool, bool) | Gets an enumerator that iterates rows through this collection |
| [GetRowByIndex](../../aspose.cells/rowcollection/getrowbyindex/)(int) | Gets the row object by the position in the list. |
| [RemoveAt](../../aspose.cells/rowcollection/removeat/)(int) | Remove the row at the specified index |

### Examples

```csharp

[C#]

//Instantiating a Workbook object
Workbook workbook = new Workbook();

//Obtaining the reference of the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
 //Get first row
Row row = worksheet.Cells.Rows[0];

[VB.NET]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()

'Obtaining the reference of the first worksheet
Dim worksheet As Worksheet = workbook.Worksheets(0)
'Get first row
Dim row as Row = worksheet.Cells.Rows(0)
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


