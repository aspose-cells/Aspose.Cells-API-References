---
title: "Enum FontSchemeType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.FontSchemeType enum. Représente le type de schéma de la police"
type: docs
url: /fr/net/aspose.cells/fontschemetype/
---
## FontSchemeType enumeration

Représente le type de schéma de la police.

```csharp
public enum FontSchemeType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Aucun |
| Major | `1` | Schéma principal. |
| Minor | `2` | Schéma secondaire. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontSchemeTypeDemo
    {
        public static void FontSchemeTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            // Obtenez la référence de la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            // Accès à la cellule "A1" de la feuille de calcul
            Cell cell = worksheet.Cells["A1"];
            // Ajout d'une valeur à la cellule "A1"
            cell.PutValue("Hello Aspose!");

            // Accédez à la police du style de cellule
            Aspose.Cells.Font font = cell.GetStyle().Font;

            // Définition du type de schéma de police sur Principal
            font.SchemeType = FontSchemeType.Major;

            // Définition d'autres propriétés de police à des fins de démonstration
            font.Name = "Arial";
            font.Size = 14;
            font.Color = System.Drawing.Color.Blue;

            // Enregistrez le classeur
            workbook.Save("FontSchemeTypeExample.xlsx");
            workbook.Save("FontSchemeTypeExample.pdf");
            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


