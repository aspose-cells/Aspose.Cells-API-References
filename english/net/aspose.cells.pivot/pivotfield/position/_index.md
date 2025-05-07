---
title: PivotField.Position
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Represents the index of PivotField in the region
type: docs
url: /net/aspose.cells.pivot/pivotfield/position/
---
## PivotField.Position property

Represents the index of [`PivotField`](../) in the region.

```csharp
public int Position { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(wb.Worksheets[1].PivotTables[0].DataField.Position, 2);
[Test]
        public void Property_Position()
        {
            string filePath = Constants.PivotTableSourcePath + @"NET47024_";

            Workbook wb = new Workbook(filePath + "Sample.xlsx");

            wb.Worksheets.Insert(1, wb.Worksheets[0].Type);
            wb.Worksheets[1].Copy(wb.Worksheets[0]);
            Assert.AreEqual(wb.Worksheets[1].PivotTables[0].DataField.Position, 2);
            wb.Save(CreateFolder(filePath) + "out.xlsx", SaveFormat.Xlsx);
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


