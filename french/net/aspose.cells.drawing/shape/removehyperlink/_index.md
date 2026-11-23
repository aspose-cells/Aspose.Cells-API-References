---
title: "Shape.RemoveHyperlink"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Shape. Supprime le lien hypertexte de la forme"
type: docs
url: /fr/net/aspose.cells.drawing/shape/removehyperlink/
---
## Shape.RemoveHyperlink method

Supprime le lien hypertexte de la forme.

```csharp
public void RemoveHyperlink()
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodRemoveHyperlinkDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme et définir le lien hypertexte
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 50);
            shape.AddHyperlink("https://www.aspose.com");

            // Supprimer le lien hypertexte
            shape.RemoveHyperlink();

            // Vérifier que le lien hypertexte est supprimé
            Console.WriteLine("Hyperlink removed: " + (shape.Hyperlink == null));

            // Enregistrez le classeur
            workbook.Save("ShapeRemoveHyperlinkDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


