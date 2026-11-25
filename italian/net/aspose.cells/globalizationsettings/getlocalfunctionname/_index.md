---
title: "GlobalizationSettings.GetLocalFunctionName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "GlobalizationSettings method. Ottiene il nome della funzione dipendente dalla locale in base al nome della funzione standard fornito"
type: docs
url: /it/net/aspose.cells/globalizationsettings/getlocalfunctionname/
---
## GlobalizationSettings.GetLocalFunctionName method

Ottiene il nome della funzione dipendente dalla locale in base al nome della funzione standard fornito.

```csharp
public virtual string GetLocalFunctionName(string standardName)
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

    public class GlobalizationSettingsMethodGetLocalFunctionNameWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta impostazioni di globalizzazione personalizzate
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            // Aggiungi dati di esempio
            worksheet.Cells["B1"].PutValue(5);
            worksheet.Cells["B2"].PutValue(15);

            // Crea una formula con il nome della funzione localizzato
            Cell cell = worksheet.Cells["B3"];
            cell.Formula = "=LOCALSUM(B1:B2)";

            try
            {
                workbook.CalculateFormula();
                Console.WriteLine($"Calculation result using localized function: {cell.DoubleValue}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Calculation error: {ex.Message}");
            }

            workbook.Save("GlobalizationSettingsFunctionDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override string GetLocalFunctionName(string standardName)
            {
                if (standardName == "SUM")
                {
                    return "LOCALSUM";
                }
                return base.GetLocalFunctionName(standardName);
            }
        }
    }
}
```

### Vedi anche

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


