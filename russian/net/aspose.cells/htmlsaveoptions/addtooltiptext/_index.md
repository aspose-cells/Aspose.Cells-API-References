---
title: "HtmlSaveOptions.AddTooltipText"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, добавлять ли подсказку, когда данные не могут быть полностью отображены. Значение по умолчанию — false"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/addtooltiptext/
---
## HtmlSaveOptions.AddTooltipText property

Указывает, добавлять ли подсказку, когда данные не могут быть полностью отображены. Значение по умолчанию: false.

```csharp
public bool AddTooltipText { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyAddTooltipTextDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите длинный текст, который превысит ширину ячейки
            worksheet.Cells["A1"].PutValue("This is a long text that will exceed cell width and need tooltip");
            worksheet.Cells.SetColumnWidth(0, 10); // Set narrow column width
            
            // Настройте параметры сохранения HTML с подсказкой
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            saveOptions.AddTooltipText = true;
            
            // Сохраните книгу
            string outputPath = "output_with_tooltip.html";
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("File saved with tooltips: " + outputPath);
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


