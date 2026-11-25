---
title: "GlobalizationSettings.Compare"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GlobalizationSettings. Confronta due valori stringa secondo determinate regole di collazione"
type: docs
url: /it/net/aspose.cells/globalizationsettings/compare/
---
## GlobalizationSettings.Compare method

Confronta due valori stringa secondo determinate regole di ordinamento.

```csharp
public virtual int Compare(string v1, string v2, bool ignoreCase)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| v1 | String | la prima stringa |
| v2 | String | la seconda stringa |
| ignoreCase | Booleano | se ignorare maiuscole/minuscole durante il confronto dei valori |

### Valore di ritorno

Intero che indica la relazione lessicale tra i due comparandi

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodCompareWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con impostazioni di globalizzazione personalizzate
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomComparisonSettings();

            try
            {
                // Dimostra l'uso diretto del metodo Compare
                GlobalizationSettings settings = workbook.Settings.GlobalizationSettings;
                int result1 = settings.Compare("Apple", "apple", true);
                int result2 = settings.Compare("Apple", "apple", false);
                
                Console.WriteLine($"Case-insensitive comparison result: {result1}");
                Console.WriteLine($"Case-sensitive comparison result: {result2}");

                // Dimostra l'effetto sulle operazioni del foglio di calcolo
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Banana");
                worksheet.Cells["A2"].PutValue("apple");
                worksheet.Cells["A3"].PutValue("Cherry");

                // Ordina i dati usando un confronto personalizzato
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
            // Implementa la logica di confronto personalizzata
            var comparison = ignoreCase ? 
                StringComparison.OrdinalIgnoreCase : 
                StringComparison.Ordinal;
            
            return string.Compare(v1?.Trim() ?? "", v2?.Trim() ?? "", comparison);
        }
    }
}
```

### Vedi anche

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


