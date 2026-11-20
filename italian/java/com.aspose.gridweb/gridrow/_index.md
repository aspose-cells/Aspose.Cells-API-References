---
title: "GridRow"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Incapsula l'oggetto che rappresenta un'unica immagine in un foglio di calcolo."
type: docs
url: /it/java/com.aspose.gridweb/gridrow/
---

**Inheritance:**
java.lang.Object
```
public class GridRow
```

Incapsula l'oggetto che rappresenta un'unica immagine in un foglio di calcolo.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int column)](#get-int-) | Ottiene la cella. |
| [getCellByIndex(int index)](#getCellByIndex-int-) | Ottieni la cella tramite indice specifico nella lista. |
| [getClass()](#getClass--) |  |
| [getFirstCell()](#getFirstCell--) | Ottiene la prima cella nella riga. |
| [getHeight()](#getHeight--) | Ottiene l'altezza della riga in unità di punti. |
| [getHidden()](#getHidden--) | Indica se la riga è nascosta. |
| [getIndex()](#getIndex--) | Ottiene l'indice di questa riga. |
| [getLastCell()](#getLastCell--) | Ottiene l'ultima cella nella riga. |
| [getLastDataCell()](#getLastDataCell--) | Ottiene l'ultima cella nella riga. |
| [getOutlineLevel()](#getOutlineLevel--) | Ottiene il livello di contorno. |
| [hashCode()](#hashCode--) |  |
| [isBlank()](#isBlank--) | Indica se la riga contiene dati |
| [iterator()](#iterator--) | Ottiene l'enumeratore delle celle |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setHeight(double value)](#setHeight-double-) | Imposta l'altezza della riga in unità di punti. |
| [setHidden(boolean value)](#setHidden-boolean-) | Indica se la riga è nascosta. |
| [setOutlineLevel(byte value)](#setOutlineLevel-byte-) | Imposta il livello di contorno. |
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
### get(int column) {#get-int-}
```
public GridCell get(int column)
```


Ottiene la cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | int | L'indice della colonna |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - 
### getCellByIndex(int index) {#getCellByIndex-int-}
```
public GridCell getCellByIndex(int index)
```


Ottieni la cella tramite indice specifico nella lista.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo Row.GetEnumerator() per iterare tutte le celle in questa riga. Questa proprietà sarà rimossa tra 12 mesi a partire da febbraio 2015. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | La posizione. |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - The Cell object.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFirstCell() {#getFirstCell--}
```
public GridCell getFirstCell()
```


Ottiene la prima cella nella riga.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getHeight() {#getHeight--}
```
public double getHeight()
```


Ottiene l'altezza della riga in unità di punti.

**Returns:**
double
### getHidden() {#getHidden--}
```
public boolean getHidden()
```


Indica se la riga è nascosta.

**Returns:**
boolean
### getIndex() {#getIndex--}
```
public int getIndex()
```


Ottiene l'indice di questa riga.

**Returns:**
int
### getLastCell() {#getLastCell--}
```
public GridCell getLastCell()
```


Ottiene l'ultima cella nella riga.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getLastDataCell() {#getLastDataCell--}
```
public GridCell getLastDataCell()
```


Ottiene l'ultima cella nella riga.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getOutlineLevel() {#getOutlineLevel--}
```
public byte getOutlineLevel()
```


Ottiene il livello di contorno.

**Returns:**
byte
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBlank() {#isBlank--}
```
public boolean isBlank()
```


Indica se la riga contiene dati

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


Ottiene l'enumeratore delle celle

**Returns:**
java.util.Iterator - L'enumeratore delle celle
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


Imposta l'altezza della riga in unità di punti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Indica se la riga è nascosta.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setOutlineLevel(byte value) {#setOutlineLevel-byte-}
```
public void setOutlineLevel(byte value)
```


Imposta il livello di contorno.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | byte |  |

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

