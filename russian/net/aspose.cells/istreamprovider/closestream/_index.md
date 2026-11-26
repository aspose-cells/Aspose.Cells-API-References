---
title: "IStreamProvider.CloseStream"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод IStreamProvider. Закрывает поток"
type: docs
url: /ru/net/aspose.cells/istreamprovider/closestream/
---
## IStreamProvider.CloseStream method

Закрывает поток.

```csharp
public void CloseStream(StreamProviderOptions options)
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

    public class IStreamProviderMethodCloseStreamWithStreamProviderOptionsDemo : IStreamProvider
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создать экземпляр демонстрационного класса, реализующего IStreamProvider
            var streamProvider = new IStreamProviderMethodCloseStreamWithStreamProviderOptionsDemo();
            
            // Создать StreamProviderOptions
            var options = new StreamProviderOptions
            {
                ResourceLoadingType = ResourceLoadingType.Default,
                CustomPath = "output_files/sheet001.htm",
                Stream = new MemoryStream()
            };

            try
            {
                // Вызовите метод CloseStream
                streamProvider.CloseStream(options);
                
                Console.WriteLine("CloseStream method executed successfully with StreamProviderOptions");
                
                // Продемонстрировать эффект — в реальном сценарии это закроет поток
                Console.WriteLine($"Stream closed status: {options.Stream == null}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing CloseStream method: {ex.Message}");
            }
            
            // Сохраните книгу
            workbook.Save("IStreamProviderCloseStreamDemo.xlsx");
        }

        public void InitStream(StreamProviderOptions options)
        {
            // Реализация, требуемая интерфейсом
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

* class [StreamProviderOptions](../../streamprovideroptions/)
* interface [IStreamProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


