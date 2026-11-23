---
title: "FindOptions.SearchBackward"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FindOptions. Indique si la recherche se fait en arrière pour les cellules"
type: docs
url: /fr/net/aspose.cells/findoptions/searchbackward/
---
## FindOptions.SearchBackward property

Indique si la recherche doit se faire en arrière pour les cellules.

```csharp
public bool SearchBackward { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertySearchBackwardDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Configurer des données d'exemple
            worksheet.Cells["A1"].PutValue("abc");
            worksheet.Cells["B2"].PutValue("abc");
            worksheet.Cells["C3"].PutValue("abc");

            FindOptions options = new FindOptions();
            options.LookInType = LookInType.Values;
            options.LookAtType = LookAtType.Contains;
            
            // Rechercher en avant (comportement par défaut)
            options.SearchBackward = false;
            Cell foundForward = worksheet.Cells.Find("abc", null, options);
            Console.WriteLine($"Forward search found at: {foundForward.Name}");

            // Rechercher en arrière
            options.SearchBackward = true;
            Cell foundBackward = worksheet.Cells.Find("abc", null, options);
            Console.WriteLine($"Backward search found at: {foundBackward.Name}");
        }
    }
}
```

### Voir aussi

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


