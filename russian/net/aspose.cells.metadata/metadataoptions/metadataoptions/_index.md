---
title: "MetadataOptions.MetadataOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор MetadataOptions. Создаёт параметры загрузки метаданных"
type: docs
url: /ru/net/aspose.cells.metadata/metadataoptions/metadataoptions/
---
## MetadataOptions constructor

Создаёт параметры загрузки метаданных.

```csharp
public MetadataOptions(MetadataType metadataType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| metadataType | MetadataType | Тип метаданных. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metadata;
    using System;

    public class MetadataOptionsMethodCtorWithMetadataTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Вызвать метод #ctor с параметром MetadataType
                MetadataOptions options = new MetadataOptions(MetadataType.Encryption);
                
                // Установить дополнительные свойства
                options.Password = "test123";
                options.KeyLength = 128;
                
                // Отобразить созданные параметры
                Console.WriteLine($"MetadataType: {options.MetadataType}");
                Console.WriteLine($"Password set: {!string.IsNullOrEmpty(options.Password)}");
                Console.WriteLine($"KeyLength: {options.KeyLength}");

                // Использовать параметры при загрузке метаданных (пример)
                // Обычно это используется с LoadOptions при открытии файла
                // Примечание: В исходном коде пытались установить MetadataOptions напрямую в LoadOptions,
                // но класс LoadOptions не имеет этого свойства в предоставленном определении.
                // Мы также оставим часть создания параметров, поскольку использование с LoadOptions
                // нельзя выполнить с текущим определением API.
                
                Console.WriteLine("MetadataOptions created successfully with MetadataType parameter");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating MetadataOptions: {ex.Message}");
            }
            
            // Сохраните книгу (хотя параметры метаданных не повлияют на эту пустую книгу)
            workbook.Save("MetadataOptionsCtorDemo.xlsx");
        }
    }
}
```

### См. также

* enum [MetadataType](../../metadatatype/)
* class [MetadataOptions](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


