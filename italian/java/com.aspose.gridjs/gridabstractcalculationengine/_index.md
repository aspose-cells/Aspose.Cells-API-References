---
title: "GridAbstractCalculationEngine"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta il motore di calcolo personalizzato dell'utente per estendere il motore di calcolo predefinito di Aspose.Cells."
type: docs
url: /it/java/com.aspose.gridjs/gridabstractcalculationengine/
---

**Inheritance:**
java.lang.Object
```
public abstract class GridAbstractCalculationEngine
```

Rappresenta il motore di calcolo personalizzato dell'utente per estendere il motore di calcolo predefinito di Aspose.Cells.

**Remarks**

L'utente non dovrebbe modificare direttamente alcuna parte della Cartella di lavoro in questa implementazione (eccetto il risultato calcolato della funzione personalizzata, che può essere impostato tramite la proprietà GridCalculationData.CalculatedValue). Altrimenti potrebbero verificarsi risultati inattesi o un'Exception. Se l'utente deve modificare dati diversi dal risultato calcolato nell'implementazione per alcune funzioni personalizzate, ad esempio modificare la formula di una cella, lo stile, ...etc., l'utente dovrebbe raccogliere tali dati in questa implementazione e modificarli al di fuori dell'ambito del calcolo delle formule.

**Example**

```
          class MyEngine extends GridAbstractCalculationEngine
         {
             public /*override*/ void calculate(GridCalculationData data)
             {
                 String funcName = data.getFunctionName().toUpperCase();
                 if ("MYFUNC".equals(funcName))
                 {   
                     //do calculation for MYFUNC here
                     int count = data.getParamCount();
                     Object res = null;
                     for (int i = 0; i <count; i++)
                     {
                         Object pv = data.getParamValue(i);
                         if (pv instanceof GridReferredArea)
                         {
                             GridReferredArea ra = (GridReferredArea)pv;
                             pv = ra.getValue(0, 0);
                         }
                         //process the parameter here
                         //res = ...;
                     }
                     data.setCalculatedValue(res);
                 }
             }
         }
```
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [GridAbstractCalculationEngine()](#GridAbstractCalculationEngine--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [calculate(GridCalculationData data)](#calculate-com.aspose.gridjs.GridCalculationData-) | Calcola una funzione con i dati forniti. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridAbstractCalculationEngine() {#GridAbstractCalculationEngine--}
```
public GridAbstractCalculationEngine()
```


### calculate(GridCalculationData data) {#calculate-com.aspose.gridjs.GridCalculationData-}
```
public abstract void calculate(GridCalculationData data)
```


Calcola una funzione con i dati forniti.

**Remarks**

L'utente dovrebbe impostare il valore calcolato per i dati forniti per tutte le funzioni (incluse le funzioni native di Excel) che desidera calcolare autonomamente in questa implementazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| data | [GridCalculationData](../../com.aspose.gridjs/gridcalculationdata) | I dati richiesti per calcolare la funzione, come nome della funzione, parametri, ...etc. |

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

