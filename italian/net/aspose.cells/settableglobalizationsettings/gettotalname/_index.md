---
title: "SettableGlobalizationSettings.GetTotalName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettableGlobalizationSettings. Ottiene il nome totale della funzione specifica"
type: docs
url: /it/net/aspose.cells/settableglobalizationsettings/gettotalname/
---
## SettableGlobalizationSettings.GetTotalName method

Ottiene il nome totale della funzione specifica.

```csharp
public override string GetTotalName(ConsolidationFunction functionType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| functionType | ConsolidationFunction | Il tipo di funzione. |

### Valore di ritorno

Il nome totale della funzione.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetTotalNameWithConsolidationFunctionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un'istanza di SettableGlobalizationSettings
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

            try
            {
                // Chiama GetTotalName con ConsolidationFunction.Sum
                string totalName = globalizationSettings.GetTotalName(ConsolidationFunction.Sum);
                
                // Visualizza il risultato
                Console.WriteLine($"Total name for Sum function: {totalName}");

                // Aggiungi dati per dimostrare l'effetto (anche se GetTotalName non modifica il foglio di calcolo)
                worksheet.Cells["A1"].PutValue("Values");
                worksheet.Cells["A2"].PutValue(10);
                worksheet.Cells["A3"].PutValue(20);
                worksheet.Cells["A4"].PutValue(30);
                worksheet.Cells["B1"].PutValue("Total");
                worksheet.Cells["B4"].Formula = "=SUM(A2:A4)";
                
                // Calcola le formule
                workbook.CalculateFormula();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTotalName method: {ex.Message}");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("SettableGlobalizationSettingsMethodGetTotalNameDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


