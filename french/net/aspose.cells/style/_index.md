---
title: Style
second_title: Référence de l'API Aspose.Cells pour .NET
description: Représente le style daffichage du document Excel tel que la police la couleur lalignement la bordure etc. Lobjet Style contient tous les attributs de style police format de nombre alignement etc. en tant que propriétés.
type: docs
weight: 5750
url: /fr/net/aspose.cells/style/
---
## Style class

Représente le style d'affichage du document Excel, tel que la police, la couleur, l'alignement, la bordure, etc. L'objet Style contient tous les attributs de style (police, format de nombre, alignement, etc.) en tant que propriétés.

```csharp
public class Style
```

## Propriétés

| Nom | La description |
| --- | --- |
| [BackgroundArgbColor](../../aspose.cells/style/backgroundargbcolor) { get; set; } | Obtient et définit la couleur d'arrière-plan avec une valeur ARGB 32 bits. |
| [BackgroundColor](../../aspose.cells/style/backgroundcolor) { get; set; } | Obtient ou définit la couleur d'arrière-plan d'un style. |
| [BackgroundThemeColor](../../aspose.cells/style/backgroundthemecolor) { get; set; } | Obtient et définit la couleur du thème d'arrière-plan. |
| [Borders](../../aspose.cells/style/borders) { get; } | Obtient le[`BorderCollection`](../bordercollection) du style. |
| [CultureCustom](../../aspose.cells/style/culturecustom) { get; set; } | Obtient et définit la chaîne de modèle dépendant de la culture pour le format de nombre. Si aucun format de nombre n'a été défini pour cet objet, null sera renvoyé. Si le format de nombre est intégré, la chaîne de modèle correspondant au nombre intégré sera renvoyée. |
| [Custom](../../aspose.cells/style/custom) { get; set; } | Représente la chaîne de format numérique personnalisé de cet objet de style. Si le format numérique personnalisé n'est pas défini (par exemple, le format numérique est intégré), "" sera renvoyé. |
| [Font](../../aspose.cells/style/font) { get; } | Obtient un[`Font`](./font) objet. |
| [ForegroundArgbColor](../../aspose.cells/style/foregroundargbcolor) { get; set; } | Obtient et définit la couleur de premier plan avec une valeur ARGB 32 bits. |
| [ForegroundColor](../../aspose.cells/style/foregroundcolor) { get; set; } | Obtient ou définit la couleur de premier plan d'un style. |
| [ForegroundThemeColor](../../aspose.cells/style/foregroundthemecolor) { get; set; } | Obtient et définit la couleur du thème de premier plan. |
| [HasBorders](../../aspose.cells/style/hasborders) { get; } | Vérifie si des bordures ont été définies pour le style. |
| [HorizontalAlignment](../../aspose.cells/style/horizontalalignment) { get; set; } | Obtient ou définit le type d'alignement horizontal du texte dans une cellule. |
| [IndentLevel](../../aspose.cells/style/indentlevel) { get; set; } | Représente le niveau de retrait de la cellule ou de la plage. Ne peut être qu'un entier de 0 à 250. |
| [InvariantCustom](../../aspose.cells/style/invariantcustom) { get; } | Obtient la chaîne de modèle indépendante de la culture pour le format de nombre. Si aucun format de nombre n'a été défini pour cet objet, la valeur nulle sera renvoyée. Si le format de nombre est intégré, la chaîne de modèle correspondant au nombre intégré sera renvoyée. |
| [IsDateTime](../../aspose.cells/style/isdatetime) { get; } | Indique si le format numérique est un format de date. |
| [IsFormulaHidden](../../aspose.cells/style/isformulahidden) { get; set; } | Représente si la formule sera masquée lorsque la feuille de calcul est protégée. |
| [IsGradient](../../aspose.cells/style/isgradient) { get; set; } | Indique si l'ombrage des cellules est un motif dégradé. |
| [IsJustifyDistributed](../../aspose.cells/style/isjustifydistributed) { get; set; } | Indique si l'alignement justifié ou réparti des cellules doit être utilisé sur la dernière ligne de texte. |
| [IsLocked](../../aspose.cells/style/islocked) { get; set; } | Obtient ou définit une valeur indiquant si une cellule peut être modifiée ou non. |
| [IsPercent](../../aspose.cells/style/ispercent) { get; } | Indique si le format numérique est un format de pourcentage. |
| [IsTextWrapped](../../aspose.cells/style/istextwrapped) { get; set; } | Obtient ou définit une valeur indiquant si le texte d'une cellule est encapsulé. |
| [Name](../../aspose.cells/style/name) { get; set; } | Obtient ou définit le nom du style. |
| [Number](../../aspose.cells/style/number) { get; set; } | Obtient ou définit le format d'affichage des nombres et des dates. Les modèles de mise en forme sont différents pour différentes régions. |
| [ParentStyle](../../aspose.cells/style/parentstyle) { get; } | Obtient le style parent de ce style. |
| [Pattern](../../aspose.cells/style/pattern) { get; set; } | Obtient ou définit le type de motif d'arrière-plan de la cellule. |
| [QuotePrefix](../../aspose.cells/style/quoteprefix) { get; set; } | Indique si la valeur de la cellule commence par un guillemet simple. |
| [RotationAngle](../../aspose.cells/style/rotationangle) { get; set; } | Représente l'angle de rotation du texte. |
| [ShrinkToFit](../../aspose.cells/style/shrinktofit) { get; set; } | Représente si le texte se réduit automatiquement pour tenir dans la largeur de colonne disponible. |
| [TextDirection](../../aspose.cells/style/textdirection) { get; set; } | Représente l'ordre de lecture du texte. |
| [VerticalAlignment](../../aspose.cells/style/verticalalignment) { get; set; } | Obtient ou définit le type d'alignement vertical du texte dans une cellule. |

