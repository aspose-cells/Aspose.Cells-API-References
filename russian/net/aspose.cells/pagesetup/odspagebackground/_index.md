---
title: "PageSetup.ODSPageBackground"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Получает фон ODS"
type: docs
url: /ru/net/aspose.cells/pagesetup/odspagebackground/
---
## PageSetup.ODSPageBackground property

Получает фон ODS.

```csharp
public OdsPageBackground ODSPageBackground { get; }
```

### Примеры

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
            
            // Установить цвет фона
            background.Type = OdsPageBackgroundType.Color;
            background.Color = Color.LightGreen;
            
            // В качестве альтернативы установить графический фон
            background.Type = OdsPageBackgroundType.Graphic;
            background.GraphicType = OdsPageBackgroundGraphicType.Tile;
            background.GraphicPositionType = OdsPageBackgroundGraphicPositionType.TopLeft;
            
            workbook.Save("ODSPageBackgroundDemo.ods");
        }
    }
}
```

### См. также

* class [OdsPageBackground](../../../aspose.cells.ods/odspagebackground/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


