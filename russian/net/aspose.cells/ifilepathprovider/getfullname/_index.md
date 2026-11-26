---
title: "IFilePathProvider.GetFullName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод IFilePathProvider. Получает полный путь к файлу по имени листа при отдельном экспорте листа в HTML. Таким образом, ссылки между листами могут быть экспортированы корректно"
type: docs
url: /ru/net/aspose.cells/ifilepathprovider/getfullname/
---
## IFilePathProvider.GetFullName method

Получает полный путь к файлу по имени листа при отдельном экспорте листа в HTML. Таким образом, ссылки между листами могут быть экспортированы корректно.

```csharp
public string GetFullName(string sheetName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetName | String | Имя листа |

### Возвращаемое значение

полный путь к файлу

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IFilePathProviderMethodGetFullNameWithStringDemo
    {
        public static void Run()
        {
            // Создать пользовательскую реализацию IFilePathProvider
            CustomFilePathProvider provider = new CustomFilePathProvider();

            // Вызвать метод GetFullName с именем листа
            string sheetName = "Sheet1";
            string fullPath = provider.GetFullName(sheetName);

            // Отобразить результат
            Console.WriteLine($"Full path for {sheetName}: {fullPath}");
        }
    }

    internal class CustomFilePathProvider : IFilePathProvider
    {
        public string GetFullName(string sheetName)
        {
            // Простая реализация, возвращающая путь, объединяющий имя листа с каталогом
            return $"C:\\Temp\\{sheetName}.xlsx";
        }
    }
}
```

### См. также

* interface [IFilePathProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


