---
title: "ICustomParser.ParseObject"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ICustomParser-Methode. Parst die gegebene Zeichenkette in ein geeignetes Wertobjekt"
type: docs
url: /de/net/aspose.cells/icustomparser/parseobject/
---
## ICustomParser.ParseObject method

Parst die gegebene Zeichenkette in ein geeignetes Wertobjekt.

```csharp
public object ParseObject(string value)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | String | Der zu parsende Zeichenkettenwert |

### Rückgabewert

Geparstes Wertobjekt aus der angegebenen Zeichenkette. Wenn die Zeichenkette nicht in ein geeignetes Wertobjekt geparst werden kann, wird null zurückgegeben.

### Beispiele

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

### Siehe auch

* interface [ICustomParser](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


