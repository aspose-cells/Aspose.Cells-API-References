---
title: "TextParagraph"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente le paramètre de paragraphe de texte."
type: docs
url: /fr/java/com.aspose.cells/textparagraph/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.FontSetting](../../com.aspose.cells/fontsetting)
```
public class TextParagraph extends FontSetting
```

Représente le paramètre de paragraphe de texte.
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlignmentType()](#getAlignmentType--) | Obtient le type d'alignement horizontal du texte du paragraphe. |
| [getBullet()](#getBullet--) | Obtient la puce. |
| [getChildren()](#getChildren--) | Obtient toutes les séquences de texte dans ce paragraphe. |
| [getClass()](#getClass--) |  |
| [getDefaultTabSize()](#getDefaultTabSize--) | Obtient la taille par défaut d'un caractère de tabulation dans ce paragraphe. |
| [getFirstLineIndent()](#getFirstLineIndent--) | Spécifie la taille de l'indentation qui sera appliquée à la première ligne de texte du paragraphe. |
| [getFont()](#getFont--) | Renvoie la police de cet objet. |
| [getFontAlignType()](#getFontAlignType--) | Détermine où, verticalement, sur une ligne de texte, les mots réels sont positionnés. |
| [getLeftMargin()](#getLeftMargin--) | Spécifie la marge gauche du paragraphe. |
| [getLength()](#getLength--) | Obtient la longueur des caractères. |
| [getLineSpace()](#getLineSpace--) | Obtient la quantité d'espace blanc vertical qui sera utilisé dans un paragraphe. |
| [getLineSpaceSizeType()](#getLineSpaceSizeType--) | Obtient la quantité d'espace blanc vertical qui sera utilisé dans un paragraphe. |
| [getRightMargin()](#getRightMargin--) | Spécifie la marge droite du paragraphe. |
| [getSpaceAfter()](#getSpaceAfter--) | Obtient la quantité d'espace blanc vertical qui sera présente après un paragraphe. |
| [getSpaceAfterSizeType()](#getSpaceAfterSizeType--) | Obtient la quantité d'espace blanc vertical qui sera présente après un paragraphe. |
| [getSpaceBefore()](#getSpaceBefore--) | Obtient la quantité d'espace blanc vertical qui sera présente avant un paragraphe. |
| [getSpaceBeforeSizeType()](#getSpaceBeforeSizeType--) | Obtient la quantité d'espace blanc vertical qui sera présente avant un paragraphe. |
| [getStartIndex()](#getStartIndex--) | Obtient l'index de départ des caractères. |
| [getStops()](#getStops--) | Obtient la liste des tabulations. |
| [getTextOptions()](#getTextOptions--) | Renvoie les options de texte. |
| [getType()](#getType--) | Obtient le type de nœud de texte. |
| [hashCode()](#hashCode--) |  |
| [isEastAsianLineBreak()](#isEastAsianLineBreak--) | Spécifie si un mot d'Asie de l'Est peut être coupé en deux et renvoyé à la ligne suivante sans qu'un trait d'union ne soit ajouté. |
| [isHangingPunctuation()](#isHangingPunctuation--) | Spécifie si la ponctuation doit être forcée à se placer sur une ligne de texte ou mise sur une ligne de texte différente. |
| [isLatinLineBreak()](#isLatinLineBreak--) | Spécifie si un mot latin peut être coupé en deux et renvoyé à la ligne suivante sans qu'un trait d'union ne soit ajouté. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlignmentType(int value)](#setAlignmentType-int-) | Définit le type d'alignement horizontal du texte du paragraphe. |
| [setDefaultTabSize(double value)](#setDefaultTabSize-double-) | Définit la taille par défaut d'un caractère de tabulation dans ce paragraphe. |
| [setEastAsianLineBreak(boolean value)](#setEastAsianLineBreak-boolean-) | Spécifie si un mot d'Asie de l'Est peut être coupé en deux et renvoyé à la ligne suivante sans qu'un trait d'union ne soit ajouté. |
| [setFirstLineIndent(double value)](#setFirstLineIndent-double-) | Spécifie la taille de l'indentation qui sera appliquée à la première ligne de texte du paragraphe. |
| [setFontAlignType(int value)](#setFontAlignType-int-) | Détermine où, verticalement, sur une ligne de texte, les mots réels sont positionnés. |
| [setHangingPunctuation(boolean value)](#setHangingPunctuation-boolean-) | Spécifie si la ponctuation doit être forcée à se placer sur une ligne de texte ou mise sur une ligne de texte différente. |
| [setLatinLineBreak(boolean value)](#setLatinLineBreak-boolean-) | Spécifie si un mot latin peut être coupé en deux et renvoyé à la ligne suivante sans qu'un trait d'union ne soit ajouté. |
| [setLeftMargin(double value)](#setLeftMargin-double-) | Spécifie la marge gauche du paragraphe. |
| [setLineSpace(double value)](#setLineSpace-double-) | Définit la quantité d'espace blanc vertical qui sera utilisée dans un paragraphe. |
| [setLineSpaceSizeType(int value)](#setLineSpaceSizeType-int-) | Définit la quantité d'espace blanc vertical qui sera utilisée dans un paragraphe. |
| [setRightMargin(double value)](#setRightMargin-double-) | Spécifie la marge droite du paragraphe. |
| [setSpaceAfter(double value)](#setSpaceAfter-double-) | Définit la quantité d'espace blanc vertical qui sera présente après un paragraphe. |
| [setSpaceAfterSizeType(int value)](#setSpaceAfterSizeType-int-) | Définit la quantité d'espace blanc vertical qui sera présente après un paragraphe. |
| [setSpaceBefore(double value)](#setSpaceBefore-double-) | Définit la quantité d'espace blanc vertical qui sera présente avant un paragraphe. |
| [setSpaceBeforeSizeType(int value)](#setSpaceBeforeSizeType-int-) | Définit la quantité d'espace blanc vertical qui sera présente avant un paragraphe. |
| [setWordArtStyle(int style)](#setWordArtStyle-int-) | Définit le style WordArt prédéfini. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getAlignmentType() {#getAlignmentType--}
```
public int getAlignmentType()
```


Obtient le type d'alignement horizontal du texte du paragraphe.

Voir [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getBullet() {#getBullet--}
```
public Bullet getBullet()
```


Obtient la puce.

**Returns:**
[Bullet](../../com.aspose.cells/bullet)
### getChildren() {#getChildren--}
```
public FontSetting[] getChildren()
```


Obtient toutes les séquences de texte dans ce paragraphe. Si ce paragraphe est vide, renvoie le paragraphe lui‑même.

**Returns:**
com.aspose.cells.FontSetting[]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDefaultTabSize() {#getDefaultTabSize--}
```
public double getDefaultTabSize()
```


Obtient la taille par défaut d'un caractère de tabulation dans ce paragraphe.

**Returns:**
double
### getFirstLineIndent() {#getFirstLineIndent--}
```
public double getFirstLineIndent()
```


Spécifie la taille de l'indentation qui sera appliquée à la première ligne de texte du paragraphe.

**Returns:**
double
### getFont() {#getFont--}
```
public Font getFont()
```


Renvoie la police de cet objet.

**Returns:**
[Font](../../com.aspose.cells/font)
### getFontAlignType() {#getFontAlignType--}
```
public int getFontAlignType()
```


Détermine où, verticalement, sur une ligne de texte, les mots réels sont positionnés. Cela concerne le placement vertical des caractères par rapport aux lignes de base.

Voir [TextFontAlignType](../../com.aspose.cells/textfontaligntype).

**Returns:**
int
### getLeftMargin() {#getLeftMargin--}
```
public double getLeftMargin()
```


Spécifie la marge gauche du paragraphe.

**Returns:**
double
### getLength() {#getLength--}
```
public int getLength()
```


Obtient la longueur des caractères.

**Returns:**
int
### getLineSpace() {#getLineSpace--}
```
public double getLineSpace()
```


Obtient la quantité d'espace blanc vertical qui sera utilisé dans un paragraphe.

**Returns:**
double
### getLineSpaceSizeType() {#getLineSpaceSizeType--}
```
public int getLineSpaceSizeType()
```


Obtient la quantité d'espace blanc vertical qui sera utilisé dans un paragraphe.

Voir [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Returns:**
int
### getRightMargin() {#getRightMargin--}
```
public double getRightMargin()
```


Spécifie la marge droite du paragraphe.

**Returns:**
double
### getSpaceAfter() {#getSpaceAfter--}
```
public double getSpaceAfter()
```


Obtient la quantité d'espace blanc vertical qui sera présente après un paragraphe.

**Returns:**
double
### getSpaceAfterSizeType() {#getSpaceAfterSizeType--}
```
public int getSpaceAfterSizeType()
```


Obtient la quantité d'espace blanc vertical qui sera présente après un paragraphe.

Voir [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Returns:**
int
### getSpaceBefore() {#getSpaceBefore--}
```
public double getSpaceBefore()
```


Obtient la quantité d'espace blanc vertical qui sera présente avant un paragraphe.

**Returns:**
double
### getSpaceBeforeSizeType() {#getSpaceBeforeSizeType--}
```
public int getSpaceBeforeSizeType()
```


Obtient la quantité d'espace blanc vertical qui sera présente avant un paragraphe.

Voir [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Returns:**
int
### getStartIndex() {#getStartIndex--}
```
public int getStartIndex()
```


Obtient l'index de départ des caractères.

**Returns:**
int
### getStops() {#getStops--}
```
public TextTabStopCollection getStops()
```


Obtient la liste des tabulations.

**Returns:**
[TextTabStopCollection](../../com.aspose.cells/texttabstopcollection)
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


Renvoie les options de texte.

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getType() {#getType--}
```
public int getType()
```


Obtient le type de nœud de texte.

Voir [TextNodeType](../../com.aspose.cells/textnodetype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isEastAsianLineBreak() {#isEastAsianLineBreak--}
```
public boolean isEastAsianLineBreak()
```


Spécifie si un mot d'Asie de l'Est peut être coupé en deux et renvoyé à la ligne suivante sans qu'un trait d'union ne soit ajouté.

**Returns:**
boolean
### isHangingPunctuation() {#isHangingPunctuation--}
```
public boolean isHangingPunctuation()
```


Spécifie si la ponctuation doit être forcée à se placer sur une ligne de texte ou mise sur une ligne de texte différente.

**Returns:**
boolean
### isLatinLineBreak() {#isLatinLineBreak--}
```
public boolean isLatinLineBreak()
```


Spécifie si un mot latin peut être coupé en deux et renvoyé à la ligne suivante sans qu'un trait d'union ne soit ajouté.

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




### setAlignmentType(int value) {#setAlignmentType-int-}
```
public void setAlignmentType(int value)
```


Définit le type d'alignement horizontal du texte du paragraphe.

Voir [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setDefaultTabSize(double value) {#setDefaultTabSize-double-}
```
public void setDefaultTabSize(double value)
```


Définit la taille par défaut d'un caractère de tabulation dans ce paragraphe.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setEastAsianLineBreak(boolean value) {#setEastAsianLineBreak-boolean-}
```
public void setEastAsianLineBreak(boolean value)
```


Spécifie si un mot d'Asie de l'Est peut être coupé en deux et renvoyé à la ligne suivante sans qu'un trait d'union ne soit ajouté.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setFirstLineIndent(double value) {#setFirstLineIndent-double-}
```
public void setFirstLineIndent(double value)
```


Spécifie la taille de l'indentation qui sera appliquée à la première ligne de texte du paragraphe.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setFontAlignType(int value) {#setFontAlignType-int-}
```
public void setFontAlignType(int value)
```


Détermine où, verticalement, sur une ligne de texte, les mots réels sont positionnés. Cela concerne le placement vertical des caractères par rapport aux lignes de base.

Voir [TextFontAlignType](../../com.aspose.cells/textfontaligntype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setHangingPunctuation(boolean value) {#setHangingPunctuation-boolean-}
```
public void setHangingPunctuation(boolean value)
```


Spécifie si la ponctuation doit être forcée à se placer sur une ligne de texte ou mise sur une ligne de texte différente.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setLatinLineBreak(boolean value) {#setLatinLineBreak-boolean-}
```
public void setLatinLineBreak(boolean value)
```


Spécifie si un mot latin peut être coupé en deux et renvoyé à la ligne suivante sans qu'un trait d'union ne soit ajouté.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setLeftMargin(double value) {#setLeftMargin-double-}
```
public void setLeftMargin(double value)
```


Spécifie la marge gauche du paragraphe.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setLineSpace(double value) {#setLineSpace-double-}
```
public void setLineSpace(double value)
```


Définit la quantité d'espace blanc vertical qui sera utilisée dans un paragraphe.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setLineSpaceSizeType(int value) {#setLineSpaceSizeType-int-}
```
public void setLineSpaceSizeType(int value)
```


Définit la quantité d'espace blanc vertical qui sera utilisée dans un paragraphe.

Voir [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setRightMargin(double value) {#setRightMargin-double-}
```
public void setRightMargin(double value)
```


Spécifie la marge droite du paragraphe.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setSpaceAfter(double value) {#setSpaceAfter-double-}
```
public void setSpaceAfter(double value)
```


Définit la quantité d'espace blanc vertical qui sera présente après un paragraphe.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setSpaceAfterSizeType(int value) {#setSpaceAfterSizeType-int-}
```
public void setSpaceAfterSizeType(int value)
```


Définit la quantité d'espace blanc vertical qui sera présente après un paragraphe.

Voir [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setSpaceBefore(double value) {#setSpaceBefore-double-}
```
public void setSpaceBefore(double value)
```


Définit la quantité d'espace blanc vertical qui sera présente avant un paragraphe.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setSpaceBeforeSizeType(int value) {#setSpaceBeforeSizeType-int-}
```
public void setSpaceBeforeSizeType(int value)
```


Définit la quantité d'espace blanc vertical qui sera présente avant un paragraphe.

Voir [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setWordArtStyle(int style) {#setWordArtStyle-int-}
```
public void setWordArtStyle(int style)
```


Définit le style WordArt prédéfini.

**Remarks**

Uniquement pour le texte de la forme/graphique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| style | int | [PresetWordArtStyle](../../com.aspose.cells/presetwordartstyle). Le style WordArt prédéfini. |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
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

