---
title: "Klass AbstractGlobalizationSettings"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.AbstractGlobalizationSettings klass. Representerar globaliseringsinställningarna"
type: docs
url: /sv/net/aspose.cells/abstractglobalizationsettings/
---
## AbstractGlobalizationSettings class

Representerar globaliseringsinställningarna.

```csharp
public abstract class AbstractGlobalizationSettings
```

## Metoder

| Namn | Beskrivning |
| --- | --- |
| virtual [Compare](../../aspose.cells/abstractglobalizationsettings/compare/)(string, string, bool) | Jämför två strängvärden enligt vissa kollationsregler. |
| virtual [GetCollationKey](../../aspose.cells/abstractglobalizationsettings/getcollationkey/)(string, bool) | Omvandlar strängen till ett jämförbart objekt enligt vissa kollationsregler. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassAbstractGlobalizationSettingsDemo
    {
        public static void Run()
        {
            // Skapa en anpassad implementation av AbstractGlobalizationSettings
            var customSettings = new CustomGlobalizationSettings();

            try
            {
                // Demonstrera Compare‑metoden
                string str1 = "Hello";
                string str2 = "hello";
                bool ignoreCase = true;

                int comparisonResult = customSettings.Compare(str1, str2, ignoreCase);
                Console.WriteLine($"Comparison result ({str1} vs {str2}, ignoreCase={ignoreCase}): {comparisonResult}");

                // Demonstrera GetCollationKey‑metoden
                string testString = "Sample";
                IComparable collationKey = customSettings.GetCollationKey(testString, ignoreCase);
                Console.WriteLine($"Collation key for '{testString}' (ignoreCase={ignoreCase}): {collationKey}");

                // Tillämpa inställningarna på en arbetsbok
                Workbook workbook = new Workbook();
                workbook.Settings.GlobalizationSettings = customSettings;

                // Lägg till lite data för att demonstrera inställningarna i praktiken
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Apple");
                worksheet.Cells["A2"].PutValue("banana");
                worksheet.Cells["A3"].PutValue("Cherry");

                // Spara arbetsboken
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

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


