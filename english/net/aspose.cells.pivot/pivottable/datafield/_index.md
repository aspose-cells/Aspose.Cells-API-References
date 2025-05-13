---
title: PivotTable.DataField
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Gets a PivotField object that represents all the data fields in a PivotTable. Readonly. It would only be created when there are two or more data fields in the Data region. Defaultly it is in row region. You can drag it to the row/column region with PivotTable.AddFieldToArea method 
type: docs
url: /net/aspose.cells.pivot/pivottable/datafield/
---
## PivotTable.DataField property

Gets a [`PivotField`](../../pivotfield/) object that represents all the data fields in a PivotTable. Read-only. It would only be created when there are two or more data fields in the Data region. Defaultly it is in row region. You can drag it to the row/column region with PivotTable.AddFieldToArea() method .

```csharp
public PivotField DataField { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(wb.Worksheets[1].PivotTables[0].DataField.Position, 2);
public void PivotTable_Property_DataField()
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

* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


