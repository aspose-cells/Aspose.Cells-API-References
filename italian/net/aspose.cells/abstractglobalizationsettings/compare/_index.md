---
title: "AbstractGlobalizationSettings.Compare"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo AbstractGlobalizationSettings. Confronta due valori di stringa secondo determinate regole di ordinamento"
type: docs
url: /it/net/aspose.cells/abstractglobalizationsettings/compare/
---
## AbstractGlobalizationSettings.Compare method

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

    public class AbstractGlobalizationSettingsMethodCompareWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Crea impostazioni di globalizzazione personalizzate che sovrascrivono il metodo Compare
            var settings = new CustomGlobalizationSettings();
            
            // Crea una cartella di lavoro con impostazioni di globalizzazione personalizzate
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = settings;

            // Prepara le stringhe da confrontare
            string string1 = "Apple";
            string string2 = "apple";
            bool ignoreCase = true;

            try
            {
                // Il metodo Compare verrà chiamato internamente durante operazioni come l'ordinamento
                // Qui dimostriamo l'uso diretto
                int comparisonResult = settings.Compare(string1, string2, ignoreCase);
                
                Console.WriteLine($"Comparison result: {comparisonResult}");
                Console.WriteLine($"Strings compared: '{string1}' and '{string2}' (Ignore case: {ignoreCase})");

                // Dimostra l'effetto ordinando i dati
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Orange");
                worksheet.Cells["A2"].PutValue("apple");
                worksheet.Cells["A3"].PutValue("Banana");
                worksheet.Cells["A4"].PutValue("Apple");

                // Crea un DataSorter e imposta l'intervallo per l'ordinamento
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

### Vedi anche

* class [AbstractGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


