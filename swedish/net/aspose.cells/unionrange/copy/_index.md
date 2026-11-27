---
title: "UnionRange.Copy"
second_title: "Aspose.Cells för .NET API‑referens"
description: "UnionRange‑metod. Kopierar området med specialklistra‑alternativ"
type: docs
url: /sv/net/aspose.cells/unionrange/copy/
---
## UnionRange.Copy method

Kopierar området med specialklistra in-alternativ.

```csharp
public void Copy(UnionRange range, PasteOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| område | UnionRange | Det källintervallet. |
| alternativ | PasteOptions | De specialklistra-alternativen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodCopyWithUnionRangePasteOptionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Source Data");
            worksheet.Cells["B1"].PutValue("Value1");
            worksheet.Cells["A2"].PutValue("More Data");
            worksheet.Cells["B2"].PutValue("Value2");

            try
            {
                // Skapa käll‑UnionRange
                UnionRange sourceRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(
                    new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });

                // Skapa destination UnionRange
                UnionRange destinationRange = worksheet.Cells.CreateRange("D1:E2").UnionRanges(
                    new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("D1:E2") });

                // Skapa PasteOptions med specifika inställningar
                PasteOptions options = new PasteOptions();
                options.PasteType = PasteType.All;
                options.SkipBlanks = true;
                options.Transpose = false;

                // Anropa Copy‑metoden
                sourceRange.Copy(destinationRange, options);

                Console.WriteLine("Copy method executed successfully");
                Console.WriteLine($"Destination range: {destinationRange.RefersTo}");

                // Spara arbetsboken
                workbook.Save("UnionRangeCopyDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling Copy: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [PasteOptions](../../pasteoptions/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


