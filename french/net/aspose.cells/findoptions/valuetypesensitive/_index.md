---
title: "FindOptions.ValueTypeSensitive"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FindOptions. Indique si le type de valeur de la cellule recherchée doit être le même que la clé recherchée"
type: docs
url: /fr/net/aspose.cells/findoptions/valuetypesensitive/
---
## FindOptions.ValueTypeSensitive property

Indique si le type de valeur de la cellule recherchée doit être le même que la clé recherchée.

```csharp
public bool ValueTypeSensitive { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyValueTypeSensitiveDemo
    {
        public static void Run()
        {
            // Créez un classeur et ajoutez des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter différents types de valeurs aux cellules
            worksheet.Cells["A1"].PutValue("100"); // Stored as string
            worksheet.Cells["A2"].PutValue(100);   // Stored as number
            worksheet.Cells["A3"].PutValue("100.0"); // Stored as string
            worksheet.Cells["A4"].PutValue(100.0);   // Stored as number

            // Créer des options de recherche avec ValueTypeSensitive = true
            FindOptions options = new FindOptions();
            options.ValueTypeSensitive = true;
            options.LookAtType = LookAtType.EntireContent;

            // Rechercher le nombre 100 (ne trouvera pas la chaîne \"100\")
            Cell foundCell = worksheet.Cells.Find(100, null, options);
            Console.WriteLine("Found cell with number 100: " + (foundCell != null ? foundCell.Name : "Not found"));

            // Rechercher la chaîne \"100\" (ne trouvera pas le nombre 100)
            foundCell = worksheet.Cells.Find("100", null, options);
            Console.WriteLine("Found cell with string \"100\": " + (foundCell != null ? foundCell.Name : "Not found"));

            // Passer à ValueTypeSensitive = false
            options.ValueTypeSensitive = false;
            
            // Désormais, les deux recherches trouveront toute cellule contenant \"100\" ou 100
            foundCell = worksheet.Cells.Find(100, null, options);
            Console.WriteLine("Found any 100 (type insensitive): " + (foundCell != null ? foundCell.Name : "Not found"));
        }
    }
}
```

### Voir aussi

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


