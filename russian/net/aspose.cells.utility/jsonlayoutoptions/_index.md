---
title: "Класс JsonLayoutOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Utility.JsonLayoutOptions. Представляет параметры типа макета json"
type: docs
url: /ru/net/aspose.cells.utility/jsonlayoutoptions/
---
## JsonLayoutOptions class

Представляет параметры типа макета JSON.

```csharp
public class JsonLayoutOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [JsonLayoutOptions](jsonlayoutoptions/)() | Конструктор загрузки параметров макета JSON. |

## Свойства

| Имя | Описание |
| --- | --- |
| [ArrayAsTable](../../aspose.cells.utility/jsonlayoutoptions/arrayastable/) { get; set; } | Обрабатывает массив как таблицу. |
| [ConvertNumericOrDate](../../aspose.cells.utility/jsonlayoutoptions/convertnumericordate/) { get; set; } | Указывает, следует ли преобразовать строку в json в числовое или датовое значение. |
| [DateFormat](../../aspose.cells.utility/jsonlayoutoptions/dateformat/) { get; set; } | Получает и задает формат значения даты. |
| [IgnoreArrayTitle](../../aspose.cells.utility/jsonlayoutoptions/ignorearraytitle/) { get; set; } | (**Obsolete.**) Указывает, следует ли игнорировать заголовок, если массив является свойством объекта. |
| [IgnoreNull](../../aspose.cells.utility/jsonlayoutoptions/ignorenull/) { get; set; } | Указывает, следует ли игнорировать нулевые значения. |
| [IgnoreObjectTitle](../../aspose.cells.utility/jsonlayoutoptions/ignoreobjecttitle/) { get; set; } | (**Obsolete.**) Указывает, следует ли игнорировать заголовок, если объект является свойством другого объекта. |
| [IgnoreTitle](../../aspose.cells.utility/jsonlayoutoptions/ignoretitle/) { get; set; } | Игнорирует заголовки атрибутов |
| [KeptSchema](../../aspose.cells.utility/jsonlayoutoptions/keptschema/) { get; set; } | Указывает, сохранять ли схему этого JSON. |
| [NumberFormat](../../aspose.cells.utility/jsonlayoutoptions/numberformat/) { get; set; } | Получает и задает формат числового значения. |
| [TitleStyle](../../aspose.cells.utility/jsonlayoutoptions/titlestyle/) { get; set; } | Получает и задает стиль заголовка. |

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class UtilityClassJsonLayoutOptionsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте JsonLayoutOptions и задайте свойства
            JsonLayoutOptions options = new JsonLayoutOptions
            {
                ArrayAsTable = true,
                ConvertNumericOrDate = true,
                IgnoreArrayTitle = false,
                IgnoreObjectTitle = false
            };

            // Пример JSON-данных
            string jsonData = @"{
                ""Name"": ""John"",
                ""Age"": 30,
                ""Departments"": [""HR"", ""Finance"", ""IT""]
            }";

            // Импортировать JSON-данные в лист
            JsonUtility.ImportData(jsonData, worksheet.Cells, 0, 0, options);

            // Сохраните книгу
            workbook.Save("JsonLayoutOptionsDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)


