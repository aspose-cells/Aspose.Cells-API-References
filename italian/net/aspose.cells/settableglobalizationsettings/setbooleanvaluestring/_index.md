---
title: "SettableGlobalizationSettings.SetBooleanValueString"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettableGlobalizationSettings. Imposta il valore stringa visualizzato per il valore booleano delle celle"
type: docs
url: /it/net/aspose.cells/settableglobalizationsettings/setbooleanvaluestring/
---
## SettableGlobalizationSettings.SetBooleanValueString method

Imposta il valore stringa di visualizzazione per il valore booleano della cella

```csharp
public void SetBooleanValueString(bool bv, string name)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| bv | Booleano | valore booleano |
| name | String | valore stringa del valore booleano |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetBooleanValueStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea impostazioni di globalizzazione personalizzate
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Imposta le stringhe personalizzate per i valori booleani
            settings.SetBooleanValueString(true, "Yes");
            settings.SetBooleanValueString(false, "No");
            
            // Applica le impostazioni alla cartella di lavoro
            workbook.Settings.GlobalizationSettings = settings;
            
            // Imposta valori booleani nelle celle
            worksheet.Cells["A1"].PutValue(true);
            worksheet.Cells["A2"].PutValue(false);
            
            // Imposta lo stile di visualizzazione per mostrare i valori booleani come testo
            Style style = workbook.CreateStyle();
            style.Custom = "BOOLEAN";
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["A2"].SetStyle(style);
            
            try
            {
                // Salva la cartella di lavoro
                workbook.Save("SetBooleanValueStringDemo.xlsx");
                Console.WriteLine("Workbook saved with custom boolean value strings.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving workbook: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


