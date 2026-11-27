---
title: "Axis.CategoryType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Axis egenskap. Representerar typen av kategori-axeln"
type: docs
url: /sv/net/aspose.cells.charts/axis/categorytype/
---
## Axis.CategoryType property

Representerar typen av kategoriaxeln.

```csharp
public CategoryType CategoryType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyCategoryTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells["A" + i].PutValue("Cat " + (i - 1));
                sheet.Cells["B" + i].PutValue(i * 10);
            }

            // Lägg till ett diagram
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 2, 25, 11);
            Chart chart = sheet.Charts[chartIndex];
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("=Sheet1!$A$1:$B$10", true);

            // Demonstrera CategoryType-egenskapen
            chart.CategoryAxis.CategoryType = Aspose.Cells.Charts.CategoryType.AutomaticScale;
            Console.WriteLine("CategoryType set to AutomaticScale");

            // Spara arbetsboken
            workbook.Save("AxisPropertyCategoryTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* enum [CategoryType](../../categorytype/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


