---
title: "Cell.GetMergedRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cell. Retourne un objet Range qui représente une plage fusionnée"
type: docs
url: /fr/net/aspose.cells/cell/getmergedrange/
---
## Cell.GetMergedRange method

Retourne un objet [`Range`](../../range/) qui représente une plage fusionnée.

```csharp
public Range GetMergedRange()
```

### Valeur de retour

[`Range`](../../range/) object. Null if this cell is not merged.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetMergedRangeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Fusionner des cellules
            cells.Merge(0, 0, 2, 2);

            // Obtenir la première cellule
            Cell cell = cells[0, 0];

            // Obtenir les informations de la plage fusionnée
            Aspose.Cells.Range mergedRange = cell.GetMergedRange();
            
            // Afficher les détails de la plage fusionnée
            Console.WriteLine("Merged Range Details:");
            Console.WriteLine($"First Row: {mergedRange.FirstRow}");
            Console.WriteLine($"First Column: {mergedRange.FirstColumn}");
            Console.WriteLine($"Row Count: {mergedRange.RowCount}");
            Console.WriteLine($"Column Count: {mergedRange.ColumnCount}");
        }
    }
}
```

### Voir aussi

* class [Range](../../range/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


