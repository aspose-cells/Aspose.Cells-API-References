---
title: "GlobalizationSettings.GetStandardBuiltInName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GlobalizationSettings. Ottiene il testo standard del nome incorporato in base al testo dipendente dalla locale fornita"
type: docs
url: /it/net/aspose.cells/globalizationsettings/getstandardbuiltinname/
---
## GlobalizationSettings.GetStandardBuiltInName method

Ottiene il testo standard del Nome incorporato in base al testo dipendente dalla locale fornito.

```csharp
public virtual string GetStandardBuiltInName(string localName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| localName | String | Testo dipendente dalla locale del Nome incorporato. La locale è stata specificata dalla Cartella di lavoro per la quale queste impostazioni sono utilizzate. |

### Valore di ritorno

Testo standard (locale en-US).

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetStandardBuiltInNameWithStringDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con impostazioni di globalizzazione personalizzate
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Inizializza le impostazioni di globalizzazione personalizzate e assegnale alla cartella di lavoro
            var globalizationSettings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = globalizationSettings;

            // Parametro di test per GetStandardBuiltInName
            string localFunctionName = "MyLocalSum";
            
            try
            {
                // Chiama GetStandardBuiltInName con il nome della funzione locale
                string standardName = globalizationSettings.GetStandardBuiltInName(localFunctionName);
                Console.WriteLine($"Local name: '{localFunctionName}' => Standard name: '{standardName}'");

                // Dimostra l'effetto utilizzando il nome locale in una formula
                worksheet.Cells["A1"].Value = 5;
                worksheet.Cells["A2"].Value = 7;
                worksheet.Cells["A3"].Formula = $"{localFunctionName}(A1:A2)";

                // Calcola la formula per mostrare l'interpretazione corretta
                workbook.CalculateFormula();
                Console.WriteLine($"Formula result: {worksheet.Cells["A3"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardBuiltInName: {ex.Message}");
            }

            // Salva la cartella di lavoro modificata
            workbook.Save("GlobalizationGetStandardBuiltInNameDemo.xlsx");
        }
    }

    // Impostazioni di globalizzazione personalizzate che sovrascrivono GetStandardBuiltInName
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetStandardBuiltInName(string localName)
        {
            // Mappa il nome della funzione locale personalizzata alla SUM standard
            if (localName.Equals("MyLocalSum", StringComparison.OrdinalIgnoreCase))
            {
                return "SUM";
            }
            return base.GetStandardBuiltInName(localName);
        }
    }
}
```

### Vedi anche

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


