---
title: "AbstractGlobalizationSettings.Compare"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AbstractGlobalizationSettings‑Methode. Vergleicht zwei Zeichenkettenwerte gemäß bestimmter Kollationsregeln"
type: docs
url: /de/net/aspose.cells/abstractglobalizationsettings/compare/
---
## AbstractGlobalizationSettings.Compare method

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

    public class AbstractGlobalizationSettingsMethodCompareWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Erstellen Sie benutzerdefinierte Globalisierungseinstellungen, die die Compare‑Methode überschreiben
            var settings = new CustomGlobalizationSettings();
            
            // Arbeitsmappe mit benutzerdefinierten Globalisierungseinstellungen erstellen
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = settings;

            // Bereiten Sie die zu vergleichenden Zeichenketten vor
            string string1 = "Apple";
            string string2 = "apple";
            bool ignoreCase = true;

            try
            {
                // Die Compare‑Methode wird intern während Vorgängen wie dem Sortieren aufgerufen
                // Wir demonstrieren hier die direkte Verwendung
                int comparisonResult = settings.Compare(string1, string2, ignoreCase);
                
                Console.WriteLine($"Comparison result: {comparisonResult}");
                Console.WriteLine($"Strings compared: '{string1}' and '{string2}' (Ignore case: {ignoreCase})");

                // Demonstrieren Sie die Wirkung durch das Sortieren von Daten
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Orange");
                worksheet.Cells["A2"].PutValue("apple");
                worksheet.Cells["A3"].PutValue("Banana");
                worksheet.Cells["A4"].PutValue("Apple");

                // Erstellen Sie einen DataSorter und legen Sie den Bereich für das Sortieren fest
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

### Siehe auch

* class [AbstractGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


