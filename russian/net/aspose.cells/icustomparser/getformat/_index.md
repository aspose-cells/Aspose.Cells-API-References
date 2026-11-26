---
title: "ICustomParser.GetFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ICustomParser. Получает шаблон форматирования, соответствующий разобранному значению при последнем вызове ParseObject"
type: docs
url: /ru/net/aspose.cells/icustomparser/getformat/
---
## ICustomParser.GetFormat method

Получает шаблон форматирования, соответствующий разобранному значению при последнем вызове [`ParseObject`](../parseobject/).

```csharp
public string GetFormat()
```

### Примечания

Возвращённый шаблон форматирования может быть использован для форматирования соответствующей ячейки (установите Style.Custom для ячейки).

### Примеры

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
   
    public class CustomParser2 : ICustomParser
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
            return "Standard numeric format";
        }
    }

    public class ICustomParser1MethodGetFormatDemo
    {
        public static void Run()
        {
            ICustomParser customParser = new CustomParser2();

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


