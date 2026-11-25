---
title: "SettableGlobalizationSettings.SetTotalName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettableGlobalizationSettings. Imposta il nome totale della funzione specifica"
type: docs
url: /it/net/aspose.cells/settableglobalizationsettings/settotalname/
---
## SettableGlobalizationSettings.SetTotalName method

Imposta il nome totale della funzione specifica.

```csharp
public void SetTotalName(ConsolidationFunction functionType, string name)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| functionType | ConsolidationFunction | Il tipo di funzione. |
| name | String | Il nome totale della funzione. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettableGlobalizationSettingsMethodSetTotalNameWithConsolidationFunctionStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea dati di esempio per il consolidamento
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["A4"].PutValue("Total");

            // Crea impostazioni di globalizzazione personalizzate
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Imposta un nome totale personalizzato per la funzione Somma
                settings.SetTotalName(ConsolidationFunction.Sum, "Custom Sum Total");
                
                // Imposta nome totale personalizzato per la funzione Media
                settings.SetTotalName(ConsolidationFunction.Average, "Custom Average Total");

                // Applica le impostazioni alla cartella di lavoro
                workbook.Settings.GlobalizationSettings = settings;

                // Verifica le impostazioni ottenendo nuovamente i valori
                string sumTotalName = settings.GetTotalName(ConsolidationFunction.Sum);
                string avgTotalName = settings.GetTotalName(ConsolidationFunction.Average);

                Console.WriteLine($"Sum total name set to: {sumTotalName}");
                Console.WriteLine($"Average total name set to: {avgTotalName}");

                // Crea una tabella pivot per dimostrare l'effetto
                worksheet.Cells["D1"].PutValue("Pivot Table");
                var pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
                var pivotTable = worksheet.PivotTables[pivotIndex];
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
                pivotTable.DataFields[0].Function = ConsolidationFunction.Sum;
                pivotTable.DataFields[1].Function = ConsolidationFunction.Average;
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                // Salva la cartella di lavoro
                workbook.Save("SetTotalNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTotalName method: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


