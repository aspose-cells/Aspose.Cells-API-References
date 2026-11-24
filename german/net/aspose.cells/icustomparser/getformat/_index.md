---
title: "ICustomParser.GetFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ICustomParser-Methode. Liefert das Formatierungsmuster, das dem beim letzten Aufruf von ParseObject geparsten Wert entspricht"
type: docs
url: /de/net/aspose.cells/icustomparser/getformat/
---
## ICustomParser.GetFormat method

Liefert das Formatierungsmuster, das dem beim letzten Aufruf von [`ParseObject`](../parseobject/) geparsten Wert entspricht.

```csharp
public string GetFormat()
```

### Hinweise

Das zurückgegebene Formatierungsmuster kann verwendet werden, um die entsprechende Zelle zu formatieren (setzen Sie Style.Custom für die Zelle).

### Beispiele

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

### Siehe auch

* interface [ICustomParser](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


