---
title: "TextEffectFormat"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Contiene proprietà e metodi che si applicano agli oggetti WordArt."
type: docs
url: /it/java/com.aspose.cells/texteffectformat/
---

**Inheritance:**
java.lang.Object
```
public class TextEffectFormat
```

Contiene proprietà e metodi che si applicano agli oggetti WordArt.

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
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFontBold()](#getFontBold--) | Indica se il carattere è in grassetto. |
| [getFontItalic()](#getFontItalic--) | Indica se il carattere è in corsivo. |
| [getFontName()](#getFontName--) | Il nome del carattere utilizzato nel WordArt. |
| [getFontSize()](#getFontSize--) | La dimensione (in punti) del carattere utilizzato nel WordArt. |
| [getPresetShape()](#getPresetShape--) | Ottiene il tipo di forma predefinita. |
| [getRotatedChars()](#getRotatedChars--) | Se true, i caratteri nel WordArt specificato sono ruotati di 90 gradi rispetto alla forma di delimitazione del WordArt. |
| [getText()](#getText--) | Il testo nel WordArt. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFontBold(boolean value)](#setFontBold-boolean-) | Indica se il carattere è in grassetto. |
| [setFontItalic(boolean value)](#setFontItalic-boolean-) | Indica se il carattere è in corsivo. |
| [setFontName(String value)](#setFontName-java.lang.String-) | Il nome del carattere utilizzato nel WordArt. |
| [setFontSize(int value)](#setFontSize-int-) | La dimensione (in punti) del carattere utilizzato nel WordArt. |
| [setPresetShape(int value)](#setPresetShape-int-) | Imposta il tipo di forma predefinita. |
| [setRotatedChars(boolean value)](#setRotatedChars-boolean-) | Se true, i caratteri nel WordArt specificato sono ruotati di 90 gradi rispetto alla forma di delimitazione del WordArt. |
| [setText(String value)](#setText-java.lang.String-) | Il testo nel WordArt. |
| [setTextEffect(int effect)](#setTextEffect-int-) | Imposta l'effetto testo predefinito. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
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


Indica se il carattere è in grassetto.

**Returns:**
boolean
### getFontItalic() {#getFontItalic--}
```
public boolean getFontItalic()
```


Indica se il carattere è in corsivo.

**Returns:**
boolean
### getFontName() {#getFontName--}
```
public String getFontName()
```


Il nome del carattere utilizzato nel WordArt.

**Returns:**
java.lang.String
### getFontSize() {#getFontSize--}
```
public int getFontSize()
```


La dimensione (in punti) del carattere utilizzato nel WordArt.

**Returns:**
int
### getPresetShape() {#getPresetShape--}
```
public int getPresetShape()
```


Ottiene il tipo di forma predefinita.

Vedi [MsoPresetTextEffectShape](../../com.aspose.cells/msopresettexteffectshape).

**Returns:**
int
### getRotatedChars() {#getRotatedChars--}
```
public boolean getRotatedChars()
```


Se true, i caratteri nel WordArt specificato sono ruotati di 90 gradi rispetto alla forma di delimitazione del WordArt.

**Returns:**
boolean
### getText() {#getText--}
```
public String getText()
```


Il testo nel WordArt.

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


Indica se il carattere è in grassetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setFontItalic(boolean value) {#setFontItalic-boolean-}
```
public void setFontItalic(boolean value)
```


Indica se il carattere è in corsivo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setFontName(String value) {#setFontName-java.lang.String-}
```
public void setFontName(String value)
```


Il nome del carattere utilizzato nel WordArt.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setFontSize(int value) {#setFontSize-int-}
```
public void setFontSize(int value)
```


La dimensione (in punti) del carattere utilizzato nel WordArt.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setPresetShape(int value) {#setPresetShape-int-}
```
public void setPresetShape(int value)
```


Imposta il tipo di forma predefinita.

Vedi [MsoPresetTextEffectShape](../../com.aspose.cells/msopresettexteffectshape).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setRotatedChars(boolean value) {#setRotatedChars-boolean-}
```
public void setRotatedChars(boolean value)
```


Se true, i caratteri nel WordArt specificato sono ruotati di 90 gradi rispetto alla forma di delimitazione del WordArt.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Il testo nel WordArt.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setTextEffect(int effect) {#setTextEffect-int-}
```
public void setTextEffect(int effect)
```


Imposta l'effetto testo predefinito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| effect | int | [MsoPresetTextEffect](../../com.aspose.cells/msopresettexteffect). L'effetto testo predefinito. |

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

