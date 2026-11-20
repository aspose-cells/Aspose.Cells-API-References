---
title: "FormulaSettings"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Impostazioni delle formule e del calcolo."
type: docs
url: /it/java/com.aspose.cells/formulasettings/
---

**Inheritance:**
java.lang.Object
```
public class FormulaSettings
```

Impostazioni delle formule e del calcolo.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculateOnOpen()](#getCalculateOnOpen--) | Indica se l'applicazione deve eseguire un calcolo completo quando la cartella di lavoro viene aperta. |
| [getCalculateOnSave()](#getCalculateOnSave--) | Indica se ricalcolare la cartella di lavoro prima di salvare il documento, quando è in modalità di calcolo manuale. |
| [getCalculationId()](#getCalculationId--) | Specifica la versione del motore di calcolo utilizzato per calcolare i valori nella cartella di lavoro. |
| [getCalculationMode()](#getCalculationMode--) | Ottiene la modalità di calcolo della cartella di lavoro in MS Excel. |
| [getClass()](#getClass--) |  |
| [getEnableCalculationChain()](#getEnableCalculationChain--) | Indica se abilitare la catena di calcolo per le formule. |
| [getEnableIterativeCalculation()](#getEnableIterativeCalculation--) | Indica se abilitare il calcolo iterativo per risolvere riferimenti circolari. |
| [getForceFullCalculation()](#getForceFullCalculation--) | Indica se calcola tutte le formule ogni volta che viene avviato un calcolo. |
| [getMaxChange()](#getMaxChange--) | La variazione massima per risolvere un riferimento circolare. |
| [getMaxIteration()](#getMaxIteration--) | Il numero massimo di iterazioni per risolvere un riferimento circolare. |
| [getPrecisionAsDisplayed()](#getPrecisionAsDisplayed--) | Indica se la precisione del risultato calcolato deve essere impostata così come viene visualizzata durante il calcolo delle formule. |
| [getPreservePaddingSpaces()](#getPreservePaddingSpaces--) | Indica se preservare quegli spazi e interruzioni di riga inseriti tra i token della formula durante il recupero e l'impostazione delle formule. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalculateOnOpen(boolean value)](#setCalculateOnOpen-boolean-) | Indica se l'applicazione deve eseguire un calcolo completo quando la cartella di lavoro viene aperta. |
| [setCalculateOnSave(boolean value)](#setCalculateOnSave-boolean-) | Indica se ricalcolare la cartella di lavoro prima di salvare il documento, quando è in modalità di calcolo manuale. |
| [setCalculationId(String value)](#setCalculationId-java.lang.String-) | Specifica la versione del motore di calcolo utilizzato per calcolare i valori nella cartella di lavoro. |
| [setCalculationMode(int value)](#setCalculationMode-int-) | Imposta la modalità di calcolo della cartella di lavoro in MS Excel. |
| [setEnableCalculationChain(boolean value)](#setEnableCalculationChain-boolean-) | Indica se abilitare la catena di calcolo per le formule. |
| [setEnableIterativeCalculation(boolean value)](#setEnableIterativeCalculation-boolean-) | Indica se abilitare il calcolo iterativo per risolvere riferimenti circolari. |
| [setForceFullCalculation(boolean value)](#setForceFullCalculation-boolean-) | Indica se calcola tutte le formule ogni volta che viene avviato un calcolo. |
| [setMaxChange(double value)](#setMaxChange-double-) | La variazione massima per risolvere un riferimento circolare. |
| [setMaxIteration(int value)](#setMaxIteration-int-) | Il numero massimo di iterazioni per risolvere un riferimento circolare. |
| [setPrecisionAsDisplayed(boolean value)](#setPrecisionAsDisplayed-boolean-) | Indica se la precisione del risultato calcolato deve essere impostata così come viene visualizzata durante il calcolo delle formule. |
| [setPreservePaddingSpaces(boolean value)](#setPreservePaddingSpaces-boolean-) | Indica se preservare quegli spazi e interruzioni di riga inseriti tra i token della formula durante il recupero e l'impostazione delle formule. |
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
### getCalculateOnOpen() {#getCalculateOnOpen--}
```
public boolean getCalculateOnOpen()
```


Indica se l'applicazione deve eseguire un calcolo completo quando la cartella di lavoro viene aperta.

**Remarks**

Questa proprietà serve solo per salvare le impostazioni nel file di foglio di calcolo risultante in modo che altre applicazioni (come MS Excel) possano comportarsi di conseguenza durante il caricamento del file risultante. Per motivi di prestazioni nella maggior parte delle applicazioni degli utenti, non calcoliamo automaticamente alcuna formula nella cartella di lavoro, indipendentemente dal valore impostato per questa proprietà.

**Returns:**
boolean
### getCalculateOnSave() {#getCalculateOnSave--}
```
public boolean getCalculateOnSave()
```


Indica se ricalcolare la cartella di lavoro prima di salvare il documento, quando è in modalità di calcolo manuale.

**Remarks**

Questa proprietà serve solo a salvare le impostazioni nel file di foglio di calcolo risultante in modo che altre applicazioni (come ms excel) possano comportarsi di conseguenza durante il caricamento e la manipolazione del file risultante. Per motivi di prestazioni per la maggior parte delle applicazioni degli utenti, non calcoliamo automaticamente alcuna formula nella cartella di lavoro, indipendentemente dal valore impostato per questa proprietà.

**Returns:**
boolean
### getCalculationId() {#getCalculationId--}
```
public String getCalculationId()
```


Specifica la versione del motore di calcolo utilizzato per calcolare i valori nella cartella di lavoro.

**Remarks**

Questa proprietà serve solo a salvare le impostazioni nel file di foglio di calcolo risultante in modo che altre applicazioni (come ms excel) possano comportarsi di conseguenza durante il caricamento e la manipolazione del file risultante. Nel caso di ms excel, se il valore di questa proprietà è inferiore all'identificatore del motore di ricalcolo associato all'applicazione che apre il file risultante, l'applicazione ricalcolerà i risultati di tutte le formule in questa cartella di lavoro immediatamente dopo il caricamento del file. Per motivi di prestazioni per la maggior parte delle applicazioni degli utenti, non calcoliamo automaticamente alcuna formula nella cartella di lavoro, indipendentemente dal valore impostato per questa proprietà.

**Returns:**
java.lang.String
### getCalculationMode() {#getCalculationMode--}
```
public int getCalculationMode()
```


Ottiene la modalità di calcolo della cartella di lavoro in MS Excel.

Vedi [CalcModeType](../../com.aspose.cells/calcmodetype).

**Remarks**

Questa proprietà serve solo a salvare le impostazioni nel file di foglio di calcolo risultante in modo che altre applicazioni (come ms excel) possano comportarsi di conseguenza durante il caricamento e la manipolazione del file risultante. Per motivi di prestazioni per la maggior parte delle applicazioni degli utenti, non calcoliamo automaticamente alcuna formula nella cartella di lavoro, indipendentemente dalla modalità impostata per questa proprietà. Se l'utente ha bisogno di calcolare le formule, si prega di chiamare sempre i metodi sugli oggetti appropriati secondo le necessità: [Workbook.calculateFormula()](../../com.aspose.cells/workbook\#calculateFormula--), [Worksheet.calculateFormula(CalculationOptions,boolean)](../../com.aspose.cells/worksheet\#calculateFormula-CalculationOptions-boolean-), [Cell.calculate(CalculationOptions)](../../com.aspose.cells/cell\#calculate-CalculationOptions-), ...etc.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEnableCalculationChain() {#getEnableCalculationChain--}
```
public boolean getEnableCalculationChain()
```


Indica se abilitare la catena di calcolo per le formule. Il valore predefinito è false.

**Remarks**

Quando ci sono molte formule nella cartella di lavoro e l'utente deve calcolarle ripetutamente modificando solo una piccola parte di esse, può essere utile per le prestazioni abilitare la catena di calcolo. D'altra parte, se la catena è abilitata, mantenere il modello della catena richiede memoria aggiuntiva e richiede anche un po' più di tempo CPU per alcune altre operazioni, come la modifica del valore o delle formule di una cella. Dopo aver cambiato questa proprietà da false a true, la catena di calcolo verrà analizzata e costruita al momento del primo calcolo della cartella di lavoro, quindi il tempo richiesto per il primo calcolo potrebbe essere superiore al calcolo normale senza catena.

**Returns:**
boolean
### getEnableIterativeCalculation() {#getEnableIterativeCalculation--}
```
public boolean getEnableIterativeCalculation()
```


Indica se abilitare il calcolo iterativo per risolvere riferimenti circolari.

**Returns:**
boolean
### getForceFullCalculation() {#getForceFullCalculation--}
```
public boolean getForceFullCalculation()
```


Indica se calcola tutte le formule ogni volta che viene avviato un calcolo.

**Remarks**

Questa proprietà serve solo a salvare le impostazioni nel file di foglio di calcolo risultante in modo che altre applicazioni (come ms excel) possano comportarsi di conseguenza durante il caricamento e la manipolazione del file risultante. Per motivi di prestazioni per la maggior parte delle applicazioni degli utenti, non calcoliamo automaticamente alcuna formula nella cartella di lavoro, indipendentemente dal valore impostato per questa proprietà.

**Returns:**
boolean
### getMaxChange() {#getMaxChange--}
```
public double getMaxChange()
```


La variazione massima per risolvere un riferimento circolare.

**Returns:**
double
### getMaxIteration() {#getMaxIteration--}
```
public int getMaxIteration()
```


Il numero massimo di iterazioni per risolvere un riferimento circolare.

**Returns:**
int
### getPrecisionAsDisplayed() {#getPrecisionAsDisplayed--}
```
public boolean getPrecisionAsDisplayed()
```


Indica se la precisione del risultato calcolato deve essere impostata così come viene visualizzata durante il calcolo delle formule.

**Returns:**
boolean
### getPreservePaddingSpaces() {#getPreservePaddingSpaces--}
```
public boolean getPreservePaddingSpaces()
```


Indica se preservare gli spazi e le interruzioni di riga che sono inseriti tra i token della formula durante il recupero e l'impostazione delle formule. Il valore predefinito è false.

**Remarks**

In generale quegli spazi e interruzioni di riga servono solo a scopo visivo; preservarli o meno non influisce sul risultato calcolato. Per motivi di prestazioni, se non vi è alcuna esigenza speciale, è preferibile non preservarli durante l'elaborazione delle formule.

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




### setCalculateOnOpen(boolean value) {#setCalculateOnOpen-boolean-}
```
public void setCalculateOnOpen(boolean value)
```


Indica se l'applicazione deve eseguire un calcolo completo quando la cartella di lavoro viene aperta.

**Remarks**

Questa proprietà serve solo per salvare le impostazioni nel file di foglio di calcolo risultante in modo che altre applicazioni (come MS Excel) possano comportarsi di conseguenza durante il caricamento del file risultante. Per motivi di prestazioni nella maggior parte delle applicazioni degli utenti, non calcoliamo automaticamente alcuna formula nella cartella di lavoro, indipendentemente dal valore impostato per questa proprietà.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setCalculateOnSave(boolean value) {#setCalculateOnSave-boolean-}
```
public void setCalculateOnSave(boolean value)
```


Indica se ricalcolare la cartella di lavoro prima di salvare il documento, quando è in modalità di calcolo manuale.

**Remarks**

Questa proprietà serve solo a salvare le impostazioni nel file di foglio di calcolo risultante in modo che altre applicazioni (come ms excel) possano comportarsi di conseguenza durante il caricamento e la manipolazione del file risultante. Per motivi di prestazioni per la maggior parte delle applicazioni degli utenti, non calcoliamo automaticamente alcuna formula nella cartella di lavoro, indipendentemente dal valore impostato per questa proprietà.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setCalculationId(String value) {#setCalculationId-java.lang.String-}
```
public void setCalculationId(String value)
```


Specifica la versione del motore di calcolo utilizzato per calcolare i valori nella cartella di lavoro.

**Remarks**

Questa proprietà serve solo a salvare le impostazioni nel file di foglio di calcolo risultante in modo che altre applicazioni (come ms excel) possano comportarsi di conseguenza durante il caricamento e la manipolazione del file risultante. Nel caso di ms excel, se il valore di questa proprietà è inferiore all'identificatore del motore di ricalcolo associato all'applicazione che apre il file risultante, l'applicazione ricalcolerà i risultati di tutte le formule in questa cartella di lavoro immediatamente dopo il caricamento del file. Per motivi di prestazioni per la maggior parte delle applicazioni degli utenti, non calcoliamo automaticamente alcuna formula nella cartella di lavoro, indipendentemente dal valore impostato per questa proprietà.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setCalculationMode(int value) {#setCalculationMode-int-}
```
public void setCalculationMode(int value)
```


Imposta la modalità di calcolo della cartella di lavoro in MS Excel.

Vedi [CalcModeType](../../com.aspose.cells/calcmodetype).

**Remarks**

Questa proprietà serve solo a salvare le impostazioni nel file di foglio di calcolo risultante in modo che altre applicazioni (come ms excel) possano comportarsi di conseguenza durante il caricamento e la manipolazione del file risultante. Per motivi di prestazioni per la maggior parte delle applicazioni degli utenti, non calcoliamo automaticamente alcuna formula nella cartella di lavoro, indipendentemente dalla modalità impostata per questa proprietà. Se l'utente ha bisogno di calcolare le formule, si prega di chiamare sempre i metodi sugli oggetti appropriati secondo le necessità: [Workbook.calculateFormula()](../../com.aspose.cells/workbook\#calculateFormula--), [Worksheet.calculateFormula(CalculationOptions,boolean)](../../com.aspose.cells/worksheet\#calculateFormula-CalculationOptions-boolean-), [Cell.calculate(CalculationOptions)](../../com.aspose.cells/cell\#calculate-CalculationOptions-), ...etc.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setEnableCalculationChain(boolean value) {#setEnableCalculationChain-boolean-}
```
public void setEnableCalculationChain(boolean value)
```


Indica se abilitare la catena di calcolo per le formule. Il valore predefinito è false.

**Remarks**

Quando ci sono molte formule nella cartella di lavoro e l'utente deve calcolarle ripetutamente modificando solo una piccola parte di esse, può essere utile per le prestazioni abilitare la catena di calcolo. D'altra parte, se la catena è abilitata, mantenere il modello della catena richiede memoria aggiuntiva e richiede anche un po' più di tempo CPU per alcune altre operazioni, come la modifica del valore o delle formule di una cella. Dopo aver cambiato questa proprietà da false a true, la catena di calcolo verrà analizzata e costruita al momento del primo calcolo della cartella di lavoro, quindi il tempo richiesto per il primo calcolo potrebbe essere superiore al calcolo normale senza catena.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEnableIterativeCalculation(boolean value) {#setEnableIterativeCalculation-boolean-}
```
public void setEnableIterativeCalculation(boolean value)
```


Indica se abilitare il calcolo iterativo per risolvere riferimenti circolari.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setForceFullCalculation(boolean value) {#setForceFullCalculation-boolean-}
```
public void setForceFullCalculation(boolean value)
```


Indica se calcola tutte le formule ogni volta che viene avviato un calcolo.

**Remarks**

Questa proprietà serve solo a salvare le impostazioni nel file di foglio di calcolo risultante in modo che altre applicazioni (come ms excel) possano comportarsi di conseguenza durante il caricamento e la manipolazione del file risultante. Per motivi di prestazioni per la maggior parte delle applicazioni degli utenti, non calcoliamo automaticamente alcuna formula nella cartella di lavoro, indipendentemente dal valore impostato per questa proprietà.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setMaxChange(double value) {#setMaxChange-double-}
```
public void setMaxChange(double value)
```


La variazione massima per risolvere un riferimento circolare.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setMaxIteration(int value) {#setMaxIteration-int-}
```
public void setMaxIteration(int value)
```


Il numero massimo di iterazioni per risolvere un riferimento circolare.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setPrecisionAsDisplayed(boolean value) {#setPrecisionAsDisplayed-boolean-}
```
public void setPrecisionAsDisplayed(boolean value)
```


Indica se la precisione del risultato calcolato deve essere impostata così come viene visualizzata durante il calcolo delle formule.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setPreservePaddingSpaces(boolean value) {#setPreservePaddingSpaces-boolean-}
```
public void setPreservePaddingSpaces(boolean value)
```


Indica se preservare gli spazi e le interruzioni di riga che sono inseriti tra i token della formula durante il recupero e l'impostazione delle formule. Il valore predefinito è false.

**Remarks**

In generale quegli spazi e interruzioni di riga servono solo a scopo visivo; preservarli o meno non influisce sul risultato calcolato. Per motivi di prestazioni, se non vi è alcuna esigenza speciale, è preferibile non preservarli durante l'elaborazione delle formule.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

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

