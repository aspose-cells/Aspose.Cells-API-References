---
title: "ActiveXControlBase"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta il controllo ActiveX."
type: docs
url: /it/java/com.aspose.cells/activexcontrolbase/
---

**Inheritance:**
java.lang.Object
```
public abstract class ActiveXControlBase
```

Rappresenta il controllo ActiveX.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackOleColor()](#getBackOleColor--) | Ottiene il colore ole dello sfondo. |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | Restituisce i dati binari del controllo. |
| [getForeOleColor()](#getForeOleColor--) | Restituisce il colore OLE del primo piano. |
| [getHeight()](#getHeight--) | Restituisce l'altezza del controllo in unità di punti. |
| [getLinkedCell()](#getLinkedCell--) | Restituisce la cella collegata. |
| [getListFillRange()](#getListFillRange--) | Restituisce l'intervallo di riempimento dell'elenco. |
| [getMouseIcon()](#getMouseIcon--) | Restituisce un'icona personalizzata da visualizzare come puntatore del mouse per il controllo. |
| [getMousePointer()](#getMousePointer--) | Restituisce il tipo di icona visualizzata come puntatore del mouse per il controllo. |
| [getShadow()](#getShadow--) | Indica se mostrare un'ombra. |
| [getType()](#getType--) | Restituisce il tipo del controllo ActiveX. |
| [getWidth()](#getWidth--) | Ottiene la larghezza del controllo in unità di punti. |
| [getWorkbook()](#getWorkbook--) | Ottiene l'oggetto [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--). |
| [hashCode()](#hashCode--) |  |
| [isVisible()](#isVisible--) | Indica se questo controllo è visibile. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackOleColor(int value)](#setBackOleColor-int-) | Imposta il colore OLE dello sfondo. |
| [setForeOleColor(int value)](#setForeOleColor-int-) | Imposta il colore OLE del primo piano. |
| [setHeight(double value)](#setHeight-double-) | Imposta l'altezza del controllo in unità di punti. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Imposta la cella collegata. |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | Imposta l'intervallo di riempimento dell'elenco. |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | Imposta un'icona personalizzata da visualizzare come puntatore del mouse per il controllo. |
| [setMousePointer(int value)](#setMousePointer-int-) | Imposta il tipo di icona visualizzata come puntatore del mouse per il controllo. |
| [setShadow(boolean value)](#setShadow-boolean-) | Indica se mostrare un'ombra. |
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
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Indica se mostrare un'ombra.

**Returns:**
boolean
### getType() {#getType--}
```
public abstract int getType()
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




### setBackOleColor(int value) {#setBackOleColor-int-}
```
public void setBackOleColor(int value)
```


Imposta il colore OLE dello sfondo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

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

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


Indica se mostrare un'ombra.

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

