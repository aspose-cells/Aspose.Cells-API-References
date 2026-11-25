---
title: "GlobalizationSettings.GetMultipleItemsName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "GlobalizationSettings method. Ottiene il nome dell'etichetta Multiple Items nella PivotTable"
type: docs
url: /it/net/aspose.cells/globalizationsettings/getmultipleitemsname/
---
## GlobalizationSettings.GetMultipleItemsName method

Ottiene il nome dell'etichetta "(Multiple Items)" nella PivotTable.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfMultipleItems() method instead.")]
public virtual string GetMultipleItemsName()
```

### Valore di ritorno

Il nome dell'etichetta "(Multiple Items)"

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Questa proprietà sarà rimossa tra 12 mesi a partire da dicembre 2022. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetMultipleItemsNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Prepara dati di esempio per la PivotTable
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["A4"].Value = "C";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Crea PivotTable
            int pivotIndex = worksheet.PivotTables.Add("D1", "A1:B4", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);

            // Configura PivotField per mostrare più elementi
            PivotField rowField = pivotTable.RowFields[0];
            rowField.IsMultipleItemSelectionAllowed = true;
            rowField.HideItem(0, false); // Select "A"
            rowField.HideItem(1, false); // Select "B"

            // Inizializza le impostazioni di globalizzazione
            GlobalizationSettings gSettings = workbook.Settings.GlobalizationSettings ?? new GlobalizationSettings();
            workbook.Settings.GlobalizationSettings = gSettings;

            try
            {
                // Chiama GetMultipleItemsName e visualizza il risultato
                string multipleItemsName = gSettings.GetMultipleItemsName();
                Console.WriteLine($"Multiple Items Name: {multipleItemsName}");

                // Aggiorna la PivotTable per applicare le impostazioni
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetMultipleItemsName: {ex.Message}");
            }

            // Salva la cartella di lavoro per mostrare la PivotTable con l'etichetta "(Multiple Items)"
            workbook.Save("GlobalizationSettingsMethodGetMultipleItemsNameDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


