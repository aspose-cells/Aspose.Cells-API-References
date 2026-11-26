---
title: "Style.ForegroundColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Style. Получает или задаёт цвет переднего плана стиля"
type: docs
url: /ru/net/aspose.cells/style/foregroundcolor/
---
## Style.ForegroundColor property

Получает или задает цвет переднего плана стиля.

```csharp
public Color ForegroundColor { get; set; }
```

### Примечания

Это означает отсутствие настройки цвета, если возвращается Color.Empty.

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyForegroundColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            Style style = workbook.CreateStyle();
            style.ForegroundColor = Color.Green;
            style.Pattern = BackgroundType.Solid;
            
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            
            Console.WriteLine("ForegroundColor set to: " + style.ForegroundColor);
            
            workbook.Save("ForegroundColorDemo.xlsx");
        }
    }
}
```

### См. также

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


