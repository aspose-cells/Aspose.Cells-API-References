---
title: "AbstractCalculationEngine"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta il motore di calcolo personalizzato dell'utente per estendere il motore di calcolo predefinito di Aspose.Cells."
type: docs
url: /it/java/com.aspose.cells/abstractcalculationengine/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractCalculationEngine
```

Rappresenta il motore di calcolo personalizzato dell'utente per estendere il motore di calcolo predefinito di Aspose.Cells.

**Remarks**

L'utente non dovrebbe modificare direttamente alcuna parte della Workbook in questa implementazione (eccetto il risultato calcolato della funzione personalizzata, che può essere impostato tramite la proprietà CalculationData.CalculatedValue). Altrimenti potrebbero verificarsi risultati inattesi o un'Exception. Se l'utente ha bisogno di modificare altri dati oltre al risultato calcolato nell'implementazione per alcune funzioni personalizzate, ad esempio modificare la formula della cella, lo stile, ...etc., l'utente dovrebbe raccogliere tali dati in questa implementazione e modificarli al di fuori dell'ambito del calcolo della formula.

**Example**

```
         class MyEngine extends AbstractCalculationEngine
         {
             public /*override*/ void calculate(CalculationData data)
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
                         if (pv instanceof ReferredArea)
                         {
                             ReferredArea ra = (ReferredArea)pv;
                             pv = ra.getValue(0, 0);
                         }
                         //process the parameter here
                         //res = ...;
                     }
                     data.setCalculatedValue(res);
                 }
             }
         }
         Workbook wb = new Workbook("custom_calc.xlsx");
         CalculationOptions opts = new CalculationOptions();
         opts.setCustomEngine(new MyEngine());
         wb.calculateFormula(opts);
