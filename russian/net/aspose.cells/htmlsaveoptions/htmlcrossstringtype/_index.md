---
title: "HtmlSaveOptions.HtmlCrossStringType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, будет ли строка, охватывающая несколько ячеек, отображаться так же, как в MS Excel при сохранении файла Excel в формате html. По умолчанию значение — Default, поэтому для строк, охватывающих несколько ячеек, разница между html‑файлами, созданными Aspose.Cells и MS Excel, небольшая. Однако производительность при создании больших html‑файлов при установке значения в Cross будет в несколько раз выше, чем при установке его в Default или Fit2Cell."
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/htmlcrossstringtype/
---
## HtmlSaveOptions.HtmlCrossStringType property

Указывает, будет ли строка, охватывающая несколько ячеек, отображаться так же, как в MS Excel при сохранении файла Excel в формате HTML. По умолчанию значение — Default, поэтому для таких строк разница между HTML‑файлами, созданными Aspose.Cells и MS Excel, небольшая. Однако при создании больших HTML‑файлов установка значения Cross повышает производительность в несколько раз по сравнению с Default или Fit2Cell.

```csharp
public HtmlCrossType HtmlCrossStringType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyHtmlCrossStringTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные, демонстрирующие поведение строк, охватывающих несколько ячеек
            worksheet.Cells["A1"].PutValue("Left Content");
            worksheet.Cells["B1"].PutValue("Right Content");
            
            // Получить и изменить стили ячеек
            Style styleA1 = worksheet.Cells["A1"].GetStyle();
            styleA1.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            worksheet.Cells["A1"].SetStyle(styleA1);
            
            Style styleB1 = worksheet.Cells["B1"].GetStyle();
            styleB1.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            worksheet.Cells["B1"].SetStyle(styleB1);

            // Настроить параметры сохранения HTML
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.HtmlCrossStringType = HtmlCrossType.CrossHideRight;

            // Сохраните книгу в HTML
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML file saved with CrossHideRight option.");
        }
    }
}
```

### См. также

* enum [HtmlCrossType](../../htmlcrosstype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


