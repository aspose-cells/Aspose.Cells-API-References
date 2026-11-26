---
title: "Интерфейс IStreamProvider"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.IStreamProvider интерфейс. Представляет поставщика экспортируемого потока"
type: docs
url: /ru/net/aspose.cells/istreamprovider/
---
## IStreamProvider interface

Представляет поставщик экспортируемого потока.

```csharp
public interface IStreamProvider
```

## Методы

| Имя | Описание |
| --- | --- |
| [CloseStream](../../aspose.cells/istreamprovider/closestream/)(StreamProviderOptions) | Закрывает поток. |
| [InitStream](../../aspose.cells/istreamprovider/initstream/)(StreamProviderOptions) | Получает поток. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class IStreamProviderDemo : IStreamProvider
    {
        // Реализация метода InitStream
        public void InitStream(StreamProviderOptions options)
        {
            string outputDir = "/test/";
            string path = outputDir + Path.GetFileName(options.DefaultPath);
            options.CustomPath = path;
            Directory.CreateDirectory(Path.GetDirectoryName(path));
            options.Stream = File.Create(path);
        }

        // Реализация метода CloseStream
        public void CloseStream(StreamProviderOptions options)
        {
            // Закройте поток, если он не null
            if (options.Stream != null)
            {
                options.Stream.Close();
            }
        }

        public static void IStreamProviderExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установите некоторые данные в листе
            worksheet.Cells["A1"].PutValue("Hello World");

            // Создайте HtmlSaveOptions и установите StreamProvider
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.StreamProvider = new IStreamProviderDemo();

            // Сохраните книгу в формате HTML
            workbook.Save("IStreamProviderExample.html", saveOptions);

            // Загрузите книгу из формата HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.StreamProvider = new IStreamProviderDemo();
            Workbook loadedWorkbook = new Workbook("IStreamProviderExample.html", loadOptions);

            // Отобразите загруженные данные
            Console.WriteLine(loadedWorkbook.Worksheets[0].Cells["A1"].StringValue);
        }
    }

}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


