---
title: "Classe Outline"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Outline. Représente un plan sur une feuille de calcul"
type: docs
url: /fr/net/aspose.cells/outline/
---
## Outline class

Représente un contour sur une feuille de calcul.

```csharp
public class Outline
```

## Propriétés

| Nom | Description |
| --- | --- |
| [SummaryColumnRight](../../aspose.cells/outline/summarycolumnright/) { get; set; } | Indique si la colonne de synthèse sera positionnée à droite des colonnes de détail dans le plan. |
| [SummaryRowBelow](../../aspose.cells/outline/summaryrowbelow/) { get; set; } | Indique si la ligne de synthèse sera positionnée sous les lignes de détail dans le plan. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OutlineDemo
    {
        public static void OutlineExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accédez à la première feuille de calcul du classeur
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accédez au plan de la feuille de calcul
            Outline outline = worksheet.Outline;
            
            // Définissez les propriétés du plan
            outline.SummaryRowBelow = true; // Indicates if the summary row will be positioned below the detail rows
            outline.SummaryColumnRight = true; // Indicates if the summary column will be positioned to the right of the detail columns
            
            // Enregistrez le classeur
            workbook.Save("OutlineExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


