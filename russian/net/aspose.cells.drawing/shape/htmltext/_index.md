---
title: "Shape.HtmlText"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает и задаёт HTML-строку, которая содержит данные и некоторые форматы в этом текстовом поле"
type: docs
url: /ru/net/aspose.cells.drawing/shape/htmltext/
---
## Shape.HtmlText property

Получает и задает HTML-строку, содержащую данные и некоторые форматы в этом текстовом поле.

```csharp
public string HtmlText { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHtmlTextDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму на лист
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // Проверьте, пустой ли HtmlText, и установите его при необходимости
            string html = shape.HtmlText;
            if (string.IsNullOrEmpty(html))
            {
                shape.HtmlText = "<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>";
            }

            // Сохраните книгу
            workbook.Save("ShapeHtmlTextDemo.xlsx");
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


