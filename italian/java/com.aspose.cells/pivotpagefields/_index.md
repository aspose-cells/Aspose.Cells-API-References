---
title: "PivotPageFields"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta gli elementi della pagina pivot se l'origine dati della tabella pivot è costituita da intervalli di consolidamento."
type: docs
url: /it/java/com.aspose.cells/pivotpagefields/
---

**Inheritance:**
java.lang.Object
```
public class PivotPageFields
```

Rappresenta gli elementi della pagina pivot se l'origine dati della tabella pivot è costituita da intervalli di consolidamento. Può contenere al massimo 4 elementi.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [PivotPageFields()](#PivotPageFields--) | Rappresenta gli elementi del campo pagina pivot. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [addIdentify(int rangeIndex, int[] pageItemIndex)](#addIdentify-int-int---) | Imposta quale etichetta dell'elemento in ogni campo pagina utilizzare per identificare l'intervallo di dati. |
| [addPageField(String[] pageItems)](#addPageField-java.lang.String---) | Aggiunge un campo pagina. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPageFieldCount()](#getPageFieldCount--) | Restituisce il numero di campi pagina. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotPageFields() {#PivotPageFields--}
```
public PivotPageFields()
```


Rappresenta gli elementi del campo pagina pivot.

### addIdentify(int rangeIndex, int[] pageItemIndex) {#addIdentify-int-int---}
```
public void addIdentify(int rangeIndex, int[] pageItemIndex)
```


Imposta quale etichetta dell'elemento in ogni campo pagina utilizzare per identificare l'intervallo di dati. pageItemIndex.Length deve essere uguale a PageFieldCount, quindi aggiungi prima il campo pagina.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rangeIndex | int | L'indice dell'intervallo di dati di consolidamento. |
| pageItemIndex | int[] | L'indice dell'elemento pagina in ciascun campo pagina. pageItemIndex[2] = 1 significa che il secondo elemento nel terzo campo è usato per identificare questo intervallo. pageItemIndex[1] = -1 indica che nessun elemento nel secondo campo è usato per identificare questo intervallo e MS creerà automaticamente un elemento \"blank\" nel secondo campo per identificare questo intervallo. |

### addPageField(String[] pageItems) {#addPageField-java.lang.String---}
```
public void addPageField(String[] pageItems)
```


Aggiunge un campo pagina.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pageItems | java.lang.String[] | Etichetta dell'elemento del campo pagina |

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
### getPageFieldCount() {#getPageFieldCount--}
```
public int getPageFieldCount()
```


Restituisce il numero di campi pagina.

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

