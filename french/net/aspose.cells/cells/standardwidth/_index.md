---
title: "Cells.StandardWidth"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cells. Obtient ou définit la largeur de colonne par défaut dans la feuille de calcul en unité de caractères"
type: docs
url: /fr/net/aspose.cells/cells/standardwidth/
---
## Cells.StandardWidth property

Obtient ou définit la largeur de colonne par défaut dans la feuille de calcul, en caractères.

```csharp
public double StandardWidth { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardWidthDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définir la largeur standard pour les colonnes
            cells.StandardWidth = 18.25;

            // Afficher la largeur standard et la largeur réelle de la première colonne
            Console.WriteLine("Standard Width: " + cells.StandardWidth);
            Console.WriteLine("Column 0 Width: " + cells.GetColumnWidth(0));

            // Vérifier que la largeur standard est appliquée (approximativement)
            if (Math.Abs(cells.GetColumnWidth(0) - cells.StandardWidth) > 1.0)
            {
                Console.WriteLine("Warning: Column width differs significantly from standard width");
            }
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


