---
title: Series.LegendEntry
second_title: Aspose.Cells for .NET API Reference
description: Series property. Gets the legend entry according to this series
type: docs
url: /net/aspose.cells.charts/series/legendentry/
---
## Series.LegendEntry property

Gets the legend entry according to this series.

```csharp
public LegendEntry LegendEntry { get; }
```

### Examples

```csharp
// Called: Console.WriteLine(series.LegendEntry.IsDeleted.ToString());  //yeilds true!
[Test]
        // http://www.aspose.com/community/forums/thread/289097/legendentry.isdeleted-not-working.aspx
        // LegendEntry.IsDeleted not working?
        public void Property_LegendEntry()
        {
            Console.WriteLine("Property_LegendEntry()");
            string infn = path + @"CELLSNET-25031\Layout+and+load+diagrams.xlsx";
            string outfn = Constants.destPath + @"CELLSNET-25031.xlsx";

            Workbook workbook = new Workbook(infn);
            Chart c = workbook.Worksheets[1].Charts[0];
            Series series = c.NSeries[0];
            series.LegendEntry.IsDeleted = false;
            Console.WriteLine(series.LegendEntry.IsDeleted.ToString());  //yeilds true! 
            Console.WriteLine(series.Name);
            Console.WriteLine(series.XValues);
            Console.WriteLine(series.Values);
            workbook.Save(outfn, SaveFormat.Xlsx);
        }
```

### See Also

* class [LegendEntry](../../legendentry/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


