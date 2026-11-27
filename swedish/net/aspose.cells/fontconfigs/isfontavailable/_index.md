---
title: "FontConfigs.IsFontAvailable"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FontConfigs-metoden. Anger om teckensnittet är tillgängligt"
type: docs
url: /sv/net/aspose.cells/fontconfigs/isfontavailable/
---
## FontConfigs.IsFontAvailable method

Indikera om teckensnittet är tillgängligt.

```csharp
public static bool IsFontAvailable(string fontName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fontName | String | teckensnittsnamn |

### Returvärde

true om teckensnittet är tillgängligt, annars false.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsMethodIsFontAvailableWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Testa teckensnittsnamn för att kontrollera tillgänglighet
            string[] testFonts = { "Arial", "Times New Roman", "NonExistentFont" };

            try
            {
                foreach (string fontName in testFonts)
                {
                    // Anropa metoden IsFontAvailable med teckensnittets namn
                    bool isAvailable = FontConfigs.IsFontAvailable(fontName);

                    // Visa resultatet
                    Console.WriteLine($"Font '{fontName}' is available: {isAvailable}");

                    // Skriv resultatet till kalkylbladet
                    int row = worksheet.Cells.MaxDataRow + 1;
                    worksheet.Cells[row, 0].PutValue($"Font '{fontName}' available:");
                    worksheet.Cells[row, 1].PutValue(isAvailable);
                }

                Console.WriteLine("Method executed successfully with parameters (String)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IsFontAvailable method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("FontConfigsMethodIsFontAvailableWithStringDemo.xlsx");
        }
    }
}
```

### Se även

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


