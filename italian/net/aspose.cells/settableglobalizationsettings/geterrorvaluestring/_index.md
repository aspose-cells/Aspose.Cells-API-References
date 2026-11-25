---
title: "SettableGlobalizationSettings.GetErrorValueString"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettableGlobalizationSettings. Ottiene il valore stringa visualizzato per il valore di errore delle celle"
type: docs
url: /it/net/aspose.cells/settableglobalizationsettings/geterrorvaluestring/
---
## SettableGlobalizationSettings.GetErrorValueString method

Ottiene il valore stringa visualizzato per il valore di errore della cella

```csharp
public override string GetErrorValueString(string err)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| err | String | valori di errore come #VALUE!,#NAME? |

### Valore di ritorno

Per impostazione predefinita restituisce il valore di errore stesso

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetErrorValueStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea impostazioni di globalizzazione personalizzate
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = settings;

            // Crea una cella con valore di errore
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("#N/A");
            Style style = workbook.CreateStyle();
            cell.SetStyle(style);
            style.Number = 10; // Set format to Error value

            try
            {
                // Chiama GetErrorValueString con la stringa del valore di errore
                string errorString = settings.GetErrorValueString("#N/A");
                
                // Visualizza il risultato
                Console.WriteLine("Error value string: " + errorString);

                // Mostra l'effetto impostando il valore di un'altra cella sulla stringa restituita
                worksheet.Cells["A2"].PutValue("Error representation: " + errorString);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetErrorValueString method: {ex.Message}");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("MethodGetErrorValueStringDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


