---
title: "Workbook.CountOfStylesInPool"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Workbook. Возвращает количество стилей в пуле стилей"
type: docs
url: /ru/net/aspose.cells/workbook/countofstylesinpool/
---
## Workbook.CountOfStylesInPool property

Получает количество стилей в пуле стилей.

```csharp
public int CountOfStylesInPool { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyCountOfStylesInPoolDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook wb = new Workbook();
            
            // Получить начальное количество стилей в пуле
            int initialStyleCount = wb.CountOfStylesInPool;
            Console.WriteLine($"Initial styles in pool: {initialStyleCount}");

            // Добавить несколько стилей, изменяя ячейки
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Стиль 1
            Style style1 = wb.CreateStyle();
            style1.Font.Name = "Arial";
            style1.Font.Size = 12;
            cells["A1"].SetStyle(style1);
            
            // Стиль 2
            Style style2 = wb.CreateStyle();
            style2.Font.Color = System.Drawing.Color.Red;
            style2.Pattern = BackgroundType.Solid;
            cells["B1"].SetStyle(style2);

            // Получить обновлённое количество стилей
            int updatedStyleCount = wb.CountOfStylesInPool;
            Console.WriteLine($"Styles after modifications: {updatedStyleCount}");

            // Сохранить, чтобы продемонстрировать сохранение стилей
            wb.Save("output.html", SaveFormat.Html);
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


