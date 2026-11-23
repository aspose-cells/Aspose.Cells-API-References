---
title: "LightCellsDataHandler.ProcessRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode LightCellsDataHandler. Commence à traiter une ligne"
type: docs
url: /fr/net/aspose.cells/icustomparser/parseobject/
---
## ICustomParser.ParseObject method

Analyse la chaîne donnée en un objet de valeur approprié.

```csharp
public object ParseObject(string value)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | String | Objet Row qui est actuellement traité. |

### Valeur de retour

Objet valeur analysée à partir de la chaîne fournie. Si la chaîne fournie ne peut pas être analysée en un objet valeur approprié, renvoie null.

### Exemples

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

### Voir aussi

* interface [ICustomParser](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


