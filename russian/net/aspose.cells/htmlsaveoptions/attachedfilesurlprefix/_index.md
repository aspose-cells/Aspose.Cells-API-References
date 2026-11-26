---
title: "HtmlSaveOptions.AttachedFilesUrlPrefix"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Укажите префикс URL вложенных файлов, таких как изображения, в HTML‑файле. Только для сохранения в поток HTML"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/attachedfilesurlprefix/
---
## HtmlSaveOptions.AttachedFilesUrlPrefix property

Укажите префикс URL вложенных файлов, например изображений, в HTML‑файле. Только при сохранении в поток HTML.

```csharp
public string AttachedFilesUrlPrefix { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyAttachedFilesUrlPrefixDemo
    {
        public static void Run()
        {
            // Создать пример рабочей книги
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test HTML Export");

            // Установите параметры сохранения HTML с AttachedFilesUrlPrefix
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            saveOptions.AttachedFilesUrlPrefix = "www.aspose.com";

            // Сохранить рабочую книгу с параметрами HTML
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);

            Console.WriteLine("HTML file saved with AttachedFilesUrlPrefix: " + saveOptions.AttachedFilesUrlPrefix);
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


