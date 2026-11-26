---
title: "Класс OdsPageBackground"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Ods.OdsPageBackground. Представляет фон страницы ODS"
type: docs
url: /ru/net/aspose.cells.ods/odspagebackground/
---
## OdsPageBackground class

Представляет фон страницы ODS.

```csharp
public class OdsPageBackground
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [OdsPageBackground](odspagebackground/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Color](../../aspose.cells.ods/odspagebackground/color/) { get; set; } | Получает и задает цвет фона. |
| [GraphicData](../../aspose.cells.ods/odspagebackground/graphicdata/) { get; set; } | Получает и задает графические данные. |
| [GraphicPositionType](../../aspose.cells.ods/odspagebackground/graphicpositiontype/) { get; set; } | Получает и задает позицию фоновой графики. |
| [GraphicType](../../aspose.cells.ods/odspagebackground/graphictype/) { get; set; } | Получает и задает тип фоновой графики страницы. |
| [IsLink](../../aspose.cells.ods/odspagebackground/islink/) { get; } | Указывает, является ли графика связанной. |
| [LinkedGraphic](../../aspose.cells.ods/odspagebackground/linkedgraphic/) { get; set; } | Получает и задает путь к связанной графике. |
| [Type](../../aspose.cells.ods/odspagebackground/type/) { get; set; } | Получает и задает тип фона страницы. |

### Примеры

```csharp
using Aspose.Cells;
using Aspose.Cells.Ods;
using System;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class OdsPageBackgroundDemo
    {
        public static void OdsPageBackgroundExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Доступ к объекту PageSetup
            PageSetup pageSetup = sheet.PageSetup;

            // Получить доступ к объекту ODSPageBackground
            OdsPageBackground odsPageBackground = pageSetup.ODSPageBackground;

            // Установите тип фона в Color
            odsPageBackground.Type = OdsPageBackgroundType.Color;

            // Установить цвет фона
            odsPageBackground.Color = Color.LightBlue;

            // Установить тип фоновой графики
            odsPageBackground.GraphicType = OdsPageBackgroundGraphicType.Tile;

            // Установить позицию фоновой графики
            odsPageBackground.GraphicPositionType = OdsPageBackgroundGraphicPositionType.CenterCenter;

            // Установить путь к связанной графике (если есть)
            odsPageBackground.LinkedGraphic = "path/to/graphic.png";

            // Сохраните книгу
            workbook.Save("OdsPageBackgroundExample.ods");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


