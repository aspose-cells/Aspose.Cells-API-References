---
title: "ExternalLinkCollection"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta la collezione di collegamenti esterni in una cartella di lavoro."
type: docs
url: /it/java/com.aspose.cells/externallinkcollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class ExternalLinkCollection implements Iterable
```

Rappresenta la collezione di collegamenti esterni in una cartella di lavoro.

**Example**

```
         //Open a file with external links
         Workbook workbook = new Workbook("book1.xls");
 
         //Change external link data source
         workbook.getWorksheets().getExternalLinks().get(0).setDataSource("d:\\link.xls");
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add(int directoryType, String fileName, String[] sheetNames)](#add-int-java.lang.String-java.lang.String---) | Aggiungi un collegamento esterno . |
| [add(String fileName, String[] sheetNames)](#add-java.lang.String-java.lang.String---) | Aggiunge un collegamento esterno. |
| [clear()](#clear--) | Rimuove tutti i collegamenti esterni. |
| [clear(boolean updateReferencesAsLocal)](#clear-boolean-) | Rimuove tutti i collegamenti esterni. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Ottiene l'elemento [ExternalLink](../../com.aspose.cells/externallink) all'indice specificato. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ottiene il numero di elementi effettivamente contenuti nella collezione. |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Ottieni un enumeratore che itera attraverso questa collezione. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Rimuove il collegamento esterno specificato dal workbook. |
| [removeAt(int index, boolean updateReferencesAsLocal)](#removeAt-int-boolean-) | Rimuove il collegamento esterno specificato dal workbook. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int directoryType, String fileName, String[] sheetNames) {#add-int-java.lang.String-java.lang.String---}
```
public int add(int directoryType, String fileName, String[] sheetNames)
```


Aggiungi un collegamento esterno .

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| directoryType | int | [DirectoryType](../../com.aspose.cells/directorytype). Il tipo di directory del nome file. |
| fileName | java.lang.String | il nome file. |
| sheetNames | java.lang.String[] | Tutti i nomi dei fogli del file esterno. |

**Returns:**
int - La posizione del nome esterno in questo elenco.
### add(String fileName, String[] sheetNames) {#add-java.lang.String-java.lang.String---}
```
public int add(String fileName, String[] sheetNames)
```


Aggiunge un collegamento esterno.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | java.lang.String | Il nome del file esterno. |
| sheetNames | java.lang.String[] | Tutti i nomi dei fogli del file esterno. |

**Returns:**
int - La posizione del nome esterno in questo elenco.
### clear() {#clear--}
```
public void clear()
```


Rimuove tutti i collegamenti esterni.

**Remarks**

Quando si rimuovono i collegamenti esterni, tutte le formule che vi fanno riferimento verranno rimosse perché i riferimenti diventano non validi.

### clear(boolean updateReferencesAsLocal) {#clear-boolean-}
```
public void clear(boolean updateReferencesAsLocal)
```


Rimuove tutti i collegamenti esterni.

**Remarks**

Se è necessario aggiornare i riferimenti, quei riferimenti ai collegamenti esterni nelle formule verranno cambiati alla cartella di lavoro corrente quando possibile. Ad esempio, la formula originale di una cella è "='externalsource.xlam'!customfunction()", dopo la rimozione dei collegamenti esterni la formula diventerà "=customfunction()"; quando la formula originale è "='[externalsource.xlam]Sheet1'!$A$1", a seconda che esista un foglio con il nome "Sheet1" nella cartella di lavoro corrente: se vero, la formula diventerà "=Sheet1!$A$1"; se falso, la formula diventerà "=\#REF!$A$1".

Se non è necessario aggiornare i riferimenti, tutte le formule con riferimenti a collegamenti esterni verranno rimosse perché tali riferimenti diventano non validi.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| updateReferencesAsLocal | boolean | Indica se aggiornare tutti i riferimenti dei collegamenti esterni nelle formule ai riferimenti della cartella di lavoro corrente. |

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
public ExternalLink get(int index)
```


Ottiene l'elemento [ExternalLink](../../com.aspose.cells/externallink) all'indice specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice basato su zero dell'elemento. |

**Returns:**
[ExternalLink](../../com.aspose.cells/externallink) - The element at the specified index.
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


Ottiene il numero di elementi effettivamente contenuti nella collezione.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### iterator() {#iterator--}
```
public Iterator iterator()
```


Ottieni un enumeratore che itera attraverso questa collezione.

**Returns:**
java.util.Iterator -
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


Rimuove il collegamento esterno specificato dal workbook.

**Remarks**

Quando si rimuove il collegamento esterno, tutte le formule che vi fanno riferimento verranno rimosse perché i riferimenti diventano non validi.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | l'indice del collegamento esterno da rimuovere. |

### removeAt(int index, boolean updateReferencesAsLocal) {#removeAt-int-boolean-}
```
public void removeAt(int index, boolean updateReferencesAsLocal)
```


Rimuove il collegamento esterno specificato dal workbook.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | l'indice del collegamento esterno da rimuovere. |
| updateReferencesAsLocal | boolean | Indica se aggiornare tutti i riferimenti del collegamento esterno specificato al riferimento della cartella di lavoro corrente. Controlla [clear(boolean)](../../com.aspose.cells/externallinkcollection\#clear-boolean-) per ulteriori dettagli su questo parametro. |

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

