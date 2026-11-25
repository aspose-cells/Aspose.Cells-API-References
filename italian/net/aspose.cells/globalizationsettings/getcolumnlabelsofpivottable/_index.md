---
title: "GlobalizationSettings.GetColumnLabelsOfPivotTable"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GlobalizationSettings. Ottiene il nome dell'etichetta Column Labels nella PivotTable"
type: docs
url: /it/net/aspose.cells/globalizationsettings/getcolumnlabelsofpivottable/
---
## GlobalizationSettings.GetColumnLabelsOfPivotTable method

Ottiene il nome dell'etichetta "Column Labels" nella PivotTable.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfColumnLabels() method instead.")]
public virtual string GetColumnLabelsOfPivotTable()
```

### Valore di ritorno

Il nome delle etichette di colonna

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Questa proprietà sarà rimossa tra 12 mesi a partire da dicembre 2022. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetColumnLabelsOfPivotTableDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola dati di esempio per la PivotTable
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Region";
            worksheet.Cells["C1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Bike";
            worksheet.Cells["B2"].Value = "North";
            worksheet.Cells["C2"].Value = 10000;
            worksheet.Cells["A3"].Value = "Bike";
            worksheet.Cells["B3"].Value = "South";
            worksheet.Cells["C3"].Value = 8000;
            worksheet.Cells["A4"].Value = "Car";
            worksheet.Cells["B4"].Value = "North";
            worksheet.Cells["C4"].Value = 25000;

            // Crea una PivotTable e ottieni il riferimento
            int pivotTableIndex = worksheet.PivotTables.Add("PivotTable", "A1:C4", "E5");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];
            
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Region
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales

            // Applica impostazioni di globalizzazione personalizzate per sovrascrivere le etichette di colonna
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // Aggiorna e calcola la PivotTable per applicare le impostazioni
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("GetColumnLabelsOfPivotTable method executed successfully. Check 'output.xlsx'.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }

    // Implementazione personalizzata di GlobalizationSettings per sovrascrivere le etichette di colonna
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetColumnLabelsOfPivotTable()
        {
            // Restituisce un'etichetta personalizzata per le intestazioni di colonna della PivotTable
            return "Sales Regions";
        }
    }
}
```

### Vedi anche

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


