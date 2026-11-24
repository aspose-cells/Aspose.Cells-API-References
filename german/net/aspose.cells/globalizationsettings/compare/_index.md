---
title: "GlobalizationSettings.Compare"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GlobalizationSettings-Methode. Vergleicht zwei Zeichenfolgenwerte nach bestimmten Sortierregeln"
type: docs
url: /de/net/aspose.cells/globalizationsettings/compare/
---
## GlobalizationSettings.Compare method

Vergleicht zwei Zeichenkettenwerte nach bestimmten Sortierregeln.

```csharp
public virtual int Compare(string v1, string v2, bool ignoreCase)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| v1 | String | die erste Zeichenfolge |
| v2 | String | die zweite Zeichenfolge |
| ignoreCase | Boolean | ob bei Vergleichen von Werten die Groß-/Kleinschreibung ignoriert werden soll |

### Rückgabewert

Ganzzahl, die die lexikalische Beziehung zwischen den beiden Vergleichswerten angibt

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodCompareWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Arbeitsmappe mit benutzerdefinierten Globalisierungseinstellungen erstellen
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomComparisonSettings();

            try
            {
                // Direkte Verwendung der Compare-Methode demonstrieren
                GlobalizationSettings settings = workbook.Settings.GlobalizationSettings;
                int result1 = settings.Compare("Apple", "apple", true);
                int result2 = settings.Compare("Apple", "apple", false);
                
                Console.WriteLine($"Case-insensitive comparison result: {result1}");
                Console.WriteLine($"Case-sensitive comparison result: {result2}");

                // Auswirkung auf Tabellenkalkulationsvorgänge demonstrieren
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Banana");
                worksheet.Cells["A2"].PutValue("apple");
                worksheet.Cells["A3"].PutValue("Cherry");

                // Daten mit benutzerdefiniertem Vergleich sortieren
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
            // Benutzerdefinierte Vergleichslogik implementieren
            var comparison = ignoreCase ? 
                StringComparison.OrdinalIgnoreCase : 
                StringComparison.Ordinal;
            
            return string.Compare(v1?.Trim() ?? "", v2?.Trim() ?? "", comparison);
        }
    }
}
```

### Siehe auch

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


