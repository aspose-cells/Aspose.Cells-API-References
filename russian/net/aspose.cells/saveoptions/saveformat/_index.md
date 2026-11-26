---
title: "SaveOptions.SaveFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SaveOptions. Получает формат сохраняемого файла"
type: docs
url: /ru/net/aspose.cells/saveoptions/saveformat/
---
## SaveOptions.SaveFormat property

Получает формат сохраняемого файла.

```csharp
public SaveFormat SaveFormat { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertySaveFormatDemo
    {
        public static void Run()
        {
            // Создать пример рабочей книги
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");

            // Продемонстрируйте различные форматы сохранения
            SaveOptions[] options = {
                new PdfSaveOptions(),
                new OoxmlSaveOptions(),
                new HtmlSaveOptions()
            };

            foreach (var saveOptions in options)
            {
                string extension = FileFormatUtil.SaveFormatToExtension(saveOptions.SaveFormat);
                Console.WriteLine($"Saving as {saveOptions.SaveFormat} with extension: {extension}");

                string outputPath = $"output_{Guid.NewGuid().ToString("N").Substring(0, 8)}{extension}";
                workbook.Save(outputPath, saveOptions);
                Console.WriteLine($"Saved to: {outputPath}");
            }

            // Очистить
            workbook.Dispose();
        }
    }
}
```

### См. также

* enum [SaveFormat](../../saveformat/)
* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


