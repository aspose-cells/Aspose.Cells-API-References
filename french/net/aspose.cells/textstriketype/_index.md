---
title: "Énumération TextStrikeType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.TextStrikeType. Ce type spécifie le type de barré"
type: docs
url: /fr/net/aspose.cells/textstriketype/
---
## TextStrikeType enumeration

Ce type spécifie le type de rayure.

```csharp
public enum TextStrikeType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Single | `0` | Un seul barré appliqué au texte. |
| Double | `1` | Un double barré appliqué au texte. Ne fonctionne que pour le texte des formes ou des graphiques. |
| None | `2` | Aucun barré n'est appliqué au texte. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TextStrikeTypeDemo
    {
        public static void TextStrikeTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            // Obtenez la référence de la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            // Accès à la cellule "A1" de la feuille de calcul
            Cell cell = worksheet.Cells["A1"];
            // Ajout d'une valeur à la cellule "A1"
            cell.PutValue("Hello Aspose!");

            // Accès à la police de la cellule
            Style style = cell.GetStyle();
            Font font = style.Font;

            // Définition du type de barré sur Simple
            font.StrikeType = TextStrikeType.Single;

            // Appliquez le style à la cellule
            cell.SetStyle(style);

            // Enregistrez le classeur
            workbook.Save("TextStrikeTypeExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


