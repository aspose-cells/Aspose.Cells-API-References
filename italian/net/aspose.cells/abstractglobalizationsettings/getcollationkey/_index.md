---
title: "AbstractGlobalizationSettings.GetCollationKey"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo AbstractGlobalizationSettings. Trasforma la stringa in un oggetto confrontabile secondo determinate regole di ordinamento"
type: docs
url: /it/net/aspose.cells/abstractglobalizationsettings/getcollationkey/
---
## AbstractGlobalizationSettings.GetCollationKey method

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

    public class AbstractGlobalizationSettingsMethodGetCollationKeyWithStringBooleanDemo
    {
        public static void Run()
        {
            // Crea impostazioni di globalizzazione personalizzate che sovrascrivono il metodo GetCollationKey
            var settings = new CustomGlobalizationSettings();
            
            // Crea una cartella di lavoro con impostazioni di globalizzazione personalizzate
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = settings;

            // Prepara la stringa per la chiave di ordinamento
            string inputString = "Sample Text";
            bool ignoreCase = true;

            try
            {
                // Chiama GetCollationKey direttamente
                IComparable collationKey = settings.GetCollationKey(inputString, ignoreCase);
                
                Console.WriteLine($"Original string: {inputString}");
                Console.WriteLine($"Collation key: {collationKey}");
                Console.WriteLine($"Ignore case: {ignoreCase}");

                // Dimostra l'effetto utilizzandolo nelle operazioni del foglio di lavoro
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Apple");
                worksheet.Cells["A2"].PutValue("banana");
                worksheet.Cells["A3"].PutValue("Cherry");

                // L'ordinamento utilizzerà internamente GetCollationKey
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

### Vedi anche

* class [AbstractGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


