---
title: "Border.LineStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Border. Obtient ou définit le type de bordure de la cellule"
type: docs
url: /fr/net/aspose.cells/border/linestyle/
---
## Border.LineStyle property

Obtient ou définit le type de bordure de la cellule.

```csharp
public CellBorderType LineStyle { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BorderPropertyLineStyleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accéder à une cellule et obtenir son style
            Cell cell = worksheet.Cells["B2"];
            Style style = cell.GetStyle();

            // Définir différents styles de ligne de bordure
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dashed;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dotted;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Double;

            // Appliquez le style à la cellule
            cell.SetStyle(style);

            // Enregistrez le classeur
            workbook.Save("BorderLineStyleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [CellBorderType](../../cellbordertype/)
* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


