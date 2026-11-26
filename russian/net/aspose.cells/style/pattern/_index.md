---
title: "Style.Pattern"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Style. Получает или задаёт тип шаблона фона ячейки"
type: docs
url: /ru/net/aspose.cells/style/pattern/
---
## Style.Pattern property

Получает или задает тип фонового узора ячейки.

```csharp
public BackgroundType Pattern { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyPatternDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Получить доступ к ячейке и её стиль
            Cell cell = cells[0, 0];
            Style style = cell.GetStyle();
            
            // Установить шаблон и цвет переднего плана
            style.Pattern = BackgroundType.Gray50;
            style.ForegroundColor = System.Drawing.Color.LightGray;
            
            // Применить стиль к ячейке
            cell.SetStyle(style);
            
            // Сохраните книгу
            workbook.Save("PatternPropertyDemo.xlsx");
        }
    }
}
```

### См. также

* enum [BackgroundType](../../backgroundtype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


