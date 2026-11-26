---
title: "Style.IsGradient"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Style. Указывает, является ли затенение ячейки градиентным шаблоном"
type: docs
url: /ru/net/aspose.cells/style/isgradient/
---
## Style.IsGradient property

Указывает, является ли затенение ячейки градиентным шаблоном.

```csharp
public bool IsGradient { get; set; }
```

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyIsGradientDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать стиль
            Style style = workbook.CreateStyle();
            
            // Установить градиентный фон
            style.SetTwoColorGradient(Color.LightBlue, Color.DarkBlue, GradientStyleType.Horizontal, 1);
            
            // Применить стиль к ячейке
            worksheet.Cells["A1"].SetStyle(style);
            
            // Проверьте, есть ли градиент у стиля
            bool isGradient = worksheet.Cells["A1"].GetStyle().IsGradient;
            
            // Вывести результат.
            Console.WriteLine("Cell A1 style has gradient: " + isGradient);
            
            // Сохраните книгу
            workbook.Save("GradientStyleDemo.xlsx");
        }
    }
}
```

### См. также

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


