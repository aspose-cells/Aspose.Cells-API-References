---
title: "CalculationOptions"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta le opzioni per il calcolo."
type: docs
url: /it/java/com.aspose.cells/calculationoptions/
---

**Inheritance:**
java.lang.Object
```
public class CalculationOptions
```

Rappresenta le opzioni per il calcolo.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [CalculationOptions()](#CalculationOptions--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalcStackSize()](#getCalcStackSize--) | La dimensione dello stack per il calcolo ricorsivo delle celle. |
| [getCalculationMonitor()](#getCalculationMonitor--) | Il monitor per l'utente per tenere traccia dell'avanzamento del calcolo delle formule. |
| [getCharacterEncoding()](#getCharacterEncoding--) | Specifica la codifica utilizzata per codificare/decodificare i caratteri durante il calcolo delle formule. |
| [getClass()](#getClass--) |  |
| [getCustomEngine()](#getCustomEngine--) | Il motore di calcolo delle formule personalizzate per estendere il motore di calcolo predefinito di Aspose.Cells. |
| [getIgnoreError()](#getIgnoreError--) | Indica se gli errori riscontrati durante il calcolo delle formule devono essere ignorati. |
| [getLinkedDataSources()](#getLinkedDataSources--) | Specifica le origini dati per i collegamenti esterni utilizzati nelle formule. |
| [getPrecisionStrategy()](#getPrecisionStrategy--) | Specifica la strategia per l'elaborazione della precisione del calcolo. |
| [getRecursive()](#getRecursive--) | Indica se calcolare ricorsivamente le celle dipendenti quando si calcola una cella che dipende da altre celle. |
| [getRefreshDynamicArrayFormula()](#getRefreshDynamicArrayFormula--) | Indica se le formule di array dinamici devono essere aggiornate prima di calcolare le formule. |
| [getUserSpecifiedRefreshDynamicArrayFormula()](#getUserSpecifiedRefreshDynamicArrayFormula--) | Indica se l'utente ha specificato esplicitamente il comportamento di aggiornamento delle formule di array dinamici prima di calcolare le formule specificate. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalcStackSize(int value)](#setCalcStackSize-int-) | La dimensione dello stack per il calcolo ricorsivo delle celle. |
| [setCalculationMonitor(AbstractCalculationMonitor value)](#setCalculationMonitor-com.aspose.cells.AbstractCalculationMonitor-) | Il monitor per l'utente per tenere traccia dell'avanzamento del calcolo delle formule. |
| [setCharacterEncoding(Encoding value)](#setCharacterEncoding-com.aspose.cells.Encoding-) | Specifica la codifica utilizzata per codificare/decodificare i caratteri durante il calcolo delle formule. |
| [setCustomEngine(AbstractCalculationEngine value)](#setCustomEngine-com.aspose.cells.AbstractCalculationEngine-) | Il motore di calcolo delle formule personalizzate per estendere il motore di calcolo predefinito di Aspose.Cells. |
| [setIgnoreError(boolean value)](#setIgnoreError-boolean-) | Indica se gli errori riscontrati durante il calcolo delle formule devono essere ignorati. |
| [setLinkedDataSources(Workbook[] value)](#setLinkedDataSources-com.aspose.cells.Workbook---) | Specifica le origini dati per i collegamenti esterni utilizzati nelle formule. |
| [setPrecisionStrategy(int value)](#setPrecisionStrategy-int-) | Specifica la strategia per l'elaborazione della precisione del calcolo. |
| [setRecursive(boolean value)](#setRecursive-boolean-) | Indica se calcolare ricorsivamente le celle dipendenti quando si calcola una cella che dipende da altre celle. |
| [setRefreshDynamicArrayFormula(boolean value)](#setRefreshDynamicArrayFormula-boolean-) | Indica se le formule di array dinamici devono essere aggiornate prima di calcolare le formule. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CalculationOptions() {#CalculationOptions--}
```
public CalculationOptions()
```


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
### getCalcStackSize() {#getCalcStackSize--}
```
public int getCalcStackSize()
```


La dimensione dello stack per il calcolo ricorsivo delle celle. Il valore predefinito è 200.

**Remarks**

Quando ci sono grandi quantità di celle da calcolare ricorsivamente nell'albero delle dipendenze, può verificarsi una StackOverflowException durante il processo di calcolo. In tal caso, l'utente dovrebbe specificare un valore più piccolo per questa proprietà. Per tali situazioni, l'utente dovrebbe determinare il valore appropriato per questa proprietà in base alle formule e ai dati reali. Tuttavia, un valore troppo piccolo può causare un degrado delle prestazioni del calcolo delle formule e un valore inferiore a 2 renderà impossibile calcolare una formula che dipende da un'altra. Quindi, se il valore specificato è inferiore a 2, verrà reimpostato a 2.

**Returns:**
int
### getCalculationMonitor() {#getCalculationMonitor--}
```
public AbstractCalculationMonitor getCalculationMonitor()
```


Il monitor per l'utente per tenere traccia dell'avanzamento del calcolo delle formule.

**Returns:**
[AbstractCalculationMonitor](../../com.aspose.cells/abstractcalculationmonitor)
### getCharacterEncoding() {#getCharacterEncoding--}
```
public Encoding getCharacterEncoding()
```


Specifica la codifica utilizzata per codificare/decodificare i caratteri durante il calcolo delle formule. Per funzioni come CHAR, CODE, il risultato calcolato dipende dalle impostazioni regionali e dal set di caratteri predefinito dell'ambiente. Con questa proprietà l'utente può specificare la codifica corretta da utilizzare per tali funzioni per ottenere il risultato previsto.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCustomEngine() {#getCustomEngine--}
```
public AbstractCalculationEngine getCustomEngine()
```


Il motore di calcolo delle formule personalizzate per estendere il motore di calcolo predefinito di Aspose.Cells.

**Returns:**
[AbstractCalculationEngine](../../com.aspose.cells/abstractcalculationengine)
### getIgnoreError() {#getIgnoreError--}
```
public boolean getIgnoreError()
```


Indica se gli errori riscontrati durante il calcolo delle formule devono essere ignorati. L'errore può essere una funzione non supportata, collegamenti esterni, ecc. Il valore predefinito è true.

**Returns:**
boolean
### getLinkedDataSources() {#getLinkedDataSources--}
```
public Workbook[] getLinkedDataSources()
```


Specifica le origini dati per i collegamenti esterni utilizzati nelle formule.

**Remarks**

Come [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---), qui è possibile specificare le origini dati per i collegamenti esterni utilizzati nelle formule da calcolare, in particolare quelli usati nella funzione INDIRECT. Per quei collegamenti esterni usati nella funzione INDIRECT, non vengono considerati parte dei collegamenti esterni della cartella di lavoro e non possono essere aggiornati da [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---). La corrispondenza di quelle cartelle di lavoro con i collegamenti esterni è determinata da [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) e [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--). Pertanto, assicurarsi che [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) sia stato specificato con il valore corretto (in genere dovrebbe coincidere con il corrispondente [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--)) per ogni cartella di lavoro affinché possano essere collegati come previsto.

**Returns:**
com.aspose.cells.Workbook[]
### getPrecisionStrategy() {#getPrecisionStrategy--}
```
public int getPrecisionStrategy()
```


Specifica la strategia per l'elaborazione della precisione del calcolo.

Vedi [CalculationPrecisionStrategy](../../com.aspose.cells/calculationprecisionstrategy).

**Returns:**
int
### getRecursive() {#getRecursive--}
```
public boolean getRecursive()
```


Indica se calcolare ricorsivamente le celle dipendenti quando si calcola una cella che dipende da altre celle. Il valore predefinito è true.

**Returns:**
boolean
### getRefreshDynamicArrayFormula() {#getRefreshDynamicArrayFormula--}
```
public boolean getRefreshDynamicArrayFormula()
```


Indica se le formule di array dinamici devono essere aggiornate prima di calcolare le formule.

**Remarks**

Se questa proprietà è stata specificata esplicitamente, il valore specificato verrà utilizzato per determinare se aggiornare le formule di array dinamici. Altrimenti ([getUserSpecifiedRefreshDynamicArrayFormula()](../../com.aspose.cells/calculationoptions\#getUserSpecifiedRefreshDynamicArrayFormula--) è false), il valore predefinito dipende dal tipo di formule da calcolare: per il calcolo delle formule del workbook, come [Workbook.calculateFormula(CalculationOptions)](../../com.aspose.cells/workbook\#calculateFormula-CalculationOptions-), questa proprietà sarà considerata true. Per altri casi, come [Cell.calculate(CalculationOptions)](../../com.aspose.cells/cell\#calculate-CalculationOptions-) o [Worksheet.calculateFormula(CalculationOptions,boolean)](../../com.aspose.cells/worksheet\#calculateFormula-CalculationOptions-boolean-), questa proprietà sarà considerata false.

**Returns:**
boolean
### getUserSpecifiedRefreshDynamicArrayFormula() {#getUserSpecifiedRefreshDynamicArrayFormula--}
```
public boolean getUserSpecifiedRefreshDynamicArrayFormula()
```


Indica se l'utente ha specificato esplicitamente il comportamento di aggiornamento delle formule di array dinamici prima di calcolare le formule specificate.

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




### setCalcStackSize(int value) {#setCalcStackSize-int-}
```
public void setCalcStackSize(int value)
```


La dimensione dello stack per il calcolo ricorsivo delle celle. Il valore predefinito è 200.

**Remarks**

Quando ci sono grandi quantità di celle da calcolare ricorsivamente nell'albero delle dipendenze, può verificarsi una StackOverflowException durante il processo di calcolo. In tal caso, l'utente dovrebbe specificare un valore più piccolo per questa proprietà. Per tali situazioni, l'utente dovrebbe determinare il valore appropriato per questa proprietà in base alle formule e ai dati reali. Tuttavia, un valore troppo piccolo può causare un degrado delle prestazioni del calcolo delle formule e un valore inferiore a 2 renderà impossibile calcolare una formula che dipende da un'altra. Quindi, se il valore specificato è inferiore a 2, verrà reimpostato a 2.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setCalculationMonitor(AbstractCalculationMonitor value) {#setCalculationMonitor-com.aspose.cells.AbstractCalculationMonitor-}
```
public void setCalculationMonitor(AbstractCalculationMonitor value)
```


Il monitor per l'utente per tenere traccia dell'avanzamento del calcolo delle formule.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [AbstractCalculationMonitor](../../com.aspose.cells/abstractcalculationmonitor) |  |

### setCharacterEncoding(Encoding value) {#setCharacterEncoding-com.aspose.cells.Encoding-}
```
public void setCharacterEncoding(Encoding value)
```


Specifica la codifica utilizzata per codificare/decodificare i caratteri durante il calcolo delle formule. Per funzioni come CHAR, CODE, il risultato calcolato dipende dalle impostazioni regionali e dal set di caratteri predefinito dell'ambiente. Con questa proprietà l'utente può specificare la codifica corretta da utilizzare per tali funzioni per ottenere il risultato previsto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setCustomEngine(AbstractCalculationEngine value) {#setCustomEngine-com.aspose.cells.AbstractCalculationEngine-}
```
public void setCustomEngine(AbstractCalculationEngine value)
```


Il motore di calcolo delle formule personalizzate per estendere il motore di calcolo predefinito di Aspose.Cells.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [AbstractCalculationEngine](../../com.aspose.cells/abstractcalculationengine) |  |

### setIgnoreError(boolean value) {#setIgnoreError-boolean-}
```
public void setIgnoreError(boolean value)
```


Indica se gli errori riscontrati durante il calcolo delle formule devono essere ignorati. L'errore può essere una funzione non supportata, collegamenti esterni, ecc. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setLinkedDataSources(Workbook[] value) {#setLinkedDataSources-com.aspose.cells.Workbook---}
```
public void setLinkedDataSources(Workbook[] value)
```


Specifica le origini dati per i collegamenti esterni utilizzati nelle formule.

**Remarks**

Come [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---), qui è possibile specificare le origini dati per i collegamenti esterni utilizzati nelle formule da calcolare, in particolare quelli usati nella funzione INDIRECT. Per quei collegamenti esterni usati nella funzione INDIRECT, non vengono considerati parte dei collegamenti esterni della cartella di lavoro e non possono essere aggiornati da [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---). La corrispondenza di quelle cartelle di lavoro con i collegamenti esterni è determinata da [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) e [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--). Pertanto, assicurarsi che [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) sia stato specificato con il valore corretto (in genere dovrebbe coincidere con il corrispondente [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--)) per ogni cartella di lavoro affinché possano essere collegati come previsto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Workbook\[\]](../../com.aspose.cells/workbook) |  |

### setPrecisionStrategy(int value) {#setPrecisionStrategy-int-}
```
public void setPrecisionStrategy(int value)
```


Specifica la strategia per l'elaborazione della precisione del calcolo.

Vedi [CalculationPrecisionStrategy](../../com.aspose.cells/calculationprecisionstrategy).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setRecursive(boolean value) {#setRecursive-boolean-}
```
public void setRecursive(boolean value)
```


Indica se calcolare ricorsivamente le celle dipendenti quando si calcola una cella che dipende da altre celle. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setRefreshDynamicArrayFormula(boolean value) {#setRefreshDynamicArrayFormula-boolean-}
```
public void setRefreshDynamicArrayFormula(boolean value)
```


Indica se le formule di array dinamici devono essere aggiornate prima di calcolare le formule.

**Remarks**

Se questa proprietà è stata specificata esplicitamente, il valore specificato verrà utilizzato per determinare se aggiornare le formule di array dinamici. Altrimenti ([getUserSpecifiedRefreshDynamicArrayFormula()](../../com.aspose.cells/calculationoptions\#getUserSpecifiedRefreshDynamicArrayFormula--) è false), il valore predefinito dipende dal tipo di formule da calcolare: per il calcolo delle formule del workbook, come [Workbook.calculateFormula(CalculationOptions)](../../com.aspose.cells/workbook\#calculateFormula-CalculationOptions-), questa proprietà sarà considerata true. Per altri casi, come [Cell.calculate(CalculationOptions)](../../com.aspose.cells/cell\#calculate-CalculationOptions-) o [Worksheet.calculateFormula(CalculationOptions,boolean)](../../com.aspose.cells/worksheet\#calculateFormula-CalculationOptions-boolean-), questa proprietà sarà considerata false.

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

