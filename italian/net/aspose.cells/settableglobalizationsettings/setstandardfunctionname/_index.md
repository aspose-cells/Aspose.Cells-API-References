---
title: "SettableGlobalizationSettings.SetStandardFunctionName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettableGlobalizationSettings. Imposta il nome della funzione dipendente dalla locale secondo il nome della funzione standard fornito"
type: docs
url: /it/net/aspose.cells/settableglobalizationsettings/setstandardfunctionname/
---
## SettableGlobalizationSettings.SetStandardFunctionName method

Imposta il nome della funzione dipendente dalla locale secondo il nome della funzione standard fornito.

```csharp
public void SetStandardFunctionName(string localName, string standardName, bool bidirectional)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| localName | String | Nome della funzione dipendente dalla locale |
| standardName | String | Nome della funzione Standard (locale en-US). |
| bidirectional | Boolean | Indica se mappare automaticamente il nome della funzione standard al nome della funzione locale. Se vero, il nome standard verrà mappato al nome locale automaticamente così l'utente non deve chiamare nuovamente [`SetLocalFunctionName`](../setlocalfunctionname/) per la stessa coppia di nomi standard e locale |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetStandardFunctionNameWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea impostazioni di globalizzazione personalizzate
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Chiama SetStandardFunctionName per mappare un nome di funzione locale al nome standard
                settings.SetStandardFunctionName("LOCAL_SUM", "SUM", true);

                // Applica le impostazioni alla cartella di lavoro
                workbook.Settings.GlobalizationSettings = settings;

                // Crea una formula usando il nome della funzione locale
                worksheet.Cells["A1"].Formula = "=LOCAL_SUM(B1:B3)";
                worksheet.Cells["B1"].Value = 10;
                worksheet.Cells["B2"].Value = 20;
                worksheet.Cells["B3"].Value = 30;

                // Calcola la formula
                workbook.CalculateFormula();

                Console.WriteLine("Formula with local function name 'LOCAL_SUM' calculated successfully.");
                Console.WriteLine($"Result: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetStandardFunctionName method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("SetStandardFunctionNameDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