```
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [AbstractCalculationEngine()](#AbstractCalculationEngine--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [calculate(CalculationData data)](#calculate-com.aspose.cells.CalculationData-) | Calcola una funzione con i dati forniti. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [forceRecalculate(String functionName)](#forceRecalculate-java.lang.String-) | Indica se forzare la ricomputazione della funzione fornita ogni volta durante il calcolo delle formule condivise. |
| [getClass()](#getClass--) |  |
| [getProcessBuiltInFunctions()](#getProcessBuiltInFunctions--) | Indica se le funzioni integrate supportate dal motore integrato debbano essere verificate ed elaborate da questa implementazione. |
| [hashCode()](#hashCode--) |  |
| [isParamArrayModeRequired()](#isParamArrayModeRequired--) | Indica se questo motore necessita che il parametro sia calcolato in modalità array. |
| [isParamLiteralRequired()](#isParamLiteralRequired--) | Indica se questo motore necessita del testo letterale del parametro durante un calcolo. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [skipCalculation()](#skipCalculation--) | Salta il calcolo per l'intera formula che fa riferimento alla funzione attualmente in valutazione. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractCalculationEngine() {#AbstractCalculationEngine--}
```
public AbstractCalculationEngine()
```


### calculate(CalculationData data) {#calculate-com.aspose.cells.CalculationData-}
```
public abstract void calculate(CalculationData data)
```


Calcola una funzione con i dati forniti.

**Remarks**

L'utente dovrebbe impostare il valore calcolato per i dati forniti per tutte le funzioni (incluse le funzioni native di Excel) che desidera calcolare autonomamente in questa implementazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| data | [CalculationData](../../com.aspose.cells/calculationdata) | i dati richiesti per calcolare la funzione, come il nome della funzione, i parametri, ...etc. |

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
### forceRecalculate(String functionName) {#forceRecalculate-java.lang.String-}
```
public boolean forceRecalculate(String functionName)
```


Indica se forzare la ricomputazione della funzione fornita ogni volta durante il calcolo delle formule condivise.

**Remarks**

Per le formule condivise, più celle condividono la stessa funzione. Se i parametri della funzione rimangono gli stessi per quelle celle, generalmente questa funzione deve essere calcolata una sola volta. Pertanto, per motivi di prestazioni, calcoliamo tale tipo di funzione una sola volta anche ([calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-) viene chiamato una sola volta, invece di essere chiamato ripetutamente per ogni cella). Tuttavia, per l'implementazione personalizzata dell'utente, potrebbe essere necessario calcolare la funzione, in particolare la funzione personalizzata, in modo diverso per celle diverse. In tal caso, l'utente deve sovrascrivere questo metodo per farlo restituire true per la funzione. E per [calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-), il valore restituito da [CalculationData.getCalculatedValue()](../../com.aspose.cells/calculationdata\#getCalculatedValue--) potrebbe essere stato inizializzato con il valore memorizzato nella cache del calcolo precedente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| functionName | java.lang.String | nome della funzione. Generalmente è il nome della funzione personalizzata. Se [getProcessBuiltInFunctions()](../../com.aspose.cells/abstractcalculationengine\#getProcessBuiltInFunctions--) è true, anche le funzioni integrate verranno verificate qui. |

**Returns:**
boolean - true se la funzione specificata deve essere sempre ricalcolata.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getProcessBuiltInFunctions() {#getProcessBuiltInFunctions--}
```
public boolean getProcessBuiltInFunctions()
```


Indica se le funzioni integrate supportate dal motore integrato debbano essere verificate ed elaborate da questa implementazione. Il valore predefinito è false.

**Remarks**

Se l'utente deve modificare la logica di calcolo di alcune funzioni integrate, questa proprietà dovrebbe essere impostata su true. Altrimenti, per motivi di prestazioni, lasciarla su false.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isParamArrayModeRequired() {#isParamArrayModeRequired--}
```
public boolean isParamArrayModeRequired()
```


Indica se questo motore necessita che il parametro sia calcolato in modalità array. Il valore predefinito è false. Se [CalculationData.getParamValueInArrayMode(int,int,int)](../../com.aspose.cells/calculationdata\#getParamValueInArrayMode-int-int-int-) è richiesto durante il calcolo delle funzioni personalizzate e l'utente non ha aggiornato la definizione per esse (tramite [Workbook.updateCustomFunctionDefinition(CustomFunctionDefinition)](../../com.aspose.cells/workbook\#updateCustomFunctionDefinition-CustomFunctionDefinition-)), questa proprietà deve essere impostata su true.

**Remarks**

Se questo motore di calcolo personalizzato necessita che il parametro sia calcolato in modalità array, saranno necessari più stack per memorizzare nella cache l'albero dei parametri e il metodo Calculate() potrebbe essere chiamato ricorsivamente per calcolare il valore del parametro. Per motivi di prestazioni, mantenere questa proprietà al valore predefinito (false) se non vi sono requisiti particolari.

**Returns:**
boolean
### isParamLiteralRequired() {#isParamLiteralRequired--}
```
public boolean isParamLiteralRequired()
```


Indica se questo motore richiede il testo letterale del parametro durante un calcolo. Il valore predefinito è false.

**Remarks**

Se questo motore di calcolo personalizzato richiede il testo letterale del parametro, saranno necessari più stack per memorizzare nella cache il testo letterale dei parametri e il metodo Calculate() potrebbe essere chiamato ricorsivamente per calcolare il valore del parametro. In generale il testo letterale non è necessario per calcolare le formule e questa proprietà dovrebbe rimanere impostata su false nella maggior parte delle implementazioni per ottenere migliori prestazioni.

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




### skipCalculation() {#skipCalculation--}
```
public void skipCalculation()
```


Salta il calcolo per l'intera formula che fa riferimento alla funzione attualmente in valutazione.

**Remarks**

Questo metodo può essere invocato nell'implementazione di [calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-) per saltare il calcolo dell'intera formula e il valore originale della formula verrà mantenuto invariato.

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

