---
title: "Cell.ContainsExternalLink"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cell. Указывает, содержит ли эта ячейка внешнюю ссылку. Применяется только, когда ячейка является ячейкой с формулой"
type: docs
url: /ru/net/aspose.cells/cell/containsexternallink/
---
## Cell.ContainsExternalLink property

Указывает, содержит ли эта ячейка внешнюю ссылку. Применяется только к ячейкам с формулой.

```csharp
public bool ContainsExternalLink { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyContainsExternalLinkDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавьте пример данных и внешнюю ссылку
            sheet.Cells["A1"].PutValue("External Link:");
            sheet.Cells["B1"].Formula = "=HYPERLINK(\"https://www.aspose.com\", \"Aspose\")";
            
            // Проверьте, содержат ли ячейки внешние ссылки
            Console.WriteLine("A1 ContainsExternalLink: " + sheet.Cells["A1"].ContainsExternalLink);
            Console.WriteLine("B1 ContainsExternalLink: " + sheet.Cells["B1"].ContainsExternalLink);
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


