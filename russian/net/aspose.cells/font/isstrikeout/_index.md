---
title: "Font.IsStrikeout"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Font. Получает или задает значение, указывающее, имеет ли шрифт одиночное зачеркивание"
type: docs
url: /ru/net/aspose.cells/font/isstrikeout/
---
## Font.IsStrikeout property

Получает или задает значение, указывающее, имеет ли шрифт одинарное зачеркивание.

```csharp
public bool IsStrikeout { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsStrikeoutDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Метод 1: Установить зачеркивание напрямую через стиль
            Cell cell1 = worksheet.Cells["A1"];
            Style style1 = cell1.GetStyle();
            style1.Font.IsStrikeout = true;
            cell1.SetStyle(style1);
            cell1.PutValue("Strikeout Text (Style)");
            
            // Метод 2: Установить зачеркивание через HTML
            Cell cell2 = worksheet.Cells["A2"];
            cell2.HtmlString = "<s>Strikeout Text (HTML)</s>";
            
            // Проверьте свойство зачеркивания
            Console.WriteLine("A1 IsStrikeout: " + cell1.GetStyle().Font.IsStrikeout);
            Console.WriteLine("A2 IsStrikeout: " + cell2.GetStyle().Font.IsStrikeout);
            
            // Сохраните для проверки
            workbook.Save("FontStrikeoutDemo.xlsx");
        }
    }
}
```

### См. также

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


