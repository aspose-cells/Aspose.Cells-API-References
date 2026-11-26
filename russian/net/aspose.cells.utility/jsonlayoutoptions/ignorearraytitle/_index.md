---
title: "JsonLayoutOptions.IgnoreArrayTitle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство JsonLayoutOptions. Указывает, следует ли игнорировать заголовок, если массив является свойством объекта"
type: docs
url: /ru/net/aspose.cells.utility/jsonlayoutoptions/ignorearraytitle/
---
## JsonLayoutOptions.IgnoreArrayTitle property

Указывает, следует ли игнорировать заголовок, если массив является свойством объекта.

```csharp
[Obsolete("Use JsonLayoutOptions.IgnoreTitle property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IgnoreArrayTitle { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство JsonLayoutOptions.IgnoreTitle. Это свойство будет удалено через 6 месяцев, начиная с февраля 2023 года. Aspose приносит извинения за любые причинённые неудобства.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;

    public class JsonLayoutOptionsPropertyIgnoreArrayTitleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Пример данных JSON с заголовками массивов
            string json = @"{
                ""Employees"": [
                    { ""Name"": ""John"", ""Age"": 30 },
                    { ""Name"": ""Jane"", ""Age"": 25 }
                ]
            }";

            // Создать JsonLayoutOptions
            JsonLayoutOptions options = new JsonLayoutOptions();
            
            // Отобразить текущее значение IgnoreArrayTitle
            Console.WriteLine("Current IgnoreArrayTitle value: " + options.IgnoreArrayTitle);

            // Первый импорт с IgnoreArrayTitle = false (по умолчанию)
            options.IgnoreArrayTitle = false;
            JsonUtility.ImportData(json, worksheet.Cells, 0, 0, options);
            Console.WriteLine("Data imported with IgnoreArrayTitle=false. Check cell A1 for 'Employees' title.");

            // Очистить лист для второго импорта
            worksheet.Cells.Clear();

            // Второй импорт с IgnoreArrayTitle = true
            options.IgnoreArrayTitle = true;
            JsonUtility.ImportData(json, worksheet.Cells, 0, 0, options);
            Console.WriteLine("Data imported with IgnoreArrayTitle=true. Check cell A1 for direct array values.");

            // Сохраните книгу
            workbook.Save("JsonLayoutOptionsIgnoreArrayTitleDemo.xlsx");
        }
    }
}
```

### См. также

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


