---
title: "OdsPageBackground.GraphicPositionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство OdsPageBackground. Получает и задает позицию графического фона"
type: docs
url: /ru/net/aspose.cells.ods/odspagebackground/graphicpositiontype/
---
## OdsPageBackground.GraphicPositionType property

Получает и задает позицию фоновой графики.

```csharp
public OdsPageBackgroundGraphicPositionType GraphicPositionType { get; set; }
```

### Примеры

```csharp
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsPageBackgroundPropertyGraphicPositionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            PageSetup pageSetup = sheet.PageSetup;
            OdsPageBackground background = pageSetup.ODSPageBackground;

            background.Type = OdsPageBackgroundType.Graphic;
            background.GraphicType = OdsPageBackgroundGraphicType.Tile;
            background.GraphicPositionType = OdsPageBackgroundGraphicPositionType.CenterCenter;
            background.LinkedGraphic = "sample/image.png";

            workbook.Save("OdsPageBackgroundGraphicPositionDemo.ods");
        }
    }
}
```

### См. также

* enum [OdsPageBackgroundGraphicPositionType](../../odspagebackgroundgraphicpositiontype/)
* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


