---
title: Chart.ShowDataTable
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Gets or sets a value indicating whether the chart displays a data table
type: docs
url: /net/aspose.cells.charts/chart/showdatatable/
---
## Chart.ShowDataTable property

Gets or sets a value indicating whether the chart displays a data table.

```csharp
public bool ShowDataTable { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(chChart.ShowDataTable, true);
[Test]
        public void Property_ShowDataTable()
        {
            //Create a new Workbook.
            Workbook workbook = new Workbook();
            //Get the first worksheet.
            Worksheet sheet = workbook.Worksheets[0];

            //Set the name of worksheet


            sheet.Cells[0, 1].PutValue("column 1");
            sheet.Cells[0, 2].PutValue("column 2");
            sheet.Cells[1, 0].PutValue("alternative 1");
            sheet.Cells[2, 0].PutValue("alternative 2");
            sheet.Cells[3, 0].PutValue("alternative 3");

            sheet.Cells[1, 1].PutValue(0.25);
            sheet.Cells[2, 1].PutValue(0.5);
            sheet.Cells[3, 1].PutValue(0.25);
            sheet.Cells[1, 2].PutValue(0.33);
            sheet.Cells[2, 2].PutValue(0.33);
            sheet.Cells[3, 2].PutValue(0.33);
            int index = workbook.Worksheets.Add(SheetType.Chart);
            sheet = workbook.Worksheets[index];

            sheet.Charts.Add(ChartType.Column, 5, 1, 20, 10);
            Chart chChart = sheet.Charts[sheet.Charts.Count - 1];
            chChart.ChartArea.Area.Formatting = FormattingType.None;
            chChart.NSeries.Add("Sheet1!B2:C4", true);

            chChart.ShowDataTable = true;
            workbook.Save(Constants.destPath + "Cellsnet42837.xlsx");
            workbook = new Workbook(Constants.destPath + "Cellsnet42837.xlsx");
            chChart = workbook.Worksheets[index].Charts[0];
            Assert.AreEqual(chChart.ShowDataTable, true);
        }
```

### See Also

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


