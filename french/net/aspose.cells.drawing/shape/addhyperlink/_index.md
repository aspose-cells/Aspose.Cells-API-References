---
title: "Shape.AddHyperlink"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Shape. Ajoute un hyperlien à la forme"
type: docs
url: /fr/net/aspose.cells.drawing/shape/addhyperlink/
---
## Shape.AddHyperlink method

Ajoute un hyperlien à la forme.

```csharp
public Hyperlink AddHyperlink(string address)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| address | String | Adresse de l'hyperlien. |

### Valeur de retour

Renvoie le nouvel objet hyperlien.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodAddHyperlinkWithStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme à la feuille de calcul
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Ajouter un hyperlien à la forme en utilisant une URL sous forme de chaîne
            Aspose.Cells.Hyperlink hyperlink = shape.AddHyperlink("https://www.aspose.com/");

            // Enregistrez le classeur
            workbook.Save("ShapeWithHyperlink.xlsx");
        }
    }
}
```

### Voir aussi

* class [Hyperlink](../../../aspose.cells/hyperlink/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


