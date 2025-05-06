---
title: WorkbookSettings.HidePivotFieldList
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Gets and sets whether hide the field list for the PivotTable
type: docs
url: /net/aspose.cells/workbooksettings/hidepivotfieldlist/
---
## WorkbookSettings.HidePivotFieldList property

Gets and sets whether hide the field list for the PivotTable.

```csharp
public bool HidePivotFieldList { get; set; }
```

### Examples

```csharp
// Called: book.Settings.HidePivotFieldList = true;
[Test]
        public void Property_HidePivotFieldList()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET43406_&quot;;
            Workbook book = new Workbook(filePath + &quot;AposePivotTableCalculateDataInput.xlsx&quot;);
            Worksheet pivotSheet = book.Worksheets.Add(&quot;Pivot Table&quot;);
            PivotTableCollection pivotTables = pivotSheet.PivotTables;
            Worksheet dataSheet = book.Worksheets[&quot;Data&quot;];
            string sourceData = String.Format(&quot;=Data!A1:{0}&quot;, Aspose.Cells.CellsHelper.CellIndexToName(dataSheet.Cells.MaxDataRow, dataSheet.Cells.MaxDataColumn));
            int pivotIndex = pivotTables.Add(sourceData, &quot;A1&quot;, &quot;PivotTable1&quot;);
            PivotTable pivotTable = pivotTables[pivotIndex];
            Style style = book.CreateStyle();
            style.Font.Size = 8;
            style.Font.Name = &quot;Calibri&quot;;
            pivotTable.PivotTableStyleType = Aspose.Cells.Pivot.PivotTableStyleType.PivotTableStyleMedium15;
            pivotTable.FormatAll(style);
            pivotTable.EnableWizard = false;
            pivotTable.EnableFieldList = true;

            pivotSheet.MoveTo(0);

            AddPivotRow(pivotTable, &quot;Property Name&quot;, &quot;Property Name&quot;, false, true, false, true, false, &quot;&quot;, false, true, false);
            AddPivotRow(pivotTable, &quot;Section Description&quot;, &quot;Section Description&quot;,
                true, true, true, true, true, &quot;&quot;, false, false, false);
            AddPivotRow(pivotTable, &quot;Account Category Two&quot;, &quot;Account Category Two&quot;,
                true, true, false, true, true, &quot;&quot;, false, true, false);

            AddPivotRow(pivotTable, &quot;Account Category Three&quot;, &quot;Account Category Three&quot;,
                true, true, false, true, true, &quot;&quot;, false, true, false);
            AddPivotRow(pivotTable, &quot;Transaction Description&quot;, &quot;Transaction Description&quot;,
                false, true, false, true, false, &quot;&quot;, false, true, false);


            AddPivotColumn(pivotTable, &quot;Range&quot;, &quot;Range&quot;, true);
            AddPivotColumn(pivotTable, &quot;PeriodDescription&quot;, &quot;Periods&quot;);
            AddPivotData(pivotTable, &quot;Amount&quot;, &quot;Values&quot;, &quot;# ##0.00&quot;);

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

            book.Save(Constants.PIVOT_CHECK_FILE_PATH + &quot;NET43406.xlsx&quot;, new OoxmlSaveOptions());
        }
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


