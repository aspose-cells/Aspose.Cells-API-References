---
title: Chart.DisplayNaAsBlank
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Indicates whether displaying N/A as blank value
type: docs
url: /net/aspose.cells.charts/chart/displaynaasblank/
---
## Chart.DisplayNaAsBlank property

Indicates whether displaying #N/A as blank value.

```csharp
public bool DisplayNaAsBlank { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine(chart.DisplayNaAsBlank);
[Test]
        public void Property_DisplayNaAsBlank()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsJava43378.xlsx&quot;);

            Workbook workbook2 = new Workbook();
            //System.out.println(&quot;post-clone&quot;);
            workbook2.Copy(workbook);
            WorksheetCollection sheets = workbook2.Worksheets;
            for (int i = 0; i &lt; sheets.Count; i++)
            {
                Worksheet sheet = sheets[i];
                ChartCollection charts = sheet.Charts;
                for (int j = 0; j &lt; charts.Count; j++)
                {
                    Chart chart = sheet.Charts[j];
                    Console.WriteLine(chart.DisplayNaAsBlank);

                }
            }
            workbook2.Save(Constants.destPath + &quot;CellsJava43378.xlsx&quot;);
        }
```

### See Also

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


