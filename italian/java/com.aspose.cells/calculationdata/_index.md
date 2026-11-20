---
title: "CalculationData"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta i dati richiesti durante il calcolo di una funzione, come i parametri del nome della funzione ...ecc."
type: docs
url: /it/java/com.aspose.cells/calculationdata/
---

**Inheritance:**
java.lang.Object
```
public class CalculationData
```

Rappresenta i dati richiesti durante il calcolo di una funzione, come il nome della funzione, i parametri, ...ecc.

**Remarks**

Tutti gli oggetti forniti da questa classe sono solo a scopo di "lettura". L'utente non dovrebbe modificare alcun dato nella Cartella di lavoro durante il processo di calcolo della formula, altrimenti potrebbero verificarsi risultati inattesi o eccezioni.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculatedValue()](#getCalculatedValue--) | Restituisce il valore calcolato per questa funzione. |
| [getCell()](#getCell--) | Restituisce l'oggetto Cell dove si trova la funzione. |
| [getCellColumn()](#getCellColumn--) | Restituisce l'indice della colonna della cella in cui si trova la funzione. |
| [getCellRow()](#getCellRow--) | Restituisce l'indice della riga della cella in cui si trova la funzione. |
| [getClass()](#getClass--) |  |
| [getFunctionName()](#getFunctionName--) | Restituisce il nome della funzione da calcolare. |
| [getParamCount()](#getParamCount--) | Restituisce il conteggio dei parametri |
| [getParamText(int index)](#getParamText-int-) | Restituisce il testo letterale del parametro all'indice specificato. |
| [getParamValue(int index)](#getParamValue-int-) | Restituisce l'oggetto valore rappresentato del parametro a un dato indice. |
| [getParamValueInArrayMode(int index, int maxRowCount, int maxColumnCount)](#getParamValueInArrayMode-int-int-int-) | Restituisce il valore/i del parametro a un dato indice. |
| [getWorkbook()](#getWorkbook--) | Restituisce l'oggetto Workbook in cui si trova la funzione. |
| [getWorksheet()](#getWorksheet--) | Restituisce l'oggetto Worksheet in cui si trova la funzione. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalculatedValue(Object value)](#setCalculatedValue-java.lang.Object-) | Imposta il valore calcolato per questa funzione. |
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
### getCalculatedValue() {#getCalculatedValue--}
```
public Object getCalculatedValue()
```


Restituisce il valore calcolato per questa funzione.

**Remarks**

L'utente dovrebbe impostare questa proprietà nel proprio motore di calcolo personalizzato per le funzioni supportate dal motore, e il valore impostato verrà restituito quando si legge la proprietà in seguito. Il valore impostato può essere di tipi possibili come [Cell.getValue()](../../com.aspose.cells/cell\#getValue--), o un array di tali valori, oppure un Range, Name, ReferredArea. Ottenere questa proprietà prima di impostare un valore farà sì che la funzione venga calcolata dal motore di calcolo predefinito di Aspose.Cells e quindi verrà restituito il valore calcolato (in genere dovrebbe essere \#NAME? per le funzioni definite dall'utente).

**Returns:**
java.lang.Object
### getCell() {#getCell--}
```
public Cell getCell()
```


Restituisce l'oggetto Cell dove si trova la funzione.

**Remarks**

Durante il calcolo di una formula senza impostarla in una cella, ad esempio tramite [Worksheet.calculateFormula(String,CalculationOptions)](../../com.aspose.cells/worksheet\#calculateFormula-String-CalculationOptions-), la formula verrà calcolata come se fosse stata impostata nella cella A1, quindi sia [getCellRow()](../../com.aspose.cells/calculationdata\#getCellRow--) sia [getCellColumn()](../../com.aspose.cells/calculationdata\#getCellColumn--) saranno 0. Tuttavia, la cella A1 nel foglio di lavoro potrebbe non essere stata istanziata. Pertanto, per questo tipo di situazione questa proprietà sarà null.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getCellColumn() {#getCellColumn--}
```
public int getCellColumn()
```


Restituisce l'indice della colonna della cella in cui si trova la funzione.

**Returns:**
int
### getCellRow() {#getCellRow--}
```
public int getCellRow()
```


Restituisce l'indice della riga della cella in cui si trova la funzione.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFunctionName() {#getFunctionName--}
```
public String getFunctionName()
```


Restituisce il nome della funzione da calcolare.

**Returns:**
java.lang.String
### getParamCount() {#getParamCount--}
```
public int getParamCount()
```


Restituisce il conteggio dei parametri

**Returns:**
int
### getParamText(int index) {#getParamText-int-}
```
public String getParamText(int index)
```


Restituisce il testo letterale del parametro all'indice specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | indice del parametro (base 0) |

**Returns:**
java.lang.String - testo letterale del parametro.
### getParamValue(int index) {#getParamValue-int-}
```
public Object getParamValue(int index)
```


Restituisce l'oggetto valore rappresentato del parametro a un dato indice.

**Remarks**

Per un parametro:

Se è un valore semplice, restituisce il valore semplice stesso;

Se è un riferimento, restituisce l'oggetto ReferredArea;

Se fa riferimento a dataset con più valori, restituisce un array di oggetti;

Se è un tipo di espressione che necessita di essere calcolata, verrà calcolata in modalità valore e generalmente verrà restituito un singolo valore in base alla cella corrente. Ad esempio, se un parametro della formula D2 è A:A+B:B, allora A2+B2 verrà calcolato e restituito. Tuttavia, se questo parametro è stato specificato in modalità array (tramite  o ), verrà restituito un array (object[][]) i cui elementi sono A1+B1, A2+B2, ....

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice del parametro (base 0) |

**Returns:**
java.lang.Object - Il valore calcolato del parametro.
### getParamValueInArrayMode(int index, int maxRowCount, int maxColumnCount) {#getParamValueInArrayMode-int-int-int-}
```
public Object[][] getParamValueInArrayMode(int index, int maxRowCount, int maxColumnCount)
```


Restituisce il valore/i del parametro a un dato indice. Se il parametro è un tipo di espressione che necessita di essere calcolata, verrà calcolata in modalità array.

**Remarks**

Per un'espressione che necessita di essere calcolata, prendendo A:A+B:B come esempio: in modalità valore verrà calcolata a un singolo valore in base alla cella corrente. Ma in modalità array, tutti i valori di A1+B1, A2+B2, A3+B3, ... verranno calcolati e usati per costruire l'array restituito. E per questo tipo di situazione è consigliabile specificare il limite per il conteggio di righe/colonne (ad esempio secondo [Cells.getMaxDataRow()](../../com.aspose.cells/cells\#getMaxDataRow--) e [Cells.getMaxDataColumn()](../../com.aspose.cells/cells\#getMaxDataColumn--)), altrimenti l'array grande restituito potrebbe aumentare il consumo di memoria con una grande quantità di dati inutili.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice del parametro (base 0) |
| maxRowCount | int | Il limite di conteggio delle righe per l'array restituito. Se è non positivo o maggiore del conteggio reale delle righe, verrà usato il conteggio reale delle righe. |
| maxColumnCount | int | Il limite di conteggio delle colonne per l'array restituito. Se è non positivo o maggiore del conteggio reale delle colonne, verrà usato il conteggio reale delle colonne. |

**Returns:**
java.lang.Object[][] - Un array che contiene tutti gli elementi rappresentati dal parametro specificato.
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


Restituisce l'oggetto Workbook in cui si trova la funzione.

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Restituisce l'oggetto Worksheet in cui si trova la funzione.

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




### setCalculatedValue(Object value) {#setCalculatedValue-java.lang.Object-}
```
public void setCalculatedValue(Object value)
```


Imposta il valore calcolato per questa funzione.

**Remarks**

L'utente dovrebbe impostare questa proprietà nel proprio motore di calcolo personalizzato per le funzioni supportate dal motore, e il valore impostato verrà restituito quando si legge la proprietà in seguito. Il valore impostato può essere di tipi possibili come [Cell.getValue()](../../com.aspose.cells/cell\#getValue--), o un array di tali valori, oppure un Range, Name, ReferredArea. Ottenere questa proprietà prima di impostare un valore farà sì che la funzione venga calcolata dal motore di calcolo predefinito di Aspose.Cells e quindi verrà restituito il valore calcolato (in genere dovrebbe essere \#NAME? per le funzioni definite dall'utente).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.Object |  |

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

