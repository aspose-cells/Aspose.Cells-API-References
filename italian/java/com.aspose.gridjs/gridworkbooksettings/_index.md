---
title: "GridWorkbookSettings"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta le impostazioni della cartella di lavoro."
type: docs
url: /it/java/com.aspose.gridjs/gridworkbooksettings/
---

**Inheritance:**
java.lang.Object
```
public class GridWorkbookSettings
```

Rappresenta le impostazioni della cartella di lavoro.

**Example**

```
         GridJsWorkbook g = new GridJsWorkbook();
 
         GridWorkbookSettings gsettings = new GridWorkbookSettings();
         g.setSettings(gsettings);
 
         //do your business
```
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [GridWorkbookSettings()](#GridWorkbookSettings--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAuthor()](#getAuthor--) | Ottiene l'autore del file. |
| [getCheckCustomNumberFormat()](#getCheckCustomNumberFormat--) | Indica se verificare il formato numerico personalizzato quando si imposta Style.Custom, il valore predefinito è false. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Indica se verificare le restrizioni del file Excel quando l'utente modifica gli oggetti correlati alle celle. |
| [getClass()](#getClass--) |  |
| [getCreateCalcChain()](#getCreateCalcChain--) | Indica se creare la catena di formule calcolate. |
| [getDate1904()](#getDate1904--) | Ottiene un valore che indica se la cartella di lavoro utilizza il sistema di data 1904. |
| [getEnableMacros()](#getEnableMacros--) | Abilita le macro; ora funziona solo quando si copia un foglio di lavoro in un altro foglio all'interno di una cartella di lavoro. |
| [getForceFullCalculate()](#getForceFullCalculate--) | Indica se calcolare completamente ogni volta che viene attivato un calcolo. |
| [getIteration()](#getIteration--) | Indica se utilizzare l'iterazione per risolvere riferimenti circolari. |
| [getMaxIteration()](#getMaxIteration--) | Restituisce o imposta il numero massimo di iterazioni per risolvere un riferimento circolare, il valore predefinito è 100. |
| [getPrecisionAsDisplayed()](#getPrecisionAsDisplayed--) | Vero se i calcoli in questa cartella di lavoro verranno eseguiti utilizzando solo la precisione dei numeri così come vengono visualizzati |
| [getReCalculateOnOpen()](#getReCalculateOnOpen--) | Indica se ricalcolare tutte le formule all'apertura del file. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Imposta l'autore del file. |
| [setCheckCustomNumberFormat(boolean value)](#setCheckCustomNumberFormat-boolean-) | Indica se verificare il formato numerico personalizzato quando si imposta Style.Custom, il valore predefinito è false. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indica se verificare le restrizioni del file Excel quando l'utente modifica gli oggetti correlati alle celle. |
| [setCreateCalcChain(boolean value)](#setCreateCalcChain-boolean-) | Indica se creare la catena di formule calcolate. |
| [setDate1904(boolean value)](#setDate1904-boolean-) | Imposta un valore che rappresenta se la cartella di lavoro utilizza il sistema di data 1904. |
| [setEnableMacros(boolean value)](#setEnableMacros-boolean-) | Abilita le macro; ora funziona solo quando si copia un foglio di lavoro in un altro foglio all'interno di una cartella di lavoro. |
| [setForceFullCalculate(boolean value)](#setForceFullCalculate-boolean-) | Indica se calcolare completamente ogni volta che viene attivato un calcolo. |
| [setIteration(boolean value)](#setIteration-boolean-) | Indica se utilizzare l'iterazione per risolvere riferimenti circolari. |
| [setMaxIteration(int value)](#setMaxIteration-int-) | Restituisce o imposta il numero massimo di iterazioni per risolvere un riferimento circolare, il valore predefinito è 100. |
| [setPrecisionAsDisplayed(boolean value)](#setPrecisionAsDisplayed-boolean-) | Vero se i calcoli in questa cartella di lavoro verranno eseguiti utilizzando solo la precisione dei numeri così come vengono visualizzati |
| [setReCalculateOnOpen(boolean value)](#setReCalculateOnOpen-boolean-) | Indica se ricalcolare tutte le formule all'apertura del file. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridWorkbookSettings() {#GridWorkbookSettings--}
```
public GridWorkbookSettings()
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
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Ottiene l'autore del file.

**Returns:**
java.lang.String
### getCheckCustomNumberFormat() {#getCheckCustomNumberFormat--}
```
public boolean getCheckCustomNumberFormat()
```


Indica se verificare il formato numerico personalizzato quando si imposta Style.Custom, il valore predefinito è false.

**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Indica se verificare le restrizioni del file Excel quando l'utente modifica oggetti correlati alle celle. Per esempio, Excel non consente l'inserimento di una stringa più lunga di 32K. Quando si inserisce un valore più lungo di 32K, ad esempio tramite Cell.PutValue(string), se questa proprietà è true, si otterrà un'Exception. Se questa proprietà è false, accetteremo la stringa inserita come valore della cella, così in seguito sarà possibile esportare la stringa completa per altri formati di file come CSV. Tuttavia, se si è impostato un valore di questo tipo non valido per il formato file Excel, non si dovrebbe salvare la cartella di lavoro in formato Excel in seguito. Altrimenti potrebbero verificarsi errori imprevisti nel file Excel generato. Il valore predefinito è false.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCreateCalcChain() {#getCreateCalcChain--}
```
public boolean getCreateCalcChain()
```


Indica se creare la catena di formule calcolate. Il valore predefinito è false.

**Returns:**
boolean
### getDate1904() {#getDate1904--}
```
public boolean getDate1904()
```


Ottiene un valore che indica se la cartella di lavoro utilizza il sistema di data 1904.

**Returns:**
boolean
### getEnableMacros() {#getEnableMacros--}
```
public boolean getEnableMacros()
```


Abilita le macro; ora funziona solo quando si copia un foglio di lavoro in un altro foglio all'interno di una cartella di lavoro.

**Returns:**
boolean
### getForceFullCalculate() {#getForceFullCalculate--}
```
public boolean getForceFullCalculate()
```


Indica se calcolare completamente ogni volta che viene attivato un calcolo.

**Returns:**
boolean
### getIteration() {#getIteration--}
```
public boolean getIteration()
```


Indica se utilizzare l'iterazione per risolvere riferimenti circolari.

**Returns:**
boolean
### getMaxIteration() {#getMaxIteration--}
```
public int getMaxIteration()
```


Restituisce o imposta il numero massimo di iterazioni per risolvere un riferimento circolare, il valore predefinito è 100.

**Returns:**
int
### getPrecisionAsDisplayed() {#getPrecisionAsDisplayed--}
```
public boolean getPrecisionAsDisplayed()
```


Vero se i calcoli in questa cartella di lavoro verranno eseguiti utilizzando solo la precisione dei numeri così come vengono visualizzati

**Returns:**
boolean
### getReCalculateOnOpen() {#getReCalculateOnOpen--}
```
public boolean getReCalculateOnOpen()
```


Indica se ricalcolare tutte le formule all'apertura del file. Il valore predefinito è true.

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




### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


Imposta l'autore del file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setCheckCustomNumberFormat(boolean value) {#setCheckCustomNumberFormat-boolean-}
```
public void setCheckCustomNumberFormat(boolean value)
```


Indica se verificare il formato numerico personalizzato quando si imposta Style.Custom, il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Indica se verificare le restrizioni del file Excel quando l'utente modifica oggetti correlati alle celle. Per esempio, Excel non consente l'inserimento di una stringa più lunga di 32K. Quando si inserisce un valore più lungo di 32K, ad esempio tramite Cell.PutValue(string), se questa proprietà è true, si otterrà un'Exception. Se questa proprietà è false, accetteremo la stringa inserita come valore della cella, così in seguito sarà possibile esportare la stringa completa per altri formati di file come CSV. Tuttavia, se si è impostato un valore di questo tipo non valido per il formato file Excel, non si dovrebbe salvare la cartella di lavoro in formato Excel in seguito. Altrimenti potrebbero verificarsi errori imprevisti nel file Excel generato. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setCreateCalcChain(boolean value) {#setCreateCalcChain-boolean-}
```
public void setCreateCalcChain(boolean value)
```


Indica se creare la catena di formule calcolate. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setDate1904(boolean value) {#setDate1904-boolean-}
```
public void setDate1904(boolean value)
```


Imposta un valore che rappresenta se la cartella di lavoro utilizza il sistema di data 1904.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEnableMacros(boolean value) {#setEnableMacros-boolean-}
```
public void setEnableMacros(boolean value)
```


Abilita le macro; ora funziona solo quando si copia un foglio di lavoro in un altro foglio all'interno di una cartella di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setForceFullCalculate(boolean value) {#setForceFullCalculate-boolean-}
```
public void setForceFullCalculate(boolean value)
```


Indica se calcolare completamente ogni volta che viene attivato un calcolo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setIteration(boolean value) {#setIteration-boolean-}
```
public void setIteration(boolean value)
```


Indica se utilizzare l'iterazione per risolvere riferimenti circolari.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setMaxIteration(int value) {#setMaxIteration-int-}
```
public void setMaxIteration(int value)
```


Restituisce o imposta il numero massimo di iterazioni per risolvere un riferimento circolare, il valore predefinito è 100.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setPrecisionAsDisplayed(boolean value) {#setPrecisionAsDisplayed-boolean-}
```
public void setPrecisionAsDisplayed(boolean value)
```


Vero se i calcoli in questa cartella di lavoro verranno eseguiti utilizzando solo la precisione dei numeri così come vengono visualizzati

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setReCalculateOnOpen(boolean value) {#setReCalculateOnOpen-boolean-}
```
public void setReCalculateOnOpen(boolean value)
```


Indica se ricalcolare tutte le formule all'apertura del file. Il valore predefinito è true.

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

