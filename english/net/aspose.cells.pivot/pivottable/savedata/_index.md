---
title: PivotTable.SaveData
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Indicates whether data for the PivotTable report is saved with the workbook
type: docs
url: /net/aspose.cells.pivot/pivottable/savedata/
---
## PivotTable.SaveData property

Indicates whether data for the PivotTable report is saved with the workbook.

```csharp
public bool SaveData { get; set; }
```

### Examples

```csharp
// Called: pivotTable.SaveData = true;
[Test]
        public void Property_SaveData()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET42799And42800And42801_&quot;;

            string template = &quot;MTR3100.xlsx&quot;;
            string excelOutput = &quot;ExcelOutput.xlsx&quot;;
            string pdfOutput = &quot;out.pdf&quot;;

            //Create WorkbookDesigner object.
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = new Workbook(filePath + excelOutput, new LoadOptions(LoadFormat.Xlsx));

            //Get all worksheet
            WorksheetCollection workSheets = designer.Workbook.Worksheets;
            Worksheet sheet = workSheets[&quot;Report&quot;];

            PivotTable pivotTable = sheet.PivotTables[0];

            //Export data table
            System.Data.DataTable dt = workSheets[&quot;DummyData&quot;].Cells.ExportDataTable(1, 0,
                122, 10, true);

            // Add default parameters
            designer.SetDataSource(&quot;BranchName&quot;, &quot;ASTON&quot;);
            designer.SetDataSource(&quot;DateName&quot;, DateTime.Now);
            designer.SetDataSource(&quot;Title&quot;, &quot;&quot;);

            //Set data source
            dt.TableName = &quot;Model&quot;;
            designer.SetDataSource(dt);

            //Process the markers.
            designer.Process();

            //Get and refresh pivot table
            if (pivotTable != null)
            {
                //Set the refresh data flag on

                //Refresh and calculate the pivot table data
                //pivotTable.MergeLabels = true;
                pivotTable.PreserveFormatting = true;
                pivotTable.SaveData = true;
                pivotTable.RefreshData();
                pivotTable.CalculateData();
                pivotTable.CalculateRange();
            }

            //Save PDF
            PdfSaveOptions options = new PdfSaveOptions();
            options.CalculateFormula = true;
            designer.Workbook.Save(Constants.PivotTableDestPath + @&quot;NET42799And42800And42801.xlsx&quot;);

            CellArea[] areas = sheet.Cells.GetMergedAreas();
            Assert.AreEqual(areas.Length, 35);
            CellArea area;
            bool b9b25 = false;
            bool b27b43 = false;
            bool f7h7 = false;
            bool j7l7 = false;
            bool b26e26 = false;
            bool b44e44 = false;
            bool c9c21 = false;
            bool i7i8 = false;
            bool d39e39 = false;
            for (int i = 0; i &lt; areas.Length; i++)
            {
                area = (CellArea)areas[i];
                if (IsEqualArea(area, CellArea.CreateCellArea(&quot;B9&quot;, &quot;B25&quot;)))
                {
                    b9b25 = true;
                }
                else if (IsEqualArea(area, CellArea.CreateCellArea(&quot;B27&quot;, &quot;B43&quot;)))
                {
                    b27b43 = true;
                }
                else if (IsEqualArea(area, CellArea.CreateCellArea(&quot;F7&quot;, &quot;H7&quot;)))
                {
                    f7h7 = true;
                }
                else if (IsEqualArea(area, CellArea.CreateCellArea(&quot;J7&quot;, &quot;L7&quot;)))
                {
                    j7l7 = true;
                }
                else if (IsEqualArea(area, CellArea.CreateCellArea(&quot;B26&quot;, &quot;E26&quot;)))
                {
                    b26e26 = true;
                }
                else if (IsEqualArea(area, CellArea.CreateCellArea(&quot;B44&quot;, &quot;E44&quot;)))
                {
                    b44e44 = true;
                }
                else if (IsEqualArea(area, CellArea.CreateCellArea(&quot;C9&quot;, &quot;C21&quot;)))
                {
                    c9c21 = true;
                }
                else if (IsEqualArea(area, CellArea.CreateCellArea(&quot;I7&quot;, &quot;I8&quot;)))
                {
                    i7i8 = true;
                }
                else if (IsEqualArea(area, CellArea.CreateCellArea(&quot;D39&quot;, &quot;E39&quot;)))
                {
                    d39e39 = true;
                }
            }
            Assert.AreEqual(b9b25 &amp;&amp; b27b43 &amp;&amp; f7h7 &amp;&amp; j7l7 &amp;&amp; b26e26 &amp;&amp; b44e44 &amp;&amp; c9c21 &amp;&amp; i7i8 &amp;&amp; d39e39, true);
            Assert.AreEqual(sheet.Cells[&quot;C43&quot;].StringValue, &quot;2 Total&quot;);
            Assert.AreEqual(sheet.Cells[&quot;C40&quot;].StringValue, &quot;1 Total&quot;);

            Assert.AreEqual(sheet.Cells[&quot;C25&quot;].StringValue, &quot;2 Total&quot;);
            Assert.AreEqual(sheet.Cells[&quot;C22&quot;].StringValue, &quot;1 Total&quot;);

            Assert.AreEqual(sheet.Cells[&quot;G8&quot;].StringValue, &quot;T.5&quot;);
            Assert.AreEqual(sheet.Cells[&quot;H8&quot;].StringValue, &quot;T.6&quot;);
            //Save Excel
            designer.Workbook.Save(Constants.PivotTableDestPath + @&quot;NET42799And42800And42801.xlsx&quot;, SaveFormat.Xlsx);
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


