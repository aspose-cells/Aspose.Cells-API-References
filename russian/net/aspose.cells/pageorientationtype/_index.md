---
title: "Перечисление PageOrientationType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.PageOrientationType. Представляет константы ориентации печати"
type: docs
url: /ru/net/aspose.cells/pageorientationtype/
---
## PageOrientationType enumeration

Представляет константы ориентации печати.

```csharp
public enum PageOrientationType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Landscape | `0` | Альбомная ориентация |
| Portrait | `1` | Книжная ориентация |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PageOrientationTypeDemo
    {
        public static void PageOrientationTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу в рабочей книге
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получите доступ к объекту PageSetup листа
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Установите ориентацию страницы в альбомную
            pageSetup.Orientation = PageOrientationType.Landscape;
            
            // Сохранить книгу в файл
            workbook.Save("PageOrientationTypeExample_Landscape.xlsx");

            // Установите ориентацию страницы в книжную
            pageSetup.Orientation = PageOrientationType.Portrait;
            
            // Сохраните книгу в другой файл
            workbook.Save("PageOrientationTypeExample_Portrait.xlsx");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


