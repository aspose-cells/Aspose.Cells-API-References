---
title: "MarkdownSaveOptions.OfficeMathOutputType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MarkdownSaveOptions. Указывает, как объекты OfficeMath экспортируются в Markdown. Значение по умолчанию — Image"
type: docs
url: /ru/net/aspose.cells/markdownsaveoptions/officemathoutputtype/
---
## MarkdownSaveOptions.OfficeMathOutputType property

Указывает, как объекты OfficeMath экспортируются в Markdown, значение по умолчанию — Image.

```csharp
public HtmlOfficeMathOutputType OfficeMathOutputType { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyOfficeMathOutputTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте пример данных, включая формулу, которая может содержать OfficeMath
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].Formula = "=SQRT(16)";

            try
            {
                // Создайте параметры сохранения Markdown
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // Отобразите текущее значение OfficeMathOutputType
                Console.WriteLine("Current OfficeMathOutputType: " + saveOptions.OfficeMathOutputType);

                // Установите OfficeMathOutputType в MathML
                saveOptions.OfficeMathOutputType = HtmlOfficeMathOutputType.MathML;
                Console.WriteLine("Changed OfficeMathOutputType to: " + saveOptions.OfficeMathOutputType);

                // Сохраните книгу с типом вывода MathML
                workbook.Save("OfficeMathOutputType_MathML.md", saveOptions);

                // Измените на тип вывода Image
                saveOptions.OfficeMathOutputType = HtmlOfficeMathOutputType.Image;
                Console.WriteLine("Changed OfficeMathOutputType to: " + saveOptions.OfficeMathOutputType);

                // Сохраните книгу с типом вывода Image
                workbook.Save("OfficeMathOutputType_Image.md", saveOptions);

                Console.WriteLine("OfficeMathOutputType demonstration completed successfully.");
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

* enum [HtmlOfficeMathOutputType](../../htmlofficemathoutputtype/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


