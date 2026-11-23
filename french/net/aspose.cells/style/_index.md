---
title: "Classe Style"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Style. Représente le style d'affichage des documents Excel tels que la couleur de police, l'alignement, la bordure, etc. L'objet Style contient tous les attributs de style tels que la police, le format numérique, l'alignement, etc., sous forme de propriétés."
type: docs
url: /fr/net/aspose.cells/style/
---
## Style class

Représente le style d'affichage du document Excel, tel que la police, la couleur, l'alignement, la bordure, etc. L'objet Style contient tous les attributs de style (police, format numérique, alignement, etc.) en tant que propriétés.

```csharp
public class Style
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [Style](style/)() | (**Obsolète.**) Initialise une nouvelle instance de la classe `Style`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [BackgroundArgbColor](../../aspose.cells/style/backgroundargbcolor/) { get; set; } | Obtient et définit la couleur d'arrière-plan avec une valeur ARGB 32 bits. |
| [BackgroundColor](../../aspose.cells/style/backgroundcolor/) { get; set; } | Obtient ou définit la couleur d'arrière-plan d'un style. |
| [BackgroundThemeColor](../../aspose.cells/style/backgroundthemecolor/) { get; set; } | Obtient et définit la couleur du thème d'arrière-plan. |
| [Borders](../../aspose.cells/style/borders/) { get; } | Obtient la [`BorderCollection`](../bordercollection/) du style. |
| [BottomBorder](../../aspose.cells/style/bottomborder/) { get; } | Obtient la bordure inférieure. |
| [CultureCustom](../../aspose.cells/style/culturecustom/) { get; set; } | Obtient et définit la chaîne de modèle dépendante de la culture pour le format numérique. Si aucun format numérique n'a été défini pour cet objet, null sera retourné. Si le format numérique est intégré, la chaîne de modèle correspondant au numéro intégré sera retournée. |
| [Custom](../../aspose.cells/style/custom/) { get; set; } | Représente la chaîne de format numérique personnalisé de cet objet style. Si le format numérique personnalisé n'est pas défini (par exemple, le format numérique est intégré), "" sera retourné. |
| [Font](../../aspose.cells/style/font/) { get; } | Obtient un objet [`Font`](./font/). |
| [ForegroundArgbColor](../../aspose.cells/style/foregroundargbcolor/) { get; set; } | Obtient et définit la couleur de premier plan avec une valeur ARGB 32 bits. |
| [ForegroundColor](../../aspose.cells/style/foregroundcolor/) { get; set; } | Obtient ou définit la couleur de premier plan d'un style. |
| [ForegroundThemeColor](../../aspose.cells/style/foregroundthemecolor/) { get; set; } | Obtient et définit la couleur du thème de premier plan. |
| [HasBorders](../../aspose.cells/style/hasborders/) { get; } | Vérifie si des bordures ont été définies pour le style. |
| [HorizontalAlignment](../../aspose.cells/style/horizontalalignment/) { get; set; } | Obtient ou définit le type d'alignement horizontal du texte dans une cellule. |
| [IndentLevel](../../aspose.cells/style/indentlevel/) { get; set; } | Représente le niveau d'indentation pour la cellule ou la plage. Ne peut être qu'un entier compris entre 0 et 250. |
| [InvariantCustom](../../aspose.cells/style/invariantcustom/) { get; } | Obtient la chaîne de modèle indépendante de la culture pour le format de nombre. Si aucun format de nombre n'a été défini pour cet objet, null sera retourné. Si le format de nombre est intégré, la chaîne de modèle correspondant au nombre intégré sera retournée. |
| [IsAlignmentApplied](../../aspose.cells/style/isalignmentapplied/) { get; set; } | Indique si le formatage d'alignement doit être appliqué. |
| [IsBorderApplied](../../aspose.cells/style/isborderapplied/) { get; set; } | Indique si le formatage des bordures doit être appliqué. |
| [IsCheckBox](../../aspose.cells/style/ischeckbox/) { get; set; } | Indique s'il s'agit d'un style de case à cocher. |
| [IsDateTime](../../aspose.cells/style/isdatetime/) { get; } | Indique si le format de nombre est un format de date. |
| [IsFillApplied](../../aspose.cells/style/isfillapplied/) { get; set; } | Indique si le formatage de remplissage doit être appliqué. |
| [IsFontApplied](../../aspose.cells/style/isfontapplied/) { get; set; } | Indique si le formatage de police doit être appliqué. |
| [IsFormulaHidden](../../aspose.cells/style/isformulahidden/) { get; set; } | Représente si la formule sera masquée lorsque la feuille de calcul est protégée. |
| [IsGradient](../../aspose.cells/style/isgradient/) { get; set; } | Indique si l'ombrage de la cellule est un motif dégradé. |
| [IsJustifyDistributed](../../aspose.cells/style/isjustifydistributed/) { get; set; } | Indique si l'alignement justifié ou réparti des cellules doit être utilisé sur la dernière ligne de texte. |
| [IsLocked](../../aspose.cells/style/islocked/) { get; set; } | Obtient ou définit une valeur indiquant si une cellule peut être modifiée ou non. |
| [IsNumberFormatApplied](../../aspose.cells/style/isnumberformatapplied/) { get; set; } | Indique si le formatage des nombres doit être appliqué. |
| [IsPercent](../../aspose.cells/style/ispercent/) { get; } | Indique si le format de nombre est un format de pourcentage. |
| [IsProtectionApplied](../../aspose.cells/style/isprotectionapplied/) { get; set; } | Indique si le formatage de protection doit être appliqué. |
| [IsTextWrapped](../../aspose.cells/style/istextwrapped/) { get; set; } | Obtient ou définit une valeur indiquant si le texte à l'intérieur d'une cellule est renvoyé à la ligne. |
| [LeftBorder](../../aspose.cells/style/leftborder/) { get; } | Obtient la bordure gauche. |
| [Name](../../aspose.cells/style/name/) { get; set; } | Obtient ou définit le nom du style. |
| [Number](../../aspose.cells/style/number/) { get; set; } | Obtient ou définit le format d'affichage des nombres et des dates. Les modèles de formatage diffèrent selon les régions. |
| [ParentStyle](../../aspose.cells/style/parentstyle/) { get; } | Obtient le style parent de ce style. |
| [Pattern](../../aspose.cells/style/pattern/) { get; set; } | Obtient ou définit le type de motif d'arrière-plan de la cellule. |
| [QuotePrefix](../../aspose.cells/style/quoteprefix/) { get; set; } | Indique si la valeur de la cellule commence par un guillemet simple. |
| [RightBorder](../../aspose.cells/style/rightborder/) { get; } | Obtient la bordure droite. |
| [RotationAngle](../../aspose.cells/style/rotationangle/) { get; set; } | Représente l'angle de rotation du texte. |
| [ShrinkToFit](../../aspose.cells/style/shrinktofit/) { get; set; } | Représente si le texte se réduit automatiquement pour s'adapter à la largeur de colonne disponible. |
| [TextDirection](../../aspose.cells/style/textdirection/) { get; set; } | Représente l'ordre de lecture du texte. |
| [TopBorder](../../aspose.cells/style/topborder/) { get; } | Obtient la bordure supérieure. |
| [VerticalAlignment](../../aspose.cells/style/verticalalignment/) { get; set; } | Obtient ou définit le type d'alignement vertical du texte dans une cellule. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Copy](../../aspose.cells/style/copy/)(Style) | Copie les données d'un autre objet style |
| override [Equals](../../aspose.cells/style/equals/)(object) | Détermine si deux instances de Style sont égales. |
| override [GetHashCode](../../aspose.cells/style/gethashcode/)() | Servir de fonction de hachage pour un objet Style. |
| [GetTwoColorGradient](../../aspose.cells/style/gettwocolorgradient/)(out Color, out Color, out GradientStyleType, out int) | (**Obsolete.**) Obtenir le paramètre de dégradé bicolore. |
| [GetTwoColorGradientSetting](../../aspose.cells/style/gettwocolorgradientsetting/)() | Obtenir le paramètre de dégradé bicolore. |
| [IsModified](../../aspose.cells/style/ismodified/)(StyleModifyFlag) | Vérifie si les propriétés spécifiées du style ont été modifiées. Utilisé pour le style de ConditionalFormattings afin de vérifier si les propriétés spécifiées de ce style doivent être utilisées lors de l'application de ConditionalFormattings sur une cellule. |
| [SetBorder](../../aspose.cells/style/setborder/#setborder)(BorderType, CellBorderType, CellsColor) | Définit les bordures du style. |
| [SetBorder](../../aspose.cells/style/setborder/#setborder_1)(BorderType, CellBorderType, Color) | Définit les bordures du style. |
| [SetCustom](../../aspose.cells/style/setcustom/)(string, bool) | Définit la chaîne de format numérique personnalisée d'une cellule. |
| [SetOutlineBorders](../../aspose.cells/style/setoutlineborders/#setoutlineborders)(CellBorderType, CellsColor) | Définir les bordures de contour |
| [SetOutlineBorders](../../aspose.cells/style/setoutlineborders/#setoutlineborders_1)(CellBorderType, Color) | Définir les bordures de contour |
| [SetPatternColor](../../aspose.cells/style/setpatterncolor/)(BackgroundType, Color, Color) | Définit la couleur d'arrière-plan. |
| [SetTwoColorGradient](../../aspose.cells/style/settwocolorgradient/)(Color, Color, GradientStyleType, int) | Définit le remplissage spécifié en un dégradé bicolore. |
| [ToJson](../../aspose.cells/style/tojson/)() | Convertir `Style` en données de structure JSON. |
| [Update](../../aspose.cells/style/update/)() | Applique le style nommé aux styles des cellules qui utilisent ce style nommé. Cela fonctionne comme en cliquant sur le bouton "ok" après avoir terminé la modification du style. S'applique uniquement au style nommé. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class StyleDemo
    {
        public static void StyleExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accédez à une cellule de la feuille de calcul
            Cell cell = worksheet.Cells["A1"];
            
            // Obtenir le style de la cellule
            Style style = cell.GetStyle();
            
            // Définir diverses propriétés du style
            style.Font.Name = "Times New Roman";
            style.Font.Color = Color.Blue;
            style.BackgroundColor = Color.Yellow;
            style.ForegroundColor = Color.Red;
            style.Pattern = BackgroundType.Solid;
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.IsTextWrapped = true;
            style.IsLocked = true;
            style.Number = 15; // Date format
            style.IndentLevel = 2;
            style.RotationAngle = 45;
            style.IsFormulaHidden = true;
            style.ShrinkToFit = true;
            style.TextDirection = TextDirectionType.RightToLeft;
            style.IsJustifyDistributed = true;
            style.QuotePrefix = true;
            style.IsGradient = true;
            style.IsNumberFormatApplied = true;
            style.IsFontApplied = true;
            style.IsAlignmentApplied = true;
            style.IsBorderApplied = true;
            style.IsFillApplied = true;
            style.IsProtectionApplied = true;
            style.BackgroundArgbColor = Color.Yellow.ToArgb();
            style.ForegroundArgbColor = Color.Red.ToArgb();
            style.Custom = "0.00%";
            style.CultureCustom = "0.00%";
            
            // Définir le style de la cellule
            cell.SetStyle(style);
            
            // Enregistrez le classeur
            workbook.Save("StyleExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


