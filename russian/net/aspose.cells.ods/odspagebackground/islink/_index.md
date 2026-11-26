---
title: "OdsPageBackground.IsLink"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство OdsPageBackground. Указывает, является ли графика связанной"
type: docs
url: /ru/net/aspose.cells.ods/odspagebackground/islink/
---
## OdsPageBackground.IsLink property

Указывает, является ли графика связанной.

```csharp
public bool IsLink { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;

    public class OdsPageBackgroundPropertyIsLinkDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook(FileFormatType.Ods);
            Worksheet worksheet = workbook.Worksheets[0];

            // Получите доступ к OdsPageBackground
            OdsPageBackground background = worksheet.PageSetup.ODSPageBackground;

            // Отобразите текущее значение IsLink
            Console.WriteLine("Current IsLink value: " + background.IsLink);

            // Измените существующие свойства фона вместо создания новых
            background.Type = OdsPageBackgroundType.Graphic;
            background.GraphicType = OdsPageBackgroundGraphicType.Position;
            background.GraphicPositionType = OdsPageBackgroundGraphicPositionType.TopLeft;
            background.LinkedGraphic = "path/to/image.png";

            // Отобразите новое значение IsLink
            Console.WriteLine("New IsLink value: " + worksheet.PageSetup.ODSPageBackground.IsLink);

            // Сохранить результат
            workbook.Save("OdsPageBackgroundIsLinkDemo.ods");
        }
    }
}
```

### См. также

* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


