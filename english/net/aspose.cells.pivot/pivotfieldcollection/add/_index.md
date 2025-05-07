---
title: PivotFieldCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: PivotFieldCollection method. Adds a PivotField Object to the specific type PivotFields
type: docs
url: /net/aspose.cells.pivot/pivotfieldcollection/add/
---
## PivotFieldCollection.Add method

Adds a PivotField Object to the specific type PivotFields.

```csharp
public int Add(PivotField pivotField)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pivotField | PivotField | a PivotField Object. |

### Return Value

the index of the PivotField Object in this PivotFields.

### Examples

```csharp
// Called: pivotTablePLSum.ColumnFields.Add(pivotTablePLSum.DataField);//move datafied to columns
[Test]
        public void Method_PivotField_()
        {
            Workbook savingsExcel = new Workbook(Constants.openPivottablePath + "28352.xls");
            PivotTableAutoFormatType pivotType = PivotTableAutoFormatType.Report5;

            //############################make pivot PL
            //Getting the pivottables collection in the sheet
            int dataSheetRow = 70; // last data row

            Worksheet SummaryPLWorksheet = savingsExcel.Worksheets[0];

            Aspose.Cells.Pivot.PivotTableCollection pivotTables = SummaryPLWorksheet.PivotTables;

            //Adding a PivotTable to the worksheet
            int index = pivotTables.Add("=Data!A1:I" + dataSheetRow.ToString(), "A2", "PivotTablePL");

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
            int indexSumPL = pivotTables.Add("=Data!A1:I" + dataSheetRow.ToString(), "J2", "PivotTablePLSum");

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
            for (int i = 0; i < 4; i++)
            {
                pivotTable.DataFields[i].NumberFormat = "#,##0";

            }
            for (int i = 4; i < 6; i++)
            {
                pivotTable.DataFields[i].NumberFormat = "#,##0.00%";

            }

            //sums
            for (int i = 0; i < 2; i++)
            {
                pivotTablePLSum.DataFields[i].NumberFormat = "#,##0";

            }

            for (int i = 2; i < 3; i++)
            {
                pivotTablePLSum.DataFields[i].NumberFormat = "#,##0.00%";

            }

            // recalculate data
            pivotTable.CalculateData();
            pivotTablePLSum.CalculateData();


            if (savingsExcel != null)
            {
                savingsExcel.Save(Constants.savePivottablePath + "28352.xls");
            }

        }
```

### See Also

* class [PivotField](../../pivotfield/)
* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


