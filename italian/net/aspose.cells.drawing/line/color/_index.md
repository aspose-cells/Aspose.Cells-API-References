---
title: "Line.Color"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Line. Rappresenta il colore della linea"
type: docs
url: /it/net/aspose.cells.drawing/line/color/
---
## Line.Color property

Rappresenta il colore della linea.

```csharp
public Color Color { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyColorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per il grafico
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Imposta i colori delle linee dell'asse
            chart.CategoryAxis.AxisLine.Color = Color.BlueViolet;
            chart.ValueAxis.AxisLine.Color = Color.BlueViolet;
            
            // Imposta il colore del carattere del titolo dell'asse
            chart.CategoryAxis.Title.Text = "Categories";
            chart.CategoryAxis.Title.Font.Color = Color.BlueViolet;

            // Salva la cartella di lavoro
            workbook.Save("LinePropertyColorDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


