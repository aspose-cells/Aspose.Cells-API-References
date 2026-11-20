---
title: "CalculationCell"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta i dati rilevanti per il calcolo di una cella che viene calcolata."
type: docs
url: /it/java/com.aspose.cells/calculationcell/
---

**Inheritance:**
java.lang.Object
```
public class CalculationCell
```

Rappresenta i dati rilevanti per il calcolo di una cella che viene calcolata.

**Remarks**

L'utente non dovrebbe modificare alcun dato nel Workbook durante il processo di calcolo della formula, altrimenti potrebbero verificarsi risultati inattesi o eccezioni. Pertanto, tutti gli oggetti forniti da questa classe (come l'oggetto Cell del [getCell()](../../com.aspose.cells/calculationcell\#getCell--)) sono destinati solo allo scopo di \"lettura\".
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCell()](#getCell--) | Ottiene l'oggetto Cell che è in fase di calcolo. |
| [getCellColumn()](#getCellColumn--) | Restituisce l'indice della colonna della cella. |
| [getCellRow()](#getCellRow--) | Restituisce l'indice della riga della cella. |
| [getClass()](#getClass--) |  |
| [getWorkbook()](#getWorkbook--) | Ottiene l'oggetto Workbook. |
| [getWorksheet()](#getWorksheet--) | Ottiene l'oggetto Worksheet in cui si trova la cella. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalculatedValue(Object v)](#setCalculatedValue-java.lang.Object-) | Imposta il valore calcolato per la cella. |
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
### getCell() {#getCell--}
```
public Cell getCell()
```


Ottiene l'oggetto Cell che è in fase di calcolo.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getCellColumn() {#getCellColumn--}
```
public int getCellColumn()
```


Restituisce l'indice della colonna della cella.

**Returns:**
int
### getCellRow() {#getCellRow--}
```
public int getCellRow()
```


Restituisce l'indice della riga della cella.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


Ottiene l'oggetto Workbook.

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Ottiene l'oggetto Worksheet in cui si trova la cella.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
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




### setCalculatedValue(Object v) {#setCalculatedValue-java.lang.Object-}
```
public void setCalculatedValue(Object v)
```


Imposta il valore calcolato per la cella.

**Remarks**

L'utente può impostare il risultato calcolato con questo metodo per ignorare il calcolo automatico per la cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| v | java.lang.Object |  |

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

