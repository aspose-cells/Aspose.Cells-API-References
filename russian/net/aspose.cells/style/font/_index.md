---
title: "Style.Font"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Style. Получает объект Font"
type: docs
url: /ru/net/aspose.cells/style/font/
---
## Style.Font property

Получает объект `Font`.

```csharp
public Font Font { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyFontDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Обратитесь к ячейке B4 и установите её шрифт полужирным
            Cell b4 = cells["B4"];
            Style b4Style = b4.GetStyle();
            b4Style.Font.IsBold = true;
            b4.SetStyle(b4Style);

            // Обратитесь к ячейке C4 и убедитесь, что её шрифт не полужирный
            Cell c4 = cells["C4"];
            Style c4Style = c4.GetStyle();
            c4Style.Font.IsBold = false;
            c4.SetStyle(c4Style);

            // Обратитесь к ячейке D4 и установите её шрифт полужирным с другим цветом
            Cell d4 = cells["D4"];
            Style d4Style = d4.GetStyle();
            d4Style.Font.IsBold = true;
            d4Style.Font.Color = Color.Red;
            d4.SetStyle(d4Style);

            // Проверьте свойства шрифта
            Console.WriteLine("B4 Font Bold: " + b4.GetStyle().Font.IsBold);
            Console.WriteLine("C4 Font Bold: " + c4.GetStyle().Font.IsBold);
            Console.WriteLine("D4 Font Bold: " + d4.GetStyle().Font.IsBold);
            Console.WriteLine("D4 Font Color: " + d4.GetStyle().Font.Color);

            // Сохраните книгу
            workbook.Save("FontPropertyDemo.xlsx");
        }
    }
}
```

### См. также

* class [Font](../../font/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


