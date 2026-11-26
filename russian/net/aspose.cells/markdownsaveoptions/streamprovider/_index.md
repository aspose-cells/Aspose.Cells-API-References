---
title: "MarkdownSaveOptions.StreamProvider"
second_title: "Справочник API Aspose.Cells для .NET"
description: "MarkdownSaveOptions свойство. Получает или задает IStreamProvider для экспорта объектов. Если null, экспортированные объекты будут сохранены в той же директории, что и выходной файл"
type: docs
url: /ru/net/aspose.cells/markdownsaveoptions/streamprovider/
---
## MarkdownSaveOptions.StreamProvider property

Получает или задает IStreamProvider для экспорта объектов. Если `null`, экспортированные объекты будут сохранены в той же директории, что и выходной файл.

```csharp
public IStreamProvider StreamProvider { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class MarkdownSaveOptionsPropertyStreamProviderDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].Value = "Hello";
            worksheet.Cells["B1"].Value = "World";

            try
            {
                // Создайте экземпляр MarkdownSaveOptions
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // Отобразите текущее значение StreamProvider (null по умолчанию)
                Console.WriteLine("Current StreamProvider: " + (saveOptions.StreamProvider == null ? "null" : "set"));

                // Создайте пользовательскую реализацию StreamProvider
                CustomStreamProvider streamProvider = new CustomStreamProvider();
                saveOptions.StreamProvider = streamProvider;

                // Отобразите обновлённое значение StreamProvider
                Console.WriteLine("Updated StreamProvider: " + (saveOptions.StreamProvider != null ? "set" : "null"));

                // Сохраните книгу с пользовательским StreamProvider
                workbook.Save("StreamProviderDemo.md", saveOptions);

                Console.WriteLine("Markdown file saved with custom StreamProvider.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    // Пользовательская реализация IStreamProvider
    public class CustomStreamProvider : IStreamProvider
    {
        public void InitStream(StreamProviderOptions options)
        {
            Console.WriteLine("Initializing stream");
        }

        public void CloseStream(StreamProviderOptions options)
        {
            Console.WriteLine("Closing stream");
        }
    }
}
```

### См. также

* interface [IStreamProvider](../../istreamprovider/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


