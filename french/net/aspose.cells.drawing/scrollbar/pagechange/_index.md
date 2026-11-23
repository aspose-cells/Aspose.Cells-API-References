---
title: "ScrollBar.PageChange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ScrollBar. Obtient ou définit le changement de page"
type: docs
url: /fr/net/aspose.cells.drawing/scrollbar/pagechange/
---
## ScrollBar.PageChange property

Obtient ou définit le changement de page

```csharp
public int PageChange { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyPageChangeDemo
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
            scrollBar.IncrementalChange = 1;
            scrollBar.PageChange = 10; // Demonstrate PageChange property
            scrollBar.LinkedCell = "A1";

            // Enregistrez le classeur
            workbook.Save("ScrollBarPropertyPageChangeDemo.xlsx");

            // Chargez le classeur enregistré pour vérifier les propriétés
            Workbook verifyWorkbook = new Workbook("ScrollBarPropertyPageChangeDemo.xlsx");
            ScrollBar verifyScrollBar = (ScrollBar)verifyWorkbook.Worksheets[0].Shapes[0];

            // Afficher la valeur de la propriété PageChange pour démontrer qu’elle a été enregistrée/chargée correctement
            Console.WriteLine("ScrollBar PageChange value: " + verifyScrollBar.PageChange);
        }
    }
}
```

### Voir aussi

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


