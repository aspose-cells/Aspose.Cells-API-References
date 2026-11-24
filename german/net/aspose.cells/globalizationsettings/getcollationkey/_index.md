---
title: "GlobalizationSettings.GetCollationKey"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GlobalizationSettings-Methode. Wandelt die Zeichenkette gemäß bestimmter Sortierregeln in ein vergleichbares Objekt um."
type: docs
url: /de/net/aspose.cells/globalizationsettings/getcollationkey/
---
## GlobalizationSettings.GetCollationKey method

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

### Siehe auch

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


