---
title: "TextEffectFormat"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Contiene propiedades y métodos que se aplican a objetos WordArt."
type: docs
url: /es/java/com.aspose.cells/texteffectformat/
---

**Inheritance:**
java.lang.Object
```
public class TextEffectFormat
```

Contiene propiedades y métodos que se aplican a objetos WordArt.

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
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFontBold()](#getFontBold--) | Indica si la fuente está en negrita. |
| [getFontItalic()](#getFontItalic--) | Indica si la fuente está en cursiva. |
| [getFontName()](#getFontName--) | El nombre de la fuente utilizada en el WordArt. |
| [getFontSize()](#getFontSize--) | El tamaño (en puntos) de la fuente utilizada en el WordArt. |
| [getPresetShape()](#getPresetShape--) | Obtiene el tipo de forma predefinida. |
| [getRotatedChars()](#getRotatedChars--) | Si es true, los caracteres en el WordArt especificado se rotan 90 grados respecto a la forma delimitadora del WordArt. |
| [getText()](#getText--) | El texto en el WordArt. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFontBold(boolean value)](#setFontBold-boolean-) | Indica si la fuente está en negrita. |
| [setFontItalic(boolean value)](#setFontItalic-boolean-) | Indica si la fuente está en cursiva. |
| [setFontName(String value)](#setFontName-java.lang.String-) | El nombre de la fuente utilizada en el WordArt. |
| [setFontSize(int value)](#setFontSize-int-) | El tamaño (en puntos) de la fuente utilizada en el WordArt. |
| [setPresetShape(int value)](#setPresetShape-int-) | Establece el tipo de forma predefinida. |
| [setRotatedChars(boolean value)](#setRotatedChars-boolean-) | Si es true, los caracteres en el WordArt especificado se rotan 90 grados respecto a la forma delimitadora del WordArt. |
| [setText(String value)](#setText-java.lang.String-) | El texto en el WordArt. |
| [setTextEffect(int effect)](#setTextEffect-int-) | Establece el efecto de texto predefinido. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
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


Indica si la fuente está en negrita.

**Returns:**
boolean
### getFontItalic() {#getFontItalic--}
```
public boolean getFontItalic()
```


Indica si la fuente está en cursiva.

**Returns:**
boolean
### getFontName() {#getFontName--}
```
public String getFontName()
```


El nombre de la fuente utilizada en el WordArt.

**Returns:**
java.lang.String
### getFontSize() {#getFontSize--}
```
public int getFontSize()
```


El tamaño (en puntos) de la fuente utilizada en el WordArt.

**Returns:**
int
### getPresetShape() {#getPresetShape--}
```
public int getPresetShape()
```


Obtiene el tipo de forma predefinida.

Ver [MsoPresetTextEffectShape](../../com.aspose.cells/msopresettexteffectshape).

**Returns:**
int
### getRotatedChars() {#getRotatedChars--}
```
public boolean getRotatedChars()
```


Si es true, los caracteres en el WordArt especificado se rotan 90 grados respecto a la forma delimitadora del WordArt.

**Returns:**
boolean
### getText() {#getText--}
```
public String getText()
```


El texto en el WordArt.

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


Indica si la fuente está en negrita.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setFontItalic(boolean value) {#setFontItalic-boolean-}
```
public void setFontItalic(boolean value)
```


Indica si la fuente está en cursiva.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setFontName(String value) {#setFontName-java.lang.String-}
```
public void setFontName(String value)
```


El nombre de la fuente utilizada en el WordArt.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setFontSize(int value) {#setFontSize-int-}
```
public void setFontSize(int value)
```


El tamaño (en puntos) de la fuente utilizada en el WordArt.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setPresetShape(int value) {#setPresetShape-int-}
```
public void setPresetShape(int value)
```


Establece el tipo de forma predefinida.

Ver [MsoPresetTextEffectShape](../../com.aspose.cells/msopresettexteffectshape).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setRotatedChars(boolean value) {#setRotatedChars-boolean-}
```
public void setRotatedChars(boolean value)
```


Si es true, los caracteres en el WordArt especificado se rotan 90 grados respecto a la forma delimitadora del WordArt.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


El texto en el WordArt.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setTextEffect(int effect) {#setTextEffect-int-}
```
public void setTextEffect(int effect)
```


Establece el efecto de texto predefinido.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| effect | int | [MsoPresetTextEffect](../../com.aspose.cells/msopresettexteffect). El efecto de texto predefinido. |

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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

