---
title: PivotTable.ColumnFields
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Returns a PivotFields object that are currently shown as column fields
type: docs
url: /net/aspose.cells.pivot/pivottable/columnfields/
---
## PivotTable.ColumnFields property

Returns a PivotFields object that are currently shown as column fields.

```csharp
public PivotFieldCollection ColumnFields { get; }
```

### Examples

```csharp
// Called: for (int i = 0; i &amp;lt; (pt.ColumnFields.Count - 1); i++)
[Test]
        public void Property_ColumnFields()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET43403And42933_&quot;;

            #region CELLSNET-43403
            Workbook wb = new Workbook(filePath + &quot;TestAspose.xlsx&quot;);
            Worksheet sheet3 = wb.Worksheets[&quot;Sheet3&quot;];

            foreach (PivotTable pivotTable in sheet3.PivotTables)
            {
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            Assert.AreEqual(sheet3.Cells[&quot;A6&quot;].StringValue, &quot;Row Labels&quot;);

            Worksheet sheet2 = wb.Worksheets[&quot;Sheet2&quot;];

            foreach (PivotTable pivotTable in sheet2.PivotTables)
            {
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            Assert.AreEqual(sheet2.Cells[&quot;A40&quot;].StringValue, &quot;Row Labels&quot;);
            wb.Save(Constants.PivotTableDestPath + @&quot;NET43403And42933.xlsx&quot;);
            #endregion

            #region CELLSNET-42933
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx);

            Workbook workBook = new Workbook(filePath + @&quot;TestPivot.xlsx&quot;, loadOptions);

            if (workBook.Worksheets[&quot;Pivot&quot;] != null)
            {

                workBook.Worksheets.RemoveAt(&quot;Pivot&quot;);

                workBook.Worksheets.RemoveAt(&quot;Evaluation Warning&quot;);

            }

            Worksheet sheet = workBook.Worksheets.Add(&quot;Pivot&quot;);


            Worksheet sourceSheet = workBook.Worksheets[&quot;Source&quot;];

            Cells cell = sourceSheet.Cells;

            Aspose.Cells.Range cellRange = cell.MaxDisplayRange;

            string sourcedata = cellRange.RefersTo.ToString();



            PivotTableCollection pivotTables = sheet.PivotTables;

            int iPivotIndex = sheet.PivotTables.Add(sourcedata, &quot;A3&quot;, &quot;PivoteTable&quot;);

            PivotTable pt = pivotTables[iPivotIndex];


            pt.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;Employee Name&quot;);

            pt.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;Employee Dept&quot;);


            pt.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, &quot;Salary&quot;);


            pt.DataFields[&quot;Salary&quot;].Function = ConsolidationFunction.Sum;


            //pt.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Column, pt.DataField);


            //pt.ColumnFields[0].DisplayName = &quot;Values&quot;;


            // uncheck subtotal country rows

            PivotFieldCollection pivotFields = pt.RowFields;

            pivotFields[0].IsAutoSubtotals = false;


            pt.IsAutoFormat = true;

            pt.AutoFormatType = PivotTableAutoFormatType.Classic;

            pt.PivotTableStyleType = PivotTableStyleType.PivotTableStyleLight16;


            for (int i = 0; i &lt; (pt.RowFields.Count - 1); i++)
            {

                pt.RowFields[i].ShowCompact = false;

                pt.RowFields[i].ShowInOutlineForm = true;

                pt.RowFields[i].ShowSubtotalAtTop = false;


            }


            for (int i = 0; i &lt; (pt.ColumnFields.Count - 1); i++)
            {

                pt.RowFields[i].ShowCompact = false;

                pt.RowFields[i].ShowInOutlineForm = true;

                pt.RowFields[i].ShowSubtotalAtTop = false;


            }


            // pt.ColumnFields[0].IsAutoSort = true;


            pt.IsGridDropZones = true;


            sheet.PivotTables[0].RefreshData();

            sheet.PivotTables[0].CalculateData();

            sheet.PivotTables[0].CalculateRange();

            Assert.AreEqual(sheet.Cells[&quot;A3&quot;].StringValue, &quot;Sum of Salary&quot;);
            Assert.AreEqual(sheet.Cells[&quot;A4&quot;].StringValue, &quot;Employee Name&quot;);
            Assert.AreEqual(sheet.Cells[&quot;B4&quot;].StringValue, &quot;Employee Dept&quot;);

            sheet.PivotTables[0].RefreshDataOnOpeningFile = false;

            sheet.AutoFitColumns();

            workBook.AcceptAllRevisions();


            //XLSX is not correct

            workBook.Save(Constants.PivotTableDestPath + @&quot;NET43403And42933outTestPivot.xlsx&quot;, SaveFormat.Xlsx);


            //XLS is correct

            workBook.Save(Constants.PivotTableDestPath + @&quot;NET43403And42933outTestPivot.xls&quot;, SaveFormat.Excel97To2003);
            #endregion
        }
```

### See Also

* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


