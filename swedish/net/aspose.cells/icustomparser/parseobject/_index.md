---
title: "ICustomParser.ParseObject"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ICustomParser-metoden. Tolkar given sträng till korrekt värdeobjekt"
type: docs
url: /sv/net/aspose.cells/icustomparser/parseobject/
---
## ICustomParser.ParseObject method

Parserar given sträng till ett lämpligt värdeobjekt.

```csharp
public object ParseObject(string value)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | String | Strängvärdet som ska tolkas |

### Returvärde

Tolkat värdeobjekt från given sträng. Om den givna strängen inte kan tolkas till ett korrekt värdeobjekt returneras null.

### Exempel

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

### Se även

* interface [ICustomParser](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


