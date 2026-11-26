---
title: "StreamProviderOptions.CustomPath"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство StreamProviderOptions. Пользовательский путь URL, сохраняемый в сгенерированном html‑файле для указанного источника. Если пользователь не задаёт его, будет использован DefaultPath. Например, данные листа будут сохранены пользователем в d/sheet001.htm, и URL, используемый в основном html‑файле, должен быть d/sheet001.htm или другой допустимый относительный путь, доступный из основного html‑файла."
type: docs
url: /ru/net/aspose.cells/streamprovideroptions/custompath/
---
## StreamProviderOptions.CustomPath property

Пользовательский путь (URL), сохранённый в сгенерированном HTML-файле для ссылочного источника. Если пользователь не задаёт его, будет использован DefaultPath. Например, данные листа будут сохранены пользователем в d:/sheet001.htm, URL, используемый в основном HTML-файле, должен быть "d:/sheet001.htm" или иной допустимый относительный путь, доступный из основного HTML-файла.

```csharp
public string CustomPath { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StreamProviderOptionsPropertyCustomPathDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Data");

            // Настройте параметры сохранения HTML с пользовательским поставщиком потоков
            string outputDir = "output";
            Directory.CreateDirectory(outputDir);
            
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportActiveWorksheetOnly = true;
            
            // Создать пользовательский провайдер потоков с CustomPath
            HtmlWithExternalResourcesProvider streamProvider = new HtmlWithExternalResourcesProvider(outputDir);
            streamProvider.streamProviderOptions.CustomPath = "resources";
            options.StreamProvider = streamProvider;

            // Сохраните книгу
            string outputFile = Path.Combine(outputDir, "output.html");
            workbook.Save(outputFile, options);

            // Проверьте, что пользовательский путь был использован
            string resourcePath = Path.Combine(outputDir, streamProvider.streamProviderOptions.CustomPath);
            Console.WriteLine($"Resources should be saved to: {resourcePath}");
        }
    }

    // Упрощённая реализация пользовательского провайдера потоков
    public class HtmlWithExternalResourcesProvider : IStreamProvider
    {
        public StreamProviderOptions streamProviderOptions = new StreamProviderOptions();
        public string _outputDirectory;

        public HtmlWithExternalResourcesProvider(string outputDirectory)
        {
            _outputDirectory = outputDirectory;
        }

        public void InitStream(StreamProviderOptions options)
        {
            // Реализация будет здесь
        }

        public void CloseStream(StreamProviderOptions options)
        {
            // Реализация будет здесь
        }
    }
}
```

### См. также

* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


