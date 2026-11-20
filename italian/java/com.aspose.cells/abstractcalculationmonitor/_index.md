---
title: "AbstractCalculationMonitor"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Monitor per l'utente per tenere traccia dell'avanzamento del calcolo delle formule."
type: docs
url: /it/java/com.aspose.cells/abstractcalculationmonitor/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractCalculationMonitor
```

Monitor per l'utente per tenere traccia dell'avanzamento del calcolo delle formule.

**Example**

```
         class MyCalculationMonitor extends AbstractCalculationMonitor
         {
             public /*override*/ void beforeCalculate(int sheetIndex, int rowIndex, int colIndex)
             {
                 if(sheetIndex!=0 || rowIndex!=0 || colIndex!=0)
                 {
                     return;
                 }
                 System.out.println("Cell A1 will be calculated.");
             }
         }
         Workbook wb = new Workbook("calc.xlsx");
         CalculationOptions opts = new CalculationOptions();
         opts.setCalculationMonitor(new MyCalculationMonitor());
         wb.calculateFormula(opts);
```
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [AbstractCalculationMonitor()](#AbstractCalculationMonitor--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [afterCalculate(int sheetIndex, int rowIndex, int colIndex)](#afterCalculate-int-int-int-) | Implementa questo metodo per eseguire operazioni dopo che una cella è stata calcolata. |
| [beforeCalculate(int sheetIndex, int rowIndex, int colIndex)](#beforeCalculate-int-int-int-) | Implementa questo metodo per eseguire operazioni prima di calcolare una cella. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculatedValue()](#getCalculatedValue--) | Ottiene il valore appena calcolato della cella. |
| [getClass()](#getClass--) |  |
| [getOriginalValue()](#getOriginalValue--) | Ottiene il valore precedente della cella calcolata. |
| [getValueChanged()](#getValueChanged--) | Indica se il valore della cella è stato modificato dopo il calcolo. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [onCircular(Iterator circularCellsData)](#onCircular-java.util.Iterator-) | Implementa questo metodo per eseguire operazioni durante il calcolo di formule con riferimenti circolari. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractCalculationMonitor() {#AbstractCalculationMonitor--}
```
public AbstractCalculationMonitor()
```


### afterCalculate(int sheetIndex, int rowIndex, int colIndex) {#afterCalculate-int-int-int-}
```
public void afterCalculate(int sheetIndex, int rowIndex, int colIndex)
```


Implementa questo metodo per eseguire operazioni dopo che una cella è stata calcolata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetIndex | int | Indice del foglio a cui appartiene la cella. |
| rowIndex | int | Indice di riga della cella |
| colIndex | int | Indice della colonna della cella |

### beforeCalculate(int sheetIndex, int rowIndex, int colIndex) {#beforeCalculate-int-int-int-}
```
public void beforeCalculate(int sheetIndex, int rowIndex, int colIndex)
```


Implementa questo metodo per eseguire operazioni prima di calcolare una cella.

**Remarks**

Per le celle nelle formule di matrice, questo metodo potrebbe non essere eseguito perché generalmente tali celle vengono calcolate insieme.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetIndex | int | Indice del foglio a cui appartiene la cella. |
| rowIndex | int | Indice di riga della cella |
| colIndex | int | Indice della colonna della cella |

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


Restituisce il valore appena calcolato della cella. Deve essere usato solo in [afterCalculate(int,int,int)](../../com.aspose.cells/abstractcalculationmonitor\#afterCalculate-int-int-int-).

**Returns:**
java.lang.Object
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getOriginalValue() {#getOriginalValue--}
```
public Object getOriginalValue()
```


Restituisce il valore precedente della cella calcolata. Deve essere usato solo in [beforeCalculate(int,int,int)](../../com.aspose.cells/abstractcalculationmonitor\#beforeCalculate-int-int-int-) e [afterCalculate(int,int,int)](../../com.aspose.cells/abstractcalculationmonitor\#afterCalculate-int-int-int-).

**Returns:**
java.lang.Object
### getValueChanged() {#getValueChanged--}
```
public boolean getValueChanged()
```


Indica se il valore della cella è stato modificato dopo il calcolo. Deve essere usato solo in [afterCalculate(int,int,int)](../../com.aspose.cells/abstractcalculationmonitor\#afterCalculate-int-int-int-).

**Returns:**
boolean
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




### onCircular(Iterator circularCellsData) {#onCircular-java.util.Iterator-}
```
public boolean onCircular(Iterator circularCellsData)
```


Implementa questo metodo per eseguire operazioni durante il calcolo di formule con riferimenti circolari.

**Remarks**

Nell'implementazione l'utente può anche impostare il valore previsto come risultato calcolato per parte/tutte quelle celle, così il motore di formule non le calcolerà ricorsivamente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| circularCellsData | java.util.Iterator | IEnumerator con elementi [CalculationCell](../../com.aspose.cells/calculationcell) che rappresentano celle dipendenti da riferimenti circolari. |

**Returns:**
boolean - Indica se il motore di formule deve calcolare quelle celle in modo circolare dopo questa chiamata. True per consentire al motore di formule di continuare a calcolare per esse. False per far sì che il motore di formule le segni semplicemente come Calcolate.
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

