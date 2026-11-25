---
title: "SettableGlobalizationSettings.GetBooleanValueString"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettableGlobalizationSettings. Ottiene la stringa di visualizzazione per il valore booleano delle celle"
type: docs
url: /it/net/aspose.cells/settableglobalizationsettings/getbooleanvaluestring/
---
## SettableGlobalizationSettings.GetBooleanValueString method

Ottiene il valore stringa visualizzato per il valore booleano della cella

```csharp
public override string GetBooleanValueString(bool bv)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| bv | Booleano | valore booleano |

### Valore di ritorno

Per impostazione predefinita restituisce "TRUE" per il valore vero e "FALSE" per il valore falso.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetBooleanValueStringWithBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea impostazioni di globalizzazione personalizzate
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Imposta le stringhe personalizzate per i valori booleani
            settings.SetBooleanValueString(true, "TRUE_CUSTOM");
            settings.SetBooleanValueString(false, "FALSE_CUSTOM");

            // Applica le impostazioni alla cartella di lavoro
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Chiama GetBooleanValueString con true
                string trueValue = settings.GetBooleanValueString(true);
                Console.WriteLine("Custom true value: " + trueValue);

                // Chiama GetBooleanValueString con false
                string falseValue = settings.GetBooleanValueString(false);
                Console.WriteLine("Custom false value: " + falseValue);

                // Dimostra l'effetto nel foglio di lavoro
                worksheet.Cells["A1"].PutValue(true);
                worksheet.Cells["A2"].PutValue(false);

                Console.WriteLine("Cell A1 value: " + worksheet.Cells["A1"].StringValue);
                Console.WriteLine("Cell A2 value: " + worksheet.Cells["A2"].StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetBooleanValueString method: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("SettableGlobalizationSettingsMethodGetBooleanValueStringDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


