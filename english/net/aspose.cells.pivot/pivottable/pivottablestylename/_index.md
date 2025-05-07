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
// Called: pivotTable.PivotTableStyleName = "MSDPivotStyle";
[Test]
        public void Property_PivotTableStyleName()
        {
            string filePath = Constants.PivotTableSourcePath + @"NET47010_";

            Workbook workbook = null;
            workbook = new Workbook(filePath + "Template.xlsx");

            //Copy MSD Styles sheet to template file
            string stypeFilePath = filePath + "MSDStylesAspose.xlsx";
            Workbook workbookStyle = null;
            workbookStyle = new Workbook(stypeFilePath);

            // Copy the first sheet of the first book into second book.
            var wsStyle = workbook.Worksheets.Add();
            workbook.Worksheets[wsStyle].Copy(workbookStyle.Worksheets["MSDStyles"]);

            var tblName = "tblOpenPositions";
            var dataSet = new DataSet();
            dataSet.ReadXml(filePath + "MyDataset.xml", XmlReadMode.ReadSchema);
            dataSet.Tables[0].TableName = tblName;

            var designer = new WorkbookDesigner { Workbook = workbook };
            designer.SetDataSource(dataSet.Tables[0]);
            // Process the smart markers
            designer.Process(true);

            var pivotWorksheet = workbook.Worksheets["PivotOpenPositions"];
            var pivotTables = pivotWorksheet.PivotTables;
            var pivotTable = pivotTables[tblName];

            pivotTable.PivotTableStyleName = "MSDPivotStyle";
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            //pivotTable.CalculateRange();

            pivotTable.RefreshDataOnOpeningFile = false;

            workbook.CalculateFormula();
            var pivotrange = pivotWorksheet.Cells.CreateRange("A2", "J25");

            var pivotWorksheetCopy = workbook.Worksheets["PivotCopy"];

            Cell sourceB2 = pivotWorksheet.Cells["B2"];
            Cell destB2 = pivotWorksheetCopy.Cells["B2"];

            var cells = pivotWorksheetCopy.Cells;
            var range2 = cells.CreateRange("A2", "J25");
            range2.Copy(pivotrange);
            pivotWorksheetCopy.AutoFitColumns();


            Style b2 = workbook.Worksheets["PivotCopy"].Cells["B2"].GetStyle();
            Style d2 = workbook.Worksheets["PivotCopy"].Cells["D2"].GetStyle();
            Style g2 = workbook.Worksheets["PivotCopy"].Cells["G2"].GetStyle();
            Style i2 = workbook.Worksheets["PivotCopy"].Cells["I2"].GetStyle();
            Assert.AreEqual(b2.ForegroundColor, Color.FromArgb(255, 255, 242, 204));
            Assert.AreEqual(d2.ForegroundColor, Color.FromArgb(255, 255, 242, 204));
            Assert.AreEqual(g2.ForegroundColor, Color.FromArgb(255, 255, 242, 204));
            Assert.AreEqual(i2.ForegroundColor, Color.FromArgb(255, 255, 242, 204));

            workbook.Save(CreateFolder(filePath) + "out.xlsx", SaveFormat.Xlsx);
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


