---
title: "Style.VerticalAlignment"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Style. Получает или задает тип вертикального выравнивания текста в ячейке"
type: docs
url: /ru/net/aspose.cells/style/verticalalignment/
---
## Style.VerticalAlignment property

Получает или задает тип вертикального выравнивания текста в ячейке.

```csharp
public TextAlignmentType VerticalAlignment { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyVerticalAlignmentDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Обратиться к ячейке A1
            Cell cell = worksheet.Cells["A1"];
            
            // Установить значение ячейки
            cell.PutValue("Vertical Alignment Demo");
            
            // Получить доступ к стилю ячейки
            Style style = cell.GetStyle();
            
            // Установить вертикальное выравнивание в Top
            style.VerticalAlignment = TextAlignmentType.Top;
            cell.SetStyle(style);
            
            // Сохраните книгу
            workbook.Save("VerticalAlignmentDemo.xlsx");
            
            Console.WriteLine("Vertical alignment set to Top for cell A1.");
        }
    }
}
```

### См. также

* enum [TextAlignmentType](../../textalignmenttype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


