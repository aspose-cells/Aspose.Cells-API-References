---
title: "ICustomParser.GetFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ICustomParser-metod. Hämtar formateringsmönstret som motsvarar det parsade värdet från det senaste anropet av ParseObject"
type: docs
url: /sv/net/aspose.cells/icustomparser/getformat/
---
## ICustomParser.GetFormat method

Hämtar formateringsmönstret som motsvarar det parsade värdet från det senaste anropet av [`ParseObject`](../parseobject/).

```csharp
public string GetFormat()
```

### Anmärkningar

Det returnerade formateringsmönstret kan användas för att formatera motsvarande cell (sätt till Style.Custom för cellen).

### Exempel

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

### Se även

* interface [ICustomParser](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


