---
title: "OdsPageBackground.Color"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad OdsPageBackground. Obtiene y establece el color del fondo"
type: docs
url: /es/net/aspose.cells.ods/odspagebackground/color/
---
## OdsPageBackground.Color property

Obtiene y establece el color del fondo.

```csharp
public Color Color { get; set; }
```

### Ejemplos

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

### Ver también

* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


