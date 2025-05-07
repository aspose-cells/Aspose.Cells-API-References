---
title: PivotField.ShowCompact
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Indicates whether display labels from the next field in the same column on the Pivot Table view
type: docs
url: /net/aspose.cells.pivot/pivotfield/showcompact/
---
## PivotField.ShowCompact property

Indicates whether display labels from the next field in the same column on the Pivot Table view

```csharp
public bool ShowCompact { get; set; }
```

### Examples

```csharp
// Called: pt.RowFields[i].ShowCompact = false;
[Test]
        public void Property_ShowCompact()
        {
            string filePath = Constants.PivotTableSourcePath + @"NET43403And42933_";

            #region CELLSNET-43403
            Workbook wb = new Workbook(filePath + "TestAspose.xlsx");
            Worksheet sheet3 = wb.Worksheets["Sheet3"];

            foreach (PivotTable pivotTable in sheet3.PivotTables)
            {
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            Assert.AreEqual(sheet3.Cells["A6"].StringValue, "Row Labels");

            Worksheet sheet2 = wb.Worksheets["Sheet2"];

            foreach (PivotTable pivotTable in sheet2.PivotTables)
            {
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            Assert.AreEqual(sheet2.Cells["A40"].StringValue, "Row Labels");
            wb.Save(Constants.PivotTableDestPath + @"NET43403And42933.xlsx");
            #endregion

            #region CELLSNET-42933
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx);

            Workbook workBook = new Workbook(filePath + @"TestPivot.xlsx", loadOptions);

            if (workBook.Worksheets["Pivot"] != null)
            {

                workBook.Worksheets.RemoveAt("Pivot");

                workBook.Worksheets.RemoveAt("Evaluation Warning");

            }

            Worksheet sheet = workBook.Worksheets.Add("Pivot");


            Worksheet sourceSheet = workBook.Worksheets["Source"];

            Cells cell = sourceSheet.Cells;

            Aspose.Cells.Range cellRange = cell.MaxDisplayRange;

            string sourcedata = cellRange.RefersTo.ToString();



            PivotTableCollection pivotTables = sheet.PivotTables;

            int iPivotIndex = sheet.PivotTables.Add(sourcedata, "A3", "PivoteTable");

            PivotTable pt = pivotTables[iPivotIndex];


            pt.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, "Employee Name");

            pt.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, "Employee Dept");


            pt.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, "Salary");


            pt.DataFields["Salary"].Function = ConsolidationFunction.Sum;


            //pt.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Column, pt.DataField);


            //pt.ColumnFields[0].DisplayName = "Values";


            // uncheck subtotal country rows

            PivotFieldCollection pivotFields = pt.RowFields;

            pivotFields[0].IsAutoSubtotals = false;


            pt.IsAutoFormat = true;

            pt.AutoFormatType = PivotTableAutoFormatType.Classic;

            pt.PivotTableStyleType = PivotTableStyleType.PivotTableStyleLight16;


            for (int i = 0; i < (pt.RowFields.Count - 1); i++)
            {

                pt.RowFields[i].ShowCompact = false;

                pt.RowFields[i].ShowInOutlineForm = true;

                pt.RowFields[i].ShowSubtotalAtTop = false;


            }


            for (int i = 0; i < (pt.ColumnFields.Count - 1); i++)
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

            Assert.AreEqual(sheet.Cells["A3"].StringValue, "Sum of Salary");
            Assert.AreEqual(sheet.Cells["A4"].StringValue, "Employee Name");
            Assert.AreEqual(sheet.Cells["B4"].StringValue, "Employee Dept");

            sheet.PivotTables[0].RefreshDataOnOpeningFile = false;

            sheet.AutoFitColumns();

            workBook.AcceptAllRevisions();


            //XLSX is not correct

            workBook.Save(Constants.PivotTableDestPath + @"NET43403And42933outTestPivot.xlsx", SaveFormat.Xlsx);


            //XLS is correct

            workBook.Save(Constants.PivotTableDestPath + @"NET43403And42933outTestPivot.xls", SaveFormat.Excel97To2003);
            #endregion
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


