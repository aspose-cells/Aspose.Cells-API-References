---
title: "SettableGlobalizationSettings.SetGrandTotalName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettableGlobalizationSettings. Imposta il nome del totale generale per una funzione specifica"
type: docs
url: /it/net/aspose.cells/settableglobalizationsettings/setgrandtotalname/
---
## SettableGlobalizationSettings.SetGrandTotalName method

Imposta il nome del totale complessivo della funzione specifica.

```csharp
public void SetGrandTotalName(ConsolidationFunction functionType, string name)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| functionType | ConsolidationFunction | Il tipo di funzione. |
| name | String | Il nome del totale generale della funzione. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettableGlobalizationSettingsMethodSetGrandTotalNameWithConsolidationFunctionStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea dati di esempio per la tabella pivot
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["A3"].PutValue("Fruit");
            worksheet.Cells["A4"].PutValue("Vegetable");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(75);

            // Crea tabella pivot
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            pivotTable.DataFields[0].Function = ConsolidationFunction.Sum;

            // Crea impostazioni di globalizzazione personalizzate
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Chiama SetGrandTotalName con ConsolidationFunction.Sum e un nome personalizzato
                settings.SetGrandTotalName(ConsolidationFunction.Sum, "Custom Grand Total");

                // Aggiorna la tabella pivot per applicare le modifiche
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("Grand total name set to 'Custom Grand Total' for Sum function");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetGrandTotalName method: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("MethodSetGrandTotalNameDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


