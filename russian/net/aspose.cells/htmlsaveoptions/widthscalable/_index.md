---
title: "HtmlSaveOptions.WidthScalable"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, экспортировать ли ширину столбца в единицах масштаба в HTML. Значение по умолчанию — false"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/widthscalable/
---
## HtmlSaveOptions.WidthScalable property

Указывает, экспортировать ли ширину столбца в единицах масштаба в HTML. Значение по умолчанию — false.

```csharp
public bool WidthScalable { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyWidthScalableDemo
    {
        public static void Run()
        {
            // Создать пример рабочей книги с тестовыми данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test WidthScalable Property");
            worksheet.Cells["B1"].PutValue(123.45);
            
            // Установите параметры сохранения HTML со свойством WidthScalable
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.WidthScalable = true; // Demonstrate setting to true
            
            // Сохранить с масштабируемой шириной
            workbook.Save("output_scalable.html", options);
            
            // Сохранить снова с фиксированной шириной
            options.WidthScalable = false;
            workbook.Save("output_fixed.html", options);
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


