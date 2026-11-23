---
title: "ShapeTextAlignment.Equals"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeTextAlignment. Détermine si cette instance a la même valeur qu'un autre objet ShapeTextAlignment spécifié"
type: docs
url: /fr/net/aspose.cells.drawing.texts/shapetextalignment/equals/
---
## ShapeTextAlignment.Equals method

Détermine si cette instance a la même valeur qu'un autre objet [`ShapeTextAlignment`](../) spécifié.

```csharp
public override bool Equals(object obj)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| obj | Object | L'objet [`ShapeTextAlignment`](../) à comparer avec cette instance. |

### Valeur de retour

true si la valeur du paramètre obj est identique à la valeur de cette instance ; sinon, false. Si obj est null, cette méthode renvoie false.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez une forme pour comparer l'alignement du texte
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;
            
            // Obtenez l'alignement du texte d'une autre forme pour comparaison
            Shape shape2 = worksheet.Shapes.AddRectangle(2, 0, 1, 0, 100, 100);
            ShapeTextAlignment obj = shape2.TextBody.TextAlignment;

            if (shapeTextAlignment.Equals((object)obj))
            {
                Console.WriteLine("Text alignments are equal");
            }
            else
            {
                Console.WriteLine("Text alignments are not equal");
            }
        }
    }
}
```

### Voir aussi

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


