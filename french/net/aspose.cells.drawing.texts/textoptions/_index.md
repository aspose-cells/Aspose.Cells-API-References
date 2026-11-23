---
title: "Classe TextOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.Texts.TextOptions. Représente les options de texte"
type: docs
url: /fr/net/aspose.cells.drawing.texts/textoptions/
---
## TextOptions class

Représente les options de texte.

```csharp
public class TextOptions : Font
```

## Propriétés

| Nom | Description |
| --- | --- |
| [ArgbColor](../../aspose.cells/font/argbcolor/) { get; set; } | Obtient et définit la couleur avec une valeur ARGB de 32 bits.(Hérité de [`Font`](../../aspose.cells/font/).) |
| [CapsType](../../aspose.cells.drawing.texts/textoptions/capstype/) { get; set; } | Obtient et définit le type de majuscules pour les textes de la forme. |
| [Charset](../../aspose.cells/font/charset/) { get; set; } | Représente le jeu de caractères.(Hérité de [`Font`](../../aspose.cells/font/).) |
| [Color](../../aspose.cells/font/color/) { get; set; } | Obtient ou définit la couleur de la police.(Hérité de [`Font`](../../aspose.cells/font/).) |
| [DoubleSize](../../aspose.cells/font/doublesize/) { get; set; } | Obtient et définit la taille double de la police.(Hérité de [`Font`](../../aspose.cells/font/).) |
| [FarEastName](../../aspose.cells.drawing.texts/textoptions/fareastname/) { get; set; } | Obtient et définit le nom FarEast. |
| [Fill](../../aspose.cells.drawing.texts/textoptions/fill/) { get; } | Représente le format de remplissage du texte. |
| [IsBold](../../aspose.cells/font/isbold/) { get; set; } | Obtient ou définit une valeur indiquant si la police est en gras.(Hérité de [`Font`](../../aspose.cells/font/).) |
| [IsItalic](../../aspose.cells/font/isitalic/) { get; set; } | Obtient ou définit une valeur indiquant si la police est en italique.(Hérité de [`Font`](../../aspose.cells/font/).) |
| [IsNormalizeHeights](../../aspose.cells.drawing.texts/textoptions/isnormalizeheights/) { get; set; } | Indique si la normalisation de la hauteur doit être appliquée à la séquence de texte. |
| [IsStrikeout](../../aspose.cells/font/isstrikeout/) { get; set; } | Obtient ou définit une valeur indiquant si la police a une seule ligne de barré.(Hérité de [`Font`](../../aspose.cells/font/).) |
| [IsSubscript](../../aspose.cells/font/issubscript/) { get; set; } | Obtient ou définit une valeur indiquant si la police est en indice.(Hérité de [`Font`](../../aspose.cells/font/).) |
| [IsSuperscript](../../aspose.cells/font/issuperscript/) { get; set; } | Obtient ou définit une valeur indiquant si la police est en exposant.(Hérité de [`Font`](../../aspose.cells/font/).) |
| [Kerning](../../aspose.cells.drawing.texts/textoptions/kerning/) { get; set; } | Spécifie la taille minimale de police à laquelle le crénage des caractères se produira pour cette séquence de texte. |
| [LanguageCode](../../aspose.cells.drawing.texts/textoptions/languagecode/) { get; set; } | Obtient et définit la langue de l'interface utilisateur. |
| [LatinName](../../aspose.cells.drawing.texts/textoptions/latinname/) { get; set; } | Obtient et définit le nom latin. |
| override [Name](../../aspose.cells.drawing.texts/textoptions/name/) { get; set; } | Obtient et définit le nom de la forme. |
| [Outline](../../aspose.cells.drawing.texts/textoptions/outline/) { get; } | Représente le format de contour du texte. |
| [SchemeType](../../aspose.cells/font/schemetype/) { get; set; } | Obtient et définit le type de schéma de la police.(Hérité de [`Font`](../../aspose.cells/font/).) |
| [ScriptOffset](../../aspose.cells/font/scriptoffset/) { get; set; } | Obtient et définit le décalage du script, en unité de pourcentage.(Hérité de [`Font`](../../aspose.cells/font/).) |
| [Shadow](../../aspose.cells.drawing.texts/textoptions/shadow/) { get; } | Représente un objet [`ShadowEffect`](../../aspose.cells.drawing/shadoweffect/) qui spécifie l'effet d'ombre pour l'élément de graphique ou la forme. |
| [Size](../../aspose.cells/font/size/) { get; set; } | Obtient ou définit la taille de la police.(Hérité de [`Font`](../../aspose.cells/font/).) |
| [Spacing](../../aspose.cells.drawing.texts/textoptions/spacing/) { get; set; } | Spécifie l'espacement entre les caractères au sein d'une séquence de texte. |
| [StrikeType](../../aspose.cells/font/striketype/) { get; set; } | Obtient le type de rayure du texte.(Hérité de [`Font`](../../aspose.cells/font/).) |
| [ThemeColor](../../aspose.cells/font/themecolor/) { get; set; } | Obtient et définit la couleur du thème.(Hérité de [`Font`](../../aspose.cells/font/).) |
| [Underline](../../aspose.cells/font/underline/) { get; set; } | Obtient ou définit le type de soulignement de la police.(Hérité de [`Font`](../../aspose.cells/font/).) |
| [UnderlineColor](../../aspose.cells.drawing.texts/textoptions/underlinecolor/) { get; set; } | Obtient ou définit la couleur du soulignement. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Equals](../../aspose.cells/font/equals/)(Font) | Vérifie si deux polices sont égales.(Hérité de [`Font`](../../aspose.cells/font/).) |
| [SetName](../../aspose.cells/font/setname/)(string, FontSchemeType) | Définit le nom et le schéma de la police.(Hérité de [`Font`](../../aspose.cells/font/).) |
| override [ToString](../../aspose.cells/font/tostring/)() | Renvoie une chaîne qui représente l'objet Cell actuel.(Hérité de [`Font`](../../aspose.cells/font/).) |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextsClassTextOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoute une forme à la feuille de calcul avec tous les paramètres requis
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);
            
            // Ajoute du texte à la forme et obtient TextOptions
            shape.TextBody.Text = "Sample Text";
            TextOptions textOptions = shape.TextBody[2].TextOptions;
            
            // Définir les options de texte
            textOptions.Fill.SolidFill.Color = System.Drawing.Color.Red;
            textOptions.Fill.SolidFill.Transparency = 0.5;
            
            // Enregistrez le classeur
            workbook.Save("TextOptionsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Font](../../aspose.cells/font/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


