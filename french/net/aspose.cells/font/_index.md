---
title: "Classe Font"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Font. Encapsule l'objet police utilisé dans une feuille de calcul"
type: docs
url: /fr/net/aspose.cells/font/
---
## Font class

Encapsule l'objet de police utilisé dans une feuille de calcul.

```csharp
public class Font
```

## Propriétés

| Nom | Description |
| --- | --- |
| [ArgbColor](../../aspose.cells/font/argbcolor/) { get; set; } | Obtient et définit la couleur avec une valeur ARGB 32 bits. |
| [CapsType](../../aspose.cells/font/capstype/) { get; set; } | (**Obsolete.**) Obtient et définit le type de majuscules du texte. |
| [Charset](../../aspose.cells/font/charset/) { get; set; } | Représente le jeu de caractères. |
| [Color](../../aspose.cells/font/color/) { get; set; } | Obtient ou définit la couleur de la police. |
| [DoubleSize](../../aspose.cells/font/doublesize/) { get; set; } | Obtient et définit la double taille de la police. |
| [IsBold](../../aspose.cells/font/isbold/) { get; set; } | Obtient ou définit une valeur indiquant si la police est en gras. |
| [IsItalic](../../aspose.cells/font/isitalic/) { get; set; } | Obtient ou définit une valeur indiquant si la police est en italique. |
| [IsNormalizeHeights](../../aspose.cells/font/isnormalizeheights/) { get; set; } | (**Obsolete.**) Indique si la normalisation de la hauteur doit être appliquée à la séquence de texte. |
| [IsStrikeout](../../aspose.cells/font/isstrikeout/) { get; set; } | Obtient ou définit une valeur indiquant si la police est à simple rature. |
| [IsSubscript](../../aspose.cells/font/issubscript/) { get; set; } | Obtient ou définit une valeur indiquant si la police est en indice. |
| [IsSuperscript](../../aspose.cells/font/issuperscript/) { get; set; } | Obtient ou définit une valeur indiquant si la police est en exposant. |
| virtual [Name](../../aspose.cells/font/name/) { get; set; } | Obtient ou définit le nom du `Font`. |
| [SchemeType](../../aspose.cells/font/schemetype/) { get; set; } | Obtient et définit le type de schéma de la police. |
| [ScriptOffset](../../aspose.cells/font/scriptoffset/) { get; set; } | Obtient et définit le décalage de script, en unité de pourcentage |
| [Size](../../aspose.cells/font/size/) { get; set; } | Obtient ou définit la taille de la police. |
| [StrikeType](../../aspose.cells/font/striketype/) { get; set; } | Obtient le type de rature du texte. |
| [ThemeColor](../../aspose.cells/font/themecolor/) { get; set; } | Obtient et définit la couleur du thème. |
| [Underline](../../aspose.cells/font/underline/) { get; set; } | Obtient ou définit le type de soulignement de la police. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Equals](../../aspose.cells/font/equals/#equals)(Font) | Vérifie si deux polices sont égales. |
| [SetName](../../aspose.cells/font/setname/)(string, FontSchemeType) | Définit le nom et le schéma de la police. |
| override [ToString](../../aspose.cells/font/tostring/)() | Renvoie une chaîne qui représente l'objet Cell actuel. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class FontDemo
    {
        public static void FontExample()
        {
            // Instanciation d'un objet Workbook
            Workbook workbook = new Workbook();

            // Obtention de la référence de la feuille de calcul nouvellement ajoutée en passant son indice de feuille
            Worksheet worksheet = workbook.Worksheets[0];

            // Accès à la cellule "A1" de la feuille de calcul
            Aspose.Cells.Cell cell = worksheet.Cells["A1"];

            // Ajout d'une valeur à la cellule "A1"
            cell.PutValue("Hello Aspose!");

            // Accéder à l'objet police du style de cellule
            Aspose.Cells.Font font = cell.GetStyle().Font;

            // Définition du nom de la police à "Times New Roman"
            font.Name = "Times New Roman";

            // Définition de la taille de la police à 14
            font.Size = 14;

            // Définition de la couleur de la police en rouge
            font.Color = Color.Red;

            // Définition des propriétés supplémentaires de la police
            font.IsBold = true;
            font.IsItalic = true;
            font.Underline = FontUnderlineType.Single;
            font.IsStrikeout = false;
            font.IsSuperscript = false;
            font.IsSubscript = false;
            font.Charset = 1;
            font.CapsType = TextCapsType.None;
            font.StrikeType = TextStrikeType.None;
            font.ScriptOffset = 0;
            font.DoubleSize = 14.0;
            font.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);
            font.ArgbColor = Color.Red.ToArgb();
            font.IsNormalizeHeights = false;
            font.SchemeType = FontSchemeType.None;

            // Enregistrement du fichier Excel
            workbook.Save("FontExample.xlsx");
            workbook.Save("FontExample.pdf");
            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


