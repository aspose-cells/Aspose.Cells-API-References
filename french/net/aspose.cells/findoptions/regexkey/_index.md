---
title: "FindOptions.RegexKey"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FindOptions. Indique si la clé recherchée est une expression régulière. Si true, la clé recherchée sera prise comme expression régulière et analysée. Sinon, la clé sera analysée selon les règles de MS Excel."
type: docs
url: /fr/net/aspose.cells/findoptions/regexkey/
---
## FindOptions.RegexKey property

Indique si la clé recherchée est une expression régulière. Si vrai, la clé recherchée sera prise comme expression régulière et analysée. Sinon, la clé sera analysée selon les règles de MS Excel.

```csharp
public bool RegexKey { get; set; }
```

### Remarques

Même si la clé de recherche a été spécifiée comme expression régulière, elle peut être reformulée selon le [`LookAtType`](../lookattype/) spécifié. Par exemple, lorsque le type est Contains (c’est la valeur par défaut pour ces options), des caractères génériques seront ajoutés automatiquement au début et à la fin de la clé de recherche pour garantir que la correspondance soit vérifiée comme "contains". Dans ce cas, les expressions régulières deviendront plus complexes et les performances diminueront également. Ainsi, pour des raisons de performance, si l’utilisateur a spécifié la règle exacte pour l’expression régulière, il n’est pas nécessaire d’utiliser [`LookAtType`](../lookattype/) comme contrainte supplémentaire et l’utilisateur peut le définir sur EntireContent pour obtenir de meilleures performances.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyRegexKeyDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir des données de test avec des chaînes correspondant à un motif
            worksheet.Cells["A1"].PutValue("[hello]");
            worksheet.Cells["A2"].PutValue("Regular text");
            worksheet.Cells["A3"].PutValue("[another_example]");

            // Créer des options de recherche avec les expressions régulières activées
            FindOptions options = new FindOptions();
            options.RegexKey = true;
            options.LookInType = LookInType.Values;
            options.LookAtType = LookAtType.Contains;

            // Rechercher les cellules correspondant au motif d’expression régulière
            string regEx = "\\[[a-zA-Z0-9_]+\\]";
            Cell foundCell = worksheet.Cells.Find(regEx, null, options);

            // Afficher le résultat
            if (foundCell != null)
            {
                Console.WriteLine("Found cell: " + foundCell.Name + " with value: " + foundCell.StringValue);
            }
            else
            {
                Console.WriteLine("No matching cells found");
            }
        }
    }
}
```

### Voir aussi

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


