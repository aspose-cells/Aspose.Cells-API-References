---
title: PivotDateTimeRangeGroupSettings.Interval
second_title: Aspose.Cells for .NET API Reference
description: PivotDateTimeRangeGroupSettings property. Gets the internal of the group
type: docs
url: /net/aspose.cells.pivot/pivotdatetimerangegroupsettings/interval/
---
## PivotDateTimeRangeGroupSettings.Interval property

Gets the internal of the group.

```csharp
public double Interval { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(1, ((PivotDateTimeRangeGroupSettings)dateBaseField.GroupSettings).Interval);
public static void PivotDateTimeRangeGroupSettings_Property_Interval(Workbook workbook)
        {
            int indPivTab;
            double stnrdRowHeight;
            string sourceDataPT, addrRngAllDta;
            Aspose.Cells.Range rngAllData;

            Worksheet wsCasPivot = workbook.Worksheets.Add("CasPivot");
            PivotTableCollection pivotTables = wsCasPivot.PivotTables;
            workbook.Worksheets.ActiveSheetIndex = 3;

            Cells casCells = workbook.Worksheets["Cas"].Cells;
            rngAllData = casCells.MaxDisplayRange;
            addrRngAllDta = rngAllData.Address;
            sourceDataPT = String.Format("=CAS!{0}", addrRngAllDta);

            //Add Pivot table to worksheet
            indPivTab = pivotTables.Add(sourceDataPT, "A1", "PivotTable2");
            // Accessing the instance of the newly added PivotTable
            PivotTable pivotTable = pivotTables[indPivTab];

            // Setting the PivotTable report shows grand totals for rows.
            pivotTable.ShowRowGrandTotals = true;
            // Setting the PivotTable report shows grand totals for columns.
            pivotTable.ShowColumnGrandTotals = true;
            //set Auto format
            pivotTable.IsAutoFormat = true;

            // Draging the first field to the row area.
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            PivotField dateBaseField = pivotTable.BaseFields["Date"];

            // Draging the second field to the column area.
            pivotTable.AddFieldToArea(PivotFieldType.Column, 2);
            PivotField colField = pivotTable.ColumnFields[0];
            colField.IsAutoSort = true;
            colField.IsAscendSort = true;

            // Draging the third field to the data area.
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            pivotTable.DataFields[0].Function = ConsolidationFunction.Count;

            // group and format Date field
            // pivotTable.SetAutoGroupField(dateBaseField);
            dateBaseField.GroupBy(1, false);
            Assert.AreEqual(1, ((PivotDateTimeRangeGroupSettings)dateBaseField.GroupSettings).Interval);
            #region Pivot table Style
            pivotTable.ShowInOutlineForm();

            //Refresh and calculate pivot table
           
            pivotTable.RefreshData();
            pivotTable.CalculateData();
           

            // Change PT background color
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.BackgroundColor = System.Drawing.Color.LightBlue;
            style.Font.IsBold = true;
            int ptMaxCol = wsCasPivot.Cells.MaxDataColumn;
            int ptMaxRow = wsCasPivot.Cells.MaxDataRow;

            for (int col = 0; col <= ptMaxCol; col++)
            {
                pivotTable.Format(0, col, style);
                pivotTable.Format(1, col, style);
                pivotTable.Format(ptMaxRow, col, style);
            }
            #endregion

            //Change workbook rows height
            stnrdRowHeight = casCells.StandardHeight;

            foreach (Worksheet sheet in workbook.Worksheets)
            {
                sheet.Cells.StandardHeight = stnrdRowHeight + 2.25;
            }

            CreateChart(wsCasPivot);

            workbook.Save(Constants.PivotTableDestPath + "example.xlsx");
        }
```

### See Also

* class [PivotDateTimeRangeGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


