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
        public void PivotTable_Property_PivotTableStyleName()
        {
            string filePath = Constants.PivotTableSourcePath + @"NET46793_";

            Workbook workbook = null;
            workbook = new Workbook(filePath + "Template.xlsx");
#if NETCOREAPP2_0
            workbook.Settings.CultureInfo = new System.Globalization.CultureInfo("en-US");
#endif

            //Copy MSD Styles sheet to template file
            Workbook workbookStyle = null;
            workbookStyle = new Workbook(filePath + "MSDStylesAspose.xlsx");

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

            workbook.CalculateFormula();

            pivotTable.PivotTableStyleName = "MSDPivotStyle";
            pivotTable.RefreshDataOnOpeningFile = false;

            pivotTable.RefreshData();
            pivotTable.CalculateData();

            Cells cells = pivotWorksheet.Cells;
            Assert.AreEqual(cells["E2"].StringValue, "321,800,298 ");
            Assert.AreEqual(cells["E4"].StringValue, "101,576,039 ");
            Assert.AreEqual(cells["E13"].StringValue, "30,261,123 ");
            Assert.AreEqual(cells["E18"].StringValue, "(9,284,040)");

            workbook.Save(CreateFolder(filePath) + "out.xlsx", SaveFormat.Xlsx);
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


