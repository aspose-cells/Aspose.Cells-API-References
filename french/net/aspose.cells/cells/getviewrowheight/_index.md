---
title: "Cells.GetViewRowHeight"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Obtient la hauteur d'une ligne spécifiée"
type: docs
url: /fr/net/aspose.cells/cells/getviewrowheight/
---
## Cells.GetViewRowHeight method

Obtient la hauteur d'une ligne spécifiée.

```csharp
public double GetViewRowHeight(int row)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | Index de ligne. |

### Valeur de retour

Hauteur de la ligne.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetViewRowHeightWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir la hauteur de la ligne 3 (en points)
            worksheet.Cells.SetRowHeight(3, 15);
            
            // Obtenir la hauteur de la ligne affichée pour la ligne 3
            double viewRowHeight = worksheet.Cells.GetViewRowHeight(3);
            
            // Afficher le résultat
            Console.WriteLine("View Row Height for row 3: " + viewRowHeight);
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


