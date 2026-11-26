---
title: "OdsPageBackground.LinkedGraphic"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство OdsPageBackground. Получает и задает путь к связанному графическому файлу"
type: docs
url: /ru/net/aspose.cells.ods/odspagebackground/linkedgraphic/
---
## OdsPageBackground.LinkedGraphic property

Получает и задает путь к связанной графике.

```csharp
public string LinkedGraphic { get; set; }
```

### Примеры

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

### См. также

* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


