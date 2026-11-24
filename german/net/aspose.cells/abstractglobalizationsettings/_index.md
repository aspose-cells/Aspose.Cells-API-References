---
title: "Klasse AbstractGlobalizationSettings"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.AbstractGlobalizationSettings Klasse. Stellt die Globalisierungseinstellungen dar"
type: docs
url: /de/net/aspose.cells/abstractglobalizationsettings/
---
## AbstractGlobalizationSettings class

Stellt die Globalisierungseinstellungen dar.

```csharp
public abstract class AbstractGlobalizationSettings
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| virtual [Compare](../../aspose.cells/abstractglobalizationsettings/compare/)(string, string, bool) | Vergleicht zwei Zeichenkettenwerte nach bestimmten Sortierregeln. |
| virtual [GetCollationKey](../../aspose.cells/abstractglobalizationsettings/getcollationkey/)(string, bool) | Wandelt die Zeichenkette in ein vergleichbares Objekt gemäß bestimmter Sortierregeln um. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassAbstractGlobalizationSettingsDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine benutzerdefinierte Implementierung von AbstractGlobalizationSettings
            var customSettings = new CustomGlobalizationSettings();

            try
            {
                // Demonstrieren Sie die Compare-Methode
                string str1 = "Hello";
                string str2 = "hello";
                bool ignoreCase = true;

                int comparisonResult = customSettings.Compare(str1, str2, ignoreCase);
                Console.WriteLine($"Comparison result ({str1} vs {str2}, ignoreCase={ignoreCase}): {comparisonResult}");

                // Demonstrieren Sie die GetCollationKey-Methode
                string testString = "Sample";
                IComparable collationKey = customSettings.GetCollationKey(testString, ignoreCase);
                Console.WriteLine($"Collation key for '{testString}' (ignoreCase={ignoreCase}): {collationKey}");

                // Wenden Sie die Einstellungen auf eine Arbeitsmappe an
                Workbook workbook = new Workbook();
                workbook.Settings.GlobalizationSettings = customSettings;

                // Fügen Sie einige Daten hinzu, um die Einstellungen in Aktion zu demonstrieren
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Apple");
                worksheet.Cells["A2"].PutValue("banana");
                worksheet.Cells["A3"].PutValue("Cherry");

                // Speichere die Arbeitsmappe
                workbook.Save("GlobalizationSettingsDemo.xlsx");
                Console.WriteLine("Workbook saved with custom globalization settings.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override int Compare(string v1, string v2, bool ignoreCase)
            {
                return string.Compare(v1, v2, ignoreCase ? StringComparison.OrdinalIgnoreCase : StringComparison.Ordinal);
            }

            public override IComparable GetCollationKey(string v, bool ignoreCase)
            {
                return ignoreCase ? v.ToLowerInvariant() : v;
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


