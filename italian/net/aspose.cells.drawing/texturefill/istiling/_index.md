---
title: "TextureFill.IsTiling"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextureFill. Indica se ripetere l'immagine come texture"
type: docs
url: /it/net/aspose.cells.drawing/texturefill/istiling/
---
## TextureFill.IsTiling property

Indica se l'immagine è ripetuta come texture.

```csharp
public bool IsTiling { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextureFillPropertyIsTilingDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta i dati del grafico
            chart.NSeries.Add("A1:B3", true);
            
            // Imposta il riempimento texture per l'area del grafico
            chart.PlotArea.Area.FillFormat.Texture = TextureType.BlueTissuePaper;
            
            // Imposta la proprietà IsTiling
            chart.PlotArea.Area.FillFormat.TextureFill.IsTiling = true;
            
            // Verifica e visualizza il valore IsTiling
            Console.WriteLine("IsTiling: " + chart.PlotArea.Area.FillFormat.TextureFill.IsTiling);
            
            // Salva la cartella di lavoro
            workbook.Save("TextureFillIsTilingDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


