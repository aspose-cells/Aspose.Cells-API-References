---
title: "FindOptions.SearchOrderByRows"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FindOptions. Indique si l'ordre de recherche est par lignes ou par colonnes"
type: docs
url: /fr/net/aspose.cells/findoptions/searchorderbyrows/
---
## FindOptions.SearchOrderByRows property

Indique si l'ordre de recherche est par lignes ou par colonnes.

```csharp
public bool SearchOrderByRows { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertySearchOrderByRowsDemo
    {
        public static void Run()
        {
            // Créez un classeur et ajoutez des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Remplir les cellules avec des données de test (recherche de \"abc\" dans l'ordre colonne-major)
            worksheet.Cells["A1"].PutValue("xyz");
            worksheet.Cells["B1"].PutValue("def");
            worksheet.Cells["A2"].PutValue("123");
            worksheet.Cells["B2"].PutValue("abc");
            worksheet.Cells["A3"].PutValue("abc");
            worksheet.Cells["B3"].PutValue("789");

            // Créer des options de recherche et définir l'ordre de recherche sur colonne-major
            FindOptions findOptions = new FindOptions();
            findOptions.SearchOrderByRows = false; // Search column by column

            // Rechercher \"abc\" - doit retourner A3 (ligne 2, colonne 0) lors d'une recherche colonne-major
            Cell foundCell = worksheet.Cells.Find("abc", null, findOptions);

            // Afficher le résultat
            Console.WriteLine($"Found 'abc' at row: {foundCell.Row}, column: {foundCell.Column}");
        }
    }
}
```

### Voir aussi

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


