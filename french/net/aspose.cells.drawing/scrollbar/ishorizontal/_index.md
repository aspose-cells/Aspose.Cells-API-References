---
title: "ScrollBar.IsHorizontal"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ScrollBar. Indique s'il s'agit d'une barre de défilement horizontale"
type: docs
url: /fr/net/aspose.cells.drawing/scrollbar/ishorizontal/
---
## ScrollBar.IsHorizontal property

Indique si c'est une barre de défilement horizontale.

```csharp
public bool IsHorizontal { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyIsHorizontalDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une barre de défilement horizontale
            Shape scrollBarShape = worksheet.Shapes.AddScrollBar(1, 0, 1, 0, 100, 20);
            ScrollBar scrollBar = (ScrollBar)scrollBarShape;
            scrollBar.IsHorizontal = true;

            // Ajouter une barre de défilement verticale pour comparaison
            Shape verticalScrollBarShape = worksheet.Shapes.AddScrollBar(1, 0, 1, 30, 20, 100);
            ScrollBar verticalScrollBar = (ScrollBar)verticalScrollBarShape;
            verticalScrollBar.IsHorizontal = false;

            // Démontrer la propriété IsHorizontal
            Console.WriteLine("Horizontal Scroll Bar IsHorizontal: " + scrollBar.IsHorizontal);
            Console.WriteLine("Vertical Scroll Bar IsHorizontal: " + verticalScrollBar.IsHorizontal);

            // Enregistrez le classeur
            workbook.Save("ScrollBarDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


