---
title: "OdsPageBackground.GraphicType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство OdsPageBackground. Получает и задает тип графики фона страницы"
type: docs
url: /ru/net/aspose.cells.ods/odspagebackground/graphictype/
---
## OdsPageBackground.GraphicType property

Получает и задает тип фоновой графики страницы.

```csharp
public OdsPageBackgroundGraphicType GraphicType { get; set; }
```

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsPageBackgroundPropertyGraphicTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            PageSetup pageSetup = sheet.PageSetup;
            OdsPageBackground odsPageBackground = pageSetup.ODSPageBackground;
            
            odsPageBackground.Type = OdsPageBackgroundType.Graphic;
            odsPageBackground.GraphicType = OdsPageBackgroundGraphicType.Tile;
            odsPageBackground.LinkedGraphic = "background.png";
            
            workbook.Save("OdsPageBackgroundGraphicTypeDemo.ods");
        }
    }
}
```

### См. также

* enum [OdsPageBackgroundGraphicType](../../odspagebackgroundgraphictype/)
* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


