---
title: "GlobalizationSettings.Compare"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GlobalizationSettings-metoden. Jämför två strängvärden enligt vissa sorteringsregler"
type: docs
url: /sv/net/aspose.cells/globalizationsettings/compare/
---
## GlobalizationSettings.Compare method

Jämför två strängvärden enligt vissa kollationsregler.

```csharp
public virtual int Compare(string v1, string v2, bool ignoreCase)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| v1 | String | den första strängen |
| v2 | String | den andra strängen |
| ignoreCase | Boolean | om skiftlägeskänslighet ska ignoreras vid jämförelse av värden |

### Returvärde

Heltal som indikerar det lexikala förhållandet mellan de två jämförelseobjekten

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodCompareWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Skapa arbetsbok med anpassade globaliseringsinställningar
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomComparisonSettings();

            try
            {
                // Demonstrera direkt användning av Compare-metoden
                GlobalizationSettings settings = workbook.Settings.GlobalizationSettings;
                int result1 = settings.Compare("Apple", "apple", true);
                int result2 = settings.Compare("Apple", "apple", false);
                
                Console.WriteLine($"Case-insensitive comparison result: {result1}");
                Console.WriteLine($"Case-sensitive comparison result: {result2}");

                // Demonstrera effekt på kalkylbladsoperationer
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Banana");
                worksheet.Cells["A2"].PutValue("apple");
                worksheet.Cells["A3"].PutValue("Cherry");

                // Sortera data med anpassad jämförelse
                DataSorter sorter = workbook.DataSorter;
                sorter.Order1 = SortOrder.Ascending;
                sorter.Key1 = 0;
                sorter.Sort(worksheet.Cells, 0, 0, 2, 0); // Corrected range to rows 0-2

                Console.WriteLine("Sorted data with custom comparison rules:");
                for (int row = 0; row < 3; row++)
                {
                    Cell cell = worksheet.Cells[row, 0];
                    Console.WriteLine(cell.StringValue);
                }

                workbook.Save("GlobalizationCompareDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CustomComparisonSettings : GlobalizationSettings
    {
        public override int Compare(string v1, string v2, bool ignoreCase)
        {
            // Implementera anpassad jämförelselogik
            var comparison = ignoreCase ? 
                StringComparison.OrdinalIgnoreCase : 
                StringComparison.Ordinal;
            
            return string.Compare(v1?.Trim() ?? "", v2?.Trim() ?? "", comparison);
        }
    }
}
```

### Se även

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


