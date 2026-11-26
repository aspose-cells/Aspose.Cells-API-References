---
title: "Перечисление OdsPageBackgroundGraphicType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Ods.OdsPageBackgroundGraphicType enum. Представляет тип оформления фона страницы с изображением"
type: docs
url: /ru/net/aspose.cells.ods/odspagebackgroundgraphictype/
---
## OdsPageBackgroundGraphicType enumeration

Представляет тип форматирования фона страницы с изображением.

```csharp
public enum OdsPageBackgroundGraphicType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Position | `0` | Установите изображение в определённую позицию. |
| Area | `1` | Растяните изображение. |
| Tile | `2` | Повторяйте изображение. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;
    using System.Drawing;

    public class OdsPageBackgroundGraphicTypeDemo
    {
        public static void OdsPageBackgroundGraphicTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Получить доступ к PageSetup листа
            PageSetup pageSetup = worksheet.PageSetup;

            // Получите доступ к ODSPageBackground из PageSetup
            OdsPageBackground odsPageBackground = pageSetup.ODSPageBackground;

            // Установить цвет фона
            odsPageBackground.Color = Color.LightBlue;

            // Установите тип фоновой графики в Tile
            odsPageBackground.GraphicType = OdsPageBackgroundGraphicType.Tile;

            // Установите путь к связанному графическому файлу (предполагая, что изображение находится в той же директории, что и исполняемый файл)
            odsPageBackground.LinkedGraphic = "background_image.png";

            // Сохраните книгу
            workbook.Save("OdsPageBackgroundGraphicTypeExample.ods");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


