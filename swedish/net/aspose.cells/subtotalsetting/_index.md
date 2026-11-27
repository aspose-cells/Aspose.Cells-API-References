---
title: "Klass SubtotalSetting"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.SubtotalSetting-klass. Representerar inställningen för delsummeringen"
type: docs
url: /sv/net/aspose.cells/subtotalsetting/
---
## SubtotalSetting class

Representerar inställningen för delsumma.

```csharp
public class SubtotalSetting
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [GroupBy](../../aspose.cells/subtotalsetting/groupby/) { get; } | Fältet att gruppera efter, som ett nollbaserat heltalsavstånd |
| [SubtotalFunction](../../aspose.cells/subtotalsetting/subtotalfunction/) { get; } | Delssummafunktionen. |
| [SummaryBelowData](../../aspose.cells/subtotalsetting/summarybelowdata/) { get; } | Anger om en sammanfattning ska läggas till under data. |
| [TotalList](../../aspose.cells/subtotalsetting/totallist/) { get; } | En array av nollbaserade fältavstånd, som anger vilka fält som delsummeringar läggs till. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassSubtotalSettingDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Lägg till exempeldata i kalkylbladet
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["B1"].PutValue("Value");
                worksheet.Cells["A2"].PutValue("Group A");
                worksheet.Cells["A3"].PutValue("Group B");
                worksheet.Cells["A4"].PutValue("Group A");
                worksheet.Cells["A5"].PutValue("Group B");
                worksheet.Cells["B2"].PutValue(100);
                worksheet.Cells["B3"].PutValue(200);
                worksheet.Cells["B4"].PutValue(300);
                worksheet.Cells["B5"].PutValue(400);

                // Definiera cellområdet för delsummeringar
                CellArea area = CellArea.CreateCellArea("A1", "B5");

                // Tillämpa delsummeringar på data
                worksheet.Cells.Subtotal(
                    area,
                    0, // Group by first column (Category)
                    ConsolidationFunction.Sum,
                    new int[] { 1 }, // Subtotal on second column (Value)
                    true,
                    true,
                    true);

                // Hämta SubtotalSetting från kalkylbladet
                SubtotalSetting subtotalSetting = worksheet.Cells.RetrieveSubtotalSetting(area);

                // Visa egenskaperna för SubtotalSetting
                Console.WriteLine("Subtotal Setting Properties:");
                Console.WriteLine($"GroupBy field index: {subtotalSetting.GroupBy}");
                Console.WriteLine($"Subtotal Function: {subtotalSetting.SubtotalFunction}");
                Console.WriteLine($"TotalList contains column index: {subtotalSetting.TotalList[0]}");
                Console.WriteLine($"Summary Below Data: {subtotalSetting.SummaryBelowData}");

                // Spara arbetsboken
                workbook.Save("SubtotalSettingDemo.xlsx");
                Console.WriteLine("SubtotalSetting demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SubtotalSetting: {ex.Message}");
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


