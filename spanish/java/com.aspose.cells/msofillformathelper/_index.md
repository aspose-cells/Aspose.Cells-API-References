---
title: "MsoFillFormatHelper"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa el formato de relleno para una forma."
type: docs
url: /es/java/com.aspose.cells/msofillformathelper/
---

**Inheritance:**
java.lang.Object
```
public class MsoFillFormatHelper
```

Representa el formato de relleno para una forma.
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackColor()](#getBackColor--) | Obtiene el color de fondo del archivo. |
| [getClass()](#getClass--) |  |
| [getForeColor()](#getForeColor--) | Obtiene el color de primer plano del relleno. |
| [getForeColorTransparency()](#getForeColorTransparency--) | Devuelve o establece el grado del color de primer plano del relleno especificado como un valor de 0.0 (opaco) a 1.0 (transparente). |
| [getImageData()](#getImageData--) | Obtiene los datos de relleno de textura y imagen. |
| [getTexture()](#getTexture--) | Obtiene el tipo de relleno de textura. |
| [hashCode()](#hashCode--) |  |
| [isVisible()](#isVisible--) | Indica si hay relleno. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackColor(Color value)](#setBackColor-com.aspose.cells.Color-) | Establece el color de fondo del archivo. |
| [setForeColor(Color value)](#setForeColor-com.aspose.cells.Color-) | Establece el color de primer plano del relleno. |
| [setForeColorTransparency(double value)](#setForeColorTransparency-double-) | Devuelve o establece el grado del color de primer plano del relleno especificado como un valor de 0.0 (opaco) a 1.0 (transparente). |
| [setImageData(byte[] value)](#setImageData-byte---) | Establece los datos de relleno de textura y imagen. |
| [setOneColorGradient(Color color, double degree, int style, int variant)](#setOneColorGradient-com.aspose.cells.Color-double-int-int-) | Establece el relleno especificado a un degradado de un solo color. |
| [setVisible(boolean value)](#setVisible-boolean-) | Indica si hay relleno. |
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
### getBackColor() {#getBackColor--}
```
public Color getBackColor()
```


Obtiene el color de fondo del archivo.

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


Obtiene el color de primer plano del relleno.

**Returns:**
[Color](../../com.aspose.cells/color)
### getForeColorTransparency() {#getForeColorTransparency--}
```
public double getForeColorTransparency()
```


Devuelve o establece el grado del color de primer plano del relleno especificado como un valor de 0.0 (opaco) a 1.0 (transparente).

**Returns:**
double
### getImageData() {#getImageData--}
```
public byte[] getImageData()
```


Obtiene los datos de relleno de textura y imagen.

**Returns:**
byte[]
### getTexture() {#getTexture--}
```
public int getTexture()
```


Obtiene el tipo de relleno de textura.

Ver [TextureType](../../com.aspose.cells/texturetype).

**Returns:**
int
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


Indica si hay relleno.

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


Establece el color de fondo del archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setForeColor(Color value) {#setForeColor-com.aspose.cells.Color-}
```
public void setForeColor(Color value)
```


Establece el color de primer plano del relleno.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setForeColorTransparency(double value) {#setForeColorTransparency-double-}
```
public void setForeColorTransparency(double value)
```


Devuelve o establece el grado del color de primer plano del relleno especificado como un valor de 0.0 (opaco) a 1.0 (transparente).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setImageData(byte[] value) {#setImageData-byte---}
```
public void setImageData(byte[] value)
```


Establece los datos de relleno de textura y imagen.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | byte[] |  |

### setOneColorGradient(Color color, double degree, int style, int variant) {#setOneColorGradient-com.aspose.cells.Color-double-int-int-}
```
public void setOneColorGradient(Color color, double degree, int style, int variant)
```


Establece el relleno especificado a un degradado de un solo color.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Un color de degradado. |
| grado | double | El grado del degradado. Puede ser un valor de 0.0 (oscuro) a 1.0 (claro). |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Estilo de sombreado del degradado. |
| variante | int | La variante de degradado. Puede ser un valor del 1 al 4, correspondiente a una de las cuatro variantes en la pestaña Degradado del cuadro de diálogo Efectos de relleno. Si el estilo es GradientStyle.FromCenter, el argumento Variant solo puede ser 1 o 2. |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Indica si hay relleno.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

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

