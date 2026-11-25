---
title: "GlobalizationSettings.GetRowLabelsNameOfPivotTable"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GlobalizationSettings. Ottiene il nome dell'etichetta Row Labels nella PivotTable"
type: docs
url: /it/net/aspose.cells/globalizationsettings/getrowlabelsnameofpivottable/
---
## GlobalizationSettings.GetRowLabelsNameOfPivotTable method

Ottiene il nome dell'etichetta "Row Labels" nella PivotTable.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfRowLabels() method instead.")]
public virtual string GetRowLabelsNameOfPivotTable()
```

### Valore di ritorno

Il nome delle etichette di riga

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Questa proprietà sarà rimossa tra 12 mesi a partire da dicembre 2022. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetRowLabelsNameOfPivotTable()
        {
            return "Custom Row Labels";
        }
    }

    public class GlobalizationSettingsMethodGetRowLabelsNameOfPivotTableDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea dati di esempio per la tabella pivot
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Product");
            cells["A2"].PutValue("Bikes");
            cells["A3"].PutValue("Cars");
            cells["B1"].PutValue("Sales");
            cells["B2"].PutValue(1000);
            cells["B3"].PutValue(2500);

            // Crea tabella pivot
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B3", "E3", "SalesPivot");
            PivotTable pivotTable = pivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product as row field

            // Applica impostazioni di globalizzazione personalizzate
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                pivotTable.RefreshData();
                pivotTable.CalculateData();
                Console.WriteLine("Pivot table created with custom row labels name.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRowLabelsNameOfPivotTable: {ex.Message}");
            }

            workbook.Save("GlobalizationSettingsMethodGetRowLabelsNameOfPivotTableDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


