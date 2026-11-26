---
title: "JsonLayoutOptions.IgnoreObjectTitle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство JsonLayoutOptions. Указывает, следует ли игнорировать заголовок, если объект является свойством другого объекта"
type: docs
url: /ru/net/aspose.cells.utility/jsonlayoutoptions/ignoreobjecttitle/
---
## JsonLayoutOptions.IgnoreObjectTitle property

Указывает, следует ли игнорировать заголовок, если объект является свойством другого объекта.

```csharp
[Obsolete("Use JsonLayoutOptions.IgnoreTitle property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IgnoreObjectTitle { get; set; }
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

    public class JsonLayoutOptionsPropertyIgnoreObjectTitleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Пример данных JSON с заголовками объектов
            string json = @"{
                ""Employees"": {
                    ""Employee"": [
                        { ""Name"": ""John"", ""Age"": 30 },
                        { ""Name"": ""Jane"", ""Age"": 25 }
                    ]
                }
            }";

            // Создать JsonLayoutOptions
            JsonLayoutOptions options = new JsonLayoutOptions();
            
            // Отобразить текущее значение IgnoreObjectTitle
            Console.WriteLine("Current IgnoreObjectTitle value: " + options.IgnoreObjectTitle);

            // Установить игнорирование заголовков объектов
            options.IgnoreObjectTitle = true;
            Console.WriteLine("Set IgnoreObjectTitle to: " + options.IgnoreObjectTitle);

            // Импортировать JSON с IgnoreObjectTitle = true
            JsonUtility.ImportData(json, worksheet.Cells, 0, 0, options);

            // Сохранить с игнорированными заголовками
            workbook.Save("IgnoreObjectTitle_True.xlsx");

            // Сбросить лист
            worksheet.Cells.Clear();

            // Установить включение заголовков объектов
            options.IgnoreObjectTitle = false;
            Console.WriteLine("Set IgnoreObjectTitle to: " + options.IgnoreObjectTitle);

            // Импортировать JSON с IgnoreObjectTitle = false
            JsonUtility.ImportData(json, worksheet.Cells, 0, 0, options);

            // Сохранить с включёнными заголовками
            workbook.Save("IgnoreObjectTitle_False.xlsx");
        }
    }
}
```

### См. также

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


