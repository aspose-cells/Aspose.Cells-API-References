---
title: PivotTable.RowFields
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Returns a PivotFields object that are currently shown as row fields
type: docs
url: /net/aspose.cells.pivot/pivottable/rowfields/
---
## PivotTable.RowFields property

Returns a PivotFields object that are currently shown as row fields.

```csharp
public PivotFieldCollection RowFields { get; }
```

### Examples

```csharp
// Called: pf = workbook.Worksheets[0].PivotTables[0].RowFields[0];
[Test]
        public void Property_RowFields()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "CELLSNET55742.xlsb");
            PivotField pf = workbook.Worksheets[0].PivotTables[0].RowFields[0];
           Assert.IsTrue(pf.PivotItems[1].GetStringValue().IndexOf("4:48:00") != -1);
            workbook.Save(Constants.PivotTableDestPath + "CELLSNET55742.xlsb");
            workbook = new Workbook(Constants.PivotTableDestPath + "CELLSNET55742.xlsb");
            pf = workbook.Worksheets[0].PivotTables[0].RowFields[0];
            Assert.IsTrue(pf.PivotItems[1].GetStringValue().IndexOf("4:48:00") != -1);
            workbook.Save(Constants.PivotTableDestPath + "CELLSNET55742.xlsx");
            workbook = new Workbook(Constants.PivotTableDestPath + "CELLSNET55742.xlsx");
            pf = workbook.Worksheets[0].PivotTables[0].RowFields[0];
            Assert.IsTrue(pf.PivotItems[1].GetStringValue().IndexOf("4:48:00") != -1);
        }
```

### See Also

* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


