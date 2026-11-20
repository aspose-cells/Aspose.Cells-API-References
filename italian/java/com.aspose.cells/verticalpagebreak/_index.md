---
title: "VerticalPageBreak"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Incapsula l'oggetto che rappresenta un'interruzione di pagina verticale."
type: docs
url: /it/java/com.aspose.cells/verticalpagebreak/
---

**Inheritance:**
java.lang.Object
```
public class VerticalPageBreak
```

Incapsula l'oggetto che rappresenta un'interruzione di pagina verticale.

**Example**

```
         Workbook excel = new Workbook();
         //Add a pagebreak at G5
         excel.getWorksheets().get(0).getHorizontalPageBreaks().add("G5");
         excel.getWorksheets().get(0).getVerticalPageBreaks().add("G5");
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Ottiene l'indice della colonna dell'interruzione di pagina verticale. |
| [getEndRow()](#getEndRow--) | Ottiene l'indice della riga finale dell'interruzione di pagina verticale. |
| [getStartRow()](#getStartRow--) | Ottiene l'indice della riga iniziale dell'interruzione di pagina verticale. |
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
### getColumn() {#getColumn--}
```
public int getColumn()
```


Ottiene l'indice della colonna dell'interruzione di pagina verticale.

**Returns:**
int
### getEndRow() {#getEndRow--}
```
public int getEndRow()
```


Ottiene l'indice della riga finale dell'interruzione di pagina verticale.

**Returns:**
int
### getStartRow() {#getStartRow--}
```
public int getStartRow()
```


Ottiene l'indice della riga iniziale dell'interruzione di pagina verticale.

**Returns:**
int
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

