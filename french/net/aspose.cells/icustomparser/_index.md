---
title: "Interface ICustomParser"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Interface Aspose.Cells.ICustomParser. Permet aux utilisateurs d'ajouter leur analyseur de valeurs personnalisé pour analyser les valeurs de chaîne en d'autres objets de valeur de cellule appropriés."
type: docs
url: /fr/net/aspose.cells/icustomparser/
---
## ICustomParser interface

Permet aux utilisateurs d'ajouter leur analyseur de valeurs personnalisé pour analyser les valeurs de chaîne en d'autres objets de valeur de cellule appropriés.

```csharp
public interface ICustomParser
```

## Méthodes

| Nom | Description |
| --- | --- |
| [GetFormat](../../aspose.cells/icustomparser/getformat/)() | Obtient le modèle de formatage correspondant à la valeur analysée lors de la dernière invocation de [`ParseObject`](./parseobject/). |
| [ParseObject](../../aspose.cells/icustomparser/parseobject/)(string) | Analyse la chaîne donnée en un objet de valeur approprié. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ICustomParserDemo
    {
        public static void ICustomParserExample()
        {
            // Implémentation d'analyseur personnalisé
            ICustomParser customParser = new CustomParser();

            // Exemple d'utilisation de la méthode ParseObject
            string valueToParse = "123.45";
            object parsedValue = customParser.ParseObject(valueToParse);
            Console.WriteLine($"Parsed Value: {parsedValue}");

            // Exemple d'utilisation de la méthode GetFormat
            string format = customParser.GetFormat();
            Console.WriteLine($"Format: {format}");
        }
    }

    // Implémentation personnalisée de ICustomParser
    public class CustomParser : ICustomParser
    {
        private string lastFormat;

        public object ParseObject(string value)
        {
            // Exemple de logique d'analyse
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

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


