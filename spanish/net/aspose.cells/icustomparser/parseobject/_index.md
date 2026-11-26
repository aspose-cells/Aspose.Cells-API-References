---
title: "ICustomParser.ParseObject"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ICustomParser. Analiza la cadena dada a un objeto de valor apropiado"
type: docs
url: /es/net/aspose.cells/icustomparser/parseobject/
---
## ICustomParser.ParseObject method

Analiza la cadena dada a un objeto de valor adecuado.

```csharp
public object ParseObject(string value)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | String | El valor de cadena a analizar |

### Valor de retorno

Objeto de valor analizado a partir de la cadena dada. Si la cadena dada no puede analizarse a un objeto de valor apropiado, devuelve null.

### Ejemplos

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

### Ver también

* interface [ICustomParser](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


