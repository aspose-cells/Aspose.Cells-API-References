---
title: "Cells.GetRowHeightInch"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Obtient la hauteur d’une ligne spécifiée en unités de pouces"
type: docs
url: /fr/net/aspose.cells/cells/getrowheightinch/
---
## Cells.GetRowHeightInch method

Obtient la hauteur d'une ligne spécifiée en pouces.

```csharp
public double GetRowHeightInch(int row)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | Indice de ligne |

### Valeur de retour

Hauteur de la ligne

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetRowHeightInchWithInt32Demo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définir la hauteur de la ligne en pouces pour la ligne 5
            cells.SetRowHeightInch(5, 1.5);

            // Obtenir la hauteur de la ligne en pouces pour la ligne 5
            double rowHeight = cells.GetRowHeightInch(5);

            // Afficher le résultat
            Console.WriteLine("Row height in inches: " + rowHeight);
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


