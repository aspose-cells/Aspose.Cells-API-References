---
title: "HtmlSaveOptions.ExportImagesAsBase64"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, сохраняются ли изображения в формате Base64 в HTML, MHTML или EPUB"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/exportimagesasbase64/
---
## HtmlSaveOptions.ExportImagesAsBase64 property

Указывает, сохраняются ли изображения в формате Base64 в HTML, MHTML или EPUB.

```csharp
public bool ExportImagesAsBase64 { get; set; }
```

### Примечания

Когда это свойство установлено в true, данные изображения экспортируются непосредственно в элементы img, и отдельные файлы не создаются.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportImagesAsBase64Demo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить изображение на лист
            worksheet.Pictures.Add(0, 0, "example.jpg");
            
            // Создать параметры сохранения HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Установите ExportImagesAsBase64 в true, чтобы внедрить изображения как строки base64
            saveOptions.ExportImagesAsBase64 = true;
            
            // Сохраните книгу в формате HTML с внедрёнными изображениями
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML with embedded images saved successfully.");
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


