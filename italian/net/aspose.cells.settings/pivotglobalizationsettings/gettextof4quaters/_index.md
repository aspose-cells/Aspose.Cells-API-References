---
title: "PivotGlobalizationSettings.GetTextOf4Quaters"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotGlobalizationSettings. Restituisce il testo locale di 4 Trimestri"
type: docs
url: /it/net/aspose.cells.settings/pivotglobalizationsettings/gettextof4quaters/
---
## PivotGlobalizationSettings.GetTextOf4Quaters method

Ottiene il testo locale di 4 trimestri.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOf4Quarters() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual string[] GetTextOf4Quaters()
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo PivotGlobalizationSettings.GetTextOf4Quarters(). Questa proprietà sarà rimossa tra 12 mesi a partire da luglio 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Settings;
    using System;

    public class PivotGlobalizationSettingsMethodGetTextOf4QuatersDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una classe di impostazioni di globalizzazione personalizzata che eredita da PivotGlobalizationSettings
            var customGlobalizationSettings = new CustomPivotGlobalizationSettings();

            try
            {
                // Chiama il metodo GetTextOf4Quaters
                string[] quarterNames = customGlobalizationSettings.GetTextOf4Quaters();

                // Stampa i nomi dei trimestri sulla console
                Console.WriteLine("Names of 4 quarters:");
                foreach (string quarterName in quarterNames)
                {
                    Console.WriteLine(quarterName);
                }

                // Aggiungi i nomi dei trimestri al foglio di lavoro
                for (int i = 0; i < quarterNames.Length; i++)
                {
                    worksheet.Cells[i, 0].PutValue(quarterNames[i]);
                }

                Console.WriteLine("Method executed successfully. Quarter names added to worksheet.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTextOf4Quaters method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("MethodGetTextOf4QuatersDemo.xlsx");
        }
    }

    // Implementazione personalizzata di PivotGlobalizationSettings per sovrascrivere GetTextOf4Quaters
    public class CustomPivotGlobalizationSettings : PivotGlobalizationSettings
    {
        public override string[] GetTextOf4Quaters()
        {
            // Restituisce nomi di trimestre personalizzati
            return new string[] { "First Quarter", "Second Quarter", 
                               "Third Quarter", "Fourth Quarter" };
        }
    }
}
```

### Vedi anche

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


