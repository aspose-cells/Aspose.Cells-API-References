---
title: "TextOptions"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente les options de texte."
type: docs
url: /fr/java/com.aspose.cells/textoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Font](../../com.aspose.cells/font)
```
public class TextOptions extends Font
```

Représente les options de texte.
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Font font)](#equals-com.aspose.cells.Font-) | Vérifie si deux polices sont égales. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgbColor()](#getArgbColor--) | Obtient la couleur avec une valeur ARGB sur 32 bits. |
| [getCapsType()](#getCapsType--) | Obtient le type de majuscules pour les textes de la forme. |
| [getCharset()](#getCharset--) | Représente le jeu de caractères. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Obtient le [Color](../../com.aspose.cells/color) de la police. |
| [getDoubleSize()](#getDoubleSize--) | Obtient la taille double de la police. |
| [getFarEastName()](#getFarEastName--) | Obtient le nom FarEast. |
| [getFill()](#getFill--) | Représente le format de remplissage du texte. |
| [getKerning()](#getKerning--) | Spécifie la taille minimale de police à laquelle le crénage des caractères se produira pour cette séquence de texte. |
| [getLanguageCode()](#getLanguageCode--) | Obtient la langue de l'interface utilisateur. |
| [getLatinName()](#getLatinName--) | Obtient le nom latin. |
| [getName()](#getName--) | Obtient le nom de la forme. |
| [getOutline()](#getOutline--) | Représente le format de contour du texte. |
| [getSchemeType()](#getSchemeType--) | Obtient le type de schéma de la police. |
| [getScriptOffset()](#getScriptOffset--) | Obtient le décalage du script,in unité de pourcentage |
| [getShadow()](#getShadow--) | Représente un objet [ShadowEffect](../../com.aspose.cells/shadoweffect) qui spécifie l'effet d'ombre pour l'élément de graphique ou la forme. |
| [getSize()](#getSize--) | Obtient la taille de la police. |
| [getSpacing()](#getSpacing--) | Spécifie l'espacement entre les caractères au sein d'un segment de texte. |
| [getStrikeType()](#getStrikeType--) | Obtient le type de rayure du texte. |
| [getThemeColor()](#getThemeColor--) | Obtient la couleur du thème. |
| [getUnderline()](#getUnderline--) | Obtient le type de soulignement de la police. |
| [getUnderlineColor()](#getUnderlineColor--) | Obtient la couleur du soulignement. |
| [hashCode()](#hashCode--) |  |
| [isBold()](#isBold--) | Obtient une valeur indiquant si la police est en gras. |
| [isItalic()](#isItalic--) | Obtient une valeur indiquant si la police est en italique. |
| [isNormalizeHeights()](#isNormalizeHeights--) | Indique si la normalisation de la hauteur doit être appliquée au segment de texte. |
| [isStrikeout()](#isStrikeout--) | Obtient une valeur indiquant si la police est à simple barré. |
| [isSubscript()](#isSubscript--) | Obtient une valeur indiquant si la police est en indice. |
| [isSuperscript()](#isSuperscript--) | Obtient une valeur indiquant si la police est en exposant. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setArgbColor(int value)](#setArgbColor-int-) | Définit la couleur avec une valeur ARGB sur 32 bits. |
| [setBold(boolean value)](#setBold-boolean-) | Définit une valeur indiquant si la police est en gras. |
| [setCapsType(int value)](#setCapsType-int-) | Définit le type de majuscules pour le texte de la forme. |
| [setCharset(int value)](#setCharset-int-) | Représente le jeu de caractères. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Définit la [Color](../../com.aspose.cells/color) de la police. |
| [setDoubleSize(double value)](#setDoubleSize-double-) | Définit la taille double de la police. |
| [setFarEastName(String value)](#setFarEastName-java.lang.String-) | Définit le nom FarEast. |
| [setItalic(boolean value)](#setItalic-boolean-) | Définit une valeur indiquant si la police est en italique. |
| [setKerning(double value)](#setKerning-double-) | Spécifie la taille minimale de police à laquelle le crénage des caractères se produira pour cette séquence de texte. |
| [setLanguageCode(int value)](#setLanguageCode-int-) | Définit la langue de l'interface utilisateur. |
| [setLatinName(String value)](#setLatinName-java.lang.String-) | Définit le nom latin. |
| [setName(String value)](#setName-java.lang.String-) | Définit le nom de la forme. |
| [setName(String name, int type)](#setName-java.lang.String-int-) | Définit le nom et le schéma de la police. |
| [setNormalizeHeights(boolean value)](#setNormalizeHeights-boolean-) | Indique si la normalisation de la hauteur doit être appliquée au segment de texte. |
| [setSchemeType(int value)](#setSchemeType-int-) | Définit le type de schéma de la police. |
| [setScriptOffset(double value)](#setScriptOffset-double-) | Définit le décalage du script,in unité de pourcentage |
| [setSize(int value)](#setSize-int-) | Définit la taille de la police. |
| [setSpacing(double value)](#setSpacing-double-) | Spécifie l'espacement entre les caractères au sein d'un segment de texte. |
| [setStrikeType(int value)](#setStrikeType-int-) | Obtient le type de rayure du texte. |
| [setStrikeout(boolean value)](#setStrikeout-boolean-) | Définit une valeur indiquant si la police est à simple barré. |
| [setSubscript(boolean value)](#setSubscript-boolean-) | Définit une valeur indiquant si la police est en indice. |
| [setSuperscript(boolean value)](#setSuperscript-boolean-) | Définit une valeur indiquant si la police est en exposant. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Définit la couleur du thème. |
| [setUnderline(int value)](#setUnderline-int-) | Définit le type de soulignement de la police. |
| [setUnderlineColor(CellsColor value)](#setUnderlineColor-com.aspose.cells.CellsColor-) | Définit la couleur du soulignement. |
| [toString()](#toString--) | Renvoie une chaîne qui représente l'objet Cell actuel. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Font font) {#equals-com.aspose.cells.Font-}
```
public boolean equals(Font font)
```


Vérifie si deux polices sont égales.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| font | [Font](../../com.aspose.cells/font) | Objet police comparé. |

**Returns:**
booléen - Vrai si égal à l'objet police comparé.
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getArgbColor() {#getArgbColor--}
```
public int getArgbColor()
```


Obtient la couleur avec une valeur ARGB sur 32 bits.

**Returns:**
int
### getCapsType() {#getCapsType--}
```
public int getCapsType()
```


Obtient le type de majuscules pour les textes de la forme.

Voir [TextCapsType](../../com.aspose.cells/textcapstype).

**Returns:**
int
### getCharset() {#getCharset--}
```
public int getCharset()
```


Représente le jeu de caractères.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColor() {#getColor--}
```
public Color getColor()
```


Obtient le [Color](../../com.aspose.cells/color) de la police.

**Returns:**
[Color](../../com.aspose.cells/color)
### getDoubleSize() {#getDoubleSize--}
```
public double getDoubleSize()
```


Obtient la taille double de la police.

**Returns:**
double
### getFarEastName() {#getFarEastName--}
```
public String getFarEastName()
```


Obtient le nom FarEast.

**Returns:**
java.lang.String
### getFill() {#getFill--}
```
public FillFormat getFill()
```


Représente le format de remplissage du texte.

**Returns:**
[FillFormat](../../com.aspose.cells/fillformat)
### getKerning() {#getKerning--}
```
public double getKerning()
```


Spécifie la taille minimale de police à laquelle le crénage des caractères se produira pour cette séquence de texte.

**Returns:**
double
### getLanguageCode() {#getLanguageCode--}
```
public int getLanguageCode()
```


Obtient la langue de l'interface utilisateur.

Voir [CountryCode](../../com.aspose.cells/countrycode).

**Returns:**
int
### getLatinName() {#getLatinName--}
```
public String getLatinName()
```


Obtient le nom latin.

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


Obtient le nom de la forme.

**Returns:**
java.lang.String
### getOutline() {#getOutline--}
```
public LineFormat getOutline()
```


Représente le format de contour du texte.

**Returns:**
[LineFormat](../../com.aspose.cells/lineformat)
### getSchemeType() {#getSchemeType--}
```
public int getSchemeType()
```


Obtient le type de schéma de la police.

Voir [FontSchemeType](../../com.aspose.cells/fontschemetype).

**Returns:**
int
### getScriptOffset() {#getScriptOffset--}
```
public double getScriptOffset()
```


Obtient le décalage du script,in unité de pourcentage

**Remarks**

Uniquement pour les formes et les graphiques.

**Returns:**
double
### getShadow() {#getShadow--}
```
public ShadowEffect getShadow()
```


Représente un objet [ShadowEffect](../../com.aspose.cells/shadoweffect) qui spécifie l'effet d'ombre pour l'élément de graphique ou la forme.

**Returns:**
[ShadowEffect](../../com.aspose.cells/shadoweffect)
### getSize() {#getSize--}
```
public int getSize()
```


Obtient la taille de la police.

**Returns:**
int
### getSpacing() {#getSpacing--}
```
public double getSpacing()
```


Spécifie l'espacement entre les caractères au sein d'un segment de texte.

**Returns:**
double
### getStrikeType() {#getStrikeType--}
```
public int getStrikeType()
```


Obtient le type de rayure du texte.

Voir [TextStrikeType](../../com.aspose.cells/textstriketype).

**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```


Obtient la couleur du thème.

**Remarks**

Si la couleur de la police n'est pas une couleur de thème, NULL sera renvoyé.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getUnderline() {#getUnderline--}
```
public int getUnderline()
```


Obtient le type de soulignement de la police.

Voir [FontUnderlineType](../../com.aspose.cells/fontunderlinetype).

**Returns:**
int
### getUnderlineColor() {#getUnderlineColor--}
```
public CellsColor getUnderlineColor()
```


Obtient la couleur du soulignement.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBold() {#isBold--}
```
public boolean isBold()
```


Obtient une valeur indiquant si la police est en gras.

**Returns:**
boolean
### isItalic() {#isItalic--}
```
public boolean isItalic()
```


Obtient une valeur indiquant si la police est en italique.

**Returns:**
boolean
### isNormalizeHeights() {#isNormalizeHeights--}
```
public boolean isNormalizeHeights()
```


Indique si la normalisation de la hauteur doit être appliquée au segment de texte.

**Remarks**

Uniquement pour les polices des formes ou des graphiques.

**Returns:**
boolean
### isStrikeout() {#isStrikeout--}
```
public boolean isStrikeout()
```


Obtient une valeur indiquant si la police est à simple barré.

**Returns:**
boolean
### isSubscript() {#isSubscript--}
```
public boolean isSubscript()
```


Obtient une valeur indiquant si la police est en indice.

**Returns:**
boolean
### isSuperscript() {#isSuperscript--}
```
public boolean isSuperscript()
```


Obtient une valeur indiquant si la police est en exposant.

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




### setArgbColor(int value) {#setArgbColor-int-}
```
public void setArgbColor(int value)
```


Définit la couleur avec une valeur ARGB sur 32 bits.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setBold(boolean value) {#setBold-boolean-}
```
public void setBold(boolean value)
```


Définit une valeur indiquant si la police est en gras.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setCapsType(int value) {#setCapsType-int-}
```
public void setCapsType(int value)
```


Définit le type de majuscules pour le texte de la forme.

Voir [TextCapsType](../../com.aspose.cells/textcapstype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setCharset(int value) {#setCharset-int-}
```
public void setCharset(int value)
```


Représente le jeu de caractères.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


Définit la [Color](../../com.aspose.cells/color) de la police.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setDoubleSize(double value) {#setDoubleSize-double-}
```
public void setDoubleSize(double value)
```


Définit la taille double de la police.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setFarEastName(String value) {#setFarEastName-java.lang.String-}
```
public void setFarEastName(String value)
```


Définit le nom FarEast.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setItalic(boolean value) {#setItalic-boolean-}
```
public void setItalic(boolean value)
```


Définit une valeur indiquant si la police est en italique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setKerning(double value) {#setKerning-double-}
```
public void setKerning(double value)
```


Spécifie la taille minimale de police à laquelle le crénage des caractères se produira pour cette séquence de texte.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setLanguageCode(int value) {#setLanguageCode-int-}
```
public void setLanguageCode(int value)
```


Définit la langue de l'interface utilisateur.

Voir [CountryCode](../../com.aspose.cells/countrycode).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setLatinName(String value) {#setLatinName-java.lang.String-}
```
public void setLatinName(String value)
```


Définit le nom latin.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Définit le nom de la forme.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setName(String name, int type) {#setName-java.lang.String-int-}
```
public void setName(String name, int type)
```


Définit le nom et le schéma de la police.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String |  |
| type | int | [FontSchemeType](../../com.aspose.cells/fontschemetype). |

### setNormalizeHeights(boolean value) {#setNormalizeHeights-boolean-}
```
public void setNormalizeHeights(boolean value)
```


Indique si la normalisation de la hauteur doit être appliquée au segment de texte.

**Remarks**

Uniquement pour les polices des formes ou des graphiques.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSchemeType(int value) {#setSchemeType-int-}
```
public void setSchemeType(int value)
```


Définit le type de schéma de la police.

Voir [FontSchemeType](../../com.aspose.cells/fontschemetype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setScriptOffset(double value) {#setScriptOffset-double-}
```
public void setScriptOffset(double value)
```


Définit le décalage du script,in unité de pourcentage

**Remarks**

Uniquement pour les formes et les graphiques.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setSize(int value) {#setSize-int-}
```
public void setSize(int value)
```


Définit la taille de la police.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setSpacing(double value) {#setSpacing-double-}
```
public void setSpacing(double value)
```


Spécifie l'espacement entre les caractères au sein d'un segment de texte.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setStrikeType(int value) {#setStrikeType-int-}
```
public void setStrikeType(int value)
```


Obtient le type de rayure du texte.

Voir [TextStrikeType](../../com.aspose.cells/textstriketype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setStrikeout(boolean value) {#setStrikeout-boolean-}
```
public void setStrikeout(boolean value)
```


Définit une valeur indiquant si la police est à simple barré.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSubscript(boolean value) {#setSubscript-boolean-}
```
public void setSubscript(boolean value)
```


Définit une valeur indiquant si la police est en indice.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSuperscript(boolean value) {#setSuperscript-boolean-}
```
public void setSuperscript(boolean value)
```


Définit une valeur indiquant si la police est en exposant.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


Définit la couleur du thème.

**Remarks**

Si la couleur de la police n'est pas une couleur de thème, NULL sera renvoyé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setUnderline(int value) {#setUnderline-int-}
```
public void setUnderline(int value)
```


Définit le type de soulignement de la police.

Voir [FontUnderlineType](../../com.aspose.cells/fontunderlinetype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setUnderlineColor(CellsColor value) {#setUnderlineColor-com.aspose.cells.CellsColor-}
```
public void setUnderlineColor(CellsColor value)
```


Définit la couleur du soulignement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### toString() {#toString--}
```
public String toString()
```


Renvoie une chaîne qui représente l'objet Cell actuel.

**Returns:**
java.lang.String -
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

