---
title: "Интерфейс IFilePathProvider"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Интерфейс Aspose.Cells.IFilePathProvider. Представляет провайдер пути экспортируемого файла"
type: docs
url: /ru/net/aspose.cells/ifilepathprovider/
---
## IFilePathProvider interface

Представляет поставщик пути экспортируемого файла.

```csharp
public interface IFilePathProvider
```

## Методы

| Имя | Описание |
| --- | --- |
| [GetFullName](../../aspose.cells/ifilepathprovider/getfullname/)(string) | Получает полный путь к файлу по имени листа при отдельном экспорте листа в HTML. Таким образом, ссылки между листами могут быть экспортированы корректно. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IFilePathProviderDemo : IFilePathProvider
    {
        // Реализация метода GetFullName из интерфейса IFilePathProvider
        public string GetFullName(string sheetName)
        {
            // Для демонстрации возвращает простой путь к файлу, основанный на имени листа
            return $"{sheetName}.html";
        }

        public static void IFilePathProviderExample()
        {
            // Создать новую книгу и добавить некоторые данные
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // Создать HtmlSaveOptions и установить FilePathProvider
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.FilePathProvider = new IFilePathProviderDemo();

            // Сохраните книгу в формате HTML
            workbook.Save("IFilePathProviderExample.html", saveOptions);

            Console.WriteLine("Workbook saved to HTML with custom file paths.");
        }
    }


}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


