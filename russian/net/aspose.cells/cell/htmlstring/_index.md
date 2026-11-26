---
title: "Cell.HtmlString"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cell. Получает и задает html-строку, содержащую данные и некоторые форматы в этой ячейке."
type: docs
url: /ru/net/aspose.cells/cell/htmlstring/
---
## Cell.HtmlString property

Получает и задает HTML-строку, содержащую данные и некоторые форматы в этой ячейке.

```csharp
public string HtmlString { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyHtmlStringDemo
    {
        public static void Run()
        {
            // Создать экземпляр рабочей книги
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Доступ к коллекции cells
            Cells cells = worksheet.Cells;
            
            // Установите HTML-строку с форматированием в ячейку A1
            cells["A1"].HtmlString = "This is <b>bold</b> and <i>italic</i> text<br>with a line break";
            
            // Сохраните книгу
            workbook.Save("HtmlStringDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


