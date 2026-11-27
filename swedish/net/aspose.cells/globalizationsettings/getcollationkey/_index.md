---
title: "GlobalizationSettings.GetCollationKey"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GlobalizationSettings-metod. Omvandlar strängen till ett jämförbart objekt enligt vissa sorteringsregler"
type: docs
url: /sv/net/aspose.cells/globalizationsettings/getcollationkey/
---
## GlobalizationSettings.GetCollationKey method

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

    public class GlobalizationSettingsMethodGetCollationKeyWithStringBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            CustomGlobalizationSettings settings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = settings;

            string inputString = "SampleText";
            bool ignoreCase = true;

            try
            {
                IComparable collationKey = settings.GetCollationKey(inputString, ignoreCase);
                Console.WriteLine($"Collation key for '{inputString}' (ignore case {ignoreCase}): {collationKey}");

                worksheet.Cells["A1"].Value = "Cherry";
                worksheet.Cells["A2"].Value = "apple";
                worksheet.Cells["A3"].Value = "Banana";

                DataSorter sorter = workbook.DataSorter;
                sorter.CaseSensitive = !ignoreCase;
                sorter.Sort(worksheet.Cells, 0, 0, 2, 0);

                Console.WriteLine("\nSorted data:");
                int minDataRow = worksheet.Cells.MinDataRow;
                int maxDataRow = worksheet.Cells.MaxDataRow;
                for (int row = minDataRow; row <= maxDataRow; row++)
                {
                    Cell cell = worksheet.Cells[row, 0];
                    Console.WriteLine(cell.StringValue);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCollationKey: {ex.Message}");
            }

            workbook.Save("GlobalizationSettingsMethodGetCollationKeyDemo.xlsx");
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override IComparable GetCollationKey(string v, bool ignoreCase)
        {
            return ignoreCase ? v.ToLowerInvariant() : v;
        }
    }
}
```

### Se även

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


