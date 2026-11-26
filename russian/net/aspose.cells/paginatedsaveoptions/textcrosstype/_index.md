---
title: "PaginatedSaveOptions.TextCrossType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PaginatedSaveOptions. Получает или задает тип отображения текста, когда ширина текста превышает ширину ячейки"
type: docs
url: /ru/net/aspose.cells/paginatedsaveoptions/textcrosstype/
---
## PaginatedSaveOptions.TextCrossType property

Получает или задает тип отображения текста, когда ширина текста превышает ширину ячейки.

```csharp
public TextCrossType TextCrossType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyTextCrossTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите длинный текст, который будет пересекать границы ячеек
            worksheet.Cells["A1"].PutValue("This is a long text that will cross cell boundaries");
            worksheet.Cells["B1"].PutValue("Another cell content");
            
            // Установите ширину столбца, чтобы текст пересекал ячейки
            worksheet.Cells.SetColumnWidth(0, 5);
            
            // Создайте параметры сохранения PDF
            PdfSaveOptions options = new PdfSaveOptions();
            
            // Продемонстрируйте TextCrossType, установив его в значение CrossKeep
            options.TextCrossType = TextCrossType.CrossKeep;
            
            // Сохранить книгу в формате PDF
            workbook.Save("TextCrossTypeDemo.pdf", options);
            
            Console.WriteLine("PDF saved with TextCrossType.CrossKeep setting");
        }
    }
}
```

### См. также

* enum [TextCrossType](../../textcrosstype/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


