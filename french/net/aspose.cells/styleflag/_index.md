---
title: "Classe StyleFlag"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.StyleFlag. Représente les indicateurs qui indiquent les propriétés de formatage appliquées"
type: docs
url: /fr/net/aspose.cells/styleflag/
---
## StyleFlag class

Représente les indicateurs qui indiquent les propriétés de formatage appliquées.

```csharp
public class StyleFlag
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [StyleFlag](styleflag/)() | Construit un objet avec tous les indicateurs à false. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Alignments](../../aspose.cells/styleflag/alignments/) { get; set; } | Le réglage d'alignement sera appliqué. |
| [All](../../aspose.cells/styleflag/all/) { get; set; } | Toutes les propriétés seront appliquées. |
| [Borders](../../aspose.cells/styleflag/borders/) { get; set; } | Tous les paramètres de bordure seront appliqués. |
| [BottomBorder](../../aspose.cells/styleflag/bottomborder/) { get; set; } | Les paramètres de bordure inférieure seront appliqués. |
| [CellShading](../../aspose.cells/styleflag/cellshading/) { get; set; } | Le paramètre d’ombrage de cellule sera appliqué. |
| [DiagonalDownBorder](../../aspose.cells/styleflag/diagonaldownborder/) { get; set; } | Les paramètres de bordure diagonale descendante seront appliqués. |
| [DiagonalUpBorder](../../aspose.cells/styleflag/diagonalupborder/) { get; set; } | Les paramètres de bordure diagonale ascendante seront appliqués. |
| [Font](../../aspose.cells/styleflag/font/) { get; set; } | Les paramètres de police seront appliqués. |
| [FontBold](../../aspose.cells/styleflag/fontbold/) { get; set; } | Le paramètre de gras de police sera appliqué. |
| [FontColor](../../aspose.cells/styleflag/fontcolor/) { get; set; } | Le paramètre de couleur de police sera appliqué. |
| [FontItalic](../../aspose.cells/styleflag/fontitalic/) { get; set; } | Le paramètre d’italique de police sera appliqué. |
| [FontName](../../aspose.cells/styleflag/fontname/) { get; set; } | Le paramètre de nom de police sera appliqué. |
| [FontScript](../../aspose.cells/styleflag/fontscript/) { get; set; } | Le paramètre de script de police sera appliqué. |
| [FontSize](../../aspose.cells/styleflag/fontsize/) { get; set; } | Le paramètre de taille de police sera appliqué. |
| [FontStrike](../../aspose.cells/styleflag/fontstrike/) { get; set; } | Le paramètre de barré de police sera appliqué. |
| [FontUnderline](../../aspose.cells/styleflag/fontunderline/) { get; set; } | Le paramètre de soulignement de police sera appliqué. |
| [HideFormula](../../aspose.cells/styleflag/hideformula/) { get; set; } | Le paramètre de masquage de formule sera appliqué. |
| [HorizontalAlignment](../../aspose.cells/styleflag/horizontalalignment/) { get; set; } | Le paramètre d’alignement horizontal sera appliqué. |
| [Indent](../../aspose.cells/styleflag/indent/) { get; set; } | Le paramètre de niveau d'indentation sera appliqué. |
| [LeftBorder](../../aspose.cells/styleflag/leftborder/) { get; set; } | Les paramètres de bordure gauche seront appliqués. |
| [Locked](../../aspose.cells/styleflag/locked/) { get; set; } | Le paramètre verrouillé sera appliqué. |
| [NumberFormat](../../aspose.cells/styleflag/numberformat/) { get; set; } | Le paramètre de format numérique sera appliqué. |
| [QuotePrefix](../../aspose.cells/styleflag/quoteprefix/) { get; set; } | Le paramètre de masquage de formule sera appliqué. |
| [RightBorder](../../aspose.cells/styleflag/rightborder/) { get; set; } | Les paramètres de bordure droite seront appliqués. |
| [Rotation](../../aspose.cells/styleflag/rotation/) { get; set; } | Le paramètre de rotation sera appliqué. |
| [ShrinkToFit](../../aspose.cells/styleflag/shrinktofit/) { get; set; } | Le paramètre de réduction pour ajuster sera appliqué. |
| [TextDirection](../../aspose.cells/styleflag/textdirection/) { get; set; } | Le paramètre de direction du texte sera appliqué. |
| [TopBorder](../../aspose.cells/styleflag/topborder/) { get; set; } | Les paramètres de bordure supérieure seront appliqués. |
| [VerticalAlignment](../../aspose.cells/styleflag/verticalalignment/) { get; set; } | Le paramètre d’alignement vertical sera appliqué. |
| [WrapText](../../aspose.cells/styleflag/wraptext/) { get; set; } | Le paramètre de retour à la ligne sera appliqué. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagDemo
    {
        public static void StyleFlagExample()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Header 1");
            worksheet.Cells["B1"].PutValue("Header 2");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["B3"].PutValue(40);

            // Créer un nouvel objet de style
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;

            // Créer un nouvel objet StyleFlag
            StyleFlag styleFlag = new StyleFlag
            {
                All = true,
                Font = true,
                FontSize = true,
                FontBold = true,
                CellShading = true
            };

            // Appliquer le style à une plage de cellules
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B1");
            range.ApplyStyle(style, styleFlag);

            // Enregistrez le classeur
            workbook.Save("StyleFlagExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


