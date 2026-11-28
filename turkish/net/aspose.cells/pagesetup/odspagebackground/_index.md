---
title: "PageSetup.ODSPageBackground"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup özelliği. ODS'nin arka planını alır"
type: docs
url: /tr/net/aspose.cells/pagesetup/odspagebackground/
---
## PageSetup.ODSPageBackground property

ODS'nin arka planını alır.

```csharp
public OdsPageBackground ODSPageBackground { get; }
```

### Örnekler

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
            
            // Renk arka planını ayarla
            background.Type = OdsPageBackgroundType.Color;
            background.Color = Color.LightGreen;
            
            // Alternatif olarak, grafik arka planını ayarla
            background.Type = OdsPageBackgroundType.Graphic;
            background.GraphicType = OdsPageBackgroundGraphicType.Tile;
            background.GraphicPositionType = OdsPageBackgroundGraphicPositionType.TopLeft;
            
            workbook.Save("ODSPageBackgroundDemo.ods");
        }
    }
}
```

### Ayrıca Bakınız

* class [OdsPageBackground](../../../aspose.cells.ods/odspagebackground/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


