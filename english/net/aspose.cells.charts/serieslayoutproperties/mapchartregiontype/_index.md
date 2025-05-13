---
title: SeriesLayoutProperties.MapChartRegionType
second_title: Aspose.Cells for .NET API Reference
description: SeriesLayoutProperties property. Gets and sets the region type of the map
type: docs
url: /net/aspose.cells.charts/serieslayoutproperties/mapchartregiontype/
---
## SeriesLayoutProperties.MapChartRegionType property

Gets and sets the region type of the map.

```csharp
public MapChartRegionType MapChartRegionType { get; set; }
```

### Examples

```csharp
// Called: series.LayoutProperties.MapChartRegionType = MapChartRegionType.CountryRegionList;
public static void SeriesLayoutProperties_Property_MapChartRegionType()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
            worksheet.Cells["A1"].PutValue("Country");
            worksheet.Cells["A2"].PutValue("USA");
            worksheet.Cells["A3"].PutValue("Canada");
            worksheet.Cells["A4"].PutValue("Mexico");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // Add a map chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Map, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Set the chart data range
            chart.SetChartDataRange("A1:B4", true);

            // Set the region type of the map chart
            foreach (Series series in chart.NSeries)
            {
                series.LayoutProperties.MapChartRegionType = MapChartRegionType.CountryRegionList;
            }

            // Save the workbook
            workbook.Save("MapChartRegionTypeExample.xlsx");

            // Output the result
            Console.WriteLine("Map chart with region type 'CountryRegionList' created successfully.");
        }
```

### See Also

* enum [MapChartRegionType](../../mapchartregiontype/)
* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


