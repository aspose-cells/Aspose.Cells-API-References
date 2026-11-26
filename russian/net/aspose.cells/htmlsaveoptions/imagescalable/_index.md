---
title: "HtmlSaveOptions.ImageScalable"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, использовать ли масштабируемую единицу для описания ширины изображения при использовании масштабируемой единицы для описания ширины столбца. Значение по умолчанию — true"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/imagescalable/
---
## HtmlSaveOptions.ImageScalable property

Указывает, использовать ли масштабируемую единицу для описания ширины изображения при использовании масштабируемой единицы для описания ширины столбца. Значение по умолчанию — true.

```csharp
public bool ImageScalable { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyImageScalableDemo
    {
        public static void Run()
        {
            // Создать пример рабочей книги с изображением
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить пример изображения в лист
            int imgIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[imgIndex];

            // Установите параметры сохранения HTML с свойством ImageScalable
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ImageScalable = false; // Images won't scale with the HTML content
            
            // Сохраните книгу в формате HTML
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML file saved with ImageScalable set to false.");
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


