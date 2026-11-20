---
title: "GridCalculationData"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta i dati richiesti durante il calcolo di una funzione, come i parametri del nome della funzione ...ecc."
type: docs
url: /it/java/com.aspose.gridjs/gridcalculationdata/
---

**Inheritance:**
java.lang.Object
```
public class GridCalculationData
```

Rappresenta i dati richiesti durante il calcolo di una funzione, come il nome della funzione, i parametri, ...ecc.

**Remarks**

Tutti gli oggetti forniti da questa classe sono solo a scopo di "lettura". L'utente non dovrebbe modificare alcun dato nella Cartella di lavoro durante il processo di calcolo della formula, altrimenti potrebbero verificarsi risultati inattesi o eccezioni.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculatedValue()](#getCalculatedValue--) | Restituisce il valore calcolato per questa funzione. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Restituisce l'indice della colonna della cella in cui si trova la funzione. |
| [getFormula()](#getFormula--) | Restituisce la formula della cella in cui si trova la funzione. |
| [getFunctionName()](#getFunctionName--) | Restituisce il nome della funzione da calcolare. |
| [getParamCount()](#getParamCount--) | Restituisce il conteggio dei parametri. |
| [getParamText(int index)](#getParamText-int-) | Restituisce il testo letterale del parametro all'indice specificato. |
| [getParamValue(int index)](#getParamValue-int-) | Restituisce l'oggetto valore rappresentato del parametro all'indice specificato. |
| [getRow()](#getRow--) | Restituisce l'indice della riga della cella in cui si trova la funzione. |
| [getSheetName()](#getSheetName--) | Restituisce il nome del foglio di lavoro in cui si trova la funzione. |
| [getStringValue()](#getStringValue--) | Restituisce il valore di visualizzazione della cella (DisplayStringValue) in cui si trova la funzione. |
| [getValue()](#getValue--) | Restituisce il valore della cella in cui si trova la funzione. |
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

L'utente dovrebbe impostare questa proprietà nel proprio motore di calcolo personalizzato per le funzioni supportate dal motore, e il valore impostato verrà restituito quando si legge questa proprietà. Leggere questa proprietà prima di impostarla farà sì che la funzione venga calcolata dal motore di calcolo predefinito di Aspose.Cells e verrà restituito il valore calcolato.

**Returns:**
java.lang.Object
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumn() {#getColumn--}
```
public int getColumn()
```


Restituisce l'indice della colonna della cella in cui si trova la funzione.

**Returns:**
int
### getFormula() {#getFormula--}
```
public String getFormula()
```


Restituisce la formula della cella in cui si trova la funzione.

**Returns:**
java.lang.String
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


Restituisce il conteggio dei parametri.

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
| indice | int | L'indice del parametro (basato su 0). |

**Returns:**
java.lang.String - Il testo letterale del parametro.
### getParamValue(int index) {#getParamValue-int-}
```
public Object getParamValue(int index)
```


Restituisce l'oggetto valore rappresentato del parametro all'indice specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice del parametro (basato su 0). |

**Returns:**
java.lang.Object - Se il parametro è un valore semplice, restituisce il valore semplice. Se il parametro è un riferimento, restituisce l'oggetto ReferredArea.
### getRow() {#getRow--}
```
public int getRow()
```


Restituisce l'indice della riga della cella in cui si trova la funzione.

**Returns:**
int
### getSheetName() {#getSheetName--}
```
public String getSheetName()
```


Restituisce il nome del foglio di lavoro in cui si trova la funzione.

**Returns:**
java.lang.String
### getStringValue() {#getStringValue--}
```
public String getStringValue()
```


Restituisce il valore di visualizzazione della cella (DisplayStringValue) in cui si trova la funzione.

**Returns:**
java.lang.String
### getValue() {#getValue--}
```
public Object getValue()
```


Restituisce il valore della cella in cui si trova la funzione.

**Returns:**
java.lang.Object
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

L'utente dovrebbe impostare questa proprietà nel proprio motore di calcolo personalizzato per le funzioni supportate dal motore, e il valore impostato verrà restituito quando si legge questa proprietà. Leggere questa proprietà prima di impostarla farà sì che la funzione venga calcolata dal motore di calcolo predefinito di Aspose.Cells e verrà restituito il valore calcolato.

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

