---
title: "Класс JsonUtility"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Utility.JsonUtility. Представляет утилитный класс для обработки json"
type: docs
url: /ru/net/aspose.cells.utility/jsonutility/
---
## JsonUtility class

Представляет вспомогательный класс для обработки JSON.

```csharp
public class JsonUtility
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [JsonUtility](jsonutility/)() | Конструктор по умолчанию. |

## Методы

| Имя | Описание |
| --- | --- |
| static [ExportRangeToJson](../../aspose.cells.utility/jsonutility/exportrangetojson/#exportrangetojson_1)(Range, ExportRangeToJsonOptions) | (**Obsolete.**) Экспорт диапазона в json файл. |
| static [ExportRangeToJson](../../aspose.cells.utility/jsonutility/exportrangetojson/#exportrangetojson)(Range, JsonSaveOptions) | Экспорт диапазона в json файл. |
| static [ImportData](../../aspose.cells.utility/jsonutility/importdata/)(string, Cells, int, int, JsonLayoutOptions) | Импортировать строку json. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.Utility;
    using System;

    public class JsonUtilityDemo
    {
        public static void JsonUtilityExample()
        {
            // Создать экземпляр JsonUtility
            JsonUtility jsonUtility = new JsonUtility();

            // Поскольку класс JsonUtility не имеет никаких свойств или методов, определённых в JSON,
            // мы продемонстрируем его создание и потенциальное использование в контексте.

            // Пример: Предположим, что JsonUtility может использоваться для обработки данных JSON каким-либо образом.
            // Примечание: Фактическое использование будет зависеть от методов и свойств, доступных в реальном классе.
            // Здесь мы просто демонстрируем создание, так как методы или свойства не предоставлены.

            Console.WriteLine("JsonUtility instance created successfully.");

            // Дополнительный код для демонстрации потенциального использования
            // Например, если бы у JsonUtility был метод для обработки JSON, он мог бы выглядеть так:
            // string jsonString = "{ \"name\": \"John\", \"age\": 30 }";
            // var result = jsonUtility.ProcessJson(jsonString);
            // Console.WriteLine("Processed JSON: " + result);

            // Поскольку методы не предоставлены, мы завершим пример здесь.
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)


