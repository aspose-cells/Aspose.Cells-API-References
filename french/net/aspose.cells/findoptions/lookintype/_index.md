---
title: "FindOptions.LookInType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FindOptions. Type de recherche"
type: docs
url: /fr/net/aspose.cells/findoptions/lookintype/
---
## FindOptions.LookInType property

Regarder dans le type.

```csharp
public LookInType LookInType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyLookInTypeDemo
    {
        public static void Run()
        {
            // Créez un classeur et ajoutez des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir des valeurs et des formules dans les cellules
            worksheet.Cells["A1"].PutValue("SearchValue");
            worksheet.Cells["A2"].Formula = "=A1";
            worksheet.Cells["B1"].PutValue("OtherValue");

            // Créer des options de recherche pour ne rechercher que dans les formules
            FindOptions options = new FindOptions
            {
                LookInType = LookInType.OnlyFormulas,
                LookAtType = LookAtType.Contains
            };

            // Rechercher la valeur dans les formules
            Cell foundCell = worksheet.Cells.Find("SearchValue", null, options);

            // Afficher le résultat
            if (foundCell != null)
            {
                Console.WriteLine($"Found at: Row {foundCell.Row}, Column {foundCell.Column}");
            }
            else
            {
                Console.WriteLine("Value not found in formulas");
            }
        }
    }
}
```

### Voir aussi

* enum [LookInType](../../lookintype/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


