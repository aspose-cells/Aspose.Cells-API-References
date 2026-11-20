---
title: "GridValidationCollection"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Incapsula una raccolta di oggetti."
type: docs
url: /it/java/com.aspose.gridweb/gridvalidationcollection/
---

**Inheritance:**
java.lang.Object
```
public class GridValidationCollection
```

Incapsula una raccolta di oggetti [GridValidation](../../com.aspose.gridweb/gridvalidation).
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add()](#add--) | Aggiungi un [GridValidation](../../com.aspose.gridweb/gridvalidation) alla raccolta. |
| [add(GridCellArea ca)](#add-com.aspose.gridweb.GridCellArea-) | Aggiunge una convalida dei dati alla raccolta. |
| [add(GridValidation validation)](#add-com.aspose.gridweb.GridValidation-) | Aggiungi un [GridValidation](../../com.aspose.gridweb/gridvalidation) alla raccolta. |
| [add(int row, int column)](#add-int-int-) | Aggiungi un [GridValidation](../../com.aspose.gridweb/gridvalidation) alla raccolta. La convalida è applicata alla cella specificata. |
| [add(String cellname)](#add-java.lang.String-) | Aggiungi un [GridValidation](../../com.aspose.gridweb/gridvalidation) alla raccolta. La convalida è applicata alla cella specificata. |
| [clear()](#clear--) | Cancella tutte le convalide. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Restituisce l'elemento [GridValidation](../../com.aspose.gridweb/gridvalidation) all'indice specificato. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Restituisce la dimensione dell'enumeratore |
| [getValidationInCell(int row, int column)](#getValidationInCell-int-int-) | Ottiene la convalida applicata alla cella specificata. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Rimuove la convalida all'indice specificato. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add() {#add--}
```
public GridValidation add()
```


Aggiungi un [GridValidation](../../com.aspose.gridweb/gridvalidation) alla raccolta.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo GridValidationCollection.Add(row,col). Questa proprietà sarà rimossa tra 12 mesi a partire da GENNAIO 2015. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the added GridValidation instance.
### add(GridCellArea ca) {#add-com.aspose.gridweb.GridCellArea-}
```
public GridValidation add(GridCellArea ca)
```


Aggiunge una convalida dei dati alla raccolta.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ca | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | L'area contiene questa convalida. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the validation.
### add(GridValidation validation) {#add-com.aspose.gridweb.GridValidation-}
```
public int add(GridValidation validation)
```


Aggiungi un [GridValidation](../../com.aspose.gridweb/gridvalidation) alla raccolta.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| validation | [GridValidation](../../com.aspose.gridweb/gridvalidation) | Un oggetto di convalida. |

**Returns:**
int - indice dell'oggetto [GridValidation](../../com.aspose.gridweb/gridvalidation).
### add(int row, int column) {#add-int-int-}
```
public GridValidation add(int row, int column)
```


Aggiungi un [GridValidation](../../com.aspose.gridweb/gridvalidation) alla raccolta. La convalida è applicata alla cella specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | L'indice della riga. |
| colonna | int | L'indice della colonna. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the added GridValidation instance.
### add(String cellname) {#add-java.lang.String-}
```
public GridValidation add(String cellname)
```


Aggiungi un [GridValidation](../../com.aspose.gridweb/gridvalidation) alla raccolta. La convalida è applicata alla cella specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellname | java.lang.String | il nome della cella. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the added GridValidation instance.
### clear() {#clear--}
```
public void clear()
```


Cancella tutte le convalide.

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
### get(int index) {#get-int-}
```
public GridValidation get(int index)
```


Restituisce l'elemento [GridValidation](../../com.aspose.gridweb/gridvalidation) all'indice specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice basato su zero dell'elemento. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - The element at the specified index.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


Restituisce la dimensione dell'enumeratore

**Returns:**
int
### getValidationInCell(int row, int column) {#getValidationInCell-int-int-}
```
public GridValidation getValidationInCell(int row, int column)
```


Ottiene la convalida applicata alla cella specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | L'indice della riga. |
| colonna | int | L'indice della colonna. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - Returns a [GridValidation](../../com.aspose.gridweb/gridvalidation) object or null if there is no validation for given cell
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




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Rimuove la convalida all'indice specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice basato su zero dell'elemento. |

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

