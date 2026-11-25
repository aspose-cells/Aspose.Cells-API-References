---
title: "Line.ThemeColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Line property. Ottiene e imposta il colore del tema"
type: docs
url: /it/net/aspose.cells.drawing/line/themecolor/
---
## Line.ThemeColor property

Ottiene e imposta il colore del tema.

```csharp
public ThemeColor ThemeColor { get; set; }
```

### Osservazioni

Se il colore di primo piano non è un colore tematico, verrà restituito NULL.

### Esempi

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyThemeColorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Series 1");
            sheet.Cells["C1"].PutValue("Series 2");
            
            for (int i = 2; i <= 6; i++)
            {
                sheet.Cells["A" + i].PutValue("Cat " + (i-1));
                sheet.Cells["B" + i].PutValue(i * 10);
                sheet.Cells["C" + i].PutValue(i * 15);
            }

            // Aggiungi un grafico a linee
            int chartIndex = sheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.SetChartDataRange("B1:C6", true);
            chart.NSeries.CategoryData = "A2:A6";

            // Personalizza l'aspetto della serie con ThemeColor
            var seriesThemes = new List<ThemeColorType> { 
                ThemeColorType.Accent1, 
                ThemeColorType.Accent2 
            };

            for (int i = 0; i < chart.NSeries.Count; i++)
            {
                chart.NSeries[i].Border.ThemeColor = new ThemeColor(seriesThemes[i], 0.6);
                chart.NSeries[i].Border.Style = LineType.Solid;
                chart.NSeries[i].Border.Weight = WeightType.MediumLine;
            }

            // Salva la cartella di lavoro
            workbook.Save("LineChartWithThemeColor.xlsx");
        }
    }
}
```

### Vedi anche

* class [ThemeColor](../../../aspose.cells/themecolor/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


