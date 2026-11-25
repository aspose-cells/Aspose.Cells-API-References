---
title: "GlobalizationSettings.GetTotalName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GlobalizationSettings. Ottiene il nome totale della funzione"
type: docs
url: /it/net/aspose.cells/globalizationsettings/gettotalname/
---
## GlobalizationSettings.GetTotalName method

Ottiene il nome totale della funzione.

```csharp
public virtual string GetTotalName(ConsolidationFunction functionType)
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
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetTotalNameWithConsolidationFunctionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Bike";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Car";
            worksheet.Cells["B3"].Value = 2500;
            worksheet.Cells["A4"].Value = "Bike";
            worksheet.Cells["B4"].Value = 1500;

            // Crea impostazioni di globalizzazione personalizzate
            var customSettings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = customSettings;

            try
            {
                // Dimostra la chiamata diretta del metodo
                Console.WriteLine("Sum Total Name: " + 
                    customSettings.GetTotalName(ConsolidationFunction.Sum));
                
                // Crea una tabella pivot per attivare l'uso di GetTotalName
                int pivotIndex = worksheet.PivotTables.Add("PivotTable", "A1:B4", "D1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
                PivotField dataField = pivotTable.DataFields[dataFieldIndex];
                dataField.Function = ConsolidationFunction.Sum;

                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("PivotTable created with custom total names");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("GlobalizationSettingsMethodGetTotalNameDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override string GetTotalName(ConsolidationFunction functionType)
            {
                return functionType switch
                {
                    ConsolidationFunction.Sum => "[Sum Custom]",
                    ConsolidationFunction.Count => "[Count Custom]",
                    _ => base.GetTotalName(functionType)
                };
            }
        }
    }
}
```

### Vedi anche

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


