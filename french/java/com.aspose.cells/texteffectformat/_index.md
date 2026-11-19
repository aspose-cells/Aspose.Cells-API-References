---
title: "TextEffectFormat"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Contient les propriétés et méthodes qui s'appliquent aux objets WordArt."
type: docs
url: /fr/java/com.aspose.cells/texteffectformat/
---

**Inheritance:**
java.lang.Object
```
public class TextEffectFormat
```

Contient les propriétés et méthodes qui s'appliquent aux objets WordArt.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         ShapeCollection shapes = workbook.getWorksheets().get(0).getShapes();
         shapes.addTextEffect(MsoPresetTextEffect.TEXT_EFFECT_1, "Aspose", "Arial", 30, false, false, 0, 0, 0, 0, 100, 200);
         TextEffectFormat textEffectFormat = shapes.get(0).getTextEffect();
         textEffectFormat.setTextEffect(MsoPresetTextEffect.TEXT_EFFECT_10);
         workbook.save("Book1.xls");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFontBold()](#getFontBold--) | Indique si la police est en gras. |
| [getFontItalic()](#getFontItalic--) | Indique si la police est en italique. |
| [getFontName()](#getFontName--) | Le nom de la police utilisée dans le WordArt. |
| [getFontSize()](#getFontSize--) | La taille (en points) de la police utilisée dans le WordArt. |
| [getPresetShape()](#getPresetShape--) | Obtient le type de forme prédéfini. |
| [getRotatedChars()](#getRotatedChars--) | Si true, les caractères du WordArt spécifié sont tournés de 90 degrés par rapport à la forme englobante du WordArt. |
| [getText()](#getText--) | Le texte dans le WordArt. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFontBold(boolean value)](#setFontBold-boolean-) | Indique si la police est en gras. |
| [setFontItalic(boolean value)](#setFontItalic-boolean-) | Indique si la police est en italique. |
| [setFontName(String value)](#setFontName-java.lang.String-) | Le nom de la police utilisée dans le WordArt. |
| [setFontSize(int value)](#setFontSize-int-) | La taille (en points) de la police utilisée dans le WordArt. |
| [setPresetShape(int value)](#setPresetShape-int-) | Définit le type de forme prédéfini. |
| [setRotatedChars(boolean value)](#setRotatedChars-boolean-) | Si true, les caractères du WordArt spécifié sont tournés de 90 degrés par rapport à la forme englobante du WordArt. |
| [setText(String value)](#setText-java.lang.String-) | Le texte dans le WordArt. |
| [setTextEffect(int effect)](#setTextEffect-int-) | Définit l'effet de texte prédéfini. |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFontBold() {#getFontBold--}
```
public boolean getFontBold()
```


Indique si la police est en gras.

**Returns:**
boolean
### getFontItalic() {#getFontItalic--}
```
public boolean getFontItalic()
```


Indique si la police est en italique.

**Returns:**
boolean
### getFontName() {#getFontName--}
```
public String getFontName()
```


Le nom de la police utilisée dans le WordArt.

**Returns:**
java.lang.String
### getFontSize() {#getFontSize--}
```
public int getFontSize()
```


La taille (en points) de la police utilisée dans le WordArt.

**Returns:**
int
### getPresetShape() {#getPresetShape--}
```
public int getPresetShape()
```


Obtient le type de forme prédéfini.

Voir [MsoPresetTextEffectShape](../../com.aspose.cells/msopresettexteffectshape).

**Returns:**
int
### getRotatedChars() {#getRotatedChars--}
```
public boolean getRotatedChars()
```


Si true, les caractères du WordArt spécifié sont tournés de 90 degrés par rapport à la forme englobante du WordArt.

**Returns:**
boolean
### getText() {#getText--}
```
public String getText()
```


Le texte dans le WordArt.

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setFontBold(boolean value) {#setFontBold-boolean-}
```
public void setFontBold(boolean value)
```


Indique si la police est en gras.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setFontItalic(boolean value) {#setFontItalic-boolean-}
```
public void setFontItalic(boolean value)
```


Indique si la police est en italique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setFontName(String value) {#setFontName-java.lang.String-}
```
public void setFontName(String value)
```


Le nom de la police utilisée dans le WordArt.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setFontSize(int value) {#setFontSize-int-}
```
public void setFontSize(int value)
```


La taille (en points) de la police utilisée dans le WordArt.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setPresetShape(int value) {#setPresetShape-int-}
```
public void setPresetShape(int value)
```


Définit le type de forme prédéfini.

Voir [MsoPresetTextEffectShape](../../com.aspose.cells/msopresettexteffectshape).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setRotatedChars(boolean value) {#setRotatedChars-boolean-}
```
public void setRotatedChars(boolean value)
```


Si true, les caractères du WordArt spécifié sont tournés de 90 degrés par rapport à la forme englobante du WordArt.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Le texte dans le WordArt.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setTextEffect(int effect) {#setTextEffect-int-}
```
public void setTextEffect(int effect)
```


Définit l'effet de texte prédéfini.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| effect | int | [MsoPresetTextEffect](../../com.aspose.cells/msopresettexteffect). L'effet de texte prédéfini. |

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

