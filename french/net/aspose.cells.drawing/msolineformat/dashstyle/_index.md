---
title: "MsoLineFormat.DashStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MsoLineFormat. Obtient ou définit le style de tiret pour la ligne spécifiée"
type: docs
url: /fr/net/aspose.cells.drawing/msolineformat/dashstyle/
---
## MsoLineFormat.DashStyle property

Obtient ou définit le style de tiret pour la ligne spécifiée.

```csharp
public MsoLineDashStyle DashStyle { get; set; }
```

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyDashStyleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une forme pour démontrer DashStyle
            Shape shape = workbook.Worksheets[0].Shapes.AddRectangle(1, 0, 1, 0, 200, 100);

            // Définir les propriétés de la ligne
            shape.LineFormat.Style = MsoLineStyle.Single;
            shape.LineFormat.Weight = 3;
            shape.LineFormat.ForeColor = Color.Blue;

            // Démontrer différents styles de tiret
            shape.LineFormat.DashStyle = MsoLineDashStyle.Solid;
            shape.Text = "Solid Line";

            // Ajouter une autre forme avec un style de tiret différent
            Shape shape2 = workbook.Worksheets[0].Shapes.AddRectangle(1, 0, 3, 0, 200, 100);
            shape2.LineFormat.Style = MsoLineStyle.Single;
            shape2.LineFormat.Weight = 3;
            shape2.LineFormat.ForeColor = Color.Red;
            shape2.LineFormat.DashStyle = MsoLineDashStyle.DashDotDot;
            shape2.Text = "DashDotDot Line";

            // Enregistrez le classeur
            workbook.Save("LineDashStyleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [MsoLineDashStyle](../../msolinedashstyle/)
* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


