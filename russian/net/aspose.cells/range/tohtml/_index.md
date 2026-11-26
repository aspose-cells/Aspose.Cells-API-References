---
title: "Range.ToHtml"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Range. Преобразовать диапазон в html"
type: docs
url: /ru/net/aspose.cells/range/tohtml/
---
## Range.ToHtml method

Преобразовать диапазон в html .

```csharp
public byte[] ToHtml(HtmlSaveOptions saveOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| saveOptions | HtmlSaveOptions | Параметры для преобразования диапазона в html. |

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodToHtmlWithHtmlSaveOptionsDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Заполнить некоторыми данными диапазон A1:J25
            for (int i = 0; i < 25; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].Value = $"Cell {i+1},{j+1}";
                }
            }

            // Создать диапазон с полностью квалифицированным именем типа
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:J25");
            
            // Создать параметры сохранения HTML
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportImagesAsBase64 = true;
            
            // Преобразовать диапазон в HTML
            byte[] htmlData = range.ToHtml(options);
            
            // Сохранить HTML в файл
            File.WriteAllBytes("output.html", htmlData);
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../../htmlsaveoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


