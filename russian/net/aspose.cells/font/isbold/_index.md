---
title: "Font.IsBold"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Font. Получает или задает значение, указывающее, является ли шрифт полужирным"
type: docs
url: /ru/net/aspose.cells/font/isbold/
---
## Font.IsBold property

Получает или задает значение, указывающее, является ли шрифт полужирным.

```csharp
public bool IsBold { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsBoldDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получить доступ к ячейке A1 и установить её значение
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Bold Text Demo");
            
            // Получить стиль ячейки и установить шрифт полужирным
            Style style = cell.GetStyle();
            style.Font.IsBold = true;
            cell.SetStyle(style);
            
            // Сохраните книгу
            workbook.Save("FontIsBoldDemo.xlsx");
            
            // Проверить свойство полужирного начертания
            Workbook loadedWorkbook = new Workbook("FontIsBoldDemo.xlsx");
            Style loadedStyle = loadedWorkbook.Worksheets[0].Cells["A1"].GetStyle();
            Console.WriteLine("IsBold property: " + loadedStyle.Font.IsBold);
        }
    }
}
```

### См. также

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


