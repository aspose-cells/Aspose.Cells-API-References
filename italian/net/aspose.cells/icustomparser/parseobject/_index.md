---
title: "ICustomParser.ParseObject"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ICustomParser. Analizza la stringa fornita in un oggetto valore corretto"
type: docs
url: /it/net/aspose.cells/icustomparser/parseobject/
---
## ICustomParser.ParseObject method

Analizza la stringa fornita in un oggetto valore appropriato.

```csharp
public object ParseObject(string value)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | String | Il valore stringa da analizzare |

### Valore di ritorno

Oggetto valore analizzato dalla stringa fornita. Se la stringa fornita non può essere analizzata in un oggetto valore corretto, restituisce null.

### Esempi

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

### Vedi anche

* interface [ICustomParser](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


