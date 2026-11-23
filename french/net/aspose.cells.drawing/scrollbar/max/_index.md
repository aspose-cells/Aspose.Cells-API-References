---
title: "ScrollBar.Max"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ScrollBar. Obtient ou définit la valeur maximale de la plage d’une barre de défilement ou d’un sélecteur"
type: docs
url: /fr/net/aspose.cells.drawing/scrollbar/max/
---
## ScrollBar.Max property

Obtient ou définit la valeur maximale de la plage d'une barre de défilement ou d'un sélecteur.

```csharp
public int Max { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyMaxDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une barre de défilement à la feuille de calcul
            Aspose.Cells.Drawing.ScrollBar scrollBar = (Aspose.Cells.Drawing.ScrollBar)worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);

            // Définir les propriétés de la barre de défilement
            scrollBar.Min = 0;
            scrollBar.Max = 100; // Demonstrating Max property usage
            scrollBar.CurrentValue = 50;
            scrollBar.IncrementalChange = 5;
            scrollBar.PageChange = 10;

            // Enregistrez le classeur
            workbook.Save("ScrollBarMaxDemo.xlsx");

            // Afficher les informations
            Console.WriteLine("ScrollBar created with Max value: " + scrollBar.Max.ToString());
            Console.WriteLine("File saved successfully.");
        }
    }
}
```

### Voir aussi

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


