---
title: "RenderingWatermark"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Marca de agua para renderizado."
type: docs
url: /es/java/com.aspose.cells/renderingwatermark/
---

**Inheritance:**
java.lang.Object
```
public class RenderingWatermark
```

Marca de agua para renderizado.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [RenderingWatermark(String text, RenderingFont renderingFont)](#RenderingWatermark-java.lang.String-com.aspose.cells.RenderingFont-) | Crea una instancia de marca de agua de texto. |
| [RenderingWatermark(byte[] imageData)](#RenderingWatermark-byte---) | Crea una instancia de marca de agua de imagen. |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFont()](#getFont--) | Obtiene la fuente de la marca de agua. |
| [getHAlignment()](#getHAlignment--) | Obtiene la alineación horizontal de la marca de agua con la página. |
| [getImage()](#getImage--) | Obtiene la imagen de la marca de agua. |
| [getOffsetX()](#getOffsetX--) | Obtiene el valor de desplazamiento para [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--) |
| [getOffsetY()](#getOffsetY--) | Obtiene el valor de desplazamiento para [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--) |
| [getOpacity()](#getOpacity--) | Obtiene la opacidad de la marca de agua en el rango [0, 1]. |
| [getRotation()](#getRotation--) | Obtiene la rotación de la marca de agua en grados. |
| [getScaleToPagePercent()](#getScaleToPagePercent--) | Obtiene la escala relativa a la página objetivo en porcentaje. |
| [getText()](#getText--) | Obtiene el texto de la marca de agua. |
| [getVAlignment()](#getVAlignment--) | Obtiene la alineación vertical de la marca de agua con la página. |
| [hashCode()](#hashCode--) |  |
| [isBackground()](#isBackground--) | Indica si la marca de agua se coloca detrás del contenido de la página. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackground(boolean value)](#setBackground-boolean-) | Indica si la marca de agua se coloca detrás del contenido de la página. |
| [setHAlignment(int value)](#setHAlignment-int-) | Establece la alineación horizontal de la marca de agua con la página. |
| [setOffsetX(float value)](#setOffsetX-float-) | Establece el valor de desplazamiento para [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--) |
| [setOffsetY(float value)](#setOffsetY-float-) | Establece el valor de desplazamiento para [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--) |
| [setOpacity(float value)](#setOpacity-float-) | Establece la opacidad de la marca de agua en el rango [0, 1]. |
| [setRotation(float value)](#setRotation-float-) | Establece la rotación de la marca de agua en grados. |
| [setScaleToPagePercent(int value)](#setScaleToPagePercent-int-) | Establece la escala relativa a la página objetivo en porcentaje. |
| [setVAlignment(int value)](#setVAlignment-int-) | Establece la alineación vertical de la marca de agua con la página. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### RenderingWatermark(String text, RenderingFont renderingFont) {#RenderingWatermark-java.lang.String-com.aspose.cells.RenderingFont-}
```
public RenderingWatermark(String text, RenderingFont renderingFont)
```


Crea una instancia de marca de agua de texto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| texto | java.lang.String | texto de marca de agua |
| renderingFont | [RenderingFont](../../com.aspose.cells/renderingfont) | fuente de marca de agua |

### RenderingWatermark(byte[] imageData) {#RenderingWatermark-byte---}
```
public RenderingWatermark(byte[] imageData)
```


Crea una instancia de marca de agua de imagen.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| imageData | byte[] |  |

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
### getFont() {#getFont--}
```
public RenderingFont getFont()
```


Obtiene la fuente de la marca de agua.

**Returns:**
[RenderingFont](../../com.aspose.cells/renderingfont)
### getHAlignment() {#getHAlignment--}
```
public int getHAlignment()
```


Obtiene la alineación horizontal de la marca de agua con la página.

Ver [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Remarks**

Solo Left, Center, Right son válidos. El predeterminado es Left.

**Returns:**
int
### getImage() {#getImage--}
```
public byte[] getImage()
```


Obtiene la imagen de la marca de agua.

**Returns:**
byte[]
### getOffsetX() {#getOffsetX--}
```
public float getOffsetX()
```


Obtiene el valor de desplazamiento para [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--)

**Returns:**
float
### getOffsetY() {#getOffsetY--}
```
public float getOffsetY()
```


Obtiene el valor de desplazamiento para [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--)

**Returns:**
float
### getOpacity() {#getOpacity--}
```
public float getOpacity()
```


Obtiene la opacidad de la marca de agua en el rango [0, 1].

**Returns:**
float
### getRotation() {#getRotation--}
```
public float getRotation()
```


Obtiene la rotación de la marca de agua en grados.

**Returns:**
float
### getScaleToPagePercent() {#getScaleToPagePercent--}
```
public int getScaleToPagePercent()
```


Obtiene la escala relativa a la página objetivo en porcentaje.

**Returns:**
int
### getText() {#getText--}
```
public String getText()
```


Obtiene el texto de la marca de agua.

**Returns:**
java.lang.String
### getVAlignment() {#getVAlignment--}
```
public int getVAlignment()
```


Obtiene la alineación vertical de la marca de agua con la página.

Ver [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Remarks**

Solo Top, Center, Bottom son válidos. El predeterminado es Top.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBackground() {#isBackground--}
```
public boolean isBackground()
```


Indica si la marca de agua se coloca detrás del contenido de la página.

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




### setBackground(boolean value) {#setBackground-boolean-}
```
public void setBackground(boolean value)
```


Indica si la marca de agua se coloca detrás del contenido de la página.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setHAlignment(int value) {#setHAlignment-int-}
```
public void setHAlignment(int value)
```


Establece la alineación horizontal de la marca de agua con la página.

Ver [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Remarks**

Solo Left, Center, Right son válidos. El predeterminado es Left.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setOffsetX(float value) {#setOffsetX-float-}
```
public void setOffsetX(float value)
```


Establece el valor de desplazamiento para [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--)

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | float |  |

### setOffsetY(float value) {#setOffsetY-float-}
```
public void setOffsetY(float value)
```


Establece el valor de desplazamiento para [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--)

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | float |  |

### setOpacity(float value) {#setOpacity-float-}
```
public void setOpacity(float value)
```


Establece la opacidad de la marca de agua en el rango [0, 1].

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | float |  |

### setRotation(float value) {#setRotation-float-}
```
public void setRotation(float value)
```


Establece la rotación de la marca de agua en grados.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | float |  |

### setScaleToPagePercent(int value) {#setScaleToPagePercent-int-}
```
public void setScaleToPagePercent(int value)
```


Establece la escala relativa a la página objetivo en porcentaje.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setVAlignment(int value) {#setVAlignment-int-}
```
public void setVAlignment(int value)
```


Establece la alineación vertical de la marca de agua con la página.

Ver [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Remarks**

Solo Top, Center, Bottom son válidos. El predeterminado es Top.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

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

