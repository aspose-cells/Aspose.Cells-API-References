---
title: "Cells.LastCell"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cells. Obtient la dernière cellule de cette feuille de calcul"
type: docs
url: /fr/net/aspose.cells/cells/lastcell/
---
## Cells.LastCell property

Obtient la dernière cellule de cette feuille de calcul.

```csharp
public Cell LastCell { get; }
```

### Remarques

Renvoie null s'il n'y a aucune donnée dans la feuille de calcul.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyLastCellDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplissez quelques données
            worksheet.Cells["A1"].Value = "Header1";
            worksheet.Cells["B1"].Value = "Header2";
            worksheet.Cells["A2"].Value = "Data1";
            worksheet.Cells["B2"].Value = "Data2";

            // Obtenir l'adresse de la dernière cellule
            Cell lastCell = worksheet.Cells.LastCell;
            Console.WriteLine("Last cell address: " + lastCell.Name);

            // Créer une plage de la première à la dernière cellule
            Aspose.Cells.Range fullRange = worksheet.Cells.CreateRange(
                worksheet.Cells.FirstCell.Name, 
                lastCell.Name);
            
            // Appliquez le formatage à la plage
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            fullRange.ApplyStyle(style, new StyleFlag { FontBold = true });

            // Enregistrez le classeur
            workbook.Save("LastCellDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


