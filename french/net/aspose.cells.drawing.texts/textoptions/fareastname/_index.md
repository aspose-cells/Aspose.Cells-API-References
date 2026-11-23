---
title: "TextOptions.FarEastName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextOptions. Obtient et définit le nom FarEast"
type: docs
url: /fr/net/aspose.cells.drawing.texts/textoptions/fareastname/
---
## TextOptions.FarEastName property

Obtient et définit le nom FarEast.

```csharp
public string FarEastName { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextOptionsPropertyFarEastNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme et définissez la police FarEastName
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            shape.Text = "Sample Text";
            shape.TextOptions.FarEastName = "宋体";

            // Enregistrez et rechargez pour vérifier
            string outputPath = "output_FarEastName.xlsx";
            workbook.Save(outputPath);

            // Recharger pour vérifier
            Workbook verifyWorkbook = new Workbook(outputPath);
            Aspose.Cells.Drawing.Shape verifyShape = verifyWorkbook.Worksheets[0].Shapes[0];
            Console.WriteLine("FarEastName: " + verifyShape.TextOptions.FarEastName);
        }
    }
}
```

### Voir aussi

* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


