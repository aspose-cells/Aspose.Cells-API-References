---
title: "MarkdownSaveOptions.ExportImagesAsBase64"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MarkdownSaveOptions. Указывает, сохраняются ли изображения в формате Base64 в Markdown. Значение по умолчанию — true"
type: docs
url: /ru/net/aspose.cells/markdownsaveoptions/exportimagesasbase64/
---
## MarkdownSaveOptions.ExportImagesAsBase64 property

Указывает, сохраняются ли изображения в формате Base64 в Markdown. Значение по умолчанию — true.

```csharp
public bool ExportImagesAsBase64 { get; set; }
```

### Примечания

Когда это свойство установлено в true, данные изображения экспортируются непосредственно в элементы img, и отдельные файлы не создаются.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyExportImagesAsBase64Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте пример данных и изображение
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue("With Image");

            // Добавить изображение на лист
            int imageIndex = worksheet.Pictures.Add(1, 1, "sample.png");

            try
            {
                // Создайте экземпляр MarkdownSaveOptions
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // Отобразите значение по умолчанию свойства ExportImagesAsBase64
                Console.WriteLine("Default ExportImagesAsBase64 value: " + saveOptions.ExportImagesAsBase64);

                // Установите ExportImagesAsBase64 в false, чтобы продемонстрировать свойство
                saveOptions.ExportImagesAsBase64 = false;
                Console.WriteLine("ExportImagesAsBase64 set to: " + saveOptions.ExportImagesAsBase64);

                // Сохраните с ExportImagesAsBase64 = false
                workbook.Save("MarkdownImagesAsFiles.md", saveOptions);

                // Установите ExportImagesAsBase64 в true
                saveOptions.ExportImagesAsBase64 = true;
                Console.WriteLine("ExportImagesAsBase64 set to: " + saveOptions.ExportImagesAsBase64);

                // Сохраните с ExportImagesAsBase64 = true
                workbook.Save("MarkdownImagesAsBase64.md", saveOptions);

                Console.WriteLine("Markdown files saved with different ExportImagesAsBase64 settings.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


