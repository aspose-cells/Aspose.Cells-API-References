---
title: "Enum SaveElementType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Saving.SaveElementType enum. Representerar vilken typ av element som ska sparas"
type: docs
url: /sv/net/aspose.cells.saving/saveelementtype/
---
## SaveElementType enumeration

Representerar vilken typ av element som bör sparas.

```csharp
public enum SaveElementType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| All | `251658239` | All data. |
| Chart | `256` | Endast diagram. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Saving;
    using System;

    public class SavingClassSaveElementTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Lägg till lite exempeldata för att demonstrera sparande
                worksheet.Cells["A1"].PutValue("Sample Data");
                worksheet.Cells["B1"].PutValue(12345);

                // Skapa ett diagram för att demonstrera diagramets spar-elementtyp
                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
                Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("A1:B1", true);

                // Demonstrera användning av SaveElementType enum‑värden
                SaveElementType chartType = SaveElementType.Chart;
                SaveElementType allType = SaveElementType.All;

                Console.WriteLine($"Chart SaveElementType value: {chartType}");
                Console.WriteLine($"All SaveElementType value: {allType}");

                // Spara arbetsboken med alla element
                OoxmlSaveOptions saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx);
                workbook.Save("SaveElementTypeDemo.xlsx", saveOptions);
                Console.WriteLine("Workbook saved successfully with all elements");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SaveElementType: {ex.Message}");
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


