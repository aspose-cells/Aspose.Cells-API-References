---
title: "GlobalizationSettings.GetCollationKey"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GlobalizationSettings. Trasforma la stringa in un oggetto confrontabile secondo determinate regole di ordinamento"
type: docs
url: /it/net/aspose.cells/globalizationsettings/getcollationkey/
---
## GlobalizationSettings.GetCollationKey method

Trasforma la stringa in un oggetto confrontabile secondo determinate regole di ordinamento.

```csharp
public virtual IComparable GetCollationKey(string v, bool ignoreCase)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| v | String | Il valore stringa deve essere confrontato con altri. |
| ignoreCase | Booleano | se ignorare maiuscole/minuscole durante il confronto dei valori |

### Valore di ritorno

L'oggetto può essere usato per confrontare o ordinare valori stringa

### Esempi

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

### Vedi anche

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


