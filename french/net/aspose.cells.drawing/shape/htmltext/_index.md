---
title: "Shape.HtmlText"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Obtient et définit la chaîne html qui contient des données et certains formats dans cette zone de texte"
type: docs
url: /fr/net/aspose.cells.drawing/shape/htmltext/
---
## Shape.HtmlText property

Obtient et définit la chaîne html qui contient des données et certains formats dans cette zone de texte.

```csharp
public string HtmlText { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHtmlTextDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme à la feuille de calcul
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // Vérifiez si HtmlText est vide et définissez-le si nécessaire
            string html = shape.HtmlText;
            if (string.IsNullOrEmpty(html))
            {
                shape.HtmlText = "<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>";
            }

            // Enregistrez le classeur
            workbook.Save("ShapeHtmlTextDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


