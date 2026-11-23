---
title: "FindOptions.Style"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FindOptions. Le format à rechercher"
type: docs
url: /fr/net/aspose.cells/findoptions/style/
---
## FindOptions.Style property

Le format à rechercher.

```csharp
public Style Style { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyStyleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer un style avec une police bleue
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Blue;

            // Appliquer le style à la cellule F2
            Cell cell = worksheet.Cells["F2"];
            cell.PutValue("SearchTarget");
            cell.SetStyle(style);

            // Créer des options de recherche avec le style
            FindOptions options = new FindOptions();
            options.Style = style;

            // Trouver la cellule avec le style correspondant
            Cell foundCell = worksheet.Cells.Find(null, null, options);

            // Afficher le nom de la cellule trouvée
            Console.WriteLine("Cell found with matching style: " + foundCell?.Name);
        }
    }
}
```

### Voir aussi

* class [Style](../../style/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


