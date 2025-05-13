---
title: PivotField.SetSubtotals
second_title: Aspose.Cells for .NET API Reference
description: PivotField method. Sets whether the specified field shows that subtotals
type: docs
url: /net/aspose.cells.pivot/pivotfield/setsubtotals/
---
## PivotField.SetSubtotals method

Sets whether the specified field shows that subtotals.

```csharp
public void SetSubtotals(PivotFieldSubtotalType subtotalType, bool shown)
```

| Parameter | Type | Description |
| --- | --- | --- |
| subtotalType | PivotFieldSubtotalType | subtotals type. |
| shown | Boolean | whether the specified field shows that subtotals. |

### Examples

```csharp
// Called: selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);
public void PivotField_Method_SetSubtotals()
{
    string filePath = Constants.PivotTableSourcePath + @"NET45267_";

    Workbook workbook = new Workbook(filePath + @"Template.xlsm");
    Worksheet selectedSheet = workbook.Worksheets["Data"];
    DataTable dt = new DataTable();
    dt.ReadXml(filePath + @"example.xml");
    selectedSheet.Cells.ImportData(dt, 1, 0, new ImportTableOptions() { IsFieldNameShown = false });
    selectedSheet = workbook.Worksheets["Exposure"];
    int iIndex = selectedSheet.PivotTables.Add("='Data'!A1:EQ15042", "A7", "IRIS007_pivot");
    PivotTable selectedPivotTable = selectedSheet.PivotTables[iIndex];
    selectedPivotTable.RefreshDataOnOpeningFile = false; // important we need it

    iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Column, "Expo Date Code");

    iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Row, "Series name");
    PivotField selectedField = selectedPivotTable.RowFields[iIndex];
    selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);

    iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Row, "Trade Type");
    selectedField = selectedPivotTable.RowFields[iIndex];
    selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);

    iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Row, "Put/Call");
    selectedField = selectedPivotTable.RowFields[iIndex];
    selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);

    iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Row, "Strike Price");
    selectedField = selectedPivotTable.RowFields[iIndex];
    selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);

    iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Row, "Hedge");
    selectedField = selectedPivotTable.RowFields[iIndex];
    selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);

    iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Row, "Hedge Name");
    selectedField = selectedPivotTable.RowFields[iIndex];
    selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);

    iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Row, "B/S");
    selectedField = selectedPivotTable.RowFields[iIndex];
    selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);

    iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Row, "Event");
    selectedField = selectedPivotTable.RowFields[iIndex];
    selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);

    iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Row, "Event Date");
    selectedField = selectedPivotTable.RowFields[iIndex];
    selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);

    iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Row, "Event Status");
    selectedField = selectedPivotTable.RowFields[iIndex];
    selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);

    iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Row, "Formula");
    selectedField = selectedPivotTable.RowFields[iIndex];
    selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);

    iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Row, "Position Product Code");
    selectedField = selectedPivotTable.RowFields[iIndex];
    selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);

    /* the row field we would like to correctly format */
    iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Row, "Position Qty");
    selectedField = selectedPivotTable.RowFields[iIndex];
    selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);
    selectedField.NumberFormat = "[Blue]#,##0;[Red]-#,##0";

    iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Row, "Pricing Dates");
    selectedField = selectedPivotTable.RowFields[iIndex];
    selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);

    iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Row, "Inco Term");
    selectedField = selectedPivotTable.RowFields[iIndex];
    selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);

    iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Data, "Expo qty");
    selectedField = selectedPivotTable.DataFields[iIndex];
    selectedField.NumberFormat = "#,##0;[Red]-#,##0";

    selectedPivotTable.RefreshData();
    selectedPivotTable.CalculateRange();
    selectedPivotTable.CalculateData();
    Assert.AreEqual(selectedSheet.Cells["M13"].StringValue, "2,550");
    Assert.AreEqual(selectedSheet.Cells["M13"].GetDisplayStyle().Font.Color, Color.FromArgb(255, 0, 0, 255));
    Assert.AreEqual(selectedSheet.Cells["M14"].StringValue, "-5,250");
    Assert.AreEqual(selectedSheet.Cells["M14"].GetDisplayStyle().Font.Color, Color.FromArgb(255, 255, 0, 0));

    workbook.Save(CreateFolder(filePath) + @"out.xlsm");
}
```

### See Also

* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


