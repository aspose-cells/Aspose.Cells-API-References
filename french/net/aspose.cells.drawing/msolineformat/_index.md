---
title: "Class MsoLineFormat"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.MsoLineFormat class. Représente le formatage des lignes et des pointes de flèche"
type: docs
url: /fr/net/aspose.cells.drawing/msolineformat/
---
## MsoLineFormat class

Représente le format des lignes et des pointes de flèche.

```csharp
public class MsoLineFormat
```

## Propriétés

| Nom | Description |
| --- | --- |
| [BackColor](../../aspose.cells.drawing/msolineformat/backcolor/) { get; set; } | Obtient et définit la couleur d'arrière-plan de la ligne de bordure. |
| [DashStyle](../../aspose.cells.drawing/msolineformat/dashstyle/) { get; set; } | Obtient ou définit le style de tiret pour la ligne spécifiée. |
| [ForeColor](../../aspose.cells.drawing/msolineformat/forecolor/) { get; set; } | Obtient et définit la couleur de premier plan de la ligne de bordure. |
| [IsVisible](../../aspose.cells.drawing/msolineformat/isvisible/) { get; set; } | Indique si l'objet est visible. |
| [Style](../../aspose.cells.drawing/msolineformat/style/) { get; set; } | Renvoie un objet Style qui représente le style de la plage spécifiée. |
| [Transparency](../../aspose.cells.drawing/msolineformat/transparency/) { get; set; } | Renvoie ou définit le degré de transparence du remplissage spécifié sous forme d'une valeur comprise entre 0.0 (opaque) et 1.0 (transparent). |
| [Weight](../../aspose.cells.drawing/msolineformat/weight/) { get; set; } | Renvoie ou définit l'épaisseur de la ligne, en unités de pt. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatDemo
    {
        public static void MsoLineFormatExample()
        {
            // Instanciez un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme d'arc à la feuille de calcul
            Aspose.Cells.Drawing.ArcShape arcShape = worksheet.Shapes.AddArc(2, 0, 2, 0, 130, 130);

            // Obtenez l'objet MsoLineFormat à partir de la forme
            MsoLineFormat lineFormat = arcShape.LineFormat;

            // Définissez les propriétés de l'objet MsoLineFormat
            lineFormat.IsVisible = true;
            lineFormat.Style = MsoLineStyle.ThickThin;
            lineFormat.ForeColor = Color.Red;
            lineFormat.BackColor = Color.Blue;
            lineFormat.DashStyle = MsoLineDashStyle.Solid;
            lineFormat.Transparency = 0.5;
            lineFormat.Weight = 2.0;

            // Enregistrez le classeur
            workbook.Save("MsoLineFormatExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


