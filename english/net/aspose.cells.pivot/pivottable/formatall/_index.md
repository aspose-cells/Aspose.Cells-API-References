---
title: PivotTable.FormatAll
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Format all the cell in the pivottable area
type: docs
url: /net/aspose.cells.pivot/pivottable/formatall/
---
## PivotTable.FormatAll method

Format all the cell in the pivottable area

```csharp
public void FormatAll(Style style)
```

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | Style which is to format |

### Examples

```csharp
// Called: pivotTable.FormatAll(style);
public void PivotTable_Method_FormatAll()
{
    string filePath = Constants.PivotTableSourcePath + @"NET43406_";
    Workbook book = new Workbook(filePath + "AposePivotTableCalculateDataInput.xlsx");
    Worksheet pivotSheet = book.Worksheets.Add("Pivot Table");
    PivotTableCollection pivotTables = pivotSheet.PivotTables;
    Worksheet dataSheet = book.Worksheets["Data"];
    string sourceData = String.Format("=Data!A1:{0}", Aspose.Cells.CellsHelper.CellIndexToName(dataSheet.Cells.MaxDataRow, dataSheet.Cells.MaxDataColumn));
    int pivotIndex = pivotTables.Add(sourceData, "A1", "PivotTable1");
    PivotTable pivotTable = pivotTables[pivotIndex];
    Style style = book.CreateStyle();
    style.Font.Size = 8;
    style.Font.Name = "Calibri";
    pivotTable.PivotTableStyleType = Aspose.Cells.Pivot.PivotTableStyleType.PivotTableStyleMedium15;
    pivotTable.FormatAll(style);
    pivotTable.EnableWizard = false;
    pivotTable.EnableFieldList = true;

    pivotSheet.MoveTo(0);

    AddPivotRow(pivotTable, "Property Name", "Property Name", false, true, false, true, false, "", false, true, false);
    AddPivotRow(pivotTable, "Section Description", "Section Description",
        true, true, true, true, true, "", false, false, false);
    AddPivotRow(pivotTable, "Account Category Two", "Account Category Two",
        true, true, false, true, true, "", false, true, false);

    AddPivotRow(pivotTable, "Account Category Three", "Account Category Three",
        true, true, false, true, true, "", false, true, false);
    AddPivotRow(pivotTable, "Transaction Description", "Transaction Description",
        false, true, false, true, false, "", false, true, false);


    AddPivotColumn(pivotTable, "Range", "Range", true);
    AddPivotColumn(pivotTable, "PeriodDescription", "Periods");
    AddPivotData(pivotTable, "Amount", "Values", "# ##0.00");

    pivotTable.ShowColumnGrandTotals = false;
    pivotTable.ShowRowGrandTotals = false;//Setting to false causes .CalculateData() to throw the exception. If set to True, the exception does not occur.

    pivotTable.IsGridDropZones = true;
    pivotTable.RefreshData();
    pivotTable.CalculateData(); // Throws Exception

    pivotTable.RefreshDataOnOpeningFile = false;

    pivotSheet.AutoFitColumns();
    pivotSheet.Cells.StandardHeight = 11.25;
    book.Worksheets.ActiveSheetIndex = 0;
    book.Settings.HidePivotFieldList = true;

    book.Save(Constants.PIVOT_CHECK_FILE_PATH + "example.xlsx", new OoxmlSaveOptions());
}
```

### See Also

* class [Style](../../../aspose.cells/style/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


