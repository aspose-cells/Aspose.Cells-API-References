---
title: "StreamProviderOptions.DefaultPath"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство StreamProviderOptions. URL пути по умолчанию, сохраняемый в сгенерированном html‑файле для указанного источника. Например, данные листа сохраняются в xxx_files/sheet001.htm, URL, используемый в основном html‑файле, должен выглядеть как srcxxx_files/sheet001.htm"
type: docs
url: /ru/net/aspose.cells/streamprovideroptions/defaultpath/
---
## StreamProviderOptions.DefaultPath property

Путь по умолчанию (URL), сохраненный в сгенерированном html‑файле для указанного источника. Например, данные листа, сохранённые в xxx_files/sheet001.htm, URL, используемый в основном html‑файле, должен выглядеть так \"src=\"xxx_files/sheet001.htm\"\"

```csharp
public string DefaultPath { get; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StreamProviderOptionsPropertyDefaultPathDemo
    {
        public static void Run()
        {
            // Создайте новую книгу
            Workbook workbook = new Workbook();
            
            // Создать StreamProviderOptions с ResourceLoadingType и DefaultPath
            StreamProviderOptions options = new StreamProviderOptions(ResourceLoadingType.Default, "1.DefaultPathExample");
            
            // Продемонстрировать использование DefaultPath
            Console.WriteLine("StreamProviderOptions DefaultPath: " + options.DefaultPath);
            
            // Пример использования параметров с потоком (упрощённая демонстрация)
            using (MemoryStream stream = new MemoryStream())
            {
                options.Stream = stream;
                
                if (options.DefaultPath.IndexOf("1.") >= 0)
                {
                    Console.WriteLine("Processing stream for path: " + options.DefaultPath);
                    // Выполнять операции с потоком
                    workbook.Save(stream, SaveFormat.Xlsx);
                }
            }
        }
    }
}
```

### См. также

* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


