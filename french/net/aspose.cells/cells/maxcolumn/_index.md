---
title: "Cells.MaxColumn"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cells. Indice de colonne maximal des cellules qui ont été instanciées dans la collection ne comprend pas la colonne où le style est défini pour toute la colonne mais aucune cellule n’a été instanciée dans celle‑ci."
type: docs
url: /fr/net/aspose.cells/cells/maxcolumn/
---
## Cells.MaxColumn property

Indice de colonne maximal des cellules qui ont été instanciées dans la collection (n'inclut pas la colonne où le style est défini pour toute la colonne mais aucune cellule n'a été instanciée).

```csharp
public int MaxColumn { get; }
```

### Remarques

Retournez -1 s’il n’y a aucune cellule instanciée.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMaxColumnDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données aux cellules
            worksheet.Cells["A1"].PutValue("Column A");
            worksheet.Cells["B1"].PutValue("Column B");
            worksheet.Cells["C1"].PutValue("Column C");
            
            // Obtenez l’indice de colonne maximal contenant des données
            int maxColumn = worksheet.Cells.MaxColumn;
            Console.WriteLine("Max column with data: " + maxColumn);

            // Ajoutez des données à la colonne suivante après la colonne maximale
            worksheet.Cells[0, maxColumn + 1].PutValue("Next Column");

            // Vérifiez la nouvelle colonne maximale
            Console.WriteLine("New max column: " + worksheet.Cells.MaxColumn);

            // Créez une autre feuille de calcul pour démontrer la copie
            Worksheet destSheet = workbook.Worksheets.Add("Destination");

            // Copiez toutes les colonnes de la source vers la destination
            destSheet.Cells.CopyColumns(worksheet.Cells, 0, 0, worksheet.Cells.MaxColumn + 1);

            Console.WriteLine("Columns copied successfully");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


