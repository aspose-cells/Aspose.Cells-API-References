---
title: "SettableGlobalizationSettings.GetStandardFunctionName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettableGlobalizationSettings. Ottiene il nome della funzione standard in base al nome della funzione dipendente dalla locale fornito"
type: docs
url: /it/net/aspose.cells/settableglobalizationsettings/getstandardfunctionname/
---
## SettableGlobalizationSettings.GetStandardFunctionName method

Ottiene il nome standard della funzione in base al nome della funzione dipendente dalla locale fornito.

```csharp
public override string GetStandardFunctionName(string localName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| localName | String | Nome della funzione dipendente dalla locale. La locale è stata specificata dalla Cartella di lavoro per la quale queste impostazioni sono utilizzate. |

### Valore di ritorno

Nome della funzione Standard (locale en-US).

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetStandardFunctionNameWithStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea impostazioni di globalizzazione personalizzate
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Imposta una mappatura del nome della funzione locale
            settings.SetStandardFunctionName("LocalSum", "SUM", true);

            // Applica le impostazioni alla cartella di lavoro
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Chiama GetStandardFunctionName con un nome di funzione locale
                string standardName = settings.GetStandardFunctionName("LocalSum");
                
                // Visualizza il risultato
                Console.WriteLine($"Standard function name for 'LocalSum' is: {standardName}");

                // Usa la funzione standard in una formula di cella
                worksheet.Cells["A1"].Formula = $"={standardName}(1,2,3)";
                worksheet.Cells["A2"].Value = 1;
                worksheet.Cells["A3"].Value = 2;
                worksheet.Cells["A4"].Value = 3;

                // Calcola la formula
                workbook.CalculateFormula();

                // Visualizza il risultato
                Console.WriteLine($"Formula result in A1: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardFunctionName method: {ex.Message}");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("SettableGlobalizationSettingsMethodGetStandardFunctionNameWithStringDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


