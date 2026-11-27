---
title: "Interface ICustomParser"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ICustomParser‑interface. Tillåter användare att lägga till sin egen värde‑parser för att tolka strängvärden till andra lämpliga cellvärdesobjekt"
type: docs
url: /sv/net/aspose.cells/icustomparser/
---
## ICustomParser interface

Tillåter användare att lägga till sin egen värdeparser för att tolka strängvärden till andra lämpliga cellvärdesobjekt.

```csharp
public interface ICustomParser
```

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [GetFormat](../../aspose.cells/icustomparser/getformat/)() | Hämtar formateringsmönstret som motsvarar det parsade värdet från den senaste anropet av [`ParseObject`](./parseobject/). |
| [ParseObject](../../aspose.cells/icustomparser/parseobject/)(string) | Parserar given sträng till ett lämpligt värdeobjekt. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ICustomParserDemo
    {
        public static void ICustomParserExample()
        {
            // Anpassad parserimplementation
            ICustomParser customParser = new CustomParser();

            // Exempel på användning av ParseObject‑metoden
            string valueToParse = "123.45";
            object parsedValue = customParser.ParseObject(valueToParse);
            Console.WriteLine($"Parsed Value: {parsedValue}");

            // Exempel på användning av GetFormat‑metoden
            string format = customParser.GetFormat();
            Console.WriteLine($"Format: {format}");
        }
    }

    // Anpassad implementation av ICustomParser
    public class CustomParser : ICustomParser
    {
        private string lastFormat;

        public object ParseObject(string value)
        {
            // Exempel på parslogik
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

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


