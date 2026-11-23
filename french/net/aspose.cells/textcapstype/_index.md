---
title: "Enumération TextCapsType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.TextCapsType enum. Ce type spécifie les types de majuscules du texte"
type: docs
url: /fr/net/aspose.cells/textcapstype/
---
## TextCapsType enumeration

Ce type spécifie les types de majuscules du texte.

```csharp
public enum TextCapsType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Pas de majuscules |
| All | `1` | Appliquer toutes les majuscules au texte. |
| Small | `2` | Appliquer des petites majuscules au texte. |

### Remarques

Peut uniquement être appliqué aux graphiques et aux formes.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TextCapsTypeDemo
    {
        public static void TextCapsTypeExample()
        {
            // Code supplémentaire pour démontrer comment l'instance peut être utilisée
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir la valeur d'une cellule
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Hello Aspose!");

            // Obtenir le style de la cellule
            Style style = cell.GetStyle();

            // Définir le type de majuscules de la police sur All Caps
            style.Font.CapsType = Aspose.Cells.TextCapsType.All;

            // Appliquez le style à la cellule
            cell.SetStyle(style);

            // Enregistrez le classeur
            workbook.Save("TextCapsTypeExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


