---
title: "StreamProviderOptions.StreamProviderOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор StreamProviderOptions. Инициализирует новый экземпляр класса StreamProviderOptions"
type: docs
url: /ru/net/aspose.cells/streamprovideroptions/streamprovideroptions/
---
## StreamProviderOptions(ResourceLoadingType, string) {#constructor_1}

Инициализирует новый экземпляр класса [`StreamProviderOptions`](../).

```csharp
public StreamProviderOptions(ResourceLoadingType loadingType, string defaultPath)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| loadingType | ResourceLoadingType | Тип для загрузки связанного ресурса. |
| defaultPath | String | Путь по умолчанию. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Microsoft.VisualBasic;
    using System;

    public class StreamProviderOptionsMethodCtorWithResourceLoadingTypeStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook("file1.xlsx");
            workbook.Settings.ResourceProvider = new StreamProvider();
            foreach (Shape shape in workbook.Worksheets[0].Shapes)
            {
                shape.ToImage("out.png", null);
            }            
        }
    }

    class StreamProvider : IStreamProvider
    {
        public void InitStream(StreamProviderOptions options)
        {
            options.Stream = File.OpenRead("example.jpg");
            options.ResourceLoadingType = ResourceLoadingType.UserProvided;
        }
        public void CloseStream(StreamProviderOptions options)
        {
            if (options.Stream != null)
            {
                options.Stream.Close();
                options.Stream = null;
            }
        }
    }
}
```

### См. также

* enum [ResourceLoadingType](../../resourceloadingtype/)
* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## StreamProviderOptions() {#constructor}

Инициализирует новый экземпляр класса [`StreamProviderOptions`](../).

```csharp
public StreamProviderOptions()
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class StreamProviderOptionsMethodCtorDemo
    {
        public static void Run()
        {
            try
            {
                // Продемонстрировать конструктор без параметров
                StreamProviderOptions options = new StreamProviderOptions();
                Console.WriteLine("Parameterless constructor:");
                Console.WriteLine($"ResourceLoadingType: {options.ResourceLoadingType}");
                Console.WriteLine($"DefaultPath: {options.DefaultPath}");

                // Создать книгу и сохранить с параметрами потока
                Workbook workbook = new Workbook();
                workbook.Worksheets[0].Cells["A1"].PutValue("StreamProviderOptions Demo");
                
                HtmlSaveOptions saveOptions = new HtmlSaveOptions();
                string outputDir = "custom_path/";
                saveOptions.StreamProvider = new ExportStreamProvider(outputDir);
                
                workbook.Save("StreamProviderOptionsDemo.html", saveOptions);
                Console.WriteLine("\nWorkbook saved with custom stream options");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing StreamProviderOptions constructor demo: {ex.Message}");
            }
        }
    }

    internal class ExportStreamProvider : IStreamProvider
    {
        private string outputDir;

        public ExportStreamProvider(string dir)
        {
            outputDir = dir;
        }

        public void InitStream(StreamProviderOptions options)
        {
            if (options.DefaultPath == null)
            {
                options.Stream = new MemoryStream();
            }
            else
            {
                string path = outputDir + Path.GetFileName(options.DefaultPath);
                options.CustomPath = path;
                Directory.CreateDirectory(Path.GetDirectoryName(path));
                options.Stream = File.Create(path);
            }
        }

        public void CloseStream(StreamProviderOptions options)
        {
            if (options != null && options.Stream != null)
            {
                options.Stream.Close();
            }
        }
    }
}
```

### См. также

* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


