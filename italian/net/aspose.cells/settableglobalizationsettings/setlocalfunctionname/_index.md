---
title: "SettableGlobalizationSettings.SetLocalFunctionName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettableGlobalizationSettings. Imposta il nome della funzione dipendente dalla locale corrispondente al nome della funzione standard fornito"
type: docs
url: /it/net/aspose.cells/settableglobalizationsettings/setlocalfunctionname/
---
## SettableGlobalizationSettings.SetLocalFunctionName method

Imposta il nome della funzione dipendente dalla locale corrispondente al nome della funzione standard fornito.

```csharp
public void SetLocalFunctionName(string standardName, string localName, bool bidirectional)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| standardName | String | Nome della funzione Standard (locale en-US). |
| localName | String | Nome della funzione dipendente dalla locale |
| bidirectional | Boolean | Indica se mappare automaticamente il nome della funzione locale al nome della funzione standard. Se vero, il nome locale verrà mappato automaticamente al nome standard così l'utente non dovrà chiamare nuovamente [`SetStandardFunctionName`](../setstandardfunctionname/) per la stessa coppia di nomi standard e locale. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetLocalFunctionNameWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea impostazioni di globalizzazione
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Chiama SetLocalFunctionName per mappare il nome della funzione standard al nome locale
                settings.SetLocalFunctionName("SUM", "SOMMA", true); // Italian localization for SUM function
                settings.SetLocalFunctionName("AVERAGE", "MEDIA", true); // Italian localization for AVERAGE function

                // Applica le impostazioni alla cartella di lavoro
                workbook.Settings.GlobalizationSettings = settings;

                // Crea formule utilizzando sia i nomi standard che quelli localizzati
                worksheet.Cells["A1"].Formula = "=SUM(B1:B5)";
                worksheet.Cells["A2"].Formula = "=SOMMA(B1:B5)";
                worksheet.Cells["A3"].Formula = "=AVERAGE(B1:B5)";
                worksheet.Cells["A4"].Formula = "=MEDIA(B1:B5)";

                // Calcola le formule
                workbook.CalculateFormula();

                Console.WriteLine("SetLocalFunctionName executed successfully with parameters (String, String, Boolean)");
                Console.WriteLine("Standard and localized function names work equivalently in formulas.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetLocalFunctionName method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("MethodSetLocalFunctionNameWithStringStringBooleanDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


