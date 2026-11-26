---
title: "Style.ForegroundArgbColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Style. Получает и задает цвет переднего плана с 32‑битным значением ARGB"
type: docs
url: /ru/net/aspose.cells/style/foregroundargbcolor/
---
## Style.ForegroundArgbColor property

Получает и задает цвет переднего плана в виде 32‑битного значения ARGB.

```csharp
public int ForegroundArgbColor { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyForegroundArgbColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создайте стиль с определённым цветом переднего плана
            Style style = workbook.CreateStyle();
            style.ForegroundColor = System.Drawing.Color.FromArgb(255, 0, 255, 0); // Green color
            style.Pattern = BackgroundType.Solid;
            
            // Применить стиль к ячейке
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            
            // Получите и отобразите значение ARGB цвета переднего плана
            int foregroundArgb = cell.GetStyle().ForegroundArgbColor;
            Console.WriteLine("Foreground ARGB Color: " + foregroundArgb);
            
            // Сохраните книгу
            workbook.Save("ForegroundColorDemo.xlsx");
        }
    }
}
```

### См. также

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


