---
title: "Cells.MinDataColumn"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cells. Index de colonne minimum de la cellule qui contient des données"
type: docs
url: /fr/net/aspose.cells/cells/mindatacolumn/
---
## Cells.MinDataColumn property

Indice de colonne minimal de la cellule contenant des données.

```csharp
public int MinDataColumn { get; }
```

### Remarques

-1 will be returned if there is no cell which contains data. This property needs to iterate and check all cells in a worksheet dynamically, so it is a time-consumed progress and should not be invoked repeatedly, such as using it directly as condition in a loop.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMinDataColumnDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Ajoutez des données aux cellules (en commençant par la colonne 2)
            cells["B1"].PutValue("Header1");
            cells["C2"].PutValue("Data1");
            cells["D3"].PutValue("Data2");
            cells["E4"].PutValue("Data3");
            
            // Obtenez l’indice de colonne minimal qui contient des données
            int minDataColumn = cells.MinDataColumn;
            
            // Afficher le résultat
            Console.WriteLine("Minimum data column index: " + minDataColumn);
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


