---
title: PivotTable.IsAutoFormat
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Indicates whether the PivotTable report is automatically formatted. Checkbox autoformat table  which is in pivottable option for Excel 2003
type: docs
url: /net/aspose.cells.pivot/pivottable/isautoformat/
---
## PivotTable.IsAutoFormat property

Indicates whether the PivotTable report is automatically formatted. Checkbox "autoformat table " which is in pivottable option for Excel 2003

```csharp
public bool IsAutoFormat { get; set; }
```

### Examples

```csharp
// Called: pivotTable.IsAutoFormat = true;
[Test]
        public void Property_IsAutoFormat()
        {
            Workbook savingsExcel = new Workbook(Constants.openPivottablePath + &quot;28352.xls&quot;);
            PivotTableAutoFormatType pivotType = PivotTableAutoFormatType.Report5;

            //############################make pivot PL
            //Getting the pivottables collection in the sheet
            int dataSheetRow = 70; // last data row

            Worksheet SummaryPLWorksheet = savingsExcel.Worksheets[0];

            Aspose.Cells.Pivot.PivotTableCollection pivotTables = SummaryPLWorksheet.PivotTables;

            //Adding a PivotTable to the worksheet
            int index = pivotTables.Add(&quot;=Data!A1:I&quot; + dataSheetRow.ToString(), &quot;A2&quot;, &quot;PivotTablePL&quot;);

            //Accessing the instance of the newly added PivotTable
            Aspose.Cells.Pivot.PivotTable pivotTable = pivotTables[index];

            //Showing the grand totals
            pivotTable.ShowRowGrandTotals = false;
            pivotTable.ShowColumnGrandTotals = false;

            //Setting the PivotTable report is automatically formatted
            pivotTable.IsAutoFormat = true;

            //Setting the PivotTable autoformat type.
            pivotTable.AutoFormatType = pivotType;

            //Draging the first 2 fields to the row area.
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, 1);

            //Draging the 4-9 fields to the column area.
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, 3);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, 4);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, 5);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, 6);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, 7);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, 8);

            //pivotTable.RefreshDataFlag = true;
            pivotTable.ColumnFields.Add(pivotTable.DataField);//move datafied to columns





            //--------------Adding a Summary PivotTable to the worksheet
            int indexSumPL = pivotTables.Add(&quot;=Data!A1:I&quot; + dataSheetRow.ToString(), &quot;J2&quot;, &quot;PivotTablePLSum&quot;);

            //Accessing the instance of the newly added PivotTable
            Aspose.Cells.Pivot.PivotTable pivotTablePLSum = pivotTables[indexSumPL];

            //Showing the grand totals
            pivotTablePLSum.ShowRowGrandTotals = true;
            pivotTablePLSum.ShowColumnGrandTotals = false;

            //Setting the PivotTable report is automatically formatted
            pivotTablePLSum.IsAutoFormat = true;

            //Setting the PivotTable autoformat type.
            pivotTablePLSum.AutoFormatType = pivotType;

            //Draging the second field to the row area.
            pivotTablePLSum.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, 1);

            //Draging the sum fields to the column area.
            pivotTablePLSum.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, 5);
            pivotTablePLSum.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, 6);
            pivotTablePLSum.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, 8);

            pivotTablePLSum.ColumnFields.Add(pivotTablePLSum.DataField);//move datafied to columns




            //Setting the number format of the first data field
            //main tables
            for (int i = 0; i &lt; 4; i++)
            {
                pivotTable.DataFields[i].NumberFormat = &quot;#,##0&quot;;

            }
            for (int i = 4; i &lt; 6; i++)
            {
                pivotTable.DataFields[i].NumberFormat = &quot;#,##0.00%&quot;;

            }

            //sums
            for (int i = 0; i &lt; 2; i++)
            {
                pivotTablePLSum.DataFields[i].NumberFormat = &quot;#,##0&quot;;

            }

            for (int i = 2; i &lt; 3; i++)
            {
                pivotTablePLSum.DataFields[i].NumberFormat = &quot;#,##0.00%&quot;;

            }

            // recalculate data
            pivotTable.CalculateData();
            pivotTablePLSum.CalculateData();


            if (savingsExcel != null)
            {
                savingsExcel.Save(Constants.savePivottablePath + &quot;28352.xls&quot;);
            }

        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


