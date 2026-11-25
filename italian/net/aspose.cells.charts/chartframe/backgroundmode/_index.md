---
title: "ChartFrame.BackgroundMode"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartFrame. Ottiene e imposta la modalità di visualizzazione dello sfondo. Questa proprietà è valida solo in Excel 2003 o versioni precedenti."
type: docs
url: /it/net/aspose.cells.charts/chartframe/backgroundmode/
---
## ChartFrame.BackgroundMode property

Ottiene e imposta la modalità di visualizzazione dello sfondo. Questa proprietà è valida solo in Excel 2003 o versioni precedenti.

```csharp
[Obsolete("Use ChartFrame.Area.FillFormat.FillType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public BackgroundMode BackgroundMode { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà ChartFrame.Area.FillFormat.FillType. Per esempio, se è necessario impostare BackgroundMode su Opaque, è possibile utilizzare il seguente codice: Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; Questa proprietà sarà rimossa tra 12 mesi a partire da febbraio 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyBackgroundModeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Orange");
            sheet.Cells["A4"].PutValue("Banana");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(50);
            sheet.Cells["B3"].PutValue(30);
            sheet.Cells["B4"].PutValue(20);

            // Aggiungi un grafico
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Imposta i dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Dimostra la proprietà BackgroundMode
            chart.ChartArea.BackgroundMode = Aspose.Cells.Charts.BackgroundMode.Transparent;
            chart.PlotArea.BackgroundMode = Aspose.Cells.Charts.BackgroundMode.Automatic;

            // Salva la cartella di lavoro
            workbook.Save("ChartBackgroundModeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [BackgroundMode](../../backgroundmode/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


