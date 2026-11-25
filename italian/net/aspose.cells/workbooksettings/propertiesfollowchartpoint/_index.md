---
title: "WorkbookSettings.PropertiesFollowChartPoint"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Indica se le proprietà dei punti dati e le etichette dei dati in tutti i grafici di questa cartella di lavoro seguono il loro riferimento"
type: docs
url: /it/net/aspose.cells/workbooksettings/propertiesfollowchartpoint/
---
## WorkbookSettings.PropertiesFollowChartPoint property

Indica se le proprietà dei punti dati e le etichette dei dati in tutti i grafici di questo workbook seguono il loro riferimento.

```csharp
public bool PropertiesFollowChartPoint { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyPropertiesFollowChartPointDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Imposta PropertiesFollowChartPoint su true
            workbook.Settings.PropertiesFollowChartPoint = true;
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
            
            // Verifica che l'impostazione sia stata salvata
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("PropertiesFollowChartPoint: " + loadedWorkbook.Settings.PropertiesFollowChartPoint);
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


