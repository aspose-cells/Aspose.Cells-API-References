---
title: "OdsPageBackground.Color"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OdsPageBackground. Ottiene e imposta il colore di sfondo"
type: docs
url: /it/net/aspose.cells.ods/odspagebackground/color/
---
## OdsPageBackground.Color property

Ottiene e imposta il colore dello sfondo.

```csharp
public Color Color { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class OdsPageBackgroundPropertyColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            PageSetup ps = workbook.Worksheets[0].PageSetup;
            OdsPageBackground b = ps.ODSPageBackground;
            
            b.Type = OdsPageBackgroundType.Color;
            b.Color = Color.Red;
            
            workbook.Save("output.ods");
            
            Workbook loadedWorkbook = new Workbook("output.ods");
            PageSetup loadedPs = loadedWorkbook.Worksheets[0].PageSetup;
            OdsPageBackground loadedB = loadedPs.ODSPageBackground;
            
            Console.WriteLine("Background Type: " + loadedB.Type);
            Console.WriteLine("Background Color: " + loadedB.Color);
        }
    }
}
```

### Vedi anche

* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


