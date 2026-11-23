---
title: "Shape.GetRichFormattings"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Shape. Retourne tous les objets Characters qui représentent une plage de caractères dans le texte"
type: docs
url: /fr/net/aspose.cells.drawing/shape/getrichformattings/
---
## Shape.GetRichFormattings method

Retourne tous les objets Characters qui représentent une plage de caractères dans le texte .

```csharp
public FontSetting[] GetRichFormattings()
```

### Valeur de retour

Tous les objets Characters

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetRichFormattingsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme avec du texte enrichi (nombre correct de paramètres pour AddRectangle)
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);
            shape.Text = "This is bold and this is italic";
            
            // Formater des parties du texte
            shape.Characters(0, 4).Font.IsBold = true;
            shape.Characters(13, 6).Font.IsItalic = true;

            // Obtenir les mises en forme de texte enrichi
            FontSetting[] formattings = shape.GetRichFormattings();

            // Afficher les informations de mise en forme
            Console.WriteLine("Rich text formattings:");
            foreach (FontSetting setting in formattings)
            {
                Console.WriteLine($"Text segment: '{shape.Text.Substring(setting.StartIndex, setting.Length)}'");
                Console.WriteLine($"Start index: {setting.StartIndex}");
                Console.WriteLine($"Length: {setting.Length}");
                Console.WriteLine($"Bold: {setting.Font.IsBold}");
                Console.WriteLine($"Italic: {setting.Font.IsItalic}");
                Console.WriteLine();
            }
        }
    }
}
```

### Voir aussi

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


