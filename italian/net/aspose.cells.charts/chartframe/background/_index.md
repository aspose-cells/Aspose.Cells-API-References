---
title: "ChartFrame.Background"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartFrame. Ottiene e imposta la modalità di visualizzazione dello sfondo. Questa proprietà è valida solo in Excel 2003 o versioni precedenti."
type: docs
url: /it/net/aspose.cells.charts/chartframe/background/
---
## ChartFrame.Background property

Ottiene e imposta la modalità di visualizzazione dello sfondo. Questa proprietà è valida solo in Excel 2003 o versioni precedenti.

```csharp
[Obsolete("Use ChartFrame.Area.FillFormat.FillType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public BackgroundMode Background { get; set; }
```

### Osservazioni

NOTA: questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà ChartFrame.Area.FillFormat.FillType. Ad esempio, se è necessario impostare BackgroundMode su Opaque, è possibile utilizzare il seguente codice: Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; Questa proprietà sarà rimossa 12 mesi dopo, a partire da GENNAIO 2012. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyBackgroundDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
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
            Chart chart = worksheet.Charts[chartIndex];

            // Configura i dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Configura le etichette dei dati con le impostazioni di sfondo
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            dataLabels.ShowValue = true;
            dataLabels.Background = BackgroundMode.Transparent;

            // Salva la cartella di lavoro
            workbook.Save("ChartBackgroundDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [BackgroundMode](../../backgroundmode/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


