---
title: "HtmlSaveOptions.StreamProvider"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Получает или задает IStreamProvider для экспорта объектов"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/streamprovider/
---
## HtmlSaveOptions.StreamProvider property

Получает или задает IStreamProvider для экспорта объектов.

```csharp
public IStreamProvider StreamProvider { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyStreamProviderDemo
    {
        public static void Run()
        {
            // Создать временный каталог для вывода
            string outputDir = Path.Combine(Path.GetTempPath(), "AsposeStreamProviderDemo");
            Directory.CreateDirectory(outputDir);

            // Создать пример рабочей книги
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("StreamProvider Demo");

            // Настроить параметры сохранения HTML с пользовательским поставщиком потоков
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.StreamProvider = new ExportStreamProvider(outputDir);

            // Сохраните книгу в формате HTML
            string outputPath = Path.Combine(outputDir, "output.html");
            workbook.Save(outputPath, options);

            Console.WriteLine($"File saved with StreamProvider to: {outputPath}");
        }
    }

    public class ExportStreamProvider : IStreamProvider
    {
        private readonly string _outputDirectory;

        public ExportStreamProvider(string outputDirectory)
        {
            _outputDirectory = outputDirectory;
        }

        public void InitStream(StreamProviderOptions options)
        {
            // Инициализация при необходимости
        }

        public Stream GetStream(StreamProviderOptions options)
        {
            string filePath = Path.Combine(_outputDirectory, options.CustomPath);
            return new FileStream(filePath, FileMode.Create);
        }

        public void CloseStream(StreamProviderOptions options)
        {
            // Реализация в соответствии с требованиями интерфейса
        }
    }
}
```

### См. также

* interface [IStreamProvider](../../istreamprovider/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


