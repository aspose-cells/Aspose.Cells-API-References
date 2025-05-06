---
title: PivotTable.ShowInOutlineForm
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Layouts the PivotTable in outline form
type: docs
url: /net/aspose.cells.pivot/pivottable/showinoutlineform/
---
## PivotTable.ShowInOutlineForm method

Layouts the PivotTable in outline form.

```csharp
public void ShowInOutlineForm()
```

### Examples

```csharp
// Called: pivotTable.ShowInOutlineForm();
public static void Method_ShowInOutlineForm(Workbook workbook)
        {
            int indPivTab;
            double stnrdRowHeight;
            string sourceDataPT, addrRngAllDta;
            Aspose.Cells.Range rngAllData;

            Worksheet wsCasPivot = workbook.Worksheets.Add(&quot;CasPivot&quot;);
            PivotTableCollection pivotTables = wsCasPivot.PivotTables;
            workbook.Worksheets.ActiveSheetIndex = 3;

            Cells casCells = workbook.Worksheets[&quot;Cas&quot;].Cells;
            rngAllData = casCells.MaxDisplayRange;
            addrRngAllDta = rngAllData.Address;
            sourceDataPT = String.Format(&quot;=CAS!{0}&quot;, addrRngAllDta);

            //Add Pivot table to worksheet
            indPivTab = pivotTables.Add(sourceDataPT, &quot;A1&quot;, &quot;PivotTable2&quot;);
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
            PivotField dateBaseField = pivotTable.BaseFields[&quot;Date&quot;];

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

            for (int col = 0; col &lt;= ptMaxCol; col++)
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

            workbook.Save(Constants.PivotTableDestPath + &quot;CellsNet54902.xlsx&quot;);
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


