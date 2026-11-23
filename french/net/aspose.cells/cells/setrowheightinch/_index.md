---
title: "Cells.SetRowHeightInch"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Définit la hauteur de la ligne en pouces"
type: docs
url: /fr/net/aspose.cells/cells/setrowheightinch/
---
## Cells.SetRowHeightInch method

Définit la hauteur de la ligne en pouces.

```csharp
public void SetRowHeightInch(int row, double inches)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | Index de ligne. |
| pouces | Double | Nombre de pouces. Il doit être compris entre 0 et 409,5/72. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetRowHeightInchWithInt32DoubleDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définir le style par défaut
            Style style = workbook.DefaultStyle;
            style.Font.Name = "Tahoma";
            style.Font.Size = 16;
            style.Font.IsBold = true;
            workbook.DefaultStyle = style;

            // Définir la hauteur des lignes en pouces
            for (int i = 0; i < 10; i++)
            {
                cells.SetRowHeightInch(i, 0.5 + (i * 0.2)); // Demonstrates SetRowHeightInch(Int32, Double)
            }

            // Enregistrez le classeur
            workbook.Save("RowHeightsInInches.xlsx");
            
            Console.WriteLine("Row heights set successfully in inches.");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


