---
title: "Font.Name"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Font. Получает или задает имя шрифта"
type: docs
url: /ru/net/aspose.cells/font/name/
---
## Font.Name property

Получает или задает имя [`Font`](../).

```csharp
public virtual string Name { get; set; }
```

### Примечания

Если это свойство используется для установки имени шрифта, то [`SchemeType`](../schemetype/) будет обновлён до None

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получите доступ к листу по умолчанию и ячейкам
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Создайте и измените стиль с свойствами шрифта
            Style style = workbook.CreateStyle();
            Font font = style.Font;
            
            // Продемонстрировать использование свойства Name
            font.Name = "Arial";  // Changed from FontNameConstants.Arial to string literal
            font.Size = 14;
            font.IsBold = true;
            
            // Применить стиль к ячейке
            cells["A1"].PutValue("Font Property Name Demo");
            cells["A1"].SetStyle(style);
            
            // Сохраните книгу
            workbook.Save("FontPropertyNameDemo.xlsx");
            
            Console.WriteLine("Demo completed. File saved as FontPropertyNameDemo.xlsx");
        }
    }
}
```

### См. также

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


