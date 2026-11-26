---
title: "Перечисление OdsPageBackgroundType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Ods.OdsPageBackgroundType. Представляет тип фона страницы ODS"
type: docs
url: /ru/net/aspose.cells.ods/odspagebackgroundtype/
---
## OdsPageBackgroundType enumeration

Представляет тип фона страницы формата ODS.

```csharp
public enum OdsPageBackgroundType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Без фона. |
| Color | `1` | Форматирует фон цветом. |
| Graphic | `2` | Форматирует фон изображением. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;
    using System.Drawing;

    public class OdsPageBackgroundTypeDemo
    {
        public static void OdsPageBackgroundTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Получить доступ к PageSetup листа
            PageSetup pageSetup = worksheet.PageSetup;

            // Получите доступ к свойству ODSPageBackground
            OdsPageBackground odsPageBackground = pageSetup.ODSPageBackground;

            // Установите тип фона в Color
            odsPageBackground.Type = OdsPageBackgroundType.Color;

            // Установить цвет фона
            odsPageBackground.Color = Color.LightBlue;

            // Сохраните книгу
            workbook.Save("OdsPageBackgroundTypeExample.ods");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


