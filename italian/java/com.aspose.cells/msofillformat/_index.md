---
title: "MsoFillFormat"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta la formattazione di riempimento per una forma."
type: docs
url: /it/java/com.aspose.cells/msofillformat/
---

**Inheritance:**
java.lang.Object
```
public class MsoFillFormat
```

Rappresenta la formattazione di riempimento per una forma.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackColor()](#getBackColor--) | Ottiene il colore di sfondo del file. |
| [getClass()](#getClass--) |  |
| [getForeColor()](#getForeColor--) | Ottiene il colore di primo piano del riempimento. |
| [getImageData()](#getImageData--) | Ottiene i dati di riempimento della Texture e dell'Immagine. |
| [getTexture()](#getTexture--) | Ottiene il tipo di riempimento della texture. |
| [getTransparency()](#getTransparency--) | Restituisce o imposta il grado di trasparenza del riempimento specificato come valore da 0,0 (opaco) a 1,0 (trasparente). |
| [hashCode()](#hashCode--) |  |
| [isVisible()](#isVisible--) | Indica se è presente un riempimento. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackColor(Color value)](#setBackColor-com.aspose.cells.Color-) | Imposta il colore di sfondo del file. |
| [setForeColor(Color value)](#setForeColor-com.aspose.cells.Color-) | Imposta il colore di primo piano del riempimento. |
| [setImageData(byte[] value)](#setImageData-byte---) | Imposta i dati di riempimento della Texture e dell'Immagine. |
| [setOneColorGradient(Color color, double degree, int style, int variant)](#setOneColorGradient-com.aspose.cells.Color-double-int-int-) | Imposta il riempimento specificato a un gradiente a un colore. |
| [setTransparency(double value)](#setTransparency-double-) | Restituisce o imposta il grado di trasparenza del riempimento specificato come valore da 0,0 (opaco) a 1,0 (trasparente). |
| [setVisible(boolean value)](#setVisible-boolean-) | Indica se è presente un riempimento. |
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
### getBackColor() {#getBackColor--}
```
public Color getBackColor()
```


Ottiene il colore di sfondo del file.

**Returns:**
[Color](../../com.aspose.cells/color)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getForeColor() {#getForeColor--}
```
public Color getForeColor()
```


Ottiene il colore di primo piano del riempimento.

**Returns:**
[Color](../../com.aspose.cells/color)
### getImageData() {#getImageData--}
```
public byte[] getImageData()
```


Ottiene i dati di riempimento della Texture e dell'Immagine.

**Returns:**
byte[]
### getTexture() {#getTexture--}
```
public int getTexture()
```


Ottiene il tipo di riempimento della texture.

Vedi [TextureType](../../com.aspose.cells/texturetype).

**Returns:**
int
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


Restituisce o imposta il grado di trasparenza del riempimento specificato come valore da 0,0 (opaco) a 1,0 (trasparente).

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Indica se è presente un riempimento.

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




### setBackColor(Color value) {#setBackColor-com.aspose.cells.Color-}
```
public void setBackColor(Color value)
```


Imposta il colore di sfondo del file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setForeColor(Color value) {#setForeColor-com.aspose.cells.Color-}
```
public void setForeColor(Color value)
```


Imposta il colore di primo piano del riempimento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setImageData(byte[] value) {#setImageData-byte---}
```
public void setImageData(byte[] value)
```


Imposta i dati di riempimento della Texture e dell'Immagine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | byte[] |  |

### setOneColorGradient(Color color, double degree, int style, int variant) {#setOneColorGradient-com.aspose.cells.Color-double-int-int-}
```
public void setOneColorGradient(Color color, double degree, int style, int variant)
```


Imposta il riempimento specificato a un gradiente a un colore.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Un colore di gradiente. |
| grado | double | Il grado del gradiente. Può essere un valore da 0.0 (scuro) a 1.0 (chiaro). |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Stile di sfumatura del gradiente. |
| variante | int | La variante del gradiente. Può essere un valore da 1 a 4, corrispondente a una delle quattro varianti nella scheda Gradiente nella finestra di dialogo Effetti di riempimento. Se lo stile è GradientStyle.FromCenter, l'argomento Variant può essere solo 1 o 2. |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


Restituisce o imposta il grado di trasparenza del riempimento specificato come valore da 0,0 (opaco) a 1,0 (trasparente).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Indica se è presente un riempimento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

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

