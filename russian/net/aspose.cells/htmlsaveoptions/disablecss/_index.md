---
title: "HtmlSaveOptions.DisableCss"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, применяются ли только встроенные стили без использования CSS. Значение по умолчанию — false."
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/disablecss/
---
## HtmlSaveOptions.DisableCss property

Указывает, применяются ли только встроенные стили без использования CSS. Значение по умолчанию — false.

```csharp
public bool DisableCss { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlSaveOptionsPropertyDisableCssDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные и форматирование.
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A1"].GetStyle().Font.IsBold = true;
            worksheet.Cells["A1"].GetStyle().Font.Color = System.Drawing.Color.Red;
            worksheet.Cells["B1"].PutValue("Formatted Cell");
            worksheet.Cells["B1"].GetStyle().Font.IsItalic = true;
            worksheet.Cells["B1"].GetStyle().Font.Underline = FontUnderlineType.Single;

            // Создать экземпляр HtmlSaveOptions
            HtmlSaveOptions options = new HtmlSaveOptions();

            // Отобразите текущее значение DisableCss.
            Console.WriteLine("Current DisableCss value: " + options.DisableCss);

            // Установите DisableCss в true (используя встроенные стили вместо CSS).
            options.DisableCss = true;
            workbook.Save("HtmlWithInlineStyles.html", options);

            // Установите DisableCss в false (используя стили CSS).
            options.DisableCss = false;
            workbook.Save("HtmlWithCssStyles.html", options);

            // Сравните выходные файлы, чтобы увидеть разницу в подходе к стилизации.
            Console.WriteLine("Files saved with different DisableCss settings.");
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


