---
title: "PageSetup.ODSPageBackground"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageSetup. تحصل على خلفية ODS"
type: docs
url: /ar/net/aspose.cells/pagesetup/odspagebackground/
---
## PageSetup.ODSPageBackground property

يحصل على خلفية ODS.

```csharp
public OdsPageBackground ODSPageBackground { get; }
```

### أمثلة

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
            
            // تعيين خلفية ملونة
            background.Type = OdsPageBackgroundType.Color;
            background.Color = Color.LightGreen;
            
            // بدلاً من ذلك، تعيين خلفية رسومية
            background.Type = OdsPageBackgroundType.Graphic;
            background.GraphicType = OdsPageBackgroundGraphicType.Tile;
            background.GraphicPositionType = OdsPageBackgroundGraphicPositionType.TopLeft;
            
            workbook.Save("ODSPageBackgroundDemo.ods");
        }
    }
}
```

### انظر أيضًا

* class [OdsPageBackground](../../../aspose.cells.ods/odspagebackground/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


