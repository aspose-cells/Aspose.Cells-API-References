---
title: "GlobalizationSettings.GetBooleanValueString"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "GlobalizationSettings method. Ottiene il valore stringa da visualizzare per il valore booleano delle celle"
type: docs
url: /it/net/aspose.cells/globalizationsettings/getbooleanvaluestring/
---
## GlobalizationSettings.GetBooleanValueString method

Ottiene il valore stringa visualizzato per il valore booleano della cella

```csharp
public virtual string GetBooleanValueString(bool bv)
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

    public class GlobalizationSettingsMethodGetBooleanValueStringWithBooleanDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro con impostazioni di globalizzazione personalizzate
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomBooleanGlobalizationSettings();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Dimostra GetBooleanValueString con entrambi i valori booleani
                var globalizationSettings = workbook.Settings.GlobalizationSettings;
                string trueResult = globalizationSettings.GetBooleanValueString(true);
                string falseResult = globalizationSettings.GetBooleanValueString(false);

                Console.WriteLine($"GetBooleanValueString(true) returns: {trueResult}");
                Console.WriteLine($"GetBooleanValueString(false) returns: {falseResult}");

                // Applica valori booleani alle celle per mostrare l'effetto del foglio di calcolo
                worksheet.Cells["A1"].PutValue(true);
                worksheet.Cells["A2"].PutValue(false);

                workbook.Save("GlobalizationBooleanDemo.xlsx");
                Console.WriteLine("Workbook saved with custom boolean representations.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetBooleanValueString: {ex.Message}");
            }
        }
    }

    // Impostazioni di globalizzazione personalizzate che sovrascrivono la rappresentazione stringa dei booleani
    public class CustomBooleanGlobalizationSettings : GlobalizationSettings
    {
        public override string GetBooleanValueString(bool bv)
        {
            return bv ? "Enabled" : "Disabled";
        }
    }
}
```

### Vedi anche

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


