---
title: "RenderingWatermark"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Filigrana per il rendering."
type: docs
url: /it/java/com.aspose.cells/renderingwatermark/
---

**Inheritance:**
java.lang.Object
```
public class RenderingWatermark
```

Filigrana per il rendering.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [RenderingWatermark(String text, RenderingFont renderingFont)](#RenderingWatermark-java.lang.String-com.aspose.cells.RenderingFont-) | Crea un'istanza della filigrana di testo. |
| [RenderingWatermark(byte[] imageData)](#RenderingWatermark-byte---) | Crea un'istanza della filigrana immagine. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFont()](#getFont--) | Ottiene il carattere della filigrana. |
| [getHAlignment()](#getHAlignment--) | Ottiene l'allineamento orizzontale della filigrana rispetto alla pagina. |
| [getImage()](#getImage--) | Ottiene l'immagine della filigrana. |
| [getOffsetX()](#getOffsetX--) | Ottiene il valore di offset per [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--) |
| [getOffsetY()](#getOffsetY--) | Ottiene il valore di offset per [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--) |
| [getOpacity()](#getOpacity--) | Ottiene l'opacità della filigrana nell'intervallo [0, 1]. |
| [getRotation()](#getRotation--) | Ottiene la rotazione della filigrana in gradi. |
| [getScaleToPagePercent()](#getScaleToPagePercent--) | Ottiene la scala relativa alla pagina di destinazione in percentuale. |
| [getText()](#getText--) | Ottiene il testo della filigrana. |
| [getVAlignment()](#getVAlignment--) | Ottiene l'allineamento verticale della filigrana rispetto alla pagina. |
| [hashCode()](#hashCode--) |  |
| [isBackground()](#isBackground--) | Indica se la filigrana è posizionata dietro i contenuti della pagina. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackground(boolean value)](#setBackground-boolean-) | Indica se la filigrana è posizionata dietro i contenuti della pagina. |
| [setHAlignment(int value)](#setHAlignment-int-) | Imposta l'allineamento orizzontale della filigrana rispetto alla pagina. |
| [setOffsetX(float value)](#setOffsetX-float-) | Imposta il valore di offset per [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--) |
| [setOffsetY(float value)](#setOffsetY-float-) | Imposta il valore di offset per [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--) |
| [setOpacity(float value)](#setOpacity-float-) | Imposta l'opacità della filigrana nell'intervallo [0, 1]. |
| [setRotation(float value)](#setRotation-float-) | Imposta la rotazione della filigrana in gradi. |
| [setScaleToPagePercent(int value)](#setScaleToPagePercent-int-) | Imposta la scala relativa alla pagina di destinazione in percentuale. |
| [setVAlignment(int value)](#setVAlignment-int-) | Imposta l'allineamento verticale della filigrana rispetto alla pagina. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### RenderingWatermark(String text, RenderingFont renderingFont) {#RenderingWatermark-java.lang.String-com.aspose.cells.RenderingFont-}
```
public RenderingWatermark(String text, RenderingFont renderingFont)
```


Crea un'istanza della filigrana di testo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| testo | java.lang.String | testo della filigrana |
| renderingFont | [RenderingFont](../../com.aspose.cells/renderingfont) | carattere della filigrana |

### RenderingWatermark(byte[] imageData) {#RenderingWatermark-byte---}
```
public RenderingWatermark(byte[] imageData)
```


Crea un'istanza della filigrana immagine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| imageData | byte[] |  |

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
### getFont() {#getFont--}
```
public RenderingFont getFont()
```


Ottiene il carattere della filigrana.

**Returns:**
[RenderingFont](../../com.aspose.cells/renderingfont)
### getHAlignment() {#getHAlignment--}
```
public int getHAlignment()
```


Ottiene l'allineamento orizzontale della filigrana rispetto alla pagina.

Vedi [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Remarks**

Solo Sinistra, Centro, Destra sono validi. Il valore predefinito è Sinistra.

**Returns:**
int
### getImage() {#getImage--}
```
public byte[] getImage()
```


Ottiene l'immagine della filigrana.

**Returns:**
byte[]
### getOffsetX() {#getOffsetX--}
```
public float getOffsetX()
```


Ottiene il valore di offset per [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--)

**Returns:**
float
### getOffsetY() {#getOffsetY--}
```
public float getOffsetY()
```


Ottiene il valore di offset per [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--)

**Returns:**
float
### getOpacity() {#getOpacity--}
```
public float getOpacity()
```


Ottiene l'opacità della filigrana nell'intervallo [0, 1].

**Returns:**
float
### getRotation() {#getRotation--}
```
public float getRotation()
```


Ottiene la rotazione della filigrana in gradi.

**Returns:**
float
### getScaleToPagePercent() {#getScaleToPagePercent--}
```
public int getScaleToPagePercent()
```


Ottiene la scala relativa alla pagina di destinazione in percentuale.

**Returns:**
int
### getText() {#getText--}
```
public String getText()
```


Ottiene il testo della filigrana.

**Returns:**
java.lang.String
### getVAlignment() {#getVAlignment--}
```
public int getVAlignment()
```


Ottiene l'allineamento verticale della filigrana rispetto alla pagina.

Vedi [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Remarks**

Solo Alto, Centro, Basso sono validi. Il valore predefinito è Alto.

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


Indica se la filigrana è posizionata dietro i contenuti della pagina.

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


Indica se la filigrana è posizionata dietro i contenuti della pagina.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHAlignment(int value) {#setHAlignment-int-}
```
public void setHAlignment(int value)
```


Imposta l'allineamento orizzontale della filigrana rispetto alla pagina.

Vedi [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Remarks**

Solo Sinistra, Centro, Destra sono validi. Il valore predefinito è Sinistra.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setOffsetX(float value) {#setOffsetX-float-}
```
public void setOffsetX(float value)
```


Imposta il valore di offset per [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--)

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | float |  |

### setOffsetY(float value) {#setOffsetY-float-}
```
public void setOffsetY(float value)
```


Imposta il valore di offset per [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--)

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | float |  |

### setOpacity(float value) {#setOpacity-float-}
```
public void setOpacity(float value)
```


Imposta l'opacità della filigrana nell'intervallo [0, 1].

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | float |  |

### setRotation(float value) {#setRotation-float-}
```
public void setRotation(float value)
```


Imposta la rotazione della filigrana in gradi.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | float |  |

### setScaleToPagePercent(int value) {#setScaleToPagePercent-int-}
```
public void setScaleToPagePercent(int value)
```


Imposta la scala relativa alla pagina di destinazione in percentuale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setVAlignment(int value) {#setVAlignment-int-}
```
public void setVAlignment(int value)
```


Imposta l'allineamento verticale della filigrana rispetto alla pagina.

Vedi [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Remarks**

Solo Alto, Centro, Basso sono validi. Il valore predefinito è Alto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

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

