---
title: PivotTable.ShowDetail
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Show the detail of one item in the data region to a new Table
type: docs
url: /net/aspose.cells.pivot/pivottable/showdetail/
---
## PivotTable.ShowDetail method

Show the detail of one item in the data region to a new Table.

```csharp
public void ShowDetail(int rowOffset, int columnOffset, bool newSheet, int destRow, int destColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | Int32 | Offset to the first data row in the data region. |
| columnOffset | Int32 | Offset to the first data column in the data region. |
| newSheet | Boolean | Show the detail to a new worksheet. |
| destRow | Int32 | The target row. |
| destColumn | Int32 | The target column. |

### Examples

```csharp
// Called: pt.ShowDetail(6, 1, true, 0, 0);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + &quot;CELLSJAVA41836.xlsx&quot;);
            PivotTable pt = workbook.Worksheets[0].PivotTables[0];
            pt.ShowDetail(6, 1, true, 0, 0);
            Worksheet sheet = workbook.Worksheets[workbook.Worksheets.Count - 1];
            Assert.AreEqual(&quot;Tennis&quot;,sheet.Cells[&quot;A4&quot;].StringValue );
            workbook.Save(Constants.PivotTableDestPath + &quot;CELLSJAVA41836.xlsx&quot;);
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


