---
title: "Cell.IsStyleSet"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cell. Indique si le style de la cellule est défini. Si renvoie false, cela signifie que cette cellule a un format de cellule par défaut"
type: docs
url: /fr/net/aspose.cells/cell/isstyleset/
---
## Cell.IsStyleSet property

Indique si le style de la cellule est défini. Si la valeur retournée est false, cela signifie que cette cellule utilise le format de cellule par défaut.

```csharp
public bool IsStyleSet { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsStyleSetDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Accédez à une cellule qui n'a pas encore été stylisée
            Cell unsetStyleCell = cells["A1"];
            Console.WriteLine($"Cell A1 IsStyleSet before styling: {unsetStyleCell.IsStyleSet}");

            // Stylisez une autre cellule
            Cell styledCell = cells["B2"];
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            styledCell.SetStyle(style);

            Console.WriteLine($"Cell B2 IsStyleSet after styling: {styledCell.IsStyleSet}");

            // Vérifiez si le style est hérité de la ligne
            Row row = cells.Rows[4];
            row.SetStyle(style);
            Cell rowInheritedCell = cells["E4"];
            Console.WriteLine($"Cell E4 IsStyleSet (inherited from row): {rowInheritedCell.IsStyleSet}");

            // Définir explicitement le style sur null pour une cellule
            Cell nullStyleCell = cells["C3"];
            nullStyleCell.SetStyle(null);
            Console.WriteLine($"Cell C3 IsStyleSet after setting null: {nullStyleCell.IsStyleSet}");
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


