---
title: "Интерфейс ICustomParser"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Интерфейс Aspose.Cells.ICustomParser. Позволяет пользователям добавить собственный парсер значений для преобразования строковых значений в другие корректные объекты значений ячеек."
type: docs
url: /ru/net/aspose.cells/icustomparser/
---
## ICustomParser interface

Позволяет пользователям добавить собственный парсер значений для преобразования строковых значений в другие соответствующие объекты значений ячеек.

```csharp
public interface ICustomParser
```

## Методы

| Имя | Описание |
| --- | --- |
| [GetFormat](../../aspose.cells/icustomparser/getformat/)() | Получает шаблон форматирования, соответствующий разобранному значению, при последнем вызове [`ParseObject`](./parseobject/). |
| [ParseObject](../../aspose.cells/icustomparser/parseobject/)(string) | Разбирает заданную строку в корректный объект значения. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ICustomParserDemo
    {
        public static void ICustomParserExample()
        {
            // Реализация пользовательского парсера
            ICustomParser customParser = new CustomParser();

            // Пример использования метода ParseObject
            string valueToParse = "123.45";
            object parsedValue = customParser.ParseObject(valueToParse);
            Console.WriteLine($"Parsed Value: {parsedValue}");

            // Пример использования метода GetFormat
            string format = customParser.GetFormat();
            Console.WriteLine($"Format: {format}");
        }
    }

    // Пользовательская реализация ICustomParser
    public class CustomParser : ICustomParser
    {
        private string lastFormat;

        public object ParseObject(string value)
        {
            // Пример логики парсинга
            if (double.TryParse(value, out double result))
            {
                lastFormat = "0.00"; // Example format
                return result;
            }
            lastFormat = null;
            return null;
        }

        public string GetFormat()
        {
            return lastFormat;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


