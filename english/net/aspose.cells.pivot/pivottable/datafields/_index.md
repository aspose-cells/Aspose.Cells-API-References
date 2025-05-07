---
title: PivotTable.DataFields
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Gets a PivotField object that represents all the data fields in a PivotTable. Readonly.It would be init only when there are two or more data fields in the DataPiovtFiels. It only use to add DataPivotField to the PivotTable row/column area . Default is in row area
type: docs
url: /net/aspose.cells.pivot/pivottable/datafields/
---
## PivotTable.DataFields property

Gets a PivotField object that represents all the data fields in a PivotTable. Read-only.It would be init only when there are two or more data fields in the DataPiovtFiels. It only use to add DataPivotField to the PivotTable row/column area . Default is in row area.

```csharp
public PivotFieldCollection DataFields { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual("='b''b'", wb.Worksheets[0].PivotTables[0].DataFields[1].GetFormula());
[Test]
        public void Property_DataFields()
        {

            Workbook wb = new Workbook(Constants.PivotTableSourcePath + "CELLSNET56419.xlsx");
           Assert.AreEqual("='b''b'",wb.Worksheets[0].PivotTables[0].DataFields[1].GetFormula());
           Assert.AreEqual("='w''e'",wb.Worksheets[0].PivotTables[0].RowFields[0].PivotItems[2].GetFormula());
            wb.Save(Constants.PivotTableDestPath + "CELLSNET56419.xlsb");
            wb = new Workbook(Constants.PivotTableDestPath + "CELLSNET56419.xlsb");
            Assert.AreEqual("='b''b'", wb.Worksheets[0].PivotTables[0].DataFields[1].GetFormula());
            Assert.AreEqual("='w''e'", wb.Worksheets[0].PivotTables[0].RowFields[0].PivotItems[2].GetFormula());
            wb.Save(Constants.PivotTableDestPath + "CELLSNET56419.xlsx");
        }
```

### See Also

* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


