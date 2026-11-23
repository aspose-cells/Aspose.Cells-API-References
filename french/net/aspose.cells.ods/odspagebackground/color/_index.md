---
title: "OdsPageBackground.Color"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété OdsPageBackground. Obtient et définit la couleur d'arrière-plan"
type: docs
url: /fr/net/aspose.cells.ods/odspagebackground/color/
---
## OdsPageBackground.Color property

Obtient et définit la couleur de l'arrière-plan.

```csharp
public Color Color { get; set; }
```

### Exemples

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

### Voir aussi

* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


