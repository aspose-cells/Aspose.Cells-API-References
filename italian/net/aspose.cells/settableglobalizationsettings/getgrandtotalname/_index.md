---
title: "SettableGlobalizationSettings.GetGrandTotalName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettableGlobalizationSettings. Ottiene il nome del totale generale della funzione"
type: docs
url: /it/net/aspose.cells/settableglobalizationsettings/getgrandtotalname/
---
## SettableGlobalizationSettings.GetGrandTotalName method

Ottiene il nome del totale generale della funzione.

```csharp
public override string GetGrandTotalName(ConsolidationFunction functionType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| functionType | ConsolidationFunction | Il tipo di funzione. |

### Valore di ritorno

Il nome del totale generale della funzione.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot; // Added this using directive
    using System;

    public class SettableGlobalizationSettingsMethodGetGrandTotalNameWithConsolidationFunctionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea impostazioni di globalizzazione personalizzate
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Imposta nomi personalizzati del totale generale per diverse funzioni di consolidamento
            settings.SetGrandTotalName(ConsolidationFunction.Sum, "Custom Sum Grand Total");
            settings.SetGrandTotalName(ConsolidationFunction.Average, "Custom Average Grand Total");
            
            // Applica le impostazioni alla cartella di lavoro
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Chiama GetGrandTotalName con diverse funzioni di consolidamento
                string sumGrandTotalName = settings.GetGrandTotalName(ConsolidationFunction.Sum);
                string avgGrandTotalName = settings.GetGrandTotalName(ConsolidationFunction.Average);
                
                // Restituisci i risultati
                Console.WriteLine("Sum Grand Total Name: " + sumGrandTotalName);
                Console.WriteLine("Average Grand Total Name: " + avgGrandTotalName);

                // Crea una tabella pivot per dimostrare l'effetto
                Cells cells = worksheet.Cells;
                cells["A1"].PutValue("Product");
                cells["B1"].PutValue("Sales");
                cells["A2"].PutValue("Apple");
                cells["B2"].PutValue(1000);
                cells["A3"].PutValue("Orange");
                cells["B3"].PutValue(2000);
                cells["A4"].PutValue("Banana");
                cells["B4"].PutValue(3000);

                PivotTableCollection pivotTables = worksheet.PivotTables;
                int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
                PivotTable pivotTable = pivotTables[index];
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
                pivotTable.DataFields[0].Function = ConsolidationFunction.Sum;
                
                // Modo corretto per aggiungere un altro campo dati con la funzione Media
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
                pivotTable.DataFields[1].Function = ConsolidationFunction.Average;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetGrandTotalName method: {ex.Message}");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("SettableGlobalizationSettingsMethodGetGrandTotalNameDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


