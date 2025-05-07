---
title: Series.XValues
second_title: Aspose.Cells for .NET API Reference
description: Series property. Represents the x values of the chart series
type: docs
url: /net/aspose.cells.charts/series/xvalues/
---
## Series.XValues property

Represents the x values of the chart series.

```csharp
public string XValues { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual("=DatePerTagPivotTable!$A$4:$A$6", chart.NSeries[0].XValues );
[Test]
        public void Property_XValues()
        {
            string filePath = Constants.PivotTableSourcePath + @"JAVA41165_";
            //Load up workbook with pivot chart
            Workbook wb = new Workbook(filePath + "aspose-pivotchart-with-dates.xlsx");
            UpdateSourceData(wb);
            wb.Settings.FormulaSettings.EnableCalculationChain = false;
            wb.CalculateFormula();

            foreach (Worksheet sheet in wb.Worksheets)
            {
                sheet.AutoFitRows();
                RefreshPivotTables(sheet);
            }

            wb.Save(Constants.PivotTableDestPath + @"JAVA41165.xlsx");
            Chart chart = wb.Worksheets["DatePerTagPivotTable"].Charts[0];
            Assert.AreEqual(1, chart.NSeries.Count);
            Assert.AreEqual("=DatePerTagPivotTable!$B$4:$B$6", chart.NSeries[0].Values);
            Assert.AreEqual("=DatePerTagPivotTable!$A$4:$A$6", chart.NSeries[0].XValues );

            wb.Save(Constants.PivotTableDestPath + @"JAVA41165.pdf");
        }
```

### See Also

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


