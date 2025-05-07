---
title: PivotField.IsCalculatedField
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Indicates whether the specified PivotTable field is calculated field
type: docs
url: /net/aspose.cells.pivot/pivotfield/iscalculatedfield/
---
## PivotField.IsCalculatedField property

Indicates whether the specified PivotTable field is calculated field.

```csharp
public bool IsCalculatedField { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(wb.Worksheets[0].PivotTables[0].BaseFields[5].IsCalculatedField, true);
[Test]
        public void Property_IsCalculatedField()
        {

            Workbook wb = new Workbook(Constants.openPivottablePath + "bb1.xlsx");

            Assert.AreEqual(wb.Worksheets[0].PivotTables[0].BaseFields[5].IsCalculatedField, true);
            Assert.AreEqual(wb.Worksheets[0].PivotTables[0].BaseFields[5].GetFormula(), "=0");
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


