---
title: "AbstractGlobalizationSettings.GetCollationKey"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AbstractGlobalizationSettings‑Methode. Wandelt die Zeichenkette gemäß bestimmter Sortierregeln in ein vergleichbares Objekt um"
type: docs
url: /de/net/aspose.cells/abstractglobalizationsettings/getcollationkey/
---
## AbstractGlobalizationSettings.GetCollationKey method

Wandelt die Zeichenkette in ein vergleichbares Objekt gemäß bestimmter Sortierregeln um.

```csharp
public virtual IComparable GetCollationKey(string v, bool ignoreCase)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| v | String | Der Zeichenkettenwert muss mit anderen verglichen werden. |
| ignoreCase | Boolean | ob bei Vergleichen von Werten die Groß-/Kleinschreibung ignoriert werden soll |

### Rückgabewert

Objekt kann verwendet werden, um Zeichenkettenwerte zu vergleichen oder zu sortieren

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractGlobalizationSettingsMethodGetCollationKeyWithStringBooleanDemo
    {
        public static void Run()
        {
            // Erstelle benutzerdefinierte Globalisierungs‑Einstellungen, die die GetCollationKey‑Methode überschreiben
            var settings = new CustomGlobalizationSettings();
            
            // Arbeitsmappe mit benutzerdefinierten Globalisierungseinstellungen erstellen
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = settings;

            // Bereite die Zeichenkette für den Sortierschlüssel vor
            string inputString = "Sample Text";
            bool ignoreCase = true;

            try
            {
                // Rufen Sie GetCollationKey direkt auf
                IComparable collationKey = settings.GetCollationKey(inputString, ignoreCase);
                
                Console.WriteLine($"Original string: {inputString}");
                Console.WriteLine($"Collation key: {collationKey}");
                Console.WriteLine($"Ignore case: {ignoreCase}");

                // Demonstrieren Sie die Wirkung durch die Verwendung in Arbeitsblatt‑Operationen
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Apple");
                worksheet.Cells["A2"].PutValue("banana");
                worksheet.Cells["A3"].PutValue("Cherry");

                // Beim Sortieren wird GetCollationKey intern verwendet
                DataSorter sorter = workbook.DataSorter;
                sorter.AddKey(0, SortOrder.Descending);

                sorter.Sort(worksheet.Cells, 0, 0, 2, 0);
                
                workbook.Save("GetCollationKeyDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during GetCollationKey operation: {ex.Message}");
            }
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override IComparable GetCollationKey(string v, bool ignoreCase)
            {
                return ignoreCase ? v.ToLowerInvariant() : v;
            }
        }

    }
}
```

### Siehe auch

* class [AbstractGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


