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
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            workbook.Worksheets[1].Cells[&quot;A1&quot;].PutValue(&quot;hello&quot;);
            workbook.Worksheets.SwapSheet(0, 1);
            Assert.AreEqual(&quot;hello&quot;, workbook.Worksheets[0].Cells[&quot;A1&quot;].StringValue);
        }
```

### See Also

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


