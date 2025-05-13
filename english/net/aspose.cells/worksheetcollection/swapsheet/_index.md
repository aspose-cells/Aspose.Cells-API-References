---
title: WorksheetCollection.SwapSheet
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection method. Swaps the two sheets
type: docs
url: /net/aspose.cells/worksheetcollection/swapsheet/
---
## WorksheetCollection.SwapSheet method

Swaps the two sheets.

```csharp
public void SwapSheet(int sheetIndex1, int sheetIndex2)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex1 | Int32 | The first worksheet. |
| sheetIndex2 | Int32 | The second worksheet. |

### Examples

```csharp
// Called: workbook.Worksheets.SwapSheet(0, 1);
public void WorksheetCollection_Method_SwapSheet()
{
    Workbook workbook = new Workbook();
    workbook.Worksheets.Add();
    workbook.Worksheets[1].Cells["A1"].PutValue("hello");
    workbook.Worksheets.SwapSheet(0, 1);
    Assert.AreEqual("hello", workbook.Worksheets[0].Cells["A1"].StringValue);
}
```

### See Also

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


