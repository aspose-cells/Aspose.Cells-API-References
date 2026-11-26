---
title: "HtmlSaveOptions.IsExpImageToTempDir"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, экспортировать ли файлы изображений во временный каталог. Только при сохранении в поток html"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/isexpimagetotempdir/
---
## HtmlSaveOptions.IsExpImageToTempDir property

Указывает, экспортировать ли файлы изображений во временный каталог. Только при сохранении в поток HTML.

```csharp
public bool IsExpImageToTempDir { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsExpImageToTempDirDemo
    {
        public static void Run()
        {
            // Создать пример рабочей книги с изображением
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить пример изображения в лист
            worksheet.Pictures.Add(0, 0, "https://www.aspose.com/templates/aspose/App_Themes/V3/images/cells/header/aspose_cells-for-net.png");

            // Установить параметры сохранения HTML с включённым IsExpImageToTempDir
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.IsExpImageToTempDir = true;
            options.ExportImagesAsBase64 = false; // Ensure images are exported as separate files

            // Сохраните книгу в формате HTML
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML saved with images exported to temp directory.");
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


