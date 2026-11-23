---
title: "Cells.FirstCell"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cells. Obtient la première cellule de cette feuille de calcul"
type: docs
url: /fr/net/aspose.cells/cells/firstcell/
---
## Cells.FirstCell property

Obtient la première cellule de cette feuille de calcul.

```csharp
public Cell FirstCell { get; }
```

### Remarques

Renvoie null s'il n'y a aucune donnée dans la feuille de calcul.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class CellsPropertyFirstCellDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B3"].PutValue(2000);
            
            // Obtenir la collection de cellules
            Cells cells = worksheet.Cells;
            
            // Démontrer la propriété FirstCell
            Cell firstCell = cells.FirstCell;
            Console.WriteLine($"First cell address: {firstCell.Name}");
            Console.WriteLine($"First cell value: {firstCell.Value}");
            
            // Créer un graphique en utilisant FirstCell et LastCell
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange($"{cells.FirstCell.Name}:{cells.LastCell.Name}", true);
            chart.ShowLegend = true;
            
            // Enregistrez le classeur
            workbook.Save("FirstCellDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


