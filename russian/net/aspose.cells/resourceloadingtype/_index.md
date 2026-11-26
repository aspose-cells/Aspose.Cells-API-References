---
title: "Перечисление ResourceLoadingType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.ResourceLoadingType enum. Представляет, как загружать связанный ресурс"
type: docs
url: /ru/net/aspose.cells/resourceloadingtype/
---
## ResourceLoadingType enumeration

Представляет способ загрузки связанного ресурса.

```csharp
public enum ResourceLoadingType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Default | `0` | Загружает этот ресурс как обычно. |
| Skip | `1` | Пропускает загрузку этого ресурса. |
| UserProvided | `2` | Использовать поток, предоставленный пользователем |

### Примеры

```csharp
using Aspose.Cells;
using System;
using System.IO;

namespace AsposeCellsExamples
{
    public class ResourceLoadingTypeDemo
    {
        public static void ResourceLoadingTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("Resource");
            worksheet.Cells["A2"].PutValue("Default");
            worksheet.Cells["A3"].PutValue("Skip");
            worksheet.Cells["A4"].PutValue("UserProvided");

            // Сохранить книгу в HTML с пользовательским провайдером потока
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html)
            {
                StreamProvider = new CustomStreamProvider()
            };

            workbook.Save("ResourceLoadingTypeExample.html", saveOptions);
        }
    }

    public class CustomStreamProvider : IStreamProvider
    {
        public void InitStream(StreamProviderOptions options)
        {
            if (options.ResourceLoadingType == ResourceLoadingType.UserProvided)
            {
                // Предоставить пользовательский поток для ресурса
                options.Stream = new MemoryStream();
            }
            else if (options.ResourceLoadingType == ResourceLoadingType.Skip)
            {
                // Пропустить загрузку ресурса
                options.Stream = Stream.Null;
            }
            else
            {
                // Загружать ресурс как обычно
                options.Stream = new FileStream(options.DefaultPath, FileMode.Open, FileAccess.Read);
            }
        }

        public void CloseStream(StreamProviderOptions options)
        {
            // Закройте поток, если он не null
            options.Stream?.Close();
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


