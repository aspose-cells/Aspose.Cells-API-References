---
title: "Font.IsNormalizeHeights"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Font. Indique si la normalisation de la hauteur doit être appliquée à la séquence de texte"
type: docs
url: /fr/net/aspose.cells/font/isnormalizeheights/
---
## Font.IsNormalizeHeights property

Indique si la normalisation de la hauteur doit être appliquée à la séquence de texte.

```csharp
[Obsolete("Use TextOptions.IsNormalizeHeights property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsNormalizeHeights { get; set; }
```

### Remarques

Uniquement pour les polices des Formes ou des Graphiques. NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété [`IsNormalizeHeights`](../../../aspose.cells.drawing.texts/textoptions/isnormalizeheights/). Cette propriété sera supprimée 12 mois plus tard, à partir de janvier 2026. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsNormalizeHeightsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Style style = workbook.CreateStyle();
            Font font = style.Font;

            // Définir la propriété IsNormalizeHeights
            font.IsNormalizeHeights = true;
            Console.WriteLine("Font IsNormalizeHeights: " + font.IsNormalizeHeights);

            // Appliquer le style à une cellule
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Test Text");

            // Vérifier la propriété
            Font cellFont = cell.GetStyle().Font;
            Console.WriteLine("Cell Font IsNormalizeHeights: " + cellFont.IsNormalizeHeights);

            // Modifier la propriété
            cellFont.IsNormalizeHeights = false;
            Console.WriteLine("Modified Cell Font IsNormalizeHeights: " + cellFont.IsNormalizeHeights);
        }
    }
}
```

### Voir aussi

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


