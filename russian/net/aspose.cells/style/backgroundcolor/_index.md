---
title: "Style.BackgroundColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Style. Получает или задает цвет фона стиля"
type: docs
url: /ru/net/aspose.cells/style/backgroundcolor/
---
## Style.BackgroundColor property

Получает или задает цвет фона стиля.

```csharp
public Color BackgroundColor { get; set; }
```

### Примечания

Если вы хотите задать цвет ячейки, используйте свойство Style.ForegroundColor. Это свойство будет действовать только в том случае, если шаблон стиля ячейки отличается от none или solid.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyBackgroundColorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создать объект стиля
            Style style = workbook.CreateStyle();
            
            // Установите цвет фона в желтый
            style.BackgroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            
            // Применить стиль к ячейке A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Cell with yellow background");
            cell.SetStyle(style);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


