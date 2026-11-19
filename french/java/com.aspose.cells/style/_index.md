---
title: "Style"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente le style d'affichage d'un document Excel tel que police, couleur, alignement, bordure, etc."
type: docs
url: /fr/java/com.aspose.cells/style/
---

**Inheritance:**
java.lang.Object
```
public class Style
```

Représente le style d'affichage d'un document Excel, tel que la police, la couleur, l'alignement, la bordure, etc. L'objet Style contient tous les attributs de style (police, format de nombre, alignement, etc.) sous forme de propriétés.

**Example**

```
         Workbook workbook = new Workbook();
 
         WorksheetCollection sheets = workbook.getWorksheets();
         Cell cell = sheets.get(0).getCells().get("A1");
         Style style =  cell.getStyle();
         style.getFont().setName("Times New Roman");
         style.getFont().setColor(Color.getBlue());
         cell.setStyle(style);
```
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [Style()](#Style--) | Initialise une nouvelle instance de la classe [Style](../../com.aspose.cells/style). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [copy(Style style)](#copy-com.aspose.cells.Style-) | Copie les données d'un autre objet style |
| [equals(Object obj)](#equals-java.lang.Object-) | Détermine si deux instances de Style sont égales. |
| [getBackgroundArgbColor()](#getBackgroundArgbColor--) | Obtient la couleur d'arrière-plan avec une valeur ARGB 32 bits. |
| [getBackgroundColor()](#getBackgroundColor--) | Obtient la couleur d'arrière-plan d'un style. |
| [getBackgroundThemeColor()](#getBackgroundThemeColor--) | Obtient la couleur du thème d'arrière-plan. |
| [getBorders()](#getBorders--) | Obtient la [BorderCollection](../../com.aspose.cells/bordercollection) du style. |
| [getBottomBorder()](#getBottomBorder--) | Obtient la bordure inférieure. |
| [getClass()](#getClass--) |  |
| [getCultureCustom()](#getCultureCustom--) | Obtient la chaîne de modèle dépendante de la culture pour le format de nombre. |
| [getCustom()](#getCustom--) | Représente la chaîne de format numérique personnalisé de cet objet style. |
| [getFont()](#getFont--) | Obtient un objet [getFont()](../../com.aspose.cells/style\#getFont--). |
| [getForegroundArgbColor()](#getForegroundArgbColor--) | Obtient la couleur de premier plan avec une valeur ARGB 32 bits. |
| [getForegroundColor()](#getForegroundColor--) | Obtient la couleur de premier plan d'un style. |
| [getForegroundThemeColor()](#getForegroundThemeColor--) | Obtient la couleur du thème d'avant-plan. |
| [getHorizontalAlignment()](#getHorizontalAlignment--) | Obtient le type d'alignement horizontal du texte dans une cellule. |
| [getIndentLevel()](#getIndentLevel--) | Représente le niveau d'indentation pour la cellule ou la plage. |
| [getInvariantCustom()](#getInvariantCustom--) | Obtient la chaîne de modèle indépendante de la culture pour le format de nombre. |
| [getLeftBorder()](#getLeftBorder--) | Obtient la bordure gauche. |
| [getName()](#getName--) | Obtient le nom du style. |
| [getNumber()](#getNumber--) | Obtient le format d'affichage des nombres et des dates. |
| [getParentStyle()](#getParentStyle--) | Obtient le style parent de ce style. |
| [getPattern()](#getPattern--) | Obtient le type de motif d'arrière-plan de la cellule. |
| [getQuotePrefix()](#getQuotePrefix--) | Indique si la valeur de la cellule commence par une apostrophe. |
| [getRightBorder()](#getRightBorder--) | Obtient la bordure droite. |
| [getRotationAngle()](#getRotationAngle--) | Représente l'angle de rotation du texte. |
| [getShrinkToFit()](#getShrinkToFit--) | Représente si le texte se réduit automatiquement pour s'adapter à la largeur de colonne disponible. |
| [getTextDirection()](#getTextDirection--) | Représente l'ordre de lecture du texte. |
| [getTopBorder()](#getTopBorder--) | Obtient la bordure supérieure. |
| [getTwoColorGradient()](#getTwoColorGradient--) | Obtient le paramètre de dégradé bicolore. |
| [getTwoColorGradientSetting()](#getTwoColorGradientSetting--) | Obtient le paramètre de dégradé bicolore. |
| [getVerticalAlignment()](#getVerticalAlignment--) | Obtient le type d'alignement vertical du texte dans une cellule. |
| [hasBorders()](#hasBorders--) | Vérifie si des bordures ont été définies pour le style. |
| [hashCode()](#hashCode--) | Servir de fonction de hachage pour un objet Style. |
| [isAlignmentApplied()](#isAlignmentApplied--) | Indique si le formatage d'alignement doit être appliqué. |
| [isBorderApplied()](#isBorderApplied--) | Indique si le formatage de bordure doit être appliqué. |
| [isCheckBox()](#isCheckBox--) | Indique s'il s'agit d'un style de case à cocher |
| [isDateTime()](#isDateTime--) | Indique si le format de nombre est un format de date. |
| [isFillApplied()](#isFillApplied--) | Indique si le formatage de remplissage doit être appliqué. |
| [isFontApplied()](#isFontApplied--) | Indique si le formatage de police doit être appliqué. |
| [isFormulaHidden()](#isFormulaHidden--) | Représente si la formule sera masquée lorsque la feuille de calcul est protégée. |
| [isGradient()](#isGradient--) | Indique si le remplissage de la cellule est un motif dégradé. |
| [isJustifyDistributed()](#isJustifyDistributed--) | Indique si l'alignement justifié ou distribué des cellules doit être utilisé sur la dernière ligne de texte. |
| [isLocked()](#isLocked--) | Obtient une valeur indiquant si une cellule peut être modifiée ou non. |
| [isModified(int modifyFlag)](#isModified-int-) | Vérifie si les propriétés spécifiées du style ont été modifiées. |
| [isNumberFormatApplied()](#isNumberFormatApplied--) | Indique si le formatage des nombres doit être appliqué. |
| [isPercent()](#isPercent--) | Indique si le format de nombre est un format pourcentage. |
| [isProtectionApplied()](#isProtectionApplied--) | Indique si le formatage de protection doit être appliqué. |
| [isTextWrapped()](#isTextWrapped--) | Obtient une valeur indiquant si le texte à l'intérieur d'une cellule est renvoyé à la ligne. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlignmentApplied(boolean value)](#setAlignmentApplied-boolean-) | Indique si le formatage d'alignement doit être appliqué. |
| [setBackgroundArgbColor(int value)](#setBackgroundArgbColor-int-) | Définit la couleur d'arrière-plan avec une valeur ARGB 32 bits. |
| [setBackgroundColor(Color value)](#setBackgroundColor-com.aspose.cells.Color-) | Définit la couleur d'arrière-plan d'un style. |
| [setBackgroundThemeColor(ThemeColor value)](#setBackgroundThemeColor-com.aspose.cells.ThemeColor-) | Définit la couleur du thème d'arrière-plan. |
| [setBorder(int borderType, int borderStyle, CellsColor borderColor)](#setBorder-int-int-com.aspose.cells.CellsColor-) | Définit les bordures du style. |
| [setBorder(int borderType, int borderStyle, Color borderColor)](#setBorder-int-int-com.aspose.cells.Color-) | Définit les bordures du style. |
| [setBorderApplied(boolean value)](#setBorderApplied-boolean-) | Indique si le formatage de bordure doit être appliqué. |
| [setCheckBox(boolean value)](#setCheckBox-boolean-) | Indique s'il s'agit d'un style de case à cocher |
| [setCultureCustom(String value)](#setCultureCustom-java.lang.String-) | Définit la chaîne de modèle dépendante de la culture pour le format de nombre. |
| [setCustom(String value)](#setCustom-java.lang.String-) | Représente la chaîne de format numérique personnalisé de cet objet style. |
| [setCustom(String custom, boolean builtinPreference)](#setCustom-java.lang.String-boolean-) | Définit la chaîne de format de nombre personnalisé d'une cellule. |
| [setFillApplied(boolean value)](#setFillApplied-boolean-) | Indique si le formatage de remplissage doit être appliqué. |
| [setFontApplied(boolean value)](#setFontApplied-boolean-) | Indique si le formatage de police doit être appliqué. |
| [setForegroundArgbColor(int value)](#setForegroundArgbColor-int-) | Définit la couleur de premier plan avec une valeur ARGB 32 bits. |
| [setForegroundColor(Color value)](#setForegroundColor-com.aspose.cells.Color-) | Définit la couleur de premier plan d'un style. |
| [setForegroundThemeColor(ThemeColor value)](#setForegroundThemeColor-com.aspose.cells.ThemeColor-) | Définit la couleur du thème de premier plan. |
| [setFormulaHidden(boolean value)](#setFormulaHidden-boolean-) | Représente si la formule sera masquée lorsque la feuille de calcul est protégée. |
| [setGradient(boolean value)](#setGradient-boolean-) | Indique si le remplissage de la cellule est un motif dégradé. |
| [setHorizontalAlignment(int value)](#setHorizontalAlignment-int-) | Définit le type d'alignement horizontal du texte dans une cellule. |
| [setIndentLevel(int value)](#setIndentLevel-int-) | Représente le niveau d'indentation pour la cellule ou la plage. |
| [setJustifyDistributed(boolean value)](#setJustifyDistributed-boolean-) | Indique si l'alignement justifié ou distribué des cellules doit être utilisé sur la dernière ligne de texte. |
| [setLocked(boolean value)](#setLocked-boolean-) | Définit une valeur indiquant si une cellule peut être modifiée ou non. |
| [setName(String value)](#setName-java.lang.String-) | Définit le nom du style. |
| [setNumber(int value)](#setNumber-int-) | Définit le format d'affichage des nombres et des dates. |
| [setNumberFormatApplied(boolean value)](#setNumberFormatApplied-boolean-) | Indique si le formatage des nombres doit être appliqué. |
| [setOutlineBorders(int borderStyle, CellsColor borderColor)](#setOutlineBorders-int-com.aspose.cells.CellsColor-) | Définir les bordures de contour |
| [setOutlineBorders(int borderStyle, Color borderColor)](#setOutlineBorders-int-com.aspose.cells.Color-) | Définir les bordures de contour |
| [setPattern(int value)](#setPattern-int-) | Définit le type de motif d'arrière-plan de la cellule. |
| [setPatternColor(int pattern, Color color1, Color color2)](#setPatternColor-int-com.aspose.cells.Color-com.aspose.cells.Color-) | Définit la couleur d'arrière-plan. |
| [setProtectionApplied(boolean value)](#setProtectionApplied-boolean-) | Indique si le formatage de protection doit être appliqué. |
| [setQuotePrefix(boolean value)](#setQuotePrefix-boolean-) | Indique si la valeur de la cellule commence par une apostrophe. |
| [setRotationAngle(int value)](#setRotationAngle-int-) | Représente l'angle de rotation du texte. |
| [setShrinkToFit(boolean value)](#setShrinkToFit-boolean-) | Représente si le texte se réduit automatiquement pour s'adapter à la largeur de colonne disponible. |
| [setTextDirection(int value)](#setTextDirection-int-) | Représente l'ordre de lecture du texte. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Définit une valeur indiquant si le texte à l'intérieur d'une cellule est renvoyé à la ligne. |
| [setTwoColorGradient(Color color1, Color color2, int gradientStyleType, int variant)](#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-) | Définit le remplissage spécifié à un dégradé à deux couleurs. |
| [setVerticalAlignment(int value)](#setVerticalAlignment-int-) | Définit le type d'alignement vertical du texte dans une cellule. |
| [toJson()](#toJson--) | Convertir [Style](../../com.aspose.cells/style) en données de structure JSON. |
| [toString()](#toString--) |  |
| [update()](#update--) | Appliquer le style nommé aux styles des cellules qui utilisent ce style nommé. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Style() {#Style--}
```
public Style()
```


Initialise une nouvelle instance de la classe [Style](../../com.aspose.cells/style).

**Remarks**

NOTE : Ce constructeur est maintenant obsolète. À la place, veuillez utiliser la méthode CellsFactory.CreateStyle(). Cette propriété sera supprimée 6 mois plus tard, depuis octobre 2016. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### copy(Style style) {#copy-com.aspose.cells.Style-}
```
public void copy(Style style)
```


Copie les données d'un autre objet style

**Remarks**

Cette méthode ne copie pas le nom du style. Si vous souhaitez copier le nom, veuillez appeler le code suivant après avoir copié le style : destStyle.Name = style.Name.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Objet Style source |

### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Détermine si deux instances de Style sont égales.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | L'objet Style à comparer avec l'objet Style actuel. |

**Returns:**
booléen - vrai si l'Objet spécifié est égal à l'Objet actuel ; sinon, faux.
### getBackgroundArgbColor() {#getBackgroundArgbColor--}
```
public int getBackgroundArgbColor()
```


Obtient la couleur d'arrière-plan avec une valeur ARGB 32 bits.

**Returns:**
int
### getBackgroundColor() {#getBackgroundColor--}
```
public Color getBackgroundColor()
```


Obtient la couleur d'arrière-plan d'un style.

**Remarks**

Si vous souhaitez définir la couleur d'une cellule, veuillez utiliser la propriété Style.ForegroundColor. Cette propriété ne prendra effet que si le motif du style de la cellule est différent de aucun ou plein.

**Returns:**
[Color](../../com.aspose.cells/color)
### getBackgroundThemeColor() {#getBackgroundThemeColor--}
```
public ThemeColor getBackgroundThemeColor()
```


Obtient la couleur du thème d'arrière-plan.

**Remarks**

Si la couleur d'arrière-plan n'est pas une couleur de thème, NULL sera renvoyé.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getBorders() {#getBorders--}
```
public BorderCollection getBorders()
```


Obtient la [BorderCollection](../../com.aspose.cells/bordercollection) du style.

**Returns:**
[BorderCollection](../../com.aspose.cells/bordercollection)
### getBottomBorder() {#getBottomBorder--}
```
public Border getBottomBorder()
```


Obtient la bordure inférieure.

**Returns:**
[Border](../../com.aspose.cells/border)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCultureCustom() {#getCultureCustom--}
```
public String getCultureCustom()
```


Obtient la chaîne de modèle dépendante de la culture pour le format numérique. Si aucun format numérique n'a été défini pour cet objet, null sera renvoyé. Si le format numérique est intégré, la chaîne de modèle correspondant au nombre intégré sera renvoyée.

**Remarks**

Pour les formats numériques intégrés, à la fois le contenu du modèle (par exemple, un format de date intégré est \"m/d/y\" pour certaines locales, mais devient \"d/m/y\" pour d'autres) et le spécificateur de format (par exemple, certaines locales utilisent un caractère différent de 'y' pour représenter la partie année du format de date) sont dépendants de la culture ; pour un format personnalisé spécifié par l'utilisateur, seuls les spécificateurs de format sont modifiés selon la culture, les autres parties du modèle de format ne seront pas modifiées.

**Returns:**
java.lang.String
### getCustom() {#getCustom--}
```
public String getCustom()
```


Représente la chaîne de format numérique personnalisé de cet objet style. Si le format numérique personnalisé n'est pas défini (par exemple, le format numérique est intégré), \"\" sera renvoyé.

**Remarks**

La chaîne personnalisée renvoyée est indépendante de la culture.

**Returns:**
java.lang.String
### getFont() {#getFont--}
```
public Font getFont()
```


Obtient un objet [getFont()](../../com.aspose.cells/style\#getFont--).

**Returns:**
[Font](../../com.aspose.cells/font)
### getForegroundArgbColor() {#getForegroundArgbColor--}
```
public int getForegroundArgbColor()
```


Obtient la couleur de premier plan avec une valeur ARGB 32 bits.

**Returns:**
int
### getForegroundColor() {#getForegroundColor--}
```
public Color getForegroundColor()
```


Obtient la couleur de premier plan d'un style.

**Remarks**

Cela signifie qu'aucun réglage de couleur n'est appliqué si Color.Empty est renvoyé.

**Returns:**
[Color](../../com.aspose.cells/color)
### getForegroundThemeColor() {#getForegroundThemeColor--}
```
public ThemeColor getForegroundThemeColor()
```


Obtient la couleur du thème d'avant-plan.

**Remarks**

Si la couleur de premier plan n'est pas une couleur de thème, NULL sera renvoyé.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getHorizontalAlignment() {#getHorizontalAlignment--}
```
public int getHorizontalAlignment()
```


Obtient le type d'alignement horizontal du texte dans une cellule.

Voir [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getIndentLevel() {#getIndentLevel--}
```
public int getIndentLevel()
```


Représente le niveau d'indentation pour la cellule ou la plage. Ne peut être qu'un entier compris entre 0 et 250.

**Remarks**

Si le type d'alignement horizontal du texte est défini sur une valeur autre que gauche ou droite, le niveau d'indentation sera réinitialisé à zéro.

**Returns:**
int
### getInvariantCustom() {#getInvariantCustom--}
```
public String getInvariantCustom()
```


Obtient la chaîne de modèle indépendante de la culture pour le format numérique. Si aucun format numérique n'a été défini pour cet objet, null sera renvoyé. Si le format numérique est intégré, la chaîne de modèle correspondant au nombre intégré sera renvoyée.

**Remarks**

Pour les formats numériques intégrés, le contenu du modèle renvoyé reste dépendant de la culture, par exemple, pour certaines locales il renvoie \"m/d/y\" et pour d'autres locales il renvoie \"d/m/y\". La différence avec [getCultureCustom()](../../com.aspose.cells/style\#getCultureCustom--) est (c'est aussi ce que signifie indépendant de la culture) : les spécificateurs de format et les séparateurs sont conservés comme standard, de sorte que '/' sera toujours utilisé comme séparateur de date/heure et \"y\" sera toujours utilisé comme partie \"année\", quel que soit le caractère spécial utilisé pour la locale spécifique.

**Returns:**
java.lang.String
### getLeftBorder() {#getLeftBorder--}
```
public Border getLeftBorder()
```


Obtient la bordure gauche.

**Returns:**
[Border](../../com.aspose.cells/border)
### getName() {#getName--}
```
public String getName()
```


Obtient le nom du style.

**Returns:**
java.lang.String
### getNumber() {#getNumber--}
```
public int getNumber()
```


Obtient le format d'affichage des nombres et des dates. Les modèles de formatage diffèrent selon les régions.

**Remarks**

Par exemple, les modèles de formatage représentés par des nombres pour la région en\\_US :

| Valeur | Type | Chaîne de format |
| ----- | ---------- | ---------------------------------------------------- |
| 0 | General | `General` |
| 1 | Decimal | `0` |
| 2 | Decimal | `0.00` |
| 3 | Decimal | `#,##0` |
| 4 | Decimal | `#,##0.00` |
| 5 | Currency | `$#,##0_);($#,##0)` |
| 6 | Currency | `$#,##0_);[Rouge](../$#,##0)` |
| 7 | Currency | `$#,##0.00_);($#,##0.00)` |
| 8 | Currency | `$#,##0.00_);[Rouge](../$#,##0.00)` |
| 9 | Percentage | `0%` |
| 10 | Percentage | `0.00%` |
| 11 | Scientific | `0.00E+00` |
| 12 | Fraction | `# ?/?` |
| 13 | Fraction | `# ??/??` |
| 14 | Date | `jj/mm/aaaa` |
| 15 | Date | `jj-mmm-aa` |
| 16 | Date | `jj-mmm` |
| 17 | Date | `mmm-aa` |
| 18 | Time | `hh:mm` |
| 19 | Time | `hh:mm:ss` |
| 20 | Time | `hh:mm` |
| 21 | Time | `hh:mm:ss` |
| 22 | Time | `jj/mm/aaaa hh:mm` |
| 37 | Accounting | `#,##0_);(#,##0)` |
| 38 | Accounting | `#,##0_);[Rouge](../#,##0)` |
| 39 | Accounting | `#,##0.00_);(#,##0.00)` |
| 40 | Accounting | `#,##0.00_);[Rouge](../#,##0.00)` |
| 41 | Accounting | `_(* #,##0_);_(* (#,##0);_(* "-"_);_(@_)` |
| 42 | Currency | `_($* #,##0_);_($* (#,##0);_($* "-"_);_(@_)` |
| 43 | Accounting | `_(* #,##0.00_);_(* (#,##0.00);_(* "-"??_);_(@_)` |
| 44 | Currency | `_($* #,##0.00_);_($* (#,##0.00);_($* "-"??_);_(@_)` |
| 45 | Time | `mm:ss` |
| 46 | Time | `[h]:mm:ss` |
| 47 | Time | `mm:ss.0` |
| 48 | Scientific | `##0.0E+0` |
| 49 | Text | `@` |

**Returns:**
int
### getParentStyle() {#getParentStyle--}
```
public Style getParentStyle()
```


Obtient le style parent de ce style.

**Returns:**
[Style](../../com.aspose.cells/style)
### getPattern() {#getPattern--}
```
public int getPattern()
```


Obtient le type de motif d'arrière-plan de la cellule.

Voir [BackgroundType](../../com.aspose.cells/backgroundtype).

**Returns:**
int
### getQuotePrefix() {#getQuotePrefix--}
```
public boolean getQuotePrefix()
```


Indique si la valeur de la cellule commence par une apostrophe.

**Returns:**
boolean
### getRightBorder() {#getRightBorder--}
```
public Border getRightBorder()
```


Obtient la bordure droite.

**Returns:**
[Border](../../com.aspose.cells/border)
### getRotationAngle() {#getRotationAngle--}
```
public int getRotationAngle()
```


Représente l'angle de rotation du texte.

**Remarks**

0: Non pivoté.

255: De haut en bas.

\-90: Vers le bas.

90: Vers le haut.

Vous pouvez définir 255 ou une valeur comprise entre -90 et 90.

**Returns:**
int
### getShrinkToFit() {#getShrinkToFit--}
```
public boolean getShrinkToFit()
```


Représente si le texte se réduit automatiquement pour s'adapter à la largeur de colonne disponible.

**Returns:**
boolean
### getTextDirection() {#getTextDirection--}
```
public int getTextDirection()
```


Représente l'ordre de lecture du texte.

Voir [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Returns:**
int
### getTopBorder() {#getTopBorder--}
```
public Border getTopBorder()
```


Obtient la bordure supérieure.

**Returns:**
[Border](../../com.aspose.cells/border)
### getTwoColorGradient() {#getTwoColorGradient--}
```
public Object[] getTwoColorGradient()
```


Obtient le paramètre de dégradé bicolore.

**Remarks**

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode Style.GetTwoColorGradientSetting(). Cette propriété sera supprimée 12 mois plus tard, depuis décembre 2022. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Returns:**
java.lang.Object[] - Retourne tous les paramètres du dégradé bicolore [0] : Color1 [1] : Color2 [2] : GradientStyleType [3] : Variant
### getTwoColorGradientSetting() {#getTwoColorGradientSetting--}
```
public TwoColorGradient getTwoColorGradientSetting()
```


Obtient le paramètre de dégradé bicolore.

**Returns:**
[TwoColorGradient](../../com.aspose.cells/twocolorgradient)
### getVerticalAlignment() {#getVerticalAlignment--}
```
public int getVerticalAlignment()
```


Obtient le type d'alignement vertical du texte dans une cellule.

Voir [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### hasBorders() {#hasBorders--}
```
public boolean hasBorders()
```


Vérifie si des bordures ont été définies pour le style.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```


Servir de fonction de hachage pour un objet Style.

**Remarks**

Cette méthode est uniquement destinée à un usage interne.

**Returns:**
int - Un code de hachage pour l'objet actuel.
### isAlignmentApplied() {#isAlignmentApplied--}
```
public boolean isAlignmentApplied()
```


Indique si le formatage d'alignement doit être appliqué.

**Remarks**

Uniquement pour le style nommé.

**Returns:**
boolean
### isBorderApplied() {#isBorderApplied--}
```
public boolean isBorderApplied()
```


Indique si le formatage de bordure doit être appliqué.

**Remarks**

Uniquement pour le style nommé.

**Returns:**
boolean
### isCheckBox() {#isCheckBox--}
```
public boolean isCheckBox()
```


Indique s'il s'agit d'un style de case à cocher

**Returns:**
boolean
### isDateTime() {#isDateTime--}
```
public boolean isDateTime()
```


Indique si le format de nombre est un format de date.

**Returns:**
boolean
### isFillApplied() {#isFillApplied--}
```
public boolean isFillApplied()
```


Indique si le formatage de remplissage doit être appliqué.

**Remarks**

Uniquement pour le style nommé.

**Returns:**
boolean
### isFontApplied() {#isFontApplied--}
```
public boolean isFontApplied()
```


Indique si le formatage de police doit être appliqué.

**Remarks**

Uniquement pour le style nommé.

**Returns:**
boolean
### isFormulaHidden() {#isFormulaHidden--}
```
public boolean isFormulaHidden()
```


Représente si la formule sera masquée lorsque la feuille de calcul est protégée.

**Returns:**
boolean
### isGradient() {#isGradient--}
```
public boolean isGradient()
```


Indique si le remplissage de la cellule est un motif dégradé.

**Returns:**
boolean
### isJustifyDistributed() {#isJustifyDistributed--}
```
public boolean isJustifyDistributed()
```


Indique si l'alignement justifié ou distribué des cellules doit être utilisé sur la dernière ligne de texte.

**Remarks**

Ceci est typique pour les alignements d'Asie de l'Est mais pas typique dans d'autres contextes. Ne fonctionne que lorsque l'alignement horizontal est distribué.

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


Obtient une valeur indiquant si une cellule peut être modifiée ou non.

**Remarks**

Le verrouillage des cellules n'a aucun effet à moins que la feuille de calcul ne soit protégée.

**Returns:**
boolean
### isModified(int modifyFlag) {#isModified-int-}
```
public boolean isModified(int modifyFlag)
```


Vérifie si les propriétés spécifiées du style ont été modifiées. Utilisé pour le style des ConditionalFormattings afin de vérifier si les propriétés spécifiées de ce style doivent être utilisées lors de l'application des ConditionalFormattings sur une cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| modifyFlag | int | [StyleModifyFlag](../../com.aspose.cells/stylemodifyflag). Indicateurs de style modifié |

**Returns:**
boolean - vrai si les propriétés spécifiées ont été modifiées
### isNumberFormatApplied() {#isNumberFormatApplied--}
```
public boolean isNumberFormatApplied()
```


Indique si le formatage des nombres doit être appliqué.

**Remarks**

Uniquement pour le style nommé.

**Returns:**
boolean
### isPercent() {#isPercent--}
```
public boolean isPercent()
```


Indique si le format de nombre est un format pourcentage.

**Returns:**
boolean
### isProtectionApplied() {#isProtectionApplied--}
```
public boolean isProtectionApplied()
```


Indique si le formatage de protection doit être appliqué.

**Remarks**

Uniquement pour le style nommé.

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


Obtient une valeur indiquant si le texte à l'intérieur d'une cellule est renvoyé à la ligne.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAlignmentApplied(boolean value) {#setAlignmentApplied-boolean-}
```
public void setAlignmentApplied(boolean value)
```


Indique si le formatage d'alignement doit être appliqué.

**Remarks**

Uniquement pour le style nommé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setBackgroundArgbColor(int value) {#setBackgroundArgbColor-int-}
```
public void setBackgroundArgbColor(int value)
```


Définit la couleur d'arrière-plan avec une valeur ARGB 32 bits.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setBackgroundColor(Color value) {#setBackgroundColor-com.aspose.cells.Color-}
```
public void setBackgroundColor(Color value)
```


Définit la couleur d'arrière-plan d'un style.

**Remarks**

Si vous souhaitez définir la couleur d'une cellule, veuillez utiliser la propriété Style.ForegroundColor. Cette propriété ne prendra effet que si le motif du style de la cellule est différent de aucun ou plein.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setBackgroundThemeColor(ThemeColor value) {#setBackgroundThemeColor-com.aspose.cells.ThemeColor-}
```
public void setBackgroundThemeColor(ThemeColor value)
```


Définit la couleur du thème d'arrière-plan.

**Remarks**

Si la couleur d'arrière-plan n'est pas une couleur de thème, NULL sera renvoyé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setBorder(int borderType, int borderStyle, CellsColor borderColor) {#setBorder-int-int-com.aspose.cells.CellsColor-}
```
public boolean setBorder(int borderType, int borderStyle, CellsColor borderColor)
```


Définit les bordures du style.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| borderType | int | [BorderType](../../com.aspose.cells/bordertype). La/les bordure(s) à définir, peut être une combinaison de [BorderType](../../com.aspose.cells/bordertype). |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Le style de la bordure. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | La couleur de la bordure. |

**Returns:**
boolean - Indique si les paramètres actuels de la bordure ont été modifiés.
### setBorder(int borderType, int borderStyle, Color borderColor) {#setBorder-int-int-com.aspose.cells.Color-}
```
public boolean setBorder(int borderType, int borderStyle, Color borderColor)
```


Définit les bordures du style.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| borderType | int | [BorderType](../../com.aspose.cells/bordertype). La/les bordure(s) à définir, peut être une combinaison de [BorderType](../../com.aspose.cells/bordertype). |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Le style de la bordure. |
| borderColor | [Color](../../com.aspose.cells/color) | La couleur de la bordure. |

**Returns:**
boolean - Indique si les paramètres actuels de la bordure ont été modifiés.
### setBorderApplied(boolean value) {#setBorderApplied-boolean-}
```
public void setBorderApplied(boolean value)
```


Indique si le formatage de bordure doit être appliqué.

**Remarks**

Uniquement pour le style nommé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setCheckBox(boolean value) {#setCheckBox-boolean-}
```
public void setCheckBox(boolean value)
```


Indique s'il s'agit d'un style de case à cocher

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setCultureCustom(String value) {#setCultureCustom-java.lang.String-}
```
public void setCultureCustom(String value)
```


Définit la chaîne de modèle dépendante de la culture pour le format de nombre. Si aucun format de nombre n'a été défini pour cet objet, null sera retourné. Si le format de nombre est intégré, la chaîne de modèle correspondant au nombre intégré sera retournée.

**Remarks**

Pour les formats numériques intégrés, à la fois le contenu du modèle (par exemple, un format de date intégré est \"m/d/y\" pour certaines locales, mais devient \"d/m/y\" pour d'autres) et le spécificateur de format (par exemple, certaines locales utilisent un caractère différent de 'y' pour représenter la partie année du format de date) sont dépendants de la culture ; pour un format personnalisé spécifié par l'utilisateur, seuls les spécificateurs de format sont modifiés selon la culture, les autres parties du modèle de format ne seront pas modifiées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setCustom(String value) {#setCustom-java.lang.String-}
```
public void setCustom(String value)
```


Représente la chaîne de format numérique personnalisé de cet objet style. Si le format numérique personnalisé n'est pas défini (par exemple, le format numérique est intégré), \"\" sera renvoyé.

**Remarks**

La chaîne personnalisée renvoyée est indépendante de la culture.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setCustom(String custom, boolean builtinPreference) {#setCustom-java.lang.String-boolean-}
```
public void setCustom(String custom, boolean builtinPreference)
```


Définit la chaîne de format de nombre personnalisé d'une cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| personnalisé | java.lang.String | Chaîne de format de nombre personnalisée, doit être le modèle InvariantCulture. |
| builtinPreference | boolean | Si la chaîne de format de nombre personnalisée fournie correspond à l'un des formats de nombre intégrés correspondant aux paramètres régionaux actuels, indique si le format de nombre doit être défini comme intégré plutôt que personnalisé. |

### setFillApplied(boolean value) {#setFillApplied-boolean-}
```
public void setFillApplied(boolean value)
```


Indique si le formatage de remplissage doit être appliqué.

**Remarks**

Uniquement pour le style nommé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setFontApplied(boolean value) {#setFontApplied-boolean-}
```
public void setFontApplied(boolean value)
```


Indique si le formatage de police doit être appliqué.

**Remarks**

Uniquement pour le style nommé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setForegroundArgbColor(int value) {#setForegroundArgbColor-int-}
```
public void setForegroundArgbColor(int value)
```


Définit la couleur de premier plan avec une valeur ARGB 32 bits.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setForegroundColor(Color value) {#setForegroundColor-com.aspose.cells.Color-}
```
public void setForegroundColor(Color value)
```


Définit la couleur de premier plan d'un style.

**Remarks**

Cela signifie qu'aucun réglage de couleur n'est appliqué si Color.Empty est renvoyé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setForegroundThemeColor(ThemeColor value) {#setForegroundThemeColor-com.aspose.cells.ThemeColor-}
```
public void setForegroundThemeColor(ThemeColor value)
```


Définit la couleur du thème de premier plan.

**Remarks**

Si la couleur de premier plan n'est pas une couleur de thème, NULL sera renvoyé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setFormulaHidden(boolean value) {#setFormulaHidden-boolean-}
```
public void setFormulaHidden(boolean value)
```


Représente si la formule sera masquée lorsque la feuille de calcul est protégée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setGradient(boolean value) {#setGradient-boolean-}
```
public void setGradient(boolean value)
```


Indique si le remplissage de la cellule est un motif dégradé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setHorizontalAlignment(int value) {#setHorizontalAlignment-int-}
```
public void setHorizontalAlignment(int value)
```


Définit le type d'alignement horizontal du texte dans une cellule.

Voir [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setIndentLevel(int value) {#setIndentLevel-int-}
```
public void setIndentLevel(int value)
```


Représente le niveau d'indentation pour la cellule ou la plage. Ne peut être qu'un entier compris entre 0 et 250.

**Remarks**

Si le type d'alignement horizontal du texte est défini sur une valeur autre que gauche ou droite, le niveau d'indentation sera réinitialisé à zéro.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setJustifyDistributed(boolean value) {#setJustifyDistributed-boolean-}
```
public void setJustifyDistributed(boolean value)
```


Indique si l'alignement justifié ou distribué des cellules doit être utilisé sur la dernière ligne de texte.

**Remarks**

Ceci est typique pour les alignements d'Asie de l'Est mais pas typique dans d'autres contextes. Ne fonctionne que lorsque l'alignement horizontal est distribué.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Définit une valeur indiquant si une cellule peut être modifiée ou non.

**Remarks**

Le verrouillage des cellules n'a aucun effet à moins que la feuille de calcul ne soit protégée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Définit le nom du style.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setNumber(int value) {#setNumber-int-}
```
public void setNumber(int value)
```


Définit le format d'affichage des nombres et des dates. Les modèles de formatage diffèrent selon les régions.

**Remarks**

Par exemple, les modèles de formatage représentés par des nombres pour la région en\\_US :

| Valeur | Type | Chaîne de format |
| ----- | ---------- | ---------------------------------------------------- |
| 0 | General | `General` |
| 1 | Decimal | `0` |
| 2 | Decimal | `0.00` |
| 3 | Decimal | `#,##0` |
| 4 | Decimal | `#,##0.00` |
| 5 | Currency | `$#,##0_);($#,##0)` |
| 6 | Currency | `$#,##0_);[Rouge](../$#,##0)` |
| 7 | Currency | `$#,##0.00_);($#,##0.00)` |
| 8 | Currency | `$#,##0.00_);[Rouge](../$#,##0.00)` |
| 9 | Percentage | `0%` |
| 10 | Percentage | `0.00%` |
| 11 | Scientific | `0.00E+00` |
| 12 | Fraction | `# ?/?` |
| 13 | Fraction | `# ??/??` |
| 14 | Date | `jj/mm/aaaa` |
| 15 | Date | `jj-mmm-aa` |
| 16 | Date | `jj-mmm` |
| 17 | Date | `mmm-aa` |
| 18 | Time | `hh:mm` |
| 19 | Time | `hh:mm:ss` |
| 20 | Time | `hh:mm` |
| 21 | Time | `hh:mm:ss` |
| 22 | Time | `jj/mm/aaaa hh:mm` |
| 37 | Accounting | `#,##0_);(#,##0)` |
| 38 | Accounting | `#,##0_);[Rouge](../#,##0)` |
| 39 | Accounting | `#,##0.00_);(#,##0.00)` |
| 40 | Accounting | `#,##0.00_);[Rouge](../#,##0.00)` |
| 41 | Accounting | `_(* #,##0_);_(* (#,##0);_(* "-"_);_(@_)` |
| 42 | Currency | `_($* #,##0_);_($* (#,##0);_($* "-"_);_(@_)` |
| 43 | Accounting | `_(* #,##0.00_);_(* (#,##0.00);_(* "-"??_);_(@_)` |
| 44 | Currency | `_($* #,##0.00_);_($* (#,##0.00);_($* "-"??_);_(@_)` |
| 45 | Time | `mm:ss` |
| 46 | Time | `[h]:mm:ss` |
| 47 | Time | `mm:ss.0` |
| 48 | Scientific | `##0.0E+0` |
| 49 | Text | `@` |

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setNumberFormatApplied(boolean value) {#setNumberFormatApplied-boolean-}
```
public void setNumberFormatApplied(boolean value)
```


Indique si le formatage des nombres doit être appliqué.

**Remarks**

Uniquement pour le style nommé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setOutlineBorders(int borderStyle, CellsColor borderColor) {#setOutlineBorders-int-com.aspose.cells.CellsColor-}
```
public void setOutlineBorders(int borderStyle, CellsColor borderColor)
```


Définir les bordures de contour

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Le type de bordures. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | La couleur des bordures |

### setOutlineBorders(int borderStyle, Color borderColor) {#setOutlineBorders-int-com.aspose.cells.Color-}
```
public void setOutlineBorders(int borderStyle, Color borderColor)
```


Définir les bordures de contour

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Le type de bordures. |
| borderColor | [Color](../../com.aspose.cells/color) | La couleur des bordures |

### setPattern(int value) {#setPattern-int-}
```
public void setPattern(int value)
```


Définit le type de motif d'arrière-plan de la cellule.

Voir [BackgroundType](../../com.aspose.cells/backgroundtype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setPatternColor(int pattern, Color color1, Color color2) {#setPatternColor-int-com.aspose.cells.Color-com.aspose.cells.Color-}
```
public void setPatternColor(int pattern, Color color1, Color color2)
```


Définit la couleur d'arrière-plan.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| pattern | int | [BackgroundType](../../com.aspose.cells/backgroundtype). Le modèle. |
| color1 | [Color](../../com.aspose.cells/color) | La couleur de premier plan. |
| color2 | [Color](../../com.aspose.cells/color) | La couleur d'arrière-plan. Fonctionne uniquement lorsque le modèle n'est pas BackgroundType.None et BackgroundType.Solid. |

### setProtectionApplied(boolean value) {#setProtectionApplied-boolean-}
```
public void setProtectionApplied(boolean value)
```


Indique si le formatage de protection doit être appliqué.

**Remarks**

Uniquement pour le style nommé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setQuotePrefix(boolean value) {#setQuotePrefix-boolean-}
```
public void setQuotePrefix(boolean value)
```


Indique si la valeur de la cellule commence par une apostrophe.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setRotationAngle(int value) {#setRotationAngle-int-}
```
public void setRotationAngle(int value)
```


Représente l'angle de rotation du texte.

**Remarks**

0: Non pivoté.

255: De haut en bas.

\-90: Vers le bas.

90: Vers le haut.

Vous pouvez définir 255 ou une valeur comprise entre -90 et 90.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setShrinkToFit(boolean value) {#setShrinkToFit-boolean-}
```
public void setShrinkToFit(boolean value)
```


Représente si le texte se réduit automatiquement pour s'adapter à la largeur de colonne disponible.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setTextDirection(int value) {#setTextDirection-int-}
```
public void setTextDirection(int value)
```


Représente l'ordre de lecture du texte.

Voir [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


Définit une valeur indiquant si le texte à l'intérieur d'une cellule est renvoyé à la ligne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setTwoColorGradient(Color color1, Color color2, int gradientStyleType, int variant) {#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-}
```
public void setTwoColorGradient(Color color1, Color color2, int gradientStyleType, int variant)
```


Définit le remplissage spécifié à un dégradé à deux couleurs.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | Une couleur de dégradé. |
| color2 | [Color](../../com.aspose.cells/color) | Deux couleurs de dégradé. |
| gradientStyleType | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Style d'ombrage du dégradé. |
| variante | int | La variante de dégradé. Peut être une valeur de 1 à 4, correspondant à l'une des quatre variantes dans l'onglet Gradient de la boîte de dialogue Remplissage d'effets. Si le style est GradientStyle.FromCenter, l'argument Variant ne peut être que 1 ou 2. |

### setVerticalAlignment(int value) {#setVerticalAlignment-int-}
```
public void setVerticalAlignment(int value)
```


Définit le type d'alignement vertical du texte dans une cellule.

Voir [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### toJson() {#toJson--}
```
public String toJson()
```


Convertir [Style](../../com.aspose.cells/style) en données de structure JSON.

**Returns:**
java.lang.String -
### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### update() {#update--}
```
public void update()
```


Applique le style nommé aux styles des cellules qui utilisent ce style nommé. Cela fonctionne comme cliquer sur le bouton "ok" après avoir terminé la modification du style. S'applique uniquement au style nommé.

### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

