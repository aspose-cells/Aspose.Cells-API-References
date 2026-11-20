---
title: "ImageActiveXControl"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta il controllo immagine."
type: docs
url: /it/java/com.aspose.cells/imageactivexcontrol/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ActiveXControlBase](../../com.aspose.cells/activexcontrolbase), [com.aspose.cells.ActiveXControl](../../com.aspose.cells/activexcontrol)
```
public class ImageActiveXControl extends ActiveXControl
```

Rappresenta il controllo immagine.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackOleColor()](#getBackOleColor--) | Ottiene il colore ole dello sfondo. |
| [getBorderOleColor()](#getBorderOleColor--) | Ottiene il colore ole dello sfondo. |
| [getBorderStyle()](#getBorderStyle--) | Ottiene il tipo di bordo utilizzato dal controllo. |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | Restituisce i dati binari del controllo. |
| [getFont()](#getFont--) | Rappresenta il carattere del controllo. |
| [getForeOleColor()](#getForeOleColor--) | Restituisce il colore OLE del primo piano. |
| [getHeight()](#getHeight--) | Restituisce l'altezza del controllo in unità di punti. |
| [getIMEMode()](#getIMEMode--) | Restituisce la modalità di esecuzione predefinita dell'Editor di metodo di input per il controllo quando riceve il fuoco. |
| [getLinkedCell()](#getLinkedCell--) | Restituisce la cella collegata. |
| [getListFillRange()](#getListFillRange--) | Restituisce l'intervallo di riempimento dell'elenco. |
| [getMouseIcon()](#getMouseIcon--) | Restituisce un'icona personalizzata da visualizzare come puntatore del mouse per il controllo. |
| [getMousePointer()](#getMousePointer--) | Restituisce il tipo di icona visualizzata come puntatore del mouse per il controllo. |
| [getPicture()](#getPicture--) | Ottiene i dati dell'immagine. |
| [getPictureAlignment()](#getPictureAlignment--) | Ottiene l'allineamento dell'immagine all'interno del Form o dell'Image. |
| [getPictureSizeMode()](#getPictureSizeMode--) | Ottiene come visualizzare l'immagine. |
| [getShadow()](#getShadow--) | Indica se mostrare un'ombra. |
| [getSpecialEffect()](#getSpecialEffect--) | Restituisce l'effetto speciale del controllo. |
| [getTextAlign()](#getTextAlign--) | Rappresenta come allineare il testo utilizzato dal controllo. |
| [getType()](#getType--) | Restituisce il tipo del controllo ActiveX. |
| [getWidth()](#getWidth--) | Ottiene la larghezza del controllo in unità di punti. |
| [getWorkbook()](#getWorkbook--) | Ottiene l'oggetto [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--). |
| [hashCode()](#hashCode--) |  |
| [isAutoSize()](#isAutoSize--) | Indica se il controllo ridimensionerà automaticamente per visualizzare tutto il contenuto. |
| [isEnabled()](#isEnabled--) | Indica se il controllo può ricevere il focus e rispondere agli eventi generati dall'utente. |
| [isLocked()](#isLocked--) | Indica se i dati nel controllo sono bloccati per la modifica. |
| [isTiled()](#isTiled--) | Indica se l'immagine è ripetuta sullo sfondo. |
| [isTransparent()](#isTransparent--) | Indica se il controllo è trasparente. |
| [isVisible()](#isVisible--) | Indica se questo controllo è visibile. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Indica se il controllo ridimensionerà automaticamente per visualizzare tutto il contenuto. |
| [setBackOleColor(int value)](#setBackOleColor-int-) | Imposta il colore OLE dello sfondo. |
| [setBorderOleColor(int value)](#setBorderOleColor-int-) | Imposta il colore OLE dello sfondo. |
| [setBorderStyle(int value)](#setBorderStyle-int-) | Imposta il tipo di bordo utilizzato dal controllo. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | Indica se il controllo può ricevere il focus e rispondere agli eventi generati dall'utente. |
| [setForeOleColor(int value)](#setForeOleColor-int-) | Imposta il colore OLE del primo piano. |
| [setHeight(double value)](#setHeight-double-) | Imposta l'altezza del controllo in unità di punti. |
| [setIMEMode(int value)](#setIMEMode-int-) | Imposta la modalità di esecuzione predefinita dell'Input Method Editor per il controllo quando riceve il focus. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Imposta la cella collegata. |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | Imposta l'intervallo di riempimento dell'elenco. |
| [setLocked(boolean value)](#setLocked-boolean-) | Indica se i dati nel controllo sono bloccati per la modifica. |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | Imposta un'icona personalizzata da visualizzare come puntatore del mouse per il controllo. |
| [setMousePointer(int value)](#setMousePointer-int-) | Imposta il tipo di icona visualizzata come puntatore del mouse per il controllo. |
| [setPicture(byte[] value)](#setPicture-byte---) | Imposta i dati dell'immagine. |
| [setPictureAlignment(int value)](#setPictureAlignment-int-) | Imposta l'allineamento dell'immagine all'interno del Form o dell'Image. |
| [setPictureSizeMode(int value)](#setPictureSizeMode-int-) | Imposta come visualizzare l'immagine. |
| [setShadow(boolean value)](#setShadow-boolean-) | Indica se mostrare un'ombra. |
| [setSpecialEffect(int value)](#setSpecialEffect-int-) | Imposta l'effetto speciale del controllo. |
| [setTextAlign(int value)](#setTextAlign-int-) | Rappresenta come allineare il testo utilizzato dal controllo. |
| [setTiled(boolean value)](#setTiled-boolean-) | Indica se l'immagine è ripetuta sullo sfondo. |
| [setTransparent(boolean value)](#setTransparent-boolean-) | Indica se il controllo è trasparente. |
| [setVisible(boolean value)](#setVisible-boolean-) | Indica se questo controllo è visibile. |
| [setWidth(double value)](#setWidth-double-) | Imposta la larghezza del controllo in unità di punti. |
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
### getBackOleColor() {#getBackOleColor--}
```
public int getBackOleColor()
```


Ottiene il colore ole dello sfondo.

**Returns:**
int
### getBorderOleColor() {#getBorderOleColor--}
```
public int getBorderOleColor()
```


Ottiene il colore ole dello sfondo.

**Returns:**
int
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```


Ottiene il tipo di bordo utilizzato dal controllo.

Vedi [ControlBorderType](../../com.aspose.cells/controlbordertype).

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getData() {#getData--}
```
public byte[] getData()
```


Restituisce i dati binari del controllo.

**Returns:**
byte[]
### getFont() {#getFont--}
```
public Font getFont()
```


Rappresenta il carattere del controllo.

**Returns:**
[Font](../../com.aspose.cells/font)
### getForeOleColor() {#getForeOleColor--}
```
public int getForeOleColor()
```


Restituisce il colore OLE del primo piano.

**Remarks**

Non si applica al controllo Image.

**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```


Restituisce l'altezza del controllo in unità di punti.

**Returns:**
double
### getIMEMode() {#getIMEMode--}
```
public int getIMEMode()
```


Restituisce la modalità di esecuzione predefinita dell'Editor di metodo di input per il controllo quando riceve il fuoco.

Vedi [InputMethodEditorMode](../../com.aspose.cells/inputmethodeditormode).

**Returns:**
int
### getLinkedCell() {#getLinkedCell--}
```
public String getLinkedCell()
```


Restituisce la cella collegata.

**Returns:**
java.lang.String
### getListFillRange() {#getListFillRange--}
```
public String getListFillRange()
```


Restituisce l'intervallo di riempimento dell'elenco.

**Returns:**
java.lang.String
### getMouseIcon() {#getMouseIcon--}
```
public byte[] getMouseIcon()
```


Restituisce un'icona personalizzata da visualizzare come puntatore del mouse per il controllo.

**Returns:**
byte[]
### getMousePointer() {#getMousePointer--}
```
public int getMousePointer()
```


Restituisce il tipo di icona visualizzata come puntatore del mouse per il controllo.

Vedi [ControlMousePointerType](../../com.aspose.cells/controlmousepointertype).

**Returns:**
int
### getPicture() {#getPicture--}
```
public byte[] getPicture()
```


Ottiene i dati dell'immagine.

**Returns:**
byte[]
### getPictureAlignment() {#getPictureAlignment--}
```
public int getPictureAlignment()
```


Ottiene l'allineamento dell'immagine all'interno del Form o dell'Image.

Vedi [ControlPictureAlignmentType](../../com.aspose.cells/controlpicturealignmenttype).

**Returns:**
int
### getPictureSizeMode() {#getPictureSizeMode--}
```
public int getPictureSizeMode()
```


Ottiene come visualizzare l'immagine.

Vedi [ControlPictureSizeMode](../../com.aspose.cells/controlpicturesizemode).

**Returns:**
int
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Indica se mostrare un'ombra.

**Returns:**
boolean
### getSpecialEffect() {#getSpecialEffect--}
```
public int getSpecialEffect()
```


Restituisce l'effetto speciale del controllo.

Vedi [ControlSpecialEffectType](../../com.aspose.cells/controlspecialeffecttype).

**Returns:**
int
### getTextAlign() {#getTextAlign--}
```
public int getTextAlign()
```


Rappresenta come allineare il testo utilizzato dal controllo.

Vedi [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Restituisce il tipo del controllo ActiveX.

Vedi [ControlType](../../com.aspose.cells/controltype).

**Returns:**
int
### getWidth() {#getWidth--}
```
public double getWidth()
```


Ottiene la larghezza del controllo in unità di punti.

**Returns:**
double
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


Ottiene l'oggetto [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--).

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoSize() {#isAutoSize--}
```
public boolean isAutoSize()
```


Indica se il controllo ridimensionerà automaticamente per visualizzare tutto il contenuto.

**Returns:**
boolean
### isEnabled() {#isEnabled--}
```
public boolean isEnabled()
```


Indica se il controllo può ricevere il focus e rispondere agli eventi generati dall'utente.

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


Indica se i dati nel controllo sono bloccati per la modifica.

**Returns:**
boolean
### isTiled() {#isTiled--}
```
public boolean isTiled()
```


Indica se l'immagine è ripetuta sullo sfondo.

**Returns:**
boolean
### isTransparent() {#isTransparent--}
```
public boolean isTransparent()
```


Indica se il controllo è trasparente.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Indica se questo controllo è visibile.

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




### setAutoSize(boolean value) {#setAutoSize-boolean-}
```
public void setAutoSize(boolean value)
```


Indica se il controllo ridimensionerà automaticamente per visualizzare tutto il contenuto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setBackOleColor(int value) {#setBackOleColor-int-}
```
public void setBackOleColor(int value)
```


Imposta il colore OLE dello sfondo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setBorderOleColor(int value) {#setBorderOleColor-int-}
```
public void setBorderOleColor(int value)
```


Imposta il colore OLE dello sfondo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setBorderStyle(int value) {#setBorderStyle-int-}
```
public void setBorderStyle(int value)
```


Imposta il tipo di bordo utilizzato dal controllo.

Vedi [ControlBorderType](../../com.aspose.cells/controlbordertype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public void setEnabled(boolean value)
```


Indica se il controllo può ricevere il focus e rispondere agli eventi generati dall'utente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setForeOleColor(int value) {#setForeOleColor-int-}
```
public void setForeOleColor(int value)
```


Imposta il colore OLE del primo piano.

**Remarks**

Non si applica al controllo Image.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


Imposta l'altezza del controllo in unità di punti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setIMEMode(int value) {#setIMEMode-int-}
```
public void setIMEMode(int value)
```


Imposta la modalità di esecuzione predefinita dell'Input Method Editor per il controllo quando riceve il focus.

Vedi [InputMethodEditorMode](../../com.aspose.cells/inputmethodeditormode).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setLinkedCell(String value) {#setLinkedCell-java.lang.String-}
```
public void setLinkedCell(String value)
```


Imposta la cella collegata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setListFillRange(String value) {#setListFillRange-java.lang.String-}
```
public void setListFillRange(String value)
```


Imposta l'intervallo di riempimento dell'elenco.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Indica se i dati nel controllo sono bloccati per la modifica.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setMouseIcon(byte[] value) {#setMouseIcon-byte---}
```
public void setMouseIcon(byte[] value)
```


Imposta un'icona personalizzata da visualizzare come puntatore del mouse per il controllo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | byte[] |  |

### setMousePointer(int value) {#setMousePointer-int-}
```
public void setMousePointer(int value)
```


Imposta il tipo di icona visualizzata come puntatore del mouse per il controllo.

Vedi [ControlMousePointerType](../../com.aspose.cells/controlmousepointertype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setPicture(byte[] value) {#setPicture-byte---}
```
public void setPicture(byte[] value)
```


Imposta i dati dell'immagine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | byte[] |  |

### setPictureAlignment(int value) {#setPictureAlignment-int-}
```
public void setPictureAlignment(int value)
```


Imposta l'allineamento dell'immagine all'interno del Form o dell'Image.

Vedi [ControlPictureAlignmentType](../../com.aspose.cells/controlpicturealignmenttype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setPictureSizeMode(int value) {#setPictureSizeMode-int-}
```
public void setPictureSizeMode(int value)
```


Imposta come visualizzare l'immagine.

Vedi [ControlPictureSizeMode](../../com.aspose.cells/controlpicturesizemode).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


Indica se mostrare un'ombra.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSpecialEffect(int value) {#setSpecialEffect-int-}
```
public void setSpecialEffect(int value)
```


Imposta l'effetto speciale del controllo.

Vedi [ControlSpecialEffectType](../../com.aspose.cells/controlspecialeffecttype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setTextAlign(int value) {#setTextAlign-int-}
```
public void setTextAlign(int value)
```


Rappresenta come allineare il testo utilizzato dal controllo.

Vedi [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setTiled(boolean value) {#setTiled-boolean-}
```
public void setTiled(boolean value)
```


Indica se l'immagine è ripetuta sullo sfondo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setTransparent(boolean value) {#setTransparent-boolean-}
```
public void setTransparent(boolean value)
```


Indica se il controllo è trasparente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Indica se questo controllo è visibile.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```


Imposta la larghezza del controllo in unità di punti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

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

