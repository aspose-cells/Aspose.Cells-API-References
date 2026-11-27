---
title: "AbstractGlobalizationSettings.GetCollationKey"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AbstractGlobalizationSettings-metoden. Omvandlar strängen till ett jämförbart objekt enligt vissa sorteringsregler"
type: docs
url: /sv/net/aspose.cells/abstractglobalizationsettings/getcollationkey/
---
## AbstractGlobalizationSettings.GetCollationKey method

Omvandlar strängen till ett jämförbart objekt enligt vissa kollationsregler.

```csharp
public virtual IComparable GetCollationKey(string v, bool ignoreCase)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| v | String | Strängvärdet måste jämföras med andra. |
| ignoreCase | Boolean | om skiftlägeskänslighet ska ignoreras vid jämförelse av värden |

### Returvärde

Object kan användas för att jämföra eller sortera strängvärden

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractGlobalizationSettingsMethodGetCollationKeyWithStringBooleanDemo
    {
        public static void Run()
        {
            // Skapa anpassade globaliseringsinställningar som åsidosätter GetCollationKey-metoden
            var settings = new CustomGlobalizationSettings();
            
            // Skapa en arbetsbok med anpassade globaliseringsinställningar
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = settings;

            // Förbered strängen för sorteringsnyckel
            string inputString = "Sample Text";
            bool ignoreCase = true;

            try
            {
                // Anropa GetCollationKey direkt
                IComparable collationKey = settings.GetCollationKey(inputString, ignoreCase);
                
                Console.WriteLine($"Original string: {inputString}");
                Console.WriteLine($"Collation key: {collationKey}");
                Console.WriteLine($"Ignore case: {ignoreCase}");

                // Visa effekten genom att använda den i kalkylbladsoperationer
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Apple");
                worksheet.Cells["A2"].PutValue("banana");
                worksheet.Cells["A3"].PutValue("Cherry");

                // Sortering kommer att använda GetCollationKey internt
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

### Se även

* class [AbstractGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


