---
title: "SplitPartInfo"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta le informazioni di un input/output per più input/output, come la pagina corrente da renderizzare durante la conversione del foglio di calcolo in immagine."
type: docs
url: /it/java/com.aspose.cells/splitpartinfo/
---

**Inheritance:**
java.lang.Object
```
public class SplitPartInfo
```

Rappresenta le informazioni di un input/output per più input/output, come la pagina corrente da renderizzare durante la conversione del foglio di calcolo in immagine.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPartIndex()](#getPartIndex--) | Indice della parte corrente nella sequenza (base 0). |
| [getSheetIndex()](#getSheetIndex--) | Indice del foglio in cui si trova la parte corrente. -1 indica che c'è un solo foglio. |
| [getSheetName()](#getSheetName--) | Nome del foglio in cui si trova la parte corrente. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
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
### getPartIndex() {#getPartIndex--}
```
public int getPartIndex()
```


Indice della parte corrente nella sequenza (base 0). -1 indica che non ci sono più parti, quindi il risultato è singolo.

**Remarks**

Se più fogli devono essere elaborati e ogni foglio è elaborato (split) separatamente, l'indice della parte inizia sempre da 0 per ogni foglio. Per esempio, quando si converte una cartella di lavoro in immagini, rappresenta l'indice della pagina di output del foglio attualmente elaborato. E -1 indica che c'è solo una pagina per il foglio corrente.

**Returns:**
int
### getSheetIndex() {#getSheetIndex--}
```
public int getSheetIndex()
```


Indice del foglio in cui si trova la parte corrente. -1 indica che c'è un solo foglio.

**Returns:**
int
### getSheetName() {#getSheetName--}
```
public String getSheetName()
```


Nome del foglio in cui si trova la parte corrente.

**Remarks**

Può essere nullo in alcune situazioni, ad esempio durante il rendering dell'intera cartella di lavoro in immagine tiff.

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

