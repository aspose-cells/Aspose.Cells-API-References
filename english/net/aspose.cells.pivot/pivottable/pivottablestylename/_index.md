---
title: PivotTable.PivotTableStyleName
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Gets and sets the pivottable style name
type: docs
url: /net/aspose.cells.pivot/pivottable/pivottablestylename/
---
## PivotTable.PivotTableStyleName property

Gets and sets the pivottable style name.

```csharp
public string PivotTableStyleName { get; set; }
```

### Examples

```csharp
// Called: pivotTable.PivotTableStyleName = &amp;quot;MSDPivotStyle&amp;quot;;
[Test]
        public void Property_PivotTableStyleName()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET47010_&quot;;

            Workbook workbook = null;
            workbook = new Workbook(filePath + &quot;Template.xlsx&quot;);

            //Copy MSD Styles sheet to template file
            string stypeFilePath = filePath + &quot;MSDStylesAspose.xlsx&quot;;
            Workbook workbookStyle = null;
            workbookStyle = new Workbook(stypeFilePath);

            // Copy the first sheet of the first book into second book.
            var wsStyle = workbook.Worksheets.Add();
            workbook.Worksheets[wsStyle].Copy(workbookStyle.Worksheets[&quot;MSDStyles&quot;]);

            var tblName = &quot;tblOpenPositions&quot;;
            var dataSet = new DataSet();
            dataSet.ReadXml(filePath + &quot;MyDataset.xml&quot;, XmlReadMode.ReadSchema);
            dataSet.Tables[0].TableName = tblName;

            var designer = new WorkbookDesigner { Workbook = workbook };
            designer.SetDataSource(dataSet.Tables[0]);
            // Process the smart markers
            designer.Process(true);

            var pivotWorksheet = workbook.Worksheets[&quot;PivotOpenPositions&quot;];
            var pivotTables = pivotWorksheet.PivotTables;
            var pivotTable = pivotTables[tblName];

            pivotTable.PivotTableStyleName = &quot;MSDPivotStyle&quot;;
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            //pivotTable.CalculateRange();

            pivotTable.RefreshDataOnOpeningFile = false;

            workbook.CalculateFormula();
            var pivotrange = pivotWorksheet.Cells.CreateRange(&quot;A2&quot;, &quot;J25&quot;);

            var pivotWorksheetCopy = workbook.Worksheets[&quot;PivotCopy&quot;];

            Cell sourceB2 = pivotWorksheet.Cells[&quot;B2&quot;];
            Cell destB2 = pivotWorksheetCopy.Cells[&quot;B2&quot;];

            var cells = pivotWorksheetCopy.Cells;
            var range2 = cells.CreateRange(&quot;A2&quot;, &quot;J25&quot;);
            range2.Copy(pivotrange);
            pivotWorksheetCopy.AutoFitColumns();


            Style b2 = workbook.Worksheets[&quot;PivotCopy&quot;].Cells[&quot;B2&quot;].GetStyle();
            Style d2 = workbook.Worksheets[&quot;PivotCopy&quot;].Cells[&quot;D2&quot;].GetStyle();
            Style g2 = workbook.Worksheets[&quot;PivotCopy&quot;].Cells[&quot;G2&quot;].GetStyle();
            Style i2 = workbook.Worksheets[&quot;PivotCopy&quot;].Cells[&quot;I2&quot;].GetStyle();
            Assert.AreEqual(b2.ForegroundColor, Color.FromArgb(255, 255, 242, 204));
            Assert.AreEqual(d2.ForegroundColor, Color.FromArgb(255, 255, 242, 204));
            Assert.AreEqual(g2.ForegroundColor, Color.FromArgb(255, 255, 242, 204));
            Assert.AreEqual(i2.ForegroundColor, Color.FromArgb(255, 255, 242, 204));

            workbook.Save(CreateFolder(filePath) + &quot;out.xlsx&quot;, SaveFormat.Xlsx);
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


