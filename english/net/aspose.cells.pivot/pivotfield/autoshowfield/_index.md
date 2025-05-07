---
title: PivotField.AutoShowField
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Represents auto show field index. 1 means PivotField itself. It should be the index of the data fields
type: docs
url: /net/aspose.cells.pivot/pivotfield/autoshowfield/
---
## PivotField.AutoShowField property

Represents auto show field index. -1 means PivotField itself. It should be the index of the data fields.

```csharp
public int AutoShowField { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(0, workbook.Worksheets[0].PivotTables[0].BaseFields[0].AutoShowField);
[Test]
        public void Property_AutoShowField()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "CELLSNET56939.xlsb");
            workbook.Save(Constants.PivotTableDestPath + "CELLSNET56939.xlsb");
            workbook = new Workbook(Constants.PivotTableDestPath + "CELLSNET56939.xlsb");
            Assert.AreEqual(5, workbook.Worksheets[0].PivotTables[0].BaseFields[0].AutoShowCount);
            Assert.AreEqual(0, workbook.Worksheets[0].PivotTables[0].BaseFields[0].AutoShowField);
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


