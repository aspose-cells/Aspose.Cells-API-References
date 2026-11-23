---
title: "Border.Color"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Border. Obtient ou définit la couleur de la bordure"
type: docs
url: /fr/net/aspose.cells/border/color/
---
## Border.Color property

Obtient ou définit la couleur de la bordure.

```csharp
public Color Color { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class BorderPropertyColorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accéder à la cellule A1
            Cell cell = worksheet.Cells["A1"];
            
            // Définir la valeur de la cellule
            cell.PutValue("Border Color Demo");
            
            // Obtenir le style de la cellule
            Style style = cell.GetStyle();
            
            // Définir les couleurs et les styles de bordure
            style.Borders[BorderType.TopBorder].Color = Color.Red;
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            
            style.Borders[BorderType.BottomBorder].Color = Color.Blue;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dotted;
            
            style.Borders[BorderType.LeftBorder].Color = Color.Green;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dashed;
            
            style.Borders[BorderType.RightBorder].Color = Color.FromArgb(255, 128, 0); // Orange
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            
            // Appliquez le style à la cellule
            cell.SetStyle(style);
            
            // Enregistrez le classeur
            workbook.Save("BorderColorDemo.xlsx");
            
            Console.WriteLine("Border color demo created successfully.");
        }
    }
}
```

### Voir aussi

* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


