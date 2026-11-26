---
title: "HtmlSaveOptions.IgnoreInvisibleShapes"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, экспортировать ли невидимые формы"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/ignoreinvisibleshapes/
---
## HtmlSaveOptions.IgnoreInvisibleShapes property

Указывает, экспортировать ли невидимые фигуры

```csharp
public bool IgnoreInvisibleShapes { get; set; }
```

### Примечания

Значение по умолчанию — false.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIgnoreInvisibleShapesDemo
    {
        public static void Run()
        {
            // Создать рабочую книгу с примерным листом
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить видимые и невидимые формы
            Shape shape1 = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 50, 50);
            shape1.IsHidden = false;
            Shape shape2 = worksheet.Shapes.AddRectangle(1, 0, 100, 100, 50, 50);
            shape2.IsHidden = true;

            // Сохранить с IgnoreInvisibleShapes = true (по умолчанию)
            HtmlSaveOptions saveOptions1 = new HtmlSaveOptions();
            saveOptions1.IgnoreInvisibleShapes = true;
            workbook.Save("output_ignore_invisible.html", saveOptions1);

            // Сохранить с IgnoreInvisibleShapes = false
            HtmlSaveOptions saveOptions2 = new HtmlSaveOptions();
            saveOptions2.IgnoreInvisibleShapes = false;
            workbook.Save("output_include_invisible.html", saveOptions2);

            Console.WriteLine("HTML files saved with different IgnoreInvisibleShapes settings.");
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


