---
title: "FindOptions.LookAtType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FindOptions. Type de recherche"
type: docs
url: /fr/net/aspose.cells/findoptions/lookattype/
---
## FindOptions.LookAtType property

Regarder le type.

```csharp
public LookAtType LookAtType { get; set; }
```

### Remarques

Lorsque [`RegexKey`](../regexkey/) est vrai et que l'utilisateur a spécifié la règle exacte pour l'expression régulière, pour des raisons de performance cette propriété doit être définie sur EntireContent. Sinon, nous reformulerons la clé de recherche afin de garantir qu'elle puisse correspondre au type spécifique. Par exemple, lorsque le type est Contains (c'est la valeur par défaut de cette propriété), nous ajouterons automatiquement des caractères génériques au début et à la fin de la clé de recherche. Dans ce cas, les expressions régulières deviendront plus complexes et les performances diminueront.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyLookAtTypeDemo
    {
        public static void Run()
        {
            // Créez un classeur et ajoutez des données
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Hello World");
            worksheet.Cells["A2"].PutValue("=1+2"); // Formula
            worksheet.Cells["A3"].PutValue("Partial match test");
            worksheet.Cells["A4"].PutValue("=A1&A3"); // Formula concatenating cells

            // Créer des options de recherche avec LookAtType.EntireContent
            FindOptions options = new FindOptions
            {
                LookInType = LookInType.OnlyFormulas,
                LookAtType = LookAtType.EntireContent
            };

            // Rechercher une formule qui correspond exactement à "=A1&A3"
            Cell cell = worksheet.Cells.Find("=A1&A3", null, options);
            Console.WriteLine("Found cell with exact formula match: " + (cell != null ? cell.Name : "null"));

            // Passer à une correspondance partielle
            options.LookAtType = LookAtType.Contains;
            cell = worksheet.Cells.Find("A3", null, options);
            Console.WriteLine("Found cell containing 'A3' in formula: " + (cell != null ? cell.Name : "null"));
        }
    }
}
```

### Voir aussi

* enum [LookAtType](../../lookattype/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


