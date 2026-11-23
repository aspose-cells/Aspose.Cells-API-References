---
title: "Shape.LineFormat"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Renvoie un objet MsoLineFormat qui contient les propriétés de formatage de ligne pour la forme spécifiée"
type: docs
url: /fr/net/aspose.cells.drawing/shape/lineformat/
---
## Shape.LineFormat property

Renvoie un objet MsoLineFormat qui contient les propriétés de formatage de ligne pour la forme spécifiée.

```csharp
[Obsolete("Use Shape.Line property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MsoLineFormat LineFormat { get; }
```

### Remarques

NOTE: Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété Shape.Line. Cette propriété sera supprimée 12 mois après juillet 2016. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLineFormatDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajoutez une forme rectangle à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            RectangleShape rectangle = worksheet.Shapes.AddRectangle(3, 0, 2, 0, 70, 130);
            
            // Définir les propriétés de la forme
            rectangle.Placement = PlacementType.FreeFloating;
            rectangle.Fill.FillType = FillType.Solid;
            rectangle.Fill.SolidFill.Color = System.Drawing.Color.Blue;
            
            // Démontrez l'utilisation de LineFormat
            rectangle.LineFormat.Weight = 3; // Set line weight
            rectangle.LineFormat.DashStyle = MsoLineDashStyle.Solid;
            rectangle.Line.SolidFill.Color = System.Drawing.Color.DarkBlue; // Correct way to set line color
            
            // Enregistrez le classeur
            workbook.Save("ShapeLineFormatDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [MsoLineFormat](../../msolineformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


