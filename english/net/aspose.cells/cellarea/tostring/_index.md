---
title: CellArea.ToString
second_title: Aspose.Cells for .NET API Reference
description: CellArea method. Returns a string represents the current cell area object
type: docs
url: /net/aspose.cells/cellarea/tostring/
---
## CellArea.ToString method

Returns a string represents the current cell area object.

```csharp
public override string ToString()
```

### Examples

```csharp
// Called: Assert.AreEqual("Aspose.Cells.CellArea(F1:F1048576)[0,5,1048575,5]", sheet.ConditionalFormattings[1].GetCellArea(0).ToString());
[Test]
       public void Method_ToString()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet48652.xlsx");

            workbook.Save(Constants.destPath + "CellsNet48652.ods");
            workbook = new Workbook(Constants.destPath + "CellsNet48652.ods");
            Worksheet sheet = workbook.Worksheets[0];
            Assert.AreEqual(2,sheet.ConditionalFormattings.Count);
           Assert.AreEqual("Aspose.Cells.CellArea(B2:D5)[1,1,4,3]", sheet.ConditionalFormattings[0].GetCellArea(0).ToString());
            Assert.AreEqual("Aspose.Cells.CellArea(F1:F1048576)[0,5,1048575,5]", sheet.ConditionalFormattings[1].GetCellArea(0).ToString());
        }
```

### See Also

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


