---
title: PivotTable.ManualUpdate
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Indicates whether the PivotTable report is recalculated only at the users request
type: docs
url: /net/aspose.cells.pivot/pivottable/manualupdate/
---
## PivotTable.ManualUpdate property

Indicates whether the PivotTable report is recalculated only at the user's request.

```csharp
public bool ManualUpdate { get; set; }
```

### Examples

```csharp
// Called: pivotTable.ManualUpdate = true;
public void PivotTable_Property_ManualUpdate()
{
    string filePath = Constants.PivotTableSourcePath + @"NET45040_";

    //License lic = new License();
    //lic.SetLicense("Aspose.Total.lic");
    Workbook workbook = new Workbook(filePath + @"template.xlsm");

    Worksheet selectedSheet = workbook.Worksheets["Data"];
    DataTable dt = new DataTable();
    dt.ReadXml(filePath + @"example.xml");
    if (dt.Rows.Count > 0) selectedSheet.Cells.ImportData(dt, 1, 0, new ImportTableOptions() { IsFieldNameShown = false });
    string pivotFormula = "='Data'!A1:EP2806";

    selectedSheet = workbook.Worksheets["Exposure"];
    workbook.Worksheets.ActiveSheetIndex = selectedSheet.Index;
    int iIndex = selectedSheet.PivotTables.Add(pivotFormula, "A7", "IRIS007_pivot");
    PivotTable pivotTable = selectedSheet.PivotTables[iIndex];
    pivotTable.PivotTableStyleType = PivotTableStyleType.None;
    pivotTable.PreserveFormatting = true;
    pivotTable.ManualUpdate = true;
    pivotTable.IsAutoFormat = false;
    pivotTable.RefreshDataOnOpeningFile = false; // important for the bug
    pivotTable.MergeLabels = false;
    pivotTable.AutoFormatType = PivotTableAutoFormatType.None;
    pivotTable.PrintDrill = false;
    pivotTable.ShowDrill = false;
    Action<PivotField> setFieldSetting = (s) =>
    {
        s.ShowCompact = false;
        s.IsRepeatItemLabels = false;
        s.InsertBlankRow = false;
        s.ShowAllItems = false;
        s.ShowSubtotalAtTop = false;
        s.ShowInOutlineForm = false;
    };
    iIndex = pivotTable.AddFieldToArea(PivotFieldType.Column, "Expo Date Code");
    PivotField selectedField = pivotTable.ColumnFields[iIndex];
    selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);
    selectedField.ShowAllItems = true;

    Action<PivotField> hideEmpty = (s) =>
    {
        string[] items = s.Items;
        for (int iItems = 0; iItems < s.ItemCount; iItems++)
        {
            if (String.IsNullOrWhiteSpace(items[iItems])) s.HideItem(iItems, true);
        }
    };
    Action<string> addRow = (cell) =>
    {
        iIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, cell);
        selectedField = pivotTable.RowFields[iIndex];
        selectedField.SetSubtotals(PivotFieldSubtotalType.None, true);
        selectedField.IsAutoSort = true;
        selectedField.IsAscendSort = true;
        setFieldSetting(selectedField);
    };
    addRow("Product");
    addRow("Series name");
    addRow("Synth Trade Type");
    addRow("Hedge");
    addRow("Hedge Name");
    addRow("Event Date");
    addRow("Event Status");

    iIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, "Expo qty");
    selectedField = pivotTable.DataFields[iIndex];
    selectedField.Function = ConsolidationFunction.Sum;
    selectedField.DisplayName = "Qty";
    selectedField.NumberFormat = "#,##0;[Red]-#,##0";

    pivotTable.RefreshData();
    pivotTable.CalculateRange();
    pivotTable.CalculateData();
    selectedSheet.AutoFitColumns();
    Assert.AreEqual(selectedSheet.Cells["D11"].StringValue, "2018285");
    workbook.Save(CreateFolder(filePath) + @"out.xlsx");
}
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