## Méthodes

| Nom | La description |
| --- | --- |
| [Copy](../../aspose.cells/style/copy)(Style) | Copie les données d'un autre objet de style |
| override [Equals](../../aspose.cells/style/equals)(object) | Détermine si deux instances de Style sont égales. |
| override [GetHashCode](../../aspose.cells/style/gethashcode)() | Sert de fonction de hachage pour un objet Style. |
| [GetTwoColorGradient](../../aspose.cells/style/gettwocolorgradient)(out Color, out Color, out GradientStyleType, out int) | Obtenez le paramètre de dégradé bicolore. |
| [IsModified](../../aspose.cells/style/ismodified)(StyleModifyFlag) | Vérifie si les propriétés spécifiées du style ont été modifiées. Utilisé pour le style de ConditionalFormattings pour vérifier si les propriétés spécifiées de ce style doivent être utilisées lors de l'application de ConditionalFormattings sur une cellule. |
| [SetBorder](../../aspose.cells/style/setborder)(BorderType, CellBorderType, Color) | Définit les bordures du style. |
| [SetCustom](../../aspose.cells/style/setcustom)(string, bool) | Définit la chaîne de format numérique personnalisé d'une cellule. |
| [SetPatternColor](../../aspose.cells/style/setpatterncolor)(BackgroundType, Color, Color) | Définit la couleur d'arrière-plan. |
| [SetTwoColorGradient](../../aspose.cells/style/settwocolorgradient)(Color, Color, GradientStyleType, int) | Définit le remplissage spécifié sur un dégradé bicolore. |
| [Update](../../aspose.cells/style/update)() | Appliquez le style nommé aux styles des cellules qui utilisent ce style nommé. Cela revient à cliquer sur le bouton "ok" après avoir fini de modifier le style. Ne s'applique qu'au style nommé. |

### Exemples

```csharp
[C#]
Workbook workbook = new Workbook();

WorksheetCollection sheets = workbook.Worksheets;
Cell cell = sheets[0].Cells["A1"];
Style style =  cell.GetStyle();
style.Font.Name = "Times New Roman";
style.Font.Color = Color.Blue;
cell.SetStyle(style);
```

### Voir également

* espace de noms [Aspose.Cells](../../aspose.cells)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
