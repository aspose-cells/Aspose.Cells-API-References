---
title: PivotTable.ShowInCompactForm
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Layouts the PivotTable in compact form
type: docs
url: /net/aspose.cells.pivot/pivottable/showincompactform/
---
## PivotTable.ShowInCompactForm method

Layouts the PivotTable in compact form.

```csharp
public void ShowInCompactForm()
```

### Examples

```csharp
// Called: pivotTable.ShowInCompactForm();
[Test]
        public void Method_ShowInCompactForm()
        {
            int maxDRow, counter, indPivTab;
            string fileCSV, originalDate, modifiedDate, sourceDataPT;
            string addrRngAllDta;
            Cells cellsTabCF;
            Aspose.Cells.Range rngAllData, rngAccDate;
            Worksheet wsTabCF;

            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv);
            loadOptions.ConvertDateTimeData = true;


            fileCSV = Constants.PivotTableSourcePath +"CellsNet54396_1.csv";
            Workbook wbCFPiv = new Workbook(fileCSV, loadOptions);
            wsTabCF = wbCFPiv.Worksheets[0];
            wsTabCF.Name = "tabCF";
            cellsTabCF = wsTabCF.Cells;
            maxDRow = cellsTabCF.MaxDataRow + 1;
            rngAllData = cellsTabCF.MaxDisplayRange;

            #region Format date on column B
            Style stDateForm = wbCFPiv.CreateStyle();
            stDateForm.Number = 14;
            rngAccDate = cellsTabCF.CreateRange($"B2:B{maxDRow}");
            counter = 0;
            foreach (Cell cell in rngAccDate)
            {
                originalDate = cell.StringValue;
                modifiedDate = originalDate.Insert(4, "-").Insert(7, "-");
                if (cell.StringValue != null)
                {
                    cell.PutValue(modifiedDate, true, true);
                }
                counter++;
            }
            //TxtLoadOptions opts = new TxtLoadOptions();
            //cellsTabCF.TextToColumns(0, 1, maxDRow, opts);
            //rngAccDate.ApplyStyle(stDateForm, new StyleFlag() { NumberFormat = true });
            cellsTabCF.Columns[1].Width = 11.14;
            #endregion

            // Pivot Table
            Worksheet wsSheet1 = wbCFPiv.Worksheets.Add("Sheet1");
            wsTabCF.MoveTo(1);
            wbCFPiv.Worksheets.ActiveSheetIndex = 0;
            PivotTableCollection pivotTables = wsSheet1.PivotTables;

            rngAllData = rngAllData.Worksheet.Cells.CreateRange(rngAllData.FirstRow, rngAllData.FirstColumn, rngAllData.RowCount - 1, rngAllData.ColumnCount);

            addrRngAllDta = rngAllData.Address;
            sourceDataPT = String.Format("=tabCF!{0}", addrRngAllDta);

            //Add Pivot table to worksheet
            indPivTab = pivotTables.Add(sourceDataPT, "A1", "PivotTbl");
            PivotTable pivotTable = pivotTables[indPivTab];

            pivotTable.AddFieldToArea(PivotFieldType.Data, 2);
            pivotTable.DataFields[0].Function = ConsolidationFunction.Count;

            pivotTable.AddFieldToArea(PivotFieldType.Row, 7);
            PivotField cfgroupField = pivotTable.RowFields[0];
            cfgroupField.ShowSubtotalAtTop = true;
            cfgroupField.IsAutoSort = true;

            pivotTable.AddFieldToArea(PivotFieldType.Row, 14);
            PivotField sevtransField = pivotTable.RowFields[1];
            sevtransField.ShowSubtotalAtTop = true;
            sevtransField.ShowAllItems = true;
            sevtransField.IsAutoSort = true;

            pivotTable.AddFieldToArea(PivotFieldType.Column, 12);
            PivotField sextransField = pivotTable.ColumnFields[0];
            sextransField.IsAutoSort = true;

            pivotTable.AddFieldToArea(PivotFieldType.Row, 1);
            PivotField accdateField = pivotTable.RowFields[2];

            PivotField dateBaseField = pivotTable.BaseFields["AccDate"];
            DateTime start = new DateTime(2020, 1, 1);
            DateTime end = new DateTime(2020, 12, 31);
            System.Collections.ArrayList groupTypeList = new System.Collections.ArrayList();
            //groupTypeList.Add(PivotGroupByType.Months);
            //groupTypeList.Add(PivotGroupByType.Years);
            //pivotTable.SetManualGroupField(dateBaseField, start, end, groupTypeList, 1);
            dateBaseField.GroupBy(start, end, new PivotGroupByType[] { PivotGroupByType.Months, PivotGroupByType.Years }, 1, false);

            pivotTable.AddFieldToArea(PivotFieldType.Page, pivotTable.RowFields[0]);
            pivotTable.RemoveField(PivotFieldType.Row, "AccDate");

            Console.WriteLine(pivotTable.RowFields[0].Name);
            for (int i = 0; i < pivotTable.RowFields.Count; i++)
            {
                Console.WriteLine($"RowField Name: {pivotTable.RowFields[i].Name}: " +
                    $"Position: {pivotTable.RowFields[i].Position}");
                Console.WriteLine($"\t\t\t" +
                    $"BaseIndex: {pivotTable.RowFields[i].BaseIndex}");
                //Console.WriteLine("\n");
            }

            pivotTable.ShowInCompactForm();
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            pivotTable.RefreshDataOnOpeningFile = true;
            //CELLSNET-54576
            Assert.AreEqual("", wsSheet1.Cells["C1"].StringValue);
            // Pivot Chart
            int indChart = wsSheet1.Charts.Add(Aspose.Cells.Charts.ChartType.Column3DClustered, 0, 5, 28, 16);
            // Setting the pivot chart data source
            wsSheet1.Charts[indChart].PivotSource = "Sheet1!PivotTbl";

            pivotTable.RefreshData();
            pivotTable.CalculateData();
            int indSlicer = wsSheet1.Slicers.Add(pivotTable, "H30", pivotTable.BaseFields["Years"]);
            //int indSlicer = wsSheet1.Slicers.Add(pivotTable, "H30", pivotTable.BaseFields[18]);
            Slicer slicer = wsSheet1.Slicers[indSlicer];
            slicer.AddPivotConnection(pivotTable);

            wbCFPiv.Save(Constants.PivotTableDestPath + "CellsNet54396_1.xlsx");
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


