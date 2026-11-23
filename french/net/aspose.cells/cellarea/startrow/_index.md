---
title: "CellArea.StartRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Champ CellArea. Obtient ou définit la ligne de départ de cette zone"
type: docs
url: /fr/net/aspose.cells/cellarea/startrow/
---
## CellArea.StartRow field

Obtient ou définit la ligne de départ de cette zone.

```csharp
public int StartRow;
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellAreaFieldStartRowDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer deux objets CellArea
            CellArea area1 = new CellArea();
            area1.StartRow = 2;
            area1.StartColumn = 1;
            area1.EndRow = 5;
            area1.EndColumn = 3;

            CellArea area2 = new CellArea();
            area2.StartRow = area1.StartRow; // Demonstrating StartRow usage
            area2.StartColumn = area1.StartColumn;
            area2.EndRow = area1.EndRow;
            area2.EndColumn = area1.EndColumn;

            // Vérifier que les zones correspondent
            if (area1.StartRow == area2.StartRow &&
                area1.StartColumn == area2.StartColumn &&
                area1.EndRow == area2.EndRow &&
                area1.EndColumn == area2.EndColumn)
            {
                Console.WriteLine("CellArea objects match successfully");
                Console.WriteLine($"StartRow: {area1.StartRow}");
            }
            else
            {
                Console.WriteLine("CellArea objects do not match");
            }
        }
    }
}
```

### Voir aussi

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


