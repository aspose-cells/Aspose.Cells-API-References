---
title: "MsoLineFormat.Style"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MsoLineFormat. Retourne un objet Style qui représente le style de la plage spécifiée"
type: docs
url: /fr/net/aspose.cells.drawing/msolineformat/style/
---
## MsoLineFormat.Style property

Renvoie un objet Style qui représente le style de la plage spécifiée.

```csharp
public MsoLineStyle Style { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyStyleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme de ligne
            Aspose.Cells.Drawing.LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 150, 10, 10);

            // Obtenir le format de ligne
            MsoLineFormat lineFormat = line.LineFormat;

            // Définir les propriétés du style de ligne
            lineFormat.Style = MsoLineStyle.ThickBetweenThin;
            lineFormat.ForeColor = System.Drawing.Color.Red;
            lineFormat.BackColor = System.Drawing.Color.White;
            lineFormat.DashStyle = MsoLineDashStyle.DashDotDot;
            lineFormat.Transparency = 0.5;
            lineFormat.Weight = 3.0;

            // Créer une autre ligne pour comparaison
            Aspose.Cells.Drawing.LineShape line2 = worksheet.Shapes.AddLine(5, 25, 100, 150, 10, 10);
            MsoLineFormat lineFormat2 = line2.LineFormat;

            // Copier le style de la première ligne vers la deuxième ligne
            lineFormat2.Style = lineFormat.Style;
            lineFormat2.ForeColor = lineFormat.ForeColor;
            lineFormat2.BackColor = lineFormat.BackColor;
            lineFormat2.DashStyle = lineFormat.DashStyle;
            lineFormat2.Transparency = lineFormat.Transparency;
            lineFormat2.Weight = lineFormat.Weight;

            // Enregistrez le classeur
            workbook.Save("MsoLineFormatStyleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [MsoLineStyle](../../msolinestyle/)
* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


