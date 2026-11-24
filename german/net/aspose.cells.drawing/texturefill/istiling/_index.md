---
title: "TextureFill.IsTiling"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextureFill-Eigenschaft. Gibt an, ob das Bild als Textur gekachelt wird"
type: docs
url: /de/net/aspose.cells.drawing/texturefill/istiling/
---
## TextureFill.IsTiling property

Gibt an, ob das Bild als Textur gekachelt wird.

```csharp
public bool IsTiling { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdaten festlegen
            chart.NSeries.Add("A1:B3", true);
            
            // Texturfüllung für den Diagrammbereich festlegen
            chart.PlotArea.Area.FillFormat.Texture = TextureType.BlueTissuePaper;
            
            // IsTiling-Eigenschaft festlegen
            chart.PlotArea.Area.FillFormat.TextureFill.IsTiling = true;
            
            // Den IsTiling-Wert überprüfen und ausgeben
            Console.WriteLine("IsTiling: " + chart.PlotArea.Area.FillFormat.TextureFill.IsTiling);
            
            // Speichere die Arbeitsmappe
            workbook.Save("TextureFillIsTilingDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


