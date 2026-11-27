---
title: "ChartCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartCollection-egenskap. Hämtar Chart‑elementet på det angivna indexet"
type: docs
url: /sv/net/aspose.cells.charts/chartcollection/item/
---
## ChartCollection indexer (1 of 2)

Hämtar [`Chart`](../../chart/) elementet på det angivna indexet.

```csharp
public Chart this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Det nollbaserade indexet för elementet. |

### Returvärde

Elementet på det angivna indexet.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            
            // Åtkomst till diagrammet via Item‑egenskapen
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets datakälla och titel
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            chart.Title.Text = "Sample Chart";
            chart.Title.TextHorizontalAlignment = TextAlignmentType.Center;
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
            
            Console.WriteLine("Chart created successfully with Item property access.");
        }
    }
}
```

### Se även

* class [Chart](../../chart/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ChartCollection indexer (2 of 2)

Hämtar diagrammet efter namn.

```csharp
public Chart this[string name] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| namn | Diagramnamnet. |

### Returvärde

Diagrammet.

### Anmärkningar

Standardnamnet för diagrammet är null. Så måste du uttryckligen ange namnet på diagrammet.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            try
            {
                // Lägg till ett diagram i kalkylbladet
                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);

                // Kom åt diagrammet med Item‑egenskapen (indexer)
                Chart chart = worksheet.Charts[chartIndex];

                // Visa information om diagrammet
                Console.WriteLine("Chart type: " + chart.Type);
                Console.WriteLine("Chart name: " + chart.Name);

                // Spara arbetsboken
                workbook.Save("ChartCollectionItemDemo.xlsx");

                Console.WriteLine("Chart created and accessed successfully using Item property.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [Chart](../../chart/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


