---
title: "Name"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta un nome definito per un intervallo di celle."
type: docs
url: /it/java/com.aspose.cells/name/
---

**Inheritance:**
java.lang.Object
```
public class Name
```

Rappresenta un nome definito per un intervallo di celle.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Accessing the first worksheet in the Excel file
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Creating a named range
         Range range = worksheet.getCells().createRange("B4", "G14");
         //Setting the name of the named range
         range.setName("TestRange");
         //Saving the modified Excel file in default (that is Excel 2000) format
         workbook.save("output.xls");
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getComment()](#getComment--) | Restituisce il commento del nome. |
| [getFullText()](#getFullText--) | Restituisce il testo completo del nome dell'oggetto con l'impostazione di ambito. |
| [getR1C1RefersTo()](#getR1C1RefersTo--) | Restituisce un riferimento R1C1 del [Name](../../com.aspose.cells/name). |
| [getRange()](#getRange--) | Restituisce l'intervallo se questo nome si riferisce a un intervallo. |
| [getRange(boolean recalculate)](#getRange-boolean-) | Restituisce l'intervallo se questo nome si riferisce a un intervallo |
| [getRange(int sheetIndex, int row, int column)](#getRange-int-int-int-) | Restituisce l'intervallo se questo nome si riferisce a un intervallo. |
| [getRanges()](#getRanges--) | Restituisce tutti gli intervalli a cui si riferisce questo nome. |
| [getRanges(boolean recalculate)](#getRanges-boolean-) | Restituisce tutti gli intervalli a cui si riferisce questo nome. |
| [getReferredAreas(boolean recalculate)](#getReferredAreas-boolean-) | Restituisce tutti i riferimenti a cui si riferisce questo nome. |
| [getRefersTo()](#getRefersTo--) | Restituisce o imposta la formula a cui il nome è definito per fare riferimento, iniziando con il segno uguale. |
| [getRefersTo(boolean isR1C1, boolean isLocal)](#getRefersTo-boolean-boolean-) | Ottieni il riferimento di questo Nome. |
| [getRefersTo(boolean isR1C1, boolean isLocal, int row, int column)](#getRefersTo-boolean-boolean-int-int-) | Ottieni il riferimento di questo Nome in base alla cella specificata. |
| [getSheetIndex()](#getSheetIndex--) | Indica se questo nome appartiene a Cartella di lavoro o Foglio di lavoro. 0 = Nome globale, altrimenti indice al foglio (basato su 1). |
| [getText()](#getText--) | Ottiene il testo del nome dell'oggetto. |
| [hashCode()](#hashCode--) |  |
| [isReferred()](#isReferred--) | Indica se questo nome è referenziato da altre formule. |
| [isVisible()](#isVisible--) | Indica se il nome è visibile. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setComment(String value)](#setComment-java.lang.String-) | Imposta il commento del nome. |
| [setR1C1RefersTo(String value)](#setR1C1RefersTo-java.lang.String-) | Imposta un riferimento R1C1 del [Name](../../com.aspose.cells/name). |
| [setRefersTo(String value)](#setRefersTo-java.lang.String-) | Restituisce o imposta la formula a cui il nome è definito per fare riferimento, iniziando con il segno uguale. |
| [setRefersTo(String refersTo, boolean isR1C1, boolean isLocal)](#setRefersTo-java.lang.String-boolean-boolean-) | Imposta il riferimento di questo Nome. |
| [setSheetIndex(int value)](#setSheetIndex-int-) | Indica se questo nome appartiene a Cartella di lavoro o Foglio di lavoro. 0 = Nome globale, altrimenti indice al foglio (basato su 1). |
| [setText(String value)](#setText-java.lang.String-) | Ottiene il testo del nome dell'oggetto. |
| [setVisible(boolean value)](#setVisible-boolean-) | Indica se il nome è visibile. |
| [toString()](#toString--) | Restituisce una stringa che rappresenta l'oggetto Range corrente. |
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
### getComment() {#getComment--}
```
public String getComment()
```


Ottiene il commento del nome. Valido solo per Excel 2007 o versioni successive.

**Returns:**
java.lang.String
### getFullText() {#getFullText--}
```
public String getFullText()
```


Restituisce il testo completo del nome dell'oggetto con l'impostazione di ambito.

**Returns:**
java.lang.String
### getR1C1RefersTo() {#getR1C1RefersTo--}
```
public String getR1C1RefersTo()
```


Restituisce un riferimento R1C1 del [Name](../../com.aspose.cells/name).

**Returns:**
java.lang.String
### getRange() {#getRange--}
```
public Range getRange()
```


Restituisce l'intervallo se questo nome si riferisce a un intervallo.

**Returns:**
[Range](../../com.aspose.cells/range) - The range.
### getRange(boolean recalculate) {#getRange-boolean-}
```
public Range getRange(boolean recalculate)
```


Restituisce l'intervallo se questo nome si riferisce a un intervallo

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ricalcola | boolean | se ricalcolarlo se questo nome è stato calcolato prima di questa chiamata. |

**Returns:**
[Range](../../com.aspose.cells/range) - The range.
### getRange(int sheetIndex, int row, int column) {#getRange-int-int-int-}
```
public Range getRange(int sheetIndex, int row, int column)
```


Ottiene l'intervallo se questo nome fa riferimento a un intervallo. Se il riferimento di questo nome non è assoluto, l'intervallo può variare per celle diverse.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetIndex | int | L'indice del foglio corrispondente. |
| riga | int | L'indice della riga corrispondente. |
| colonna | int | L'indice della colonna corrispondente |

**Returns:**
[Range](../../com.aspose.cells/range) - The range.
### getRanges() {#getRanges--}
```
public Range[] getRanges()
```


Restituisce tutti gli intervalli a cui si riferisce questo nome.

**Returns:**
com.aspose.cells.Range[] - Tutti gli intervalli.
### getRanges(boolean recalculate) {#getRanges-boolean-}
```
public Range[] getRanges(boolean recalculate)
```


Restituisce tutti gli intervalli a cui si riferisce questo nome.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ricalcola | boolean | se ricalcolarlo se questo nome è stato calcolato prima di questa chiamata. |

**Returns:**
com.aspose.cells.Range[] - Tutti gli intervalli.
### getReferredAreas(boolean recalculate) {#getReferredAreas-boolean-}
```
public ReferredArea[] getReferredAreas(boolean recalculate)
```


Restituisce tutti i riferimenti a cui si riferisce questo nome.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ricalcola | boolean | se ricalcolarlo se questo nome è stato calcolato prima di questa chiamata. |

**Returns:**
com.aspose.cells.ReferredArea[] - Tutti gli intervalli.
### getRefersTo() {#getRefersTo--}
```
public String getRefersTo()
```


Restituisce o imposta la formula a cui il nome è definito per fare riferimento, iniziando con il segno uguale.

**Returns:**
java.lang.String
### getRefersTo(boolean isR1C1, boolean isLocal) {#getRefersTo-boolean-boolean-}
```
public String getRefersTo(boolean isR1C1, boolean isLocal)
```


Ottieni il riferimento di questo Nome.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isR1C1 | boolean | Indica se il riferimento deve essere formattato come R1C1. |
| isLocal | boolean | Indica se il riferimento deve essere formattato in base alla lingua locale. |

**Returns:**
java.lang.String
### getRefersTo(boolean isR1C1, boolean isLocal, int row, int column) {#getRefersTo-boolean-boolean-int-int-}
```
public String getRefersTo(boolean isR1C1, boolean isLocal, int row, int column)
```


Ottieni il riferimento di questo Nome in base alla cella specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isR1C1 | boolean | Indica se il riferimento deve essere formattato come R1C1. |
| isLocal | boolean | Indica se il riferimento deve essere formattato in base alla lingua locale. |
| riga | int | L'indice di riga della cella. |
| colonna | int | L'indice di colonna della cella. |

**Returns:**
java.lang.String
### getSheetIndex() {#getSheetIndex--}
```
public int getSheetIndex()
```


Indica se questo nome appartiene a Cartella di lavoro o Foglio di lavoro. 0 = Nome globale, altrimenti indice al foglio (basato su 1).

**Returns:**
int
### getText() {#getText--}
```
public String getText()
```


Ottiene il testo del nome dell'oggetto.

**Returns:**
java.lang.String
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


Indica se questo nome è referenziato da altre formule.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Indica se il nome è visibile.

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




### setComment(String value) {#setComment-java.lang.String-}
```
public void setComment(String value)
```


Imposta il commento del nome. Valido solo per Excel 2007 o versioni successive.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setR1C1RefersTo(String value) {#setR1C1RefersTo-java.lang.String-}
```
public void setR1C1RefersTo(String value)
```


Imposta un riferimento R1C1 del [Name](../../com.aspose.cells/name).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setRefersTo(String value) {#setRefersTo-java.lang.String-}
```
public void setRefersTo(String value)
```


Restituisce o imposta la formula a cui il nome è definito per fare riferimento, iniziando con il segno uguale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setRefersTo(String refersTo, boolean isR1C1, boolean isLocal) {#setRefersTo-java.lang.String-boolean-boolean-}
```
public void setRefersTo(String refersTo, boolean isR1C1, boolean isLocal)
```


Imposta il riferimento di questo Nome.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| refersTo | java.lang.String | Il riferimento. |
| isR1C1 | boolean | Indica se il riferimento è in formato R1C1. |
| isLocal | boolean | Se il riferimento è formattato per locale. |

### setSheetIndex(int value) {#setSheetIndex-int-}
```
public void setSheetIndex(int value)
```


Indica se questo nome appartiene a Cartella di lavoro o Foglio di lavoro. 0 = Nome globale, altrimenti indice al foglio (basato su 1).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Ottiene il testo del nome dell'oggetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Indica se il nome è visibile.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### toString() {#toString--}
```
public String toString()
```


Restituisce una stringa che rappresenta l'oggetto Range corrente.

**Returns:**
java.lang.String -
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

