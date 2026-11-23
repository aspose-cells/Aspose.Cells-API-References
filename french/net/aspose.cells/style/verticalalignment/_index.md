---
title: "Style.VerticalAlignment"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Style. Obtient ou définit le type d'alignement vertical du texte dans une cellule"
type: docs
url: /fr/net/aspose.cells/style/verticalalignment/
---
## Style.VerticalAlignment property

Obtient ou définit le type d'alignement vertical du texte dans une cellule.

```csharp
public TextAlignmentType VerticalAlignment { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyVerticalAlignmentDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accéder à la cellule A1
            Cell cell = worksheet.Cells["A1"];
            
            // Définir la valeur de la cellule
            cell.PutValue("Vertical Alignment Demo");
            
            // Accédez au style de la cellule
            Style style = cell.GetStyle();
            
            // Définissez l'alignement vertical sur Haut
            style.VerticalAlignment = TextAlignmentType.Top;
            cell.SetStyle(style);
            
            // Enregistrez le classeur
            workbook.Save("VerticalAlignmentDemo.xlsx");
            
            Console.WriteLine("Vertical alignment set to Top for cell A1.");
        }
    }
}
```

### Voir aussi

* enum [TextAlignmentType](../../textalignmenttype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


