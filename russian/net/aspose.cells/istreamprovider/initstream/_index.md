---
title: "IStreamProvider.InitStream"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод IStreamProvider. Получает поток"
type: docs
url: /ru/net/aspose.cells/istreamprovider/initstream/
---
## IStreamProvider.InitStream method

Получает поток.

```csharp
public void InitStream(StreamProviderOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| опции | StreamProviderOptions |  |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class IStreamProviderMethodInitStreamWithStreamProviderOptionsDemo : IStreamProvider
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создать экземпляр демонстрационного класса, реализующего IStreamProvider
            var streamProvider = new IStreamProviderMethodInitStreamWithStreamProviderOptionsDemo();
            
            // Подготовьте StreamProviderOptions
            StreamProviderOptions options = new StreamProviderOptions
            {
                ResourceLoadingType = ResourceLoadingType.Default,
                CustomPath = "custom_path",
                Stream = new MemoryStream()
            };

            try
            {
                // Вызовите метод InitStream с параметром StreamProviderOptions
                streamProvider.InitStream(options);
                
                Console.WriteLine("InitStream method executed successfully with StreamProviderOptions parameter");
                
                // Продемонстрировать эффект — в этом случае мы просто показываем, что поток инициализирован
                Console.WriteLine($"Stream initialized: {options.Stream != null}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InitStream method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("MethodInitStreamWithStreamProviderOptionsDemo.xlsx");
        }

        public void InitStream(StreamProviderOptions options)
        {
            // Реализация InitStream
            Console.WriteLine($"Initializing stream with ResourceLoadingType: {options.ResourceLoadingType}");
        }

        public void CloseStream(StreamProviderOptions options)
        {
            // Реализация CloseStream
            if (options.Stream != null)
            {
                options.Stream.Close();
            }
        }
    }
}
```

### См. также

* class [StreamProviderOptions](../../streamprovideroptions/)
* interface [IStreamProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


