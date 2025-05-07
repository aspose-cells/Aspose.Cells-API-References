---
title: PivotTable.BaseFields
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Returns all base pivot fields in the PivotTable
type: docs
url: /net/aspose.cells.pivot/pivottable/basefields/
---
## PivotTable.BaseFields property

Returns all base pivot fields in the PivotTable.

```csharp
public PivotFieldCollection BaseFields { get; }
```

### Examples

```csharp
// Called: PivotFieldCollection fields = workbook.Worksheets[1].PivotTables[0].BaseFields;
[Test]
        public void Property_BaseFields()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "CELLSNET52671.xlsx");
            PivotFieldCollection fields = workbook.Worksheets[1].PivotTables[0].BaseFields;
            Assert.AreEqual("=ABS('ns1:TRN_AMOUNT')", fields[fields.Count - 1].GetFormula());
        }
```

### See Also

* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


