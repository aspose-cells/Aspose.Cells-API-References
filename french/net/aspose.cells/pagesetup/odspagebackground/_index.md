---
title: "PageSetup.ODSPageBackground"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PageSetup. Obtient l'arrière-plan de ODS"
type: docs
url: /fr/net/aspose.cells/pagesetup/odspagebackground/
---
## PageSetup.ODSPageBackground property

Obtient l'arrière-plan de ODS.

```csharp
public OdsPageBackground ODSPageBackground { get; }
```

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyODSPageBackgroundDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            OdsPageBackground background = sheet.PageSetup.ODSPageBackground;
            
            // Définir l'arrière-plan couleur
            background.Type = OdsPageBackgroundType.Color;
            background.Color = Color.LightGreen;
            
            // Sinon, définissez l'arrière-plan graphique
            background.Type = OdsPageBackgroundType.Graphic;
            background.GraphicType = OdsPageBackgroundGraphicType.Tile;
            background.GraphicPositionType = OdsPageBackgroundGraphicPositionType.TopLeft;
            
            workbook.Save("ODSPageBackgroundDemo.ods");
        }
    }
}
```

### Voir aussi

* class [OdsPageBackground](../../../aspose.cells.ods/odspagebackground/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


