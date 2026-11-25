---
title: "SettableGlobalizationSettings.GetLocalFunctionName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettableGlobalizationSettings. Ottiene il nome della funzione dipendente dalla locale in base al nome della funzione standard fornito"
type: docs
url: /it/net/aspose.cells/settableglobalizationsettings/getlocalfunctionname/
---
## SettableGlobalizationSettings.GetLocalFunctionName method

Ottiene il nome della funzione dipendente dalla locale in base al nome della funzione standard fornito.

```csharp
public override string GetLocalFunctionName(string standardName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| standardName | String | Nome della funzione Standard (locale en-US). |

### Valore di ritorno

Nome della funzione dipendente dalla locale. La locale è stata specificata dalla Cartella di lavoro per la quale queste impostazioni sono utilizzate.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetLocalFunctionNameWithStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea impostazioni di globalizzazione personalizzate
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Imposta un nome di funzione locale personalizzato per "SUM"
            settings.SetLocalFunctionName("SUM", "SOMME", true);

            // Applica le impostazioni alla cartella di lavoro
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Chiama GetLocalFunctionName per recuperare il nome localizzato
                string localName = settings.GetLocalFunctionName("SUM");
                
                // Visualizza il risultato
                Console.WriteLine($"Localized function name for 'SUM': {localName}");

                // Usa la funzione localizzata in una cella
                worksheet.Cells["A1"].Formula = "=SOMME(B1:B5)";
                worksheet.Cells["B1"].PutValue(1);
                worksheet.Cells["B2"].PutValue(2);
                worksheet.Cells["B3"].PutValue(3);
                worksheet.Cells["B4"].PutValue(4);
                worksheet.Cells["B5"].PutValue(5);

                // Calcola le formule
                workbook.CalculateFormula();

                // Visualizza il risultato
                Console.WriteLine($"Calculation result with localized function: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetLocalFunctionName method: {ex.Message}");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("MethodGetLocalFunctionNameWithStringDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


