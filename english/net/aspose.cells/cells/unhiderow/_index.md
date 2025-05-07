---
title: Cells.UnhideRow
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Unhides a row
type: docs
url: /net/aspose.cells/cells/unhiderow/
---
## Cells.UnhideRow method

Unhides a row.

```csharp
public void UnhideRow(int row, double height)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index. |
| height | Double | Row height. The row's height will be changed only when the row is hidden and given height value is positive. |

### Examples

```csharp
// Called: workbook.Worksheets[0].Cells.UnhideRow(5, 12.75);
[Test]
        public void Method_Double_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET40592.xlsm");
            //workbook.Worksheets[0].Cells.UngroupRows(5, 9,true);
            workbook.Worksheets[0].Cells.UnhideRow(5, 12.75);
            Assert.AreEqual(workbook.Worksheets[0].Shapes[0].Height!= 0 , true);
            workbook.Save(Constants.destPath + "CellsNet40592.xlsm");
            workbook = new Workbook(Constants.sourcePath + "BEFORE-UPLOAD_EDIT3.xlsm");
            workbook.Worksheets[0].Cells.UnhideRow(33, 12.75);
          
          
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


