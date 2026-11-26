---
title: "Workbook.DefaultStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Workbook. Получает или задает объект Style по умолчанию книги"
type: docs
url: /ru/net/aspose.cells/workbook/defaultstyle/
---
## Workbook.DefaultStyle property

Получает или задает объект по умолчанию [`Style`](../../style/) workbook.

```csharp
public Style DefaultStyle { get; set; }
```

### Примечания

Свойство DefaultStyle полезно для реализации стиля для всей книги Workbook.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyDefaultStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Получить стиль по умолчанию и изменить его шрифт
            Style defaultStyle = workbook.DefaultStyle;
            defaultStyle.Font.Name = "Tahoma";
            defaultStyle.Font.Size = 12;
            
            // Применить измененный стиль обратно как стиль по умолчанию
            workbook.DefaultStyle = defaultStyle;
            
            // Создать лист и добавить текст со стилем по умолчанию
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This text uses the default Tahoma font");
            
            // Сохраните книгу
            workbook.Save("DefaultStyleDemo.xlsx");
        }
    }
}
```

### См. также

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


