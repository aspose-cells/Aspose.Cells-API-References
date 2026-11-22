---
title: "OdsPageBackground.LinkedGraphic"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية OdsPageBackground. تحصل وتعيّن مسار الرسم المرتبط"
type: docs
url: /ar/net/aspose.cells.ods/odspagebackground/linkedgraphic/
---
## OdsPageBackground.LinkedGraphic property

يحصل ويضبط مسار الرسمة المرتبطة.

```csharp
public string LinkedGraphic { get; set; }
```

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsPageBackgroundPropertyLinkedGraphicDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            PageSetup pageSetup = worksheet.PageSetup;
            OdsPageBackground odsPageBackground = pageSetup.ODSPageBackground;

            odsPageBackground.Color = Color.LightBlue;
            odsPageBackground.GraphicType = OdsPageBackgroundGraphicType.Tile;
            odsPageBackground.LinkedGraphic = "background_image.png";

            workbook.Save("OdsPageBackgroundLinkedGraphicDemo.ods");
        }
    }
}
```

### انظر أيضًا

* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


