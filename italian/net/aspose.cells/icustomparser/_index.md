---
title: "Interfaccia ICustomParser"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Interfaccia Aspose.Cells.ICustomParser. Consente agli utenti di aggiungere il proprio parser di valori personalizzato per analizzare valori stringa in altri oggetti valore di cella appropriati"
type: docs
url: /it/net/aspose.cells/icustomparser/
---
## ICustomParser interface

Consente agli utenti di aggiungere il proprio parser di valori personalizzato per analizzare valori stringa in altri oggetti di valore cella appropriati.

```csharp
public interface ICustomParser
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetFormat](../../aspose.cells/icustomparser/getformat/)() | Ottiene il modello di formattazione corrispondente al valore analizzato dall'ultima invocazione di [`ParseObject`](./parseobject/). |
| [ParseObject](../../aspose.cells/icustomparser/parseobject/)(string) | Analizza la stringa fornita in un oggetto valore appropriato. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ICustomParserDemo
    {
        public static void ICustomParserExample()
        {
            // Implementazione del parser personalizzato
            ICustomParser customParser = new CustomParser();

            // Esempio di utilizzo del metodo ParseObject
            string valueToParse = "123.45";
            object parsedValue = customParser.ParseObject(valueToParse);
            Console.WriteLine($"Parsed Value: {parsedValue}");

            // Esempio di utilizzo del metodo GetFormat
            string format = customParser.GetFormat();
            Console.WriteLine($"Format: {format}");
        }
    }

    // Implementazione personalizzata di ICustomParser
    public class CustomParser : ICustomParser
    {
        private string lastFormat;

        public object ParseObject(string value)
        {
            // Esempio di logica di parsing
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

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


