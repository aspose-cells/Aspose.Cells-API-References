---
title: "Style.Borders"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Style. Obtient le BorderCollection du style"
type: docs
url: /fr/net/aspose.cells/style/borders/
---
## Style.Borders property

Obtient le [`BorderCollection`](../../bordercollection/) du style.

```csharp
public BorderCollection Borders { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyBordersDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtenir la cellule et son style
            Cell cell = worksheet.Cells["A1"];
            Style style = cell.GetStyle();
            
            // Définir différents styles de bordure
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Medium;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dashed;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dotted;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thick;
            
            // Appliquez le style à la cellule
            cell.SetStyle(style);
            
            // Enregistrez le classeur
            workbook.Save("BorderStylesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [BorderCollection](../../bordercollection/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


