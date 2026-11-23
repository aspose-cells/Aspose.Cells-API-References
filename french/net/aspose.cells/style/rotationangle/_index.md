---
title: "Style.RotationAngle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Style. Représente l'angle de rotation du texte"
type: docs
url: /fr/net/aspose.cells/style/rotationangle/
---
## Style.RotationAngle property

Représente l'angle de rotation du texte.

```csharp
public int RotationAngle { get; set; }
```

### Remarques

0 : Non tourné.

255 : De haut en bas.

-90: Downward.

90 : Vers le haut.

Vous pouvez définir 255 ou une valeur comprise entre -90 et 90.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyRotationAngleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créez un style avec différents angles de rotation
            Style style1 = workbook.CreateStyle();
            style1.RotationAngle = -90;
            worksheet.Cells["B2"].PutValue("Text rotated -90°");
            worksheet.Cells["B2"].SetStyle(style1);

            Style style2 = workbook.CreateStyle();
            style2.RotationAngle = 90;
            worksheet.Cells["C3"].PutValue("Text rotated 90°");
            worksheet.Cells["C3"].SetStyle(style2);

            Style style3 = workbook.CreateStyle();
            style3.RotationAngle = 255;
            worksheet.Cells["D4"].PutValue("Text rotated 255°");
            worksheet.Cells["D4"].SetStyle(style3);

            // Enregistrez le classeur
            workbook.Save("output_rotation_angles.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


