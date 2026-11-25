---
title: "ICustomParser.GetFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ICustomParser. Ottiene il modello di formattazione corrispondente al valore analizzato dall'ultima invocazione di ParseObject"
type: docs
url: /it/net/aspose.cells/icustomparser/getformat/
---
## ICustomParser.GetFormat method

Ottiene il modello di formattazione corrispondente al valore analizzato dall'ultima invocazione di [`ParseObject`](../parseobject/).

```csharp
public string GetFormat()
```

### Osservazioni

Il modello di formattazione restituito può essere usato per formattare la cella corrispondente (impostare su Style.Custom per la cella).

### Esempi

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

### Vedi anche

* interface [ICustomParser](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


