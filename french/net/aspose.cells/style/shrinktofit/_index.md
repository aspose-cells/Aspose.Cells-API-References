---
title: "Style.ShrinkToFit"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Style. Représente si le texte se réduit automatiquement pour s'adapter à la largeur de colonne disponible"
type: docs
url: /fr/net/aspose.cells/style/shrinktofit/
---
## Style.ShrinkToFit property

Représente si le texte se réduit automatiquement pour s'adapter à la largeur de colonne disponible.

```csharp
public bool ShrinkToFit { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyShrinkToFitDemo
    {
        public static void Run()
        {
            // Créer un objet classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accéder à la collection de cellules
            Cells cells = worksheet.Cells;
            
            // Définir du texte dans la cellule A1 qui est plus long que la largeur de la colonne
            cells["A1"].PutValue("This is a long text that needs shrinking to fit");
            
            // Définir la largeur de la colonne pour qu'elle soit plus petite que la longueur du texte
            cells.SetColumnWidth(0, 10);
            
            // Obtenir le style de la cellule A1
            Style style = cells["A1"].GetStyle();
            
            // Définir ShrinkToFit sur true
            style.ShrinkToFit = true;
            
            // Appliquer le style à la cellule A1
            cells["A1"].SetStyle(style);
            
            // Enregistrez le classeur
            workbook.Save("ShrinkToFitDemo.xlsx");
            
            Console.WriteLine("ShrinkToFit demo completed successfully.");
        }
    }
}
```

### Voir aussi

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


