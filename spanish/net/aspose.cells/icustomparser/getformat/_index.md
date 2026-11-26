---
title: "ICustomParser.GetFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ICustomParser. Obtiene el patrón de formato correspondiente al valor analizado por la última invocación de ParseObject"
type: docs
url: /es/net/aspose.cells/icustomparser/getformat/
---
## ICustomParser.GetFormat method

Obtiene el patrón de formato correspondiente al valor analizado por la última invocación de [`ParseObject`](../parseobject/).

```csharp
public string GetFormat()
```

### Observaciones

El patrón de formato devuelto puede usarse para dar formato a la celda correspondiente (establecer en Style.Custom para la celda).

### Ejemplos

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

### Ver también

* interface [ICustomParser](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


