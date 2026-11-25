---
title: "GlobalizationSettings.GetGrandTotalName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GlobalizationSettings. Ottiene il nome del totale generale della funzione"
type: docs
url: /it/net/aspose.cells/globalizationsettings/getgrandtotalname/
---
## GlobalizationSettings.GetGrandTotalName method

Ottiene il nome del totale generale della funzione.

```csharp
public virtual string GetGrandTotalName(ConsolidationFunction functionType)
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
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetGrandTotalNameWithConsolidationFunctionDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e accedi al primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola dati di esempio per la tabella pivot
            CreateSampleData(worksheet);

            // Istanzia impostazioni di globalizzazione personalizzate
            var globalizationSettings = new CustomGlobalizationSettings();
            
            try
            {
                // Dimostra la chiamata diretta del metodo
                string grandTotalName = globalizationSettings.GetGrandTotalName(ConsolidationFunction.Sum);
                Console.WriteLine($"Grand Total Name: {grandTotalName}");

                // Applica la personalizzazione alle impostazioni della cartella di lavoro
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                // Crea una tabella pivot per dimostrare l'effetto
                CreatePivotTable(worksheet);

                Console.WriteLine("Method executed successfully. Check output file.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetGrandTotalName method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("GrandTotalNameDemo.xlsx");
        }

        private static void CreateSampleData(Worksheet worksheet)
        {
            var cells = worksheet.Cells;
            cells["A1"].Value = "Category";
            cells["B1"].Value = "Value";
            cells["A2"].Value = "Electronics";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Furniture";
            cells["B3"].Value = 1500;
            cells["A4"].Value = "Electronics";
            cells["B4"].Value = 800;
        }

        private static void CreatePivotTable(Worksheet worksheet)
        {
            // Crea una tabella pivot usando l'intervallo di dati di esempio
            int pivotTableIndex = worksheet.PivotTables.Add("PivotTable", "A1:B4", "D1");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];

            // Configura i campi della tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            PivotField dataField = pivotTable.DataFields[dataFieldIndex];
            dataField.Function = ConsolidationFunction.Sum;

            // Aggiorna la tabella per applicare le impostazioni
            pivotTable.RefreshData();
            pivotTable.CalculateData();
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetGrandTotalName(ConsolidationFunction functionType)
        {
            // Implementazione personalizzata basata sulla funzione di consolidamento
            return functionType == ConsolidationFunction.Sum 
                ? "**[Sum Total]**" 
                : base.GetGrandTotalName(functionType);
        }
    }
}
```

### Vedi anche

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


