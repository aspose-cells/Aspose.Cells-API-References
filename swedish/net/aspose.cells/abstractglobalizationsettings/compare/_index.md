---
title: "AbstractGlobalizationSettings.Compare"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AbstractGlobalizationSettings-metoden. Jämför två strängvärden enligt vissa sorteringsregler"
type: docs
url: /sv/net/aspose.cells/abstractglobalizationsettings/compare/
---
## AbstractGlobalizationSettings.Compare method

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

    public class AbstractGlobalizationSettingsMethodCompareWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Skapa anpassade globaliseringsinställningar som åsidosätter Compare-metoden
            var settings = new CustomGlobalizationSettings();
            
            // Skapa en arbetsbok med anpassade globaliseringsinställningar
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = settings;

            // Förbered strängarna för jämförelse
            string string1 = "Apple";
            string string2 = "apple";
            bool ignoreCase = true;

            try
            {
                // Compare-metoden kommer att anropas internt under operationer som sortering
                // Vi demonstrerar direkt användning här
                int comparisonResult = settings.Compare(string1, string2, ignoreCase);
                
                Console.WriteLine($"Comparison result: {comparisonResult}");
                Console.WriteLine($"Strings compared: '{string1}' and '{string2}' (Ignore case: {ignoreCase})");

                // Visa effekten genom att sortera data
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Orange");
                worksheet.Cells["A2"].PutValue("apple");
                worksheet.Cells["A3"].PutValue("Banana");
                worksheet.Cells["A4"].PutValue("Apple");

                // Skapa en DataSorter och ange intervallet för sortering
                DataSorter sorter = workbook.DataSorter;
                sorter.AddKey(0, SortOrder.Ascending);

                sorter.Sort(worksheet.Cells, 0, 0, 3, 0);
                workbook.Save("StringComparisonDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during string comparison: {ex.Message}");
            }
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override int Compare(string v1, string v2, bool ignoreCase)
            {
                return String.Compare(v1, v2, ignoreCase);
            }
        }
    }
}
```

### Se även

* class [AbstractGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


