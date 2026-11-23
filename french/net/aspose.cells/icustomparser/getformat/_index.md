---
title: "ICustomParser.GetFormat"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ICustomParser. Obtient le modèle de formatage correspondant à la valeur analysée lors de la dernière invocation de ParseObject"
type: docs
url: /fr/net/aspose.cells/icustomparser/getformat/
---
## ICustomParser.GetFormat method

Obtient le modèle de formatage correspondant à la valeur analysée lors de la dernière invocation de [`ParseObject`](../parseobject/).

```csharp
public string GetFormat()
```

### Remarques

Le modèle de formatage retourné peut être utilisé pour formater la cellule correspondante (définissez Style.Custom pour la cellule).

### Exemples

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

### Voir aussi

* interface [ICustomParser](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


