---
title: PivotTable.Fields
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Gets the specific fields by the field type
type: docs
url: /net/aspose.cells.pivot/pivottable/fields/
---
## PivotTable.Fields method

Gets the specific fields by the field type.

```csharp
[Obsolete("Use PivotField.GetFields() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotFieldCollection Fields(PivotFieldType fieldType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | PivotFieldType | the field type. |

### Return Value

the specific field collection

### Remarks

NOTE: This method is now obsolete. Instead, please use PivotField.GetFields() method. This method will be removed 12 months later since May 2024. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: pf = pt.Fields(PivotFieldType.Data)[fp];
public void PivotTable_Method_Fields()
{
    string filePath = Constants.PivotTableSourcePath + @"NET42427_";
    string savePath = CreateFolder(filePath);

    Workbook wb = new Workbook(FileFormatType.Pdf);
    Worksheet ws = wb.Worksheets[wb.Worksheets.Add()];
    ws.Name = "Sheet";

    ws.Cells[0, 0].PutValue("X");
    ws.Cells[0, 1].PutValue("Y");
    ws.Cells[0, 2].PutValue("Data");

    ws.Cells[1, 0].PutValue("A");
    ws.Cells[1, 1].PutValue("C");
    ws.Cells[1, 2].PutValue(10);

    ws.Cells[2, 0].PutValue("A");
    ws.Cells[2, 1].PutValue("D");
    ws.Cells[2, 2].PutValue(25);

    ws.Cells[3, 0].PutValue("B");
    ws.Cells[3, 1].PutValue("C");
    ws.Cells[3, 2].PutValue(30);

    ws.Cells[4, 0].PutValue("B");
    ws.Cells[4, 1].PutValue("D");
    ws.Cells[4, 2].PutValue(45);

    PivotTableCollection ptc = ws.PivotTables;
    int index = ptc.Add("=Sheet!A1:C5", "A7", "PivotTable1");
    PivotTable pt = ptc[index];

    int fp; PivotField pf;

    fp = pt.AddFieldToArea(PivotFieldType.Row, "X");
    pf = pt.Fields(PivotFieldType.Row)[fp];

    fp = pt.AddFieldToArea(PivotFieldType.Column, "Y");
    pf = pt.Fields(PivotFieldType.Column)[fp];

    fp = pt.AddFieldToArea(PivotFieldType.Data, "Data");
    pf = pt.Fields(PivotFieldType.Data)[fp];

    fp = pt.AddFieldToArea(PivotFieldType.Data, "Data");
    pf = pt.Fields(PivotFieldType.Data)[fp];
    pf.ShowValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOfColumn;

    pt.AddFieldToArea(PivotFieldType.Column, pt.DataField);
    wb.Save(savePath + "out.xlsx");
    wb.Save(savePath + "out.pdf");
    pt.RefreshData();
    pt.CalculateData();

    Assert.AreEqual(ws.Cells["C10"].StringValue, "25.00%");
    Assert.AreEqual(ws.Cells["E10"].StringValue, "35.71%");
    Assert.AreEqual(ws.Cells["G10"].StringValue, "31.82%");
           
}
```

### See Also

* class [PivotFieldCollection](../../pivotfieldcollection/)
* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


