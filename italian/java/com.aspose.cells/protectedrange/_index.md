---
title: "ProtectedRange"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Un intervallo specificato che può essere modificato quando la protezione del foglio è ATTIVA."
type: docs
url: /it/java/com.aspose.cells/protectedrange/
---

**Inheritance:**
java.lang.Object
```
public class ProtectedRange
```

Un intervallo specificato che può essere modificato quando la protezione del foglio è ATTIVA.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [addArea(int startRow, int startColumn, int endRow, int endColumn)](#addArea-int-int-int-int-) | Aggiunge un'area di riferimento a questo |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAreas()](#getAreas--) | Ottiene tutte le aree di riferimento. |
| [getCellArea()](#getCellArea--) | Ottiene il [getCellArea()](../../com.aspose.cells/protectedrange\\#getCellArea--) oggetto che rappresenta l'area della cella da proteggere. |
| [getClass()](#getClass--) |  |
| [getName()](#getName--) | Ottiene il titolo dell'intervallo. |
| [getPassword()](#getPassword--) | Rappresenta la password per proteggere l'intervallo. |
| [getSecurityDescriptor()](#getSecurityDescriptor--) | Il descrittore di sicurezza definisce gli account utente che possono modificare questo intervallo senza fornire una password per accedere all'intervallo. |
| [hashCode()](#hashCode--) |  |
| [isProtectedWithPassword()](#isProtectedWithPassword--) | Indica se il foglio di lavoro è protetto da password. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setName(String value)](#setName-java.lang.String-) | Ottiene il titolo dell'intervallo. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Rappresenta la password per proteggere l'intervallo. |
| [setSecurityDescriptor(String value)](#setSecurityDescriptor-java.lang.String-) | Il descrittore di sicurezza definisce gli account utente che possono modificare questo intervallo senza fornire una password per accedere all'intervallo. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addArea(int startRow, int startColumn, int endRow, int endColumn) {#addArea-int-int-int-int-}
```
public void addArea(int startRow, int startColumn, int endRow, int endColumn)
```


Aggiunge un'area di riferimento a questo

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | int | Riga di inizio. |
| startColumn | int | La colonna di inizio. |
| endRow | int | La riga finale. |
| endColumn | int | La colonna finale. |

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
### getAreas() {#getAreas--}
```
public CellArea[] getAreas()
```


Ottiene tutte le aree di riferimento.

**Returns:**
com.aspose.cells.CellArea[] - Restituisce tutte le aree di riferimento.
### getCellArea() {#getCellArea--}
```
public CellArea getCellArea()
```


Ottiene il [getCellArea()](../../com.aspose.cells/protectedrange\\#getCellArea--) oggetto che rappresenta l'area della cella da proteggere.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getName() {#getName--}
```
public String getName()
```


Ottiene il titolo dell'intervallo. Questo è usato come descrittore, non come definizione di intervallo denominato.

**Returns:**
java.lang.String
### getPassword() {#getPassword--}
```
public String getPassword()
```


Rappresenta la password per proteggere l'intervallo.

**Returns:**
java.lang.String
### getSecurityDescriptor() {#getSecurityDescriptor--}
```
public String getSecurityDescriptor()
```


Il descrittore di sicurezza definisce gli account utente che possono modificare questo intervallo senza fornire una password per accedere all'intervallo.

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isProtectedWithPassword() {#isProtectedWithPassword--}
```
public boolean isProtectedWithPassword()
```


Indica se il foglio di lavoro è protetto da password.

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




### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Ottiene il titolo dell'intervallo. Questo è usato come descrittore, non come definizione di intervallo denominato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


Rappresenta la password per proteggere l'intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setSecurityDescriptor(String value) {#setSecurityDescriptor-java.lang.String-}
```
public void setSecurityDescriptor(String value)
```


Il descrittore di sicurezza definisce gli account utente che possono modificare questo intervallo senza fornire una password per accedere all'intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

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

