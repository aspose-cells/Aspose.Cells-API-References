---
title: "Style.HasBorders"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Style. Vérifie si des bordures ont été définies pour le style"
type: docs
url: /fr/net/aspose.cells/style/hasborders/
---
## Style.HasBorders property

Vérifie si des bordures ont été définies pour le style.

```csharp
public bool HasBorders { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyHasBordersDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Accéder à la cellule A1 et vérifier si elle possède des bordures (devrait être false par défaut)
            Cell cellA1 = cells["A1"];
            Console.WriteLine("Cell A1 has borders: " + cellA1.GetStyle().HasBorders);

            // Créer un style avec des bordures
            Style styleWithBorders = workbook.CreateStyle();
            styleWithBorders.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            styleWithBorders.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;

            // Appliquer le style à la cellule B1
            Cell cellB1 = cells["B1"];
            cellB1.SetStyle(styleWithBorders);

            // Vérifier si la cellule B1 possède des bordures (devrait être true maintenant)
            Console.WriteLine("Cell B1 has borders: " + cellB1.GetStyle().HasBorders);

            // Enregistrez le classeur
            workbook.Save("HasBordersDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


