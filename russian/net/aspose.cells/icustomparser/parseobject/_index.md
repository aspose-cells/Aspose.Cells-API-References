---
title: "ICustomParser.ParseObject"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ICustomParser. Разбирает заданную строку в соответствующий объект значения"
type: docs
url: /ru/net/aspose.cells/icustomparser/parseobject/
---
## ICustomParser.ParseObject method

Разбирает заданную строку в корректный объект значения.

```csharp
public object ParseObject(string value)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | String | Строковое значение для разбора |

### Возвращаемое значение

Объект значения, полученный из заданной строки. Если строку нельзя разобрать в соответствующий объект значения, возвращается null.

### Примеры

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{

    public class CustomParser : ICustomParser
    {
        public object ParseObject(string s)
        {
            if (double.TryParse(s, out double result))
            {
                return result;
            }
            return s;
        }

        public string GetFormat()
        {
            return "Numeric or string format";
        }
    }

    public class ICustomParserMethodParseObjectWithStringDemo
    {
        public static void Run()
        {
            ICustomParser customParser = new CustomParser();
            string valueToParse = "123.45";
            object parsedValue = customParser.ParseObject(valueToParse);
            Console.WriteLine($"Parsed Value: {parsedValue}");

            string format = customParser.GetFormat();
            Console.WriteLine($"Format: {format}");
        }
    }
}
```

### См. также

* interface [ICustomParser](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


