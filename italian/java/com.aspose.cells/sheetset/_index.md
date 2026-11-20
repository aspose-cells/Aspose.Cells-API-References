---
title: "SheetSet"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Descrive un insieme di fogli."
type: docs
url: /it/java/com.aspose.cells/sheetset/
---

**Inheritance:**
java.lang.Object
```
public class SheetSet
```

Descrive un insieme di fogli.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [SheetSet(int[] sheetIndexes)](#SheetSet-int---) | Crea un set di fogli basato su indici di foglio esatti. |
| [SheetSet(String[] sheetNames)](#SheetSet-java.lang.String---) | Crea un set di fogli basato su nomi di foglio esatti. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActive()](#getActive--) | Ottiene un set con il foglio attivo della cartella di lavoro. |
| [getAll()](#getAll--) | Ottiene un set con tutti i fogli della cartella di lavoro nel loro ordine originale. |
| [getClass()](#getClass--) |  |
| [getVisible()](#getVisible--) | Ottiene un set con i fogli visibili della cartella di lavoro nel loro ordine originale. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SheetSet(int[] sheetIndexes) {#SheetSet-int---}
```
public SheetSet(int[] sheetIndexes)
```


Crea un set di fogli basato su indici di foglio esatti.

**Remarks**

Se viene incontrato un foglio che non è nella cartella di lavoro, verrà generata un'eccezione durante il rendering.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetIndexes | int[] | indici di foglio basati su zero. |

### SheetSet(String[] sheetNames) {#SheetSet-java.lang.String---}
```
public SheetSet(String[] sheetNames)
```


Crea un set di fogli basato su nomi di foglio esatti.

**Remarks**

Se viene incontrato un foglio che non è nella cartella di lavoro, verrà generata un'eccezione durante il rendering.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetNames | java.lang.String[] | nomi dei fogli. |

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
### getActive() {#getActive--}
```
public static SheetSet getActive()
```


Ottiene un set con il foglio attivo della cartella di lavoro.

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getAll() {#getAll--}
```
public static SheetSet getAll()
```


Ottiene un set con tutti i fogli della cartella di lavoro nel loro ordine originale.

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getVisible() {#getVisible--}
```
public static SheetSet getVisible()
```


Ottiene un set con i fogli visibili della cartella di lavoro nel loro ordine originale.

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
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

