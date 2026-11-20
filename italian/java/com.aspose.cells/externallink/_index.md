---
title: "ExternalLink"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta un collegamento esterno in una cartella di lavoro."
type: docs
url: /it/java/com.aspose.cells/externallink/
---

**Inheritance:**
java.lang.Object
```
public class ExternalLink
```

Rappresenta un collegamento esterno in una cartella di lavoro.

**Example**

```
         //Open a file with external links
         Workbook workbook = new Workbook("book1.xls");
 
         //Get External Link 
         ExternalLink externalLink = workbook.getWorksheets().getExternalLinks().get(0);
 
         //Change External Link's Data Source
         externalLink.setDataSource("d:\\link.xls");
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [addExternalName(String text, String referTo)](#addExternalName-java.lang.String-java.lang.String-) | Aggiunge un nome esterno. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDataSource()](#getDataSource--) | Rappresenta la fonte dati del collegamento esterno. |
| [getOriginalDataSource()](#getOriginalDataSource--) | Rappresenta la fonte dati memorizzata del collegamento esterno. |
| [getPathType()](#getPathType--) | Ottieni il tipo di percorso di questo collegamento esterno |
| [getType()](#getType--) | Restituisce il tipo di collegamento esterno. |
| [hashCode()](#hashCode--) |  |
| [isReferred()](#isReferred--) | Indica se questo collegamento esterno è referenziato da altri. |
| [isVisible()](#isVisible--) | Indica se questo collegamento esterno è visibile in MS Excel. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDataSource(String value)](#setDataSource-java.lang.String-) | Rappresenta la fonte dati del collegamento esterno. |
| [setOriginalDataSource(String value)](#setOriginalDataSource-java.lang.String-) | Rappresenta la fonte dati memorizzata del collegamento esterno. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addExternalName(String text, String referTo) {#addExternalName-java.lang.String-java.lang.String-}
```
public void addExternalName(String text, String referTo)
```


Aggiunge un nome esterno.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| testo | java.lang.String | Il testo del nome esterno. Se il nome esterno appartiene a un foglio di lavoro, il testo dovrebbe essere come Sheet1!Text. |
| referTo | java.lang.String | Il referTo del nome esterno. Deve essere una cella o l'intervallo. |

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
### getDataSource() {#getDataSource--}
```
public String getDataSource()
```


Rappresenta la fonte dati del collegamento esterno.

**Returns:**
java.lang.String
### getOriginalDataSource() {#getOriginalDataSource--}
```
public String getOriginalDataSource()
```


Rappresenta la fonte dati memorizzata del collegamento esterno.

**Returns:**
java.lang.String
### getPathType() {#getPathType--}
```
public String getPathType()
```


Ottieni il tipo di percorso di questo collegamento esterno

**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```


Restituisce il tipo di collegamento esterno.

See [ExternalLinkType](../../com.aspose.cells/externallinktype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isReferred() {#isReferred--}
```
public boolean isReferred()
```


Indica se questo collegamento esterno è referenziato da altri.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Indica se questo collegamento esterno è visibile in MS Excel.

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




### setDataSource(String value) {#setDataSource-java.lang.String-}
```
public void setDataSource(String value)
```


Rappresenta la fonte dati del collegamento esterno.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setOriginalDataSource(String value) {#setOriginalDataSource-java.lang.String-}
```
public void setOriginalDataSource(String value)
```


Rappresenta la fonte dati memorizzata del collegamento esterno.

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

