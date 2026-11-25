---
title: "GlobalizationSettings.GetEmptyDataName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GlobalizationSettings. Ottiene il nome dell'etichetta vuota nella Tabella Pivot"
type: docs
url: /it/net/aspose.cells/globalizationsettings/getemptydataname/
---
## GlobalizationSettings.GetEmptyDataName method

Ottiene il nome dell'etichetta "(blank)" nella Tabella Pivot.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfEmptyData() method instead.")]
public virtual string GetEmptyDataName()
```

### Valore di ritorno

Il nome dei dati vuoti

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Questa proprietà sarà rimossa tra 12 mesi a partire da dicembre 2022. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetEmptyDataNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea dati di esempio con celle vuote
            object[,] data = new object[,]
            {
                {"Category", "Sales"},
                {"Electronics", 1500},
                {null, 2000}, // Empty category cell
                {"Furniture", 3000}
            };

            // Popola il foglio di lavoro
            int rows = data.GetLength(0);
            int cols = data.GetLength(1);
            for (int i = 0; i < rows; i++)
            {
                for (int j = 0; j < cols; j++)
                {
                    worksheet.Cells[i, j].PutValue(data[i, j]);
                }
            }

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "SalesPivot");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            // Corretto: Rimuovi l'assegnazione non valida del risultato di AddFieldToArea
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Configura le impostazioni di globalizzazione personalizzate
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // Aggiorna la tabella pivot per applicare la localizzazione
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                // Dimostra la chiamata diretta del metodo
                string emptyName = workbook.Settings.GlobalizationSettings.GetEmptyDataName();
                Console.WriteLine($"Custom empty data label: {emptyName}");

                workbook.Save("GlobalizationGetEmptyDataNameDemo.xlsx");
                Console.WriteLine("Demo executed successfully. Check output file.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            [Obsolete]
            public override string GetEmptyDataName()
            {
                return "[[UNSPECIFIED]]"; // Custom empty data label
            }
        }
    }
}
```

### Vedi anche

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


