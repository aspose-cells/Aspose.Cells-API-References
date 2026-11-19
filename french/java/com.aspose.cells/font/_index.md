---
title: "Font"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Encapsule l'objet police utilisé dans une feuille de calcul."
type: docs
url: /fr/java/com.aspose.cells/font/
---

**Inheritance:**
java.lang.Object
```
public class Font
```

Encapsule l'objet police utilisé dans une feuille de calcul.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         //Accessing the "A1" cell from the worksheet
         Cell cell = worksheet.getCells().get("A1");
 
         //Adding some value to the "A1" cell
         cell.putValue("Hello Aspose!");
 
         Font font = cell.getStyle().getFont();
 
         //Setting the font name to "Times New Roman"
         font.setName("Times New Roman");
 
         //Setting font size to 14
         font.setSize(14);
 
         //setting font color as Red
         font.setColor(com.aspose.cells.Color.getRed());           
 
         //Saving the Excel file
         workbook.save("dest.xls");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Font font)](#equals-com.aspose.cells.Font-) | Vérifie si deux polices sont égales. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgbColor()](#getArgbColor--) | Obtient la couleur avec une valeur ARGB sur 32 bits. |
| [getCapsType()](#getCapsType--) | Obtient le type de majuscules du texte. |
| [getCharset()](#getCharset--) | Représente le jeu de caractères. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Obtient le [Color](../../com.aspose.cells/color) de la police. |
| [getDoubleSize()](#getDoubleSize--) | Obtient la taille double de la police. |
| [getName()](#getName--) | Obtient le nom de la [Font](../../com.aspose.cells/font). |
| [getSchemeType()](#getSchemeType--) | Obtient le type de schéma de la police. |
| [getScriptOffset()](#getScriptOffset--) | Obtient le décalage du script,in unité de pourcentage |
| [getSize()](#getSize--) | Obtient la taille de la police. |
| [getStrikeType()](#getStrikeType--) | Obtient le type de rayure du texte. |
| [getThemeColor()](#getThemeColor--) | Obtient la couleur du thème. |
| [getUnderline()](#getUnderline--) | Obtient le type de soulignement de la police. |
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
| [setCapsType(int value)](#setCapsType-int-) | Définit le type de majuscules du texte. |
| [setCharset(int value)](#setCharset-int-) | Représente le jeu de caractères. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Définit la [Color](../../com.aspose.cells/color) de la police. |
| [setDoubleSize(double value)](#setDoubleSize-double-) | Définit la taille double de la police. |
| [setItalic(boolean value)](#setItalic-boolean-) | Définit une valeur indiquant si la police est en italique. |
| [setName(String value)](#setName-java.lang.String-) | Définit le nom de la [Font](../../com.aspose.cells/font). |
| [setName(String name, int type)](#setName-java.lang.String-int-) | Définit le nom et le schéma de la police. |
| [setNormalizeHeights(boolean value)](#setNormalizeHeights-boolean-) | Indique si la normalisation de la hauteur doit être appliquée au segment de texte. |
| [setSchemeType(int value)](#setSchemeType-int-) | Définit le type de schéma de la police. |
| [setScriptOffset(double value)](#setScriptOffset-double-) | Définit le décalage du script,in unité de pourcentage |
| [setSize(int value)](#setSize-int-) | Définit la taille de la police. |
| [setStrikeType(int value)](#setStrikeType-int-) | Obtient le type de rayure du texte. |
| [setStrikeout(boolean value)](#setStrikeout-boolean-) | Définit une valeur indiquant si la police est à simple barré. |
| [setSubscript(boolean value)](#setSubscript-boolean-) | Définit une valeur indiquant si la police est en indice. |
| [setSuperscript(boolean value)](#setSuperscript-boolean-) | Définit une valeur indiquant si la police est en exposant. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Définit la couleur du thème. |
| [setUnderline(int value)](#setUnderline-int-) | Définit le type de soulignement de la police. |
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


Obtient le type de majuscules du texte.

Voir [TextCapsType](../../com.aspose.cells/textcapstype).

**Remarks**

Uniquement pour les polices des formes ou des graphiques. NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété [TextOptions.getCapsType()](../../com.aspose.cells/textoptions\#getCapsType--). Cette propriété sera supprimée 12 mois après janvier 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

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
### getName() {#getName--}
```
public String getName()
```


Obtient le nom de la [Font](../../com.aspose.cells/font).

**Remarks**

Si cette propriété est utilisée pour définir le nom de la police, le [getSchemeType()](../../com.aspose.cells/font\#getSchemeType--) sera mis à jour vers [FontSchemeType.NONE](../../com.aspose.cells/fontschemetype\#NONE).

**Returns:**
java.lang.String
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
### getSize() {#getSize--}
```
public int getSize()
```


Obtient la taille de la police.

**Returns:**
int
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

Uniquement pour les polices des formes ou des graphiques. NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété [TextOptions.isNormalizeHeights()](../../com.aspose.cells/textoptions\#isNormalizeHeights--). Cette propriété sera supprimée 12 mois après janvier 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

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


Définit le type de majuscules du texte.

Voir [TextCapsType](../../com.aspose.cells/textcapstype).

**Remarks**

Uniquement pour les polices des formes ou des graphiques. NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété [TextOptions.getCapsType()](../../com.aspose.cells/textoptions\#getCapsType--). Cette propriété sera supprimée 12 mois après janvier 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

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

### setItalic(boolean value) {#setItalic-boolean-}
```
public void setItalic(boolean value)
```


Définit une valeur indiquant si la police est en italique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Définit le nom de la [Font](../../com.aspose.cells/font).

**Remarks**

Si cette propriété est utilisée pour définir le nom de la police, le [getSchemeType()](../../com.aspose.cells/font\#getSchemeType--) sera mis à jour vers [FontSchemeType.NONE](../../com.aspose.cells/fontschemetype\#NONE).

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

Uniquement pour les polices des formes ou des graphiques. NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété [TextOptions.isNormalizeHeights()](../../com.aspose.cells/textoptions\#isNormalizeHeights--). Cette propriété sera supprimée 12 mois après janvier 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

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

