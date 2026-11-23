---
title: "PivotTable.RowRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Retourne un objet CellArea qui représente la plage contenant la zone de lignes dans le rapport du tableau croisé dynamique. Lecture seule"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/rowrange/
---
## PivotTable.RowRange property

Renvoie un objet CellArea qui représente la plage contenant la zone de lignes dans le rapport du PivotTable. Lecture seule.

```csharp
public CellArea RowRange { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyRowRangeDemo
    {
        public static void Run()
        {
            // Créer un classeur à partir du fichier Excel source
            Workbook workbook = new Workbook("example.xlsx");
            
            // Rafraîchir tous les tableaux croisés dynamiques dans le classeur
            workbook.Worksheets.RefreshAll();
            
            // Obtenez le premier tableau croisé dynamique de la première feuille de calcul
            PivotTable pivotTable = workbook.Worksheets[0].PivotTables[0];
            
            // Obtenez la plage de lignes du tableau croisé dynamique
            CellArea rowRange = pivotTable.RowRange;
            
            // Affichez les coordonnées de la plage de lignes
            Console.WriteLine("PivotTable Row Range:");
            Console.WriteLine($"Start Row: {rowRange.StartRow}");
            Console.WriteLine($"End Row: {rowRange.EndRow}");
            Console.WriteLine($"Start Column: {rowRange.StartColumn}");
            Console.WriteLine($"End Column: {rowRange.EndColumn}");
            
            // Obtenez la plage de colonnes du tableau croisé dynamique
            CellArea columnRange = pivotTable.ColumnRange;
            
            // Affichez les coordonnées de la plage de colonnes
            Console.WriteLine("\nPivotTable Column Range:");
            Console.WriteLine($"Start Row: {columnRange.StartRow}");
            Console.WriteLine($"End Row: {columnRange.EndRow}");
            Console.WriteLine($"Start Column: {columnRange.StartColumn}");
            Console.WriteLine($"End Column: {columnRange.EndColumn}");
        }
    }
}
```

### Voir aussi

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


