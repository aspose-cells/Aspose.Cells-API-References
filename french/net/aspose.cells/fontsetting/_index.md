---
title: "Classe FontSetting"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.FontSetting. Représente une plage de caractères dans le texte de la cellule"
type: docs
url: /fr/net/aspose.cells/fontsetting/
---
## FontSetting class

Représente une plage de caractères dans le texte de la cellule.

```csharp
public class FontSetting
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [FontSetting](fontsetting/)(int, int, WorksheetCollection) |  |

## Propriétés

| Nom | Description |
| --- | --- |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Renvoie la police de cet objet. |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Obtient la longueur des caractères. |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Obtient l'index de départ des caractères. |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Renvoie les options de texte. |
| virtual [Type](../../aspose.cells/fontsetting/type/) { get; } | Obtient le type de nœud de texte. |

## Méthodes

| Nom | Description |
| --- | --- |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle/)(PresetWordArtStyle) | Définit le style WordArt prédéfini. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class FontSettingDemo
    {
        public static void FontSettingExample()
        {
            // Instanciation d'un objet Workbook
            Workbook workbook = new Workbook();

            // Ajout d'une nouvelle feuille de calcul à l'objet Excel
            workbook.Worksheets.Add();

            // Obtention de la référence de la feuille de calcul nouvellement ajoutée en passant son indice de feuille
            Worksheet worksheet = workbook.Worksheets[0];

            // Accès à la cellule "A1" de la feuille de calcul
            Aspose.Cells.Cell cell = worksheet.Cells["A1"];

            // Ajout d'une valeur à la cellule "A1"
            cell.PutValue("Visit Aspose!");

            // Obtention de la plage de caractères
            FontSetting character = cell.Characters(6, 7);

            // Définir la police des caractères sélectionnés en gras
            character.Font.IsBold = true;

            // Définir la couleur de police des caractères sélectionnés en bleu
            character.Font.Color = Color.Blue;

            // Enregistrement du fichier Excel
            workbook.Save("FontSettingExample.xlsx");
            workbook.Save("FontSettingExample.pdf");

        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


