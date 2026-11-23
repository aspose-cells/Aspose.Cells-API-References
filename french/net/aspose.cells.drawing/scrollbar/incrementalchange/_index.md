---
title: "ScrollBar.IncrementalChange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ScrollBar. Obtient ou définit la quantité d’incrémentation de la barre de défilement ou du sélecteur lors d’un défilement d’une ligne"
type: docs
url: /fr/net/aspose.cells.drawing/scrollbar/incrementalchange/
---
## ScrollBar.IncrementalChange property

Obtient ou définit la quantité d'incrémentation d'une ligne de la barre de défilement ou du sélecteur.

```csharp
public int IncrementalChange { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyIncrementalChangeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une barre de défilement à la feuille de calcul
            ScrollBar scrollBar = worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);

            // Définir les propriétés de la barre de défilement
            scrollBar.Min = 0;
            scrollBar.Max = 100;
            scrollBar.CurrentValue = 50;
            scrollBar.IncrementalChange = 5; // This is the key property we're demonstrating
            scrollBar.PageChange = 20;

            // Afficher les propriétés de la barre de défilement
            Console.WriteLine("Scroll Bar Properties:");
            Console.WriteLine("Min: " + scrollBar.Min);
            Console.WriteLine("Max: " + scrollBar.Max);
            Console.WriteLine("Current Value: " + scrollBar.CurrentValue);
            Console.WriteLine("Incremental Change: " + scrollBar.IncrementalChange);
            Console.WriteLine("Page Change: " + scrollBar.PageChange);

            // Modifier le changement incrémental
            scrollBar.IncrementalChange = 10;
            Console.WriteLine("\nModified Incremental Change: " + scrollBar.IncrementalChange);

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


