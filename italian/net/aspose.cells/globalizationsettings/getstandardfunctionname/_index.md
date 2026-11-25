---
title: "GlobalizationSettings.GetStandardFunctionName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GlobalizationSettings. Ottiene il nome della funzione standard in base al nome della funzione dipendente dalla locale fornito"
type: docs
url: /it/net/aspose.cells/globalizationsettings/getstandardfunctionname/
---
## GlobalizationSettings.GetStandardFunctionName method

Ottiene il nome standard della funzione in base al nome della funzione dipendente dalla locale fornito.

```csharp
public virtual string GetStandardFunctionName(string localName)
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

    public class GlobalizationSettingsMethodGetStandardFunctionNameWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Prepara dati di esempio
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["A2"].PutValue(15);
            
            // Crea impostazioni di globalizzazione personalizzate e assegnale alla cartella di lavoro
            var customSettings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = customSettings;

            try
            {
                // Dimostra GetStandardFunctionName con il nome della funzione SUM in tedesco
                string localName = "SUMME";
                string standardName = customSettings.GetStandardFunctionName(localName);
                
                Console.WriteLine($"Local function name: {localName}");
                Console.WriteLine($"Standard function name: {standardName}");

                // Applica il nome della funzione localizzato nella formula
                worksheet.Cells["A3"].Formula = "=SUMME(A1:A2)";
                workbook.CalculateFormula();
                
                Console.WriteLine($"Formula result: {worksheet.Cells["A3"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardFunctionName method: {ex.Message}");
            }

            workbook.Save("MethodGetStandardFunctionNameDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override string GetStandardFunctionName(string localName)
            {
                // Converti il nome della funzione tedesca in inglese standard
                if (localName.Equals("SUMME", StringComparison.OrdinalIgnoreCase))
                {
                    return "SUM";
                }
                return base.GetStandardFunctionName(localName);
            }
        }
    }
}
```

### Vedi anche

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


