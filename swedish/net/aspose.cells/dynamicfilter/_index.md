---
title: "Class DynamicFilter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.DynamicFilter-klass. Representerar det dynamiska filtret"
type: docs
url: /sv/net/aspose.cells/dynamicfilter/
---
## DynamicFilter class

Representerar det dynamiska filtret.

```csharp
public class DynamicFilter
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [DynamicFilterType](../../aspose.cells/dynamicfilter/dynamicfiltertype/) { get; set; } | Hämtar och anger typen för detta dynamiska filter. |
| [MaxValue](../../aspose.cells/dynamicfilter/maxvalue/) { get; set; } | Hämtar och anger det maximala värdet för det dynamiska filtret. |
| [Value](../../aspose.cells/dynamicfilter/value/) { get; set; } | Hämtar och anger värdet för det dynamiska filtret. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassDynamicFilterDemo
    {
        public static void Run()
        {
            try
            {
                // Skapa en arbetsbok och ett kalkylblad (valfritt för sammanhang)
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Name = "DemoSheet";

                // Fyll i några exempel på numeriska data
                worksheet.Cells["A1"].PutValue("Numbers");
                worksheet.Cells["A2"].PutValue(10);
                worksheet.Cells["A3"].PutValue(20);
                worksheet.Cells["A4"].PutValue(30);
                worksheet.Cells["A5"].PutValue(40);
                worksheet.Cells["A6"].PutValue(50);

                // Definiera ett autofilterintervall
                worksheet.AutoFilter.Range = "A1:A6";

                // Applicera ett dynamiskt filter (AboveAverage) på den första kolumnen
                worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.AboveAverage);

                // Hämta DynamicFilter-instansen som skapats av AutoFilter
                DynamicFilter filter = (DynamicFilter)worksheet.AutoFilter.FilterColumns[0].Filter;

                // Ställ in ytterligare egenskaper om så önskas
                filter.Value = 25;      // Example custom value
                filter.MaxValue = 45;   // Example max value

                // Visa de inställda egenskaperna
                Console.WriteLine($"DynamicFilterType: {filter.DynamicFilterType}");
                Console.WriteLine($"Value: {filter.Value}");
                Console.WriteLine($"MaxValue: {filter.MaxValue}");

                // Uppdatera filtret för att tillämpa ändringarna
                worksheet.AutoFilter.Refresh();

                // Spara arbetsboken (de filtrerade data kommer att sparas)
                workbook.Save("DynamicFilterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with DynamicFilter: {ex.Message}");
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


