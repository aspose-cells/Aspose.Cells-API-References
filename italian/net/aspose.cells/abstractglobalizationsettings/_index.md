---
title: "Class AbstractGlobalizationSettings"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.AbstractGlobalizationSettings. Rappresenta le impostazioni di globalizzazione"
type: docs
url: /it/net/aspose.cells/abstractglobalizationsettings/
---
## AbstractGlobalizationSettings class

Rappresenta le impostazioni di globalizzazione.

```csharp
public abstract class AbstractGlobalizationSettings
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| virtual [Compare](../../aspose.cells/abstractglobalizationsettings/compare/)(string, string, bool) | Confronta due valori stringa secondo determinate regole di ordinamento. |
| virtual [GetCollationKey](../../aspose.cells/abstractglobalizationsettings/getcollationkey/)(string, bool) | Trasforma la stringa in un oggetto confrontabile secondo determinate regole di ordinamento. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassAbstractGlobalizationSettingsDemo
    {
        public static void Run()
        {
            // Crea un'implementazione personalizzata di AbstractGlobalizationSettings
            var customSettings = new CustomGlobalizationSettings();

            try
            {
                // Dimostra il metodo Compare
                string str1 = "Hello";
                string str2 = "hello";
                bool ignoreCase = true;

                int comparisonResult = customSettings.Compare(str1, str2, ignoreCase);
                Console.WriteLine($"Comparison result ({str1} vs {str2}, ignoreCase={ignoreCase}): {comparisonResult}");

                // Dimostra il metodo GetCollationKey
                string testString = "Sample";
                IComparable collationKey = customSettings.GetCollationKey(testString, ignoreCase);
                Console.WriteLine($"Collation key for '{testString}' (ignoreCase={ignoreCase}): {collationKey}");

                // Applica le impostazioni a una cartella di lavoro
                Workbook workbook = new Workbook();
                workbook.Settings.GlobalizationSettings = customSettings;

                // Aggiungi alcuni dati per dimostrare le impostazioni in azione
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Apple");
                worksheet.Cells["A2"].PutValue("banana");
                worksheet.Cells["A3"].PutValue("Cherry");

                // Salva la cartella di lavoro
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

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


