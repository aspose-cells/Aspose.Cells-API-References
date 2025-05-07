---
title: PivotConditionalFormat.ScopeType
second_title: Aspose.Cells for .NET API Reference
description: PivotConditionalFormat property. Get and set scope type for the pivot table conditional format 
type: docs
url: /net/aspose.cells.pivot/pivotconditionalformat/scopetype/
---
## PivotConditionalFormat.ScopeType property

Get and set scope type for the pivot table conditional format .

```csharp
public PivotConditionFormatScopeType ScopeType { get; set; }
```

### Examples

```csharp
// Called: pivForCond.ScopeType = PivotConditionFormatScopeType.Data;
[Test]
        public void Property_ScopeType()
        {
            byte[] SrcDataByteArray = Encoding.ASCII.GetBytes(
 $@"City,Product,Sales
Paris,Cream,2300
Paris,Lotion,1600
Tunis,Cream,900
Tunis,Lotion,1400
Tunis,Cream,3090
Tunis,Lotion,6000
Paris,Cream,4320");

            // Create a memory stream from the source data
            MemoryStream dataStream = new MemoryStream(SrcDataByteArray);

            // Create LoadOptions class object to load the comma-separated data given above
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Csv);

            // Instantiate a workbook class object having above mentioned data
            Workbook wbCSV = new Workbook(dataStream, loadOptions);

            // Get access to the first worksheet in the collection
            Worksheet targetSheet = wbCSV.Worksheets[0];

            // Get collection of pivot tables in the target worksheet
            Aspose.Cells.Pivot.PivotTableCollection pvTablesCollection = targetSheet.PivotTables;

            // Get pivot table index after adding a new pivot table by provding source data range and destination cell
            int iNewPivotTable = pvTablesCollection.Add("=A1:C8", "F3", "MyPivotTable");

            // Get the instance of newly added pivot table for further processing
            Aspose.Cells.Pivot.PivotTable excelPivot = pvTablesCollection[iNewPivotTable];

            // Hide the grand total for rows in the output Excel file
            excelPivot.ShowRowGrandTotals = false;
            excelPivot.ShowColumnGrandTotals = false;

            // Add the first field to the column area
            excelPivot.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Column, 0);
            // Add the second field to the row area
            excelPivot.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, 1);
            // Add the third field to the data area
            excelPivot.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, 2);


            // Conditional formatting

            //int ind = targetSheet.ConditionalFormattings.Add();
            //FormatConditionCollection fcs = targetSheet.ConditionalFormattings[ind];
            //CellArea cellArea = new CellArea()
            //{
            //    StartRow = 1,
            //    EndRow = 7,
            //    StartColumn = 2,
            //    EndColumn = 2
            //};
            //fcs.AddArea(cellArea);

            //int indexCond = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "1", null);
            //fcs[indexCond].Style.BackgroundColor = ColorTranslator.FromHtml("#e39e9e");



            int ind = excelPivot.ConditionalFormats.Add();
            PivotConditionalFormat pivForCond = excelPivot.ConditionalFormats[ind];
            pivForCond.ScopeType = PivotConditionFormatScopeType.Data;
            //pivForCond.AddDataAreaCondition(excelPivot.DataFields[0]);

            PivotArea pivotArea = new PivotArea(excelPivot);
            pivotArea.SelectField(PivotFieldType.Data, excelPivot.DataFields[0]);
            pivForCond.PivotAreas.Add(pivotArea);

            int indexCond = pivForCond.FormatConditions.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "1", null);
            pivForCond.FormatConditions[indexCond].Style.BackgroundColor = ColorTranslator.FromHtml("#e39e9e");
            pivForCond.FormatConditions.AddArea(excelPivot.DataBodyRange);
            //excelPivot.RefreshData();
            //excelPivot.CalculateData();
            //pivForCond.SetConditionalAreas();


            // Saving the output Excel file with pivot table
            wbCSV.Save(Constants.PivotTableDestPath + "CELLSNET-57427.xlsx");
            wbCSV = new Workbook(Constants.PivotTableDestPath + "CELLSNET-57427.xlsx");
            Assert.AreEqual(1, wbCSV.Worksheets[0].ConditionalFormattings.Count);

            System.Console.WriteLine("Done");
        }
```

### See Also

* enum [PivotConditionFormatScopeType](../../pivotconditionformatscopetype/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


