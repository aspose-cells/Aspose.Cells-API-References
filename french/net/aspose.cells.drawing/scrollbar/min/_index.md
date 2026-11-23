---
title: "ScrollBar.Min"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ScrollBar. Obtient ou définit la valeur minimale d'une plage de barre de défilement ou de spinner"
type: docs
url: /fr/net/aspose.cells.drawing/scrollbar/min/
---
## ScrollBar.Min property

Obtient ou définit la valeur minimale de la plage d'une barre de défilement ou d'un sélecteur

```csharp
public int Min { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyMinDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une barre de défilement à la feuille de calcul
            Aspose.Cells.Drawing.ScrollBar scrollBar = (Aspose.Cells.Drawing.ScrollBar)worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);

            // Définir les propriétés de la barre de défilement
            scrollBar.Min = 10;
            scrollBar.Max = 100;
            scrollBar.CurrentValue = 50;  // Changed from Value to CurrentValue
            scrollBar.IncrementalChange = 5;
            scrollBar.PageChange = 20;

            // Afficher la valeur de la propriété Min
            Console.WriteLine("ScrollBar Min Value: " + scrollBar.Min);

            // Enregistrez le classeur
            workbook.Save("ScrollBarMinDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


