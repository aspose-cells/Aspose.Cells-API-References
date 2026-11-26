---
title: "StreamProviderOptions.Stream"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство StreamProviderOptions. Получает/устанавливает поток"
type: docs
url: /ru/net/aspose.cells/streamprovideroptions/stream/
---
## StreamProviderOptions.Stream property

Получает/задаёт поток

```csharp
public Stream Stream { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StreamProviderOptionsPropertyStreamDemo
    {
        public static void Run()
        {
            // Создать экземпляр StreamProviderOptions
            StreamProviderOptions options = new StreamProviderOptions();
            
            // Случай 1: Когда путь по умолчанию не установлен — использовать MemoryStream
            options.Stream = new MemoryStream();
            Console.WriteLine("Using MemoryStream: " + (options.Stream is MemoryStream));

            // Случай 2: Смоделировать наличие пути по умолчанию — использовать FileStream
            string outputDir = "output/";
            string defaultPath = "testfile.txt"; // Store path separately since DefaultPath is read-only
            string path = outputDir + Path.GetFileName(defaultPath);
            Directory.CreateDirectory(Path.GetDirectoryName(path));
            options.Stream = File.Create(path);
            Console.WriteLine("Using FileStream: " + (options.Stream is FileStream));
            
            // Очистить
            options.Stream.Dispose();
            if (File.Exists(path))
            {
                File.Delete(path);
            }
        }
    }
}
```

### См. также

* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


