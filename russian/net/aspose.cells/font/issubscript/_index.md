---
title: "Font.IsSubscript"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Font. Получает или задает значение, указывающее, является ли шрифт нижним индексом"
type: docs
url: /ru/net/aspose.cells/font/issubscript/
---
## Font.IsSubscript property

Получает или задает значение, указывающее, является ли шрифт нижним индексом.

```csharp
public bool IsSubscript { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsSubscriptDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте стиль с текстом в нижнем индексе
            Style subscriptStyle = workbook.CreateStyle();
            subscriptStyle.Font.IsSubscript = true;

            // Создайте стиль с текстом в верхнем индексе для сравнения
            Style superscriptStyle = workbook.CreateStyle();
            superscriptStyle.Font.IsSuperscript = true;

            // Применить стили к ячейкам
            worksheet.Cells["A1"].PutValue("Subscript Text");
            worksheet.Cells["A1"].SetStyle(subscriptStyle);

            worksheet.Cells["A2"].PutValue("Superscript Text");
            worksheet.Cells["A2"].SetStyle(superscriptStyle);

            // Проверьте и отобразите стили
            Console.WriteLine("A1 IsSubscript: " + worksheet.Cells["A1"].GetStyle().Font.IsSubscript);
            Console.WriteLine("A1 IsSuperscript: " + worksheet.Cells["A1"].GetStyle().Font.IsSuperscript);
            Console.WriteLine("A2 IsSubscript: " + worksheet.Cells["A2"].GetStyle().Font.IsSubscript);
            Console.WriteLine("A2 IsSuperscript: " + worksheet.Cells["A2"].GetStyle().Font.IsSuperscript);

            // Сохраните книгу
            workbook.Save("FontPropertyIsSubscriptDemo.ods");
        }
    }
}
```

### См. также

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


