---
title: "Shape.Characters"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Shape. Renvoie un objet Characters qui représente une plage de caractères dans le texte"
type: docs
url: /fr/net/aspose.cells.drawing/shape/characters/
---
## Shape.Characters method

Renvoie un objet Characters qui représente une plage de caractères dans le texte.

```csharp
public FontSetting Characters(int startIndex, int length)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| startIndex | Int32 | L'index du début du caractère. |
| longueur | Int32 | Le nombre de caractères. |

### Valeur de retour

Objet Characters.

### Remarques

Cette méthode ne fonctionne que sur une forme avec titre.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodCharactersWithInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme avec du texte
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);
            shape.Text = "Sample Text";

            // Obtenir les caractères à partir de l'index 0 avec une longueur de 4
            FontSetting fontSetting = shape.Characters(0, 4);
            
            // Modifier les paramètres de police
            fontSetting.Font.Color = System.Drawing.Color.Red;
            fontSetting.Font.Size = 14;
            fontSetting.Font.IsBold = true;

            // Enregistrez le classeur
            workbook.Save("ShapeCharactersDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


