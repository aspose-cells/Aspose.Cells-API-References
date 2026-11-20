---
title: "VbaProjectReferenceCollection"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta tutti i riferimenti del progetto VBA."
type: docs
url: /it/java/com.aspose.cells/vbaprojectreferencecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class VbaProjectReferenceCollection extends CollectionBase
```

Rappresenta tutti i riferimenti del progetto VBA.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
          // Init VBA project.
         VbaProject vbaProject = workbook.getVbaProject();
         // Add vba project reference
         vbaProject.getReferences().addRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
         //Saving the Excel file
         workbook.save("book1.xlsm");
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Aggiunge un elemento all'istanza di CollectionBase. |
| [addControlReferernce(String name, String libid, String twiddledlibid, String extendedLibid)](#addControlReferernce-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | Aggiungi un riferimento a una libreria di tipo twiddled e alla sua libreria di tipo estesa. |
| [addControlRefrernce(String name, String libid, String twiddledlibid, String extendedLibid)](#addControlRefrernce-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | Aggiungi un riferimento a una libreria di tipo twiddled e alla sua libreria di tipo estesa. |
| [addProjectReferernce(String name, String absoluteLibid, String relativeLibid)](#addProjectReferernce-java.lang.String-java.lang.String-java.lang.String-) | Aggiunge un riferimento a un progetto VBA esterno. |
| [addProjectRefrernce(String name, String absoluteLibid, String relativeLibid)](#addProjectRefrernce-java.lang.String-java.lang.String-java.lang.String-) | Aggiunge un riferimento a un progetto VBA esterno. |
| [addRegisteredReference(String name, String libid)](#addRegisteredReference-java.lang.String-java.lang.String-) | Aggiungi un riferimento a una libreria di tipo Automation. |
| [clear()](#clear--) | Rimuove tutti gli oggetti dall'istanza di CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | Restituisce se l'istanza contiene questo oggetto |
| [copy(VbaProjectReferenceCollection source)](#copy-com.aspose.cells.VbaProjectReferenceCollection-) | Copia i riferimenti da un altro progetto VBA. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int i)](#get-int-) | Ottieni il riferimento nell'elenco mediante l'indice. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ottiene il numero di elementi contenuti nell'istanza di CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determina l'indice di un elemento specifico nell'istanza di CollectionBase. |
| [iterator()](#iterator--) | Restituisce un enumeratore che itera attraverso l'istanza di CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Rimuove l'elemento all'indice specificato. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Aggiunge un elemento all'istanza di CollectionBase.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| o | java.lang.Object | L'Object da aggiungere all'istanza di CollectionBase. |

**Returns:**
int - La posizione in cui è stato inserito il nuovo elemento.
### addControlReferernce(String name, String libid, String twiddledlibid, String extendedLibid) {#addControlReferernce-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public int addControlReferernce(String name, String libid, String twiddledlibid, String extendedLibid)
```


Aggiungi un riferimento a una libreria di tipo twiddled e alla sua libreria di tipo estesa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Il nome del riferimento. |
| libid | java.lang.String | L'identificatore di una libreria di tipo Automation. |
| twiddledlibid | java.lang.String | L'identificatore di una libreria di tipo twiddled |
| extendedLibid | java.lang.String | L'identificatore di una libreria di tipo estesa |

**Returns:**
int -
### addControlRefrernce(String name, String libid, String twiddledlibid, String extendedLibid) {#addControlRefrernce-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public int addControlRefrernce(String name, String libid, String twiddledlibid, String extendedLibid)
```


Aggiungi un riferimento a una libreria di tipo twiddled e alla sua libreria di tipo estesa.

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo VbaProjectReferenceCollection.AddControlReferernce(). Questo metodo sarà rimosso tra 12 mesi a partire da luglio 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Il nome del riferimento. |
| libid | java.lang.String | L'identificatore di una libreria di tipo Automation. |
| twiddledlibid | java.lang.String | L'identificatore di una libreria di tipo twiddled |
| extendedLibid | java.lang.String | L'identificatore di una libreria di tipo estesa |

**Returns:**
int -
### addProjectReferernce(String name, String absoluteLibid, String relativeLibid) {#addProjectReferernce-java.lang.String-java.lang.String-java.lang.String-}
```
public int addProjectReferernce(String name, String absoluteLibid, String relativeLibid)
```


Aggiunge un riferimento a un progetto VBA esterno.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Il nome del riferimento. |
| absoluteLibid | java.lang.String | L'identificatore del progetto VBA di riferimento con un percorso assoluto. |
| relativeLibid | java.lang.String | L'identificatore del progetto VBA di riferimento con un percorso relativo. |

**Returns:**
int -
### addProjectRefrernce(String name, String absoluteLibid, String relativeLibid) {#addProjectRefrernce-java.lang.String-java.lang.String-java.lang.String-}
```
public int addProjectRefrernce(String name, String absoluteLibid, String relativeLibid)
```


Aggiunge un riferimento a un progetto VBA esterno.

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo VbaProjectReferenceCollection.AddProjectReferernce(). Questo metodo sarà rimosso tra 12 mesi a partire da luglio 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Il nome del riferimento. |
| absoluteLibid | java.lang.String | L'identificatore del progetto VBA di riferimento con un percorso assoluto. |
| relativeLibid | java.lang.String | L'identificatore del progetto VBA di riferimento con un percorso relativo. |

**Returns:**
int -
### addRegisteredReference(String name, String libid) {#addRegisteredReference-java.lang.String-java.lang.String-}
```
public int addRegisteredReference(String name, String libid)
```


Aggiungi un riferimento a una libreria di tipo Automation.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Il nome del riferimento. |
| libid | java.lang.String | L'identificatore di una libreria di tipo Automation. |

**Returns:**
int -
### clear() {#clear--}
```
public void clear()
```


Rimuove tutti gli oggetti dall'istanza di CollectionBase.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Restituisce se l'istanza contiene questo oggetto

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| o | java.lang.Object | oggetto di test |

**Returns:**
boolean - Se l'istanza contiene questo oggetto
### copy(VbaProjectReferenceCollection source) {#copy-com.aspose.cells.VbaProjectReferenceCollection-}
```
public void copy(VbaProjectReferenceCollection source)
```


Copia i riferimenti da un altro progetto VBA.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| source | [VbaProjectReferenceCollection](../../com.aspose.cells/vbaprojectreferencecollection) | I riferimenti di origine. |

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
### get(int i) {#get-int-}
```
public VbaProjectReference get(int i)
```


Ottieni il riferimento nell'elenco mediante l'indice.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| i | int | L'indice. |

**Returns:**
[VbaProjectReference](../../com.aspose.cells/vbaprojectreference) - 
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


Ottiene il numero di elementi contenuti nell'istanza di CollectionBase.

**Returns:**
int - Il numero di elementi contenuti nell'istanza di CollectionBase.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


Determina l'indice di un elemento specifico nell'istanza di CollectionBase.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| o | java.lang.Object | Determina l'indice di un elemento specifico nell'istanza di CollectionBase. |

**Returns:**
int - L'indice del valore se trovato nella lista; altrimenti, -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Restituisce un enumeratore che itera attraverso l'istanza di CollectionBase.

**Returns:**
java.util.Iterator - Un iteratore per l'istanza di CollectionBase.
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


Rimuove l'elemento all'indice specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice basato su zero dell'elemento da rimuovere. |

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

