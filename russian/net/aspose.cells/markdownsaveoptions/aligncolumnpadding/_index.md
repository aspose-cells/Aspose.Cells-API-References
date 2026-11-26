---
title: "MarkdownSaveOptions.AlignColumnPadding"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MarkdownSaveOptions. Указывает, включено ли выравнивание столбцов для генерируемых таблиц Markdown. Когда включено, столбцы выравниваются путем заполнения содержимого ячеек указанным символом, обычно пробелом. Установите 0, чтобы отключить выравнивание столбцов по умолчанию."
type: docs
url: /ru/net/aspose.cells/markdownsaveoptions/aligncolumnpadding/
---
## MarkdownSaveOptions.AlignColumnPadding property

Указывает, включено ли выравнивание столбцов для сгенерированных таблиц Markdown. При включении столбцы выравниваются путем заполнения содержимого ячеек указанным символом (обычно ' ' для пробелов). Установите "\\0", чтобы отключить выравнивание столбцов (по умолчанию).

```csharp
public char AlignColumnPadding { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyAlignColumnPaddingDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные, чтобы продемонстрировать выравнивание столбцов.
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["C1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = "1.99";
            worksheet.Cells["C2"].Value = "10";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["B3"].Value = "0.99";
            worksheet.Cells["C3"].Value = "20";

            // Создайте экземпляр MarkdownSaveOptions
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

            try
            {
                // Отобразите значение AlignColumnPadding по умолчанию.
                Console.WriteLine("Default AlignColumnPadding value: '" +
                    saveOptions.AlignColumnPadding + "'");

                // Установите AlignColumnPadding в символ пробела для выравнивания столбцов.
                saveOptions.AlignColumnPadding = ' ';

                // Отобразить обновлённое значение
                Console.WriteLine("Updated AlignColumnPadding value: '" +
                    saveOptions.AlignColumnPadding + "'");

                // Сохраните книгу в формате markdown с выравниванием столбцов.
                workbook.Save("AlignColumnPaddingDemo.md", saveOptions);
                Console.WriteLine("Markdown file saved with column alignment enabled.");
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


