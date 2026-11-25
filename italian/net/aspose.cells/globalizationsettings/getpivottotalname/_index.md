---
title: "GlobalizationSettings.GetPivotTotalName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GlobalizationSettings. Ottiene il nome dell'etichetta Total nella PivotTable. È necessario sovrascrivere questo metodo quando la PivotTable contiene due o più PivotFields nell'area dati"
type: docs
url: /it/net/aspose.cells/globalizationsettings/getpivottotalname/
---
## GlobalizationSettings.GetPivotTotalName method

Ottiene il nome dell'etichetta "Total" nella PivotTable. È necessario sovrascrivere questo metodo quando la PivotTable contiene due o più PivotFields nell'area dati.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfTotal() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual string GetPivotTotalName()
```

### Valore di ritorno

Il nome dell'etichetta "Total"

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Questa proprietà sarà rimossa tra 12 mesi a partire da dicembre 2022. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetPivotTotalNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola dati di esempio
            worksheet.Cells["A1"].Value = "Region";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["C1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "North"; worksheet.Cells["B2"].Value = 1000; worksheet.Cells["C2"].Value = 50;
            worksheet.Cells["A3"].Value = "South"; worksheet.Cells["B3"].Value = 2000; worksheet.Cells["C3"].Value = 70;
            worksheet.Cells["A4"].Value = "West"; worksheet.Cells["B4"].Value = 3000; worksheet.Cells["C4"].Value = 110;

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E5", "SalesPivot");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Region
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Quantity

            // Crea e configura le impostazioni di globalizzazione
            var customSettings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = customSettings;

            try
            {
                // Dimostra la chiamata diretta del metodo
                Console.WriteLine("Custom Total Name: " + customSettings.GetPivotTotalName());

                // Elabora la tabella pivot
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("Pivot table created with custom total name.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("MethodGetPivotTotalNameDemo.xlsx");
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetPivotTotalName()
        {
            return "Custom Total";
        }
    }
}
```

### Vedi anche

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


