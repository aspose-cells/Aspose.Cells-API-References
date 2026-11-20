---
title: "HorizontalPageBreak"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Incapsula l'oggetto che rappresenta un'interruzione di pagina orizzontale."
type: docs
url: /it/java/com.aspose.cells/horizontalpagebreak/
---

**Inheritance:**
java.lang.Object
```
public class HorizontalPageBreak
```

Incapsula l'oggetto che rappresenta un'interruzione di pagina orizzontale.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         //Add a page break at cell Y30
         int Index = worksheet.getHorizontalPageBreaks().add("Y30");
 
         //get the newly added horizontal page break
         HorizontalPageBreak hPageBreak = worksheet.getHorizontalPageBreaks().get(Index);
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getEndColumn()](#getEndColumn--) | Restituisce l'indice della colonna finale di questa interruzione di pagina orizzontale. |
| [getRow()](#getRow--) | Restituisce l'indice della riga basato su zero. |
| [getStartColumn()](#getStartColumn--) | Restituisce l'indice della colonna iniziale di questa interruzione di pagina orizzontale. |
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
### getEndColumn() {#getEndColumn--}
```
public int getEndColumn()
```


Restituisce l'indice della colonna finale di questa interruzione di pagina orizzontale.

**Returns:**
int
### getRow() {#getRow--}
```
public int getRow()
```


Restituisce l'indice della riga basato su zero.

**Returns:**
int
### getStartColumn() {#getStartColumn--}
```
public int getStartColumn()
```


Restituisce l'indice della colonna iniziale di questa interruzione di pagina orizzontale.

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

