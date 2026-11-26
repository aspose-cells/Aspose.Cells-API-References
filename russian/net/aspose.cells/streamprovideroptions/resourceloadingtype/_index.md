---
title: "StreamProviderOptions.ResourceLoadingType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство StreamProviderOptions. Получает и устанавливает тип загружаемого ресурса"
type: docs
url: /ru/net/aspose.cells/streamprovideroptions/resourceloadingtype/
---
## StreamProviderOptions.ResourceLoadingType property

Получает и задает тип загружаемого ресурса.

```csharp
public ResourceLoadingType ResourceLoadingType { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StreamProviderOptionsPropertyResourceLoadingTypeDemo
    {
        public static void Run()
        {
            // Создать рабочую книгу с параметрами StreamProviderOptions
            var options = new StreamProviderOptions
            {
                ResourceLoadingType = ResourceLoadingType.UserProvided
            };

            // Продемонстрировать различные варианты загрузки ресурсов
            if (options.ResourceLoadingType == ResourceLoadingType.UserProvided)
            {
                // Предоставить пользовательский MemoryStream
                options.Stream = new MemoryStream();
                Console.WriteLine("Using user-provided memory stream");
            }
            else if (options.ResourceLoadingType == ResourceLoadingType.Skip)
            {
                // Пропустить загрузку, используя null stream
                options.Stream = Stream.Null;
                Console.WriteLine("Skipping resource loading");
            }
            else
            {
                // Поведение загрузки файлов по умолчанию
                string defaultPath = "default_resource.txt";
                options.Stream = new FileStream(defaultPath, FileMode.Open, FileAccess.Read);
                Console.WriteLine("Loading resource from default path");
            }

            // Очистка
            options.Stream?.Dispose();
        }
    }
}
```

### См. также

* enum [ResourceLoadingType](../../resourceloadingtype/)
* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


