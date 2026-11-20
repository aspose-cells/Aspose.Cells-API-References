---
title: "GridWorkbookSettings"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta le impostazioni della cartella di lavoro."
type: docs
url: /it/java/com.aspose.gridweb/gridworkbooksettings/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Serializable
```
public class GridWorkbookSettings implements Serializable
```

Rappresenta le impostazioni della cartella di lavoro.

**Example**

```
         GridWeb gridweb = new GridWeb();
         GridWorkbookSettings gsettings = new GridWorkbookSettings();
         gridweb.setSettings(gsettings);
 
         //do your business
```
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [GridWorkbookSettings()](#GridWorkbookSettings--) | costruttore predefinito |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAuthor()](#getAuthor--) | Ottiene l'autore del file. |
| [getCheckCustomNumberFormat()](#getCheckCustomNumberFormat--) | Ottiene se controllare il formato numerico personalizzato quando si imposta Style.Custom. |
| [getClass()](#getClass--) |  |
| [getCreateCalcChain()](#getCreateCalcChain--) | Ottiene se creare la catena di formule calcolate. |
| [getDate1904()](#getDate1904--) | Ottiene il valore che indica se la cartella di lavoro utilizza il sistema di data 1904. |
| [getEnableMacros()](#getEnableMacros--) | Ottiene se abilitare le macro; ora funziona solo quando si copia un foglio di lavoro in un altro foglio di lavoro in una cartella di lavoro. |
| [getForceFullCalculate()](#getForceFullCalculate--) | Ottiene se calcola completamente ogni volta quando viene avviato un calcolo. |
| [getIteration()](#getIteration--) | Ottiene se utilizzare l'iterazione per risolvere riferimenti circolari. |
| [getMaxIteration()](#getMaxIteration--) | Ottiene il numero massimo di iterazioni per risolvere un riferimento circolare, il valore predefinito è 100. |
| [getPrecisionAsDisplayed()](#getPrecisionAsDisplayed--) | Vero se i calcoli in questa cartella di lavoro verranno eseguiti utilizzando solo la precisione dei numeri così come vengono visualizzati |
| [getPreservePaddingSpaces()](#getPreservePaddingSpaces--) | Indica se preservare quegli spazi e interruzioni di riga inseriti tra i token della formula durante l'ottenimento e l'impostazione delle formule. |
| [getReCalculateOnOpen()](#getReCalculateOnOpen--) | Ottiene se ricalcolare tutte le formule all'apertura del file. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Imposta l'autore del file. |
| [setCheckCustomNumberFormat(boolean value)](#setCheckCustomNumberFormat-boolean-) | Imposta se verificare il formato numerico personalizzato quando si imposta Style.Custom. |
| [setCreateCalcChain(boolean value)](#setCreateCalcChain-boolean-) | Imposta se creare una catena di formule calcolate. |
| [setDate1904(boolean value)](#setDate1904-boolean-) | Imposta il valore che indica se la cartella di lavoro utilizza il sistema di data 1904. |
| [setEnableMacros(boolean value)](#setEnableMacros-boolean-) | Imposta se abilitare le macro; ora funziona solo quando si copia un foglio di lavoro in un altro foglio all'interno di una cartella di lavoro. |
| [setForceFullCalculate(boolean value)](#setForceFullCalculate-boolean-) | Imposta se calcola completamente ogni volta quando viene avviato un calcolo. |
| [setIteration(boolean value)](#setIteration-boolean-) | Imposta se utilizzare l'iterazione per risolvere riferimenti circolari. |
| [setMaxIteration(int value)](#setMaxIteration-int-) | Imposta il numero massimo di iterazioni per risolvere un riferimento circolare, il valore predefinito è 100. |
| [setPrecisionAsDisplayed(boolean value)](#setPrecisionAsDisplayed-boolean-) | Vero se i calcoli in questa cartella di lavoro verranno eseguiti utilizzando solo la precisione dei numeri così come vengono visualizzati |
| [setPreservePaddingSpaces(boolean value)](#setPreservePaddingSpaces-boolean-) | Indica se preservare quegli spazi e interruzioni di riga inseriti tra i token della formula durante l'ottenimento e l'impostazione delle formule. |
| [setReCalculateOnOpen(boolean value)](#setReCalculateOnOpen-boolean-) | Imposta se ricalcolare tutte le formule all'apertura del file. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridWorkbookSettings() {#GridWorkbookSettings--}
```
public GridWorkbookSettings()
```


costruttore predefinito

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


Ottiene se controllare il formato numerico personalizzato quando si imposta Style.Custom.

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


Ottiene se creare una catena di formule calcolate. Il valore predefinito è false.

**Returns:**
boolean
### getDate1904() {#getDate1904--}
```
public boolean getDate1904()
```


Ottiene il valore che indica se la cartella di lavoro utilizza il sistema di data 1904.

**Returns:**
boolean
### getEnableMacros() {#getEnableMacros--}
```
public boolean getEnableMacros()
```


Ottiene se abilitare le macro; ora funziona solo quando si copia un foglio di lavoro in un altro foglio di lavoro in una cartella di lavoro.

**Returns:**
boolean
### getForceFullCalculate() {#getForceFullCalculate--}
```
public boolean getForceFullCalculate()
```


Ottiene se calcola completamente ogni volta quando viene avviato un calcolo.

**Returns:**
boolean
### getIteration() {#getIteration--}
```
public boolean getIteration()
```


Ottiene se utilizzare l'iterazione per risolvere riferimenti circolari.

**Returns:**
boolean
### getMaxIteration() {#getMaxIteration--}
```
public int getMaxIteration()
```


Ottiene il numero massimo di iterazioni per risolvere un riferimento circolare, il valore predefinito è 100.

**Returns:**
int
### getPrecisionAsDisplayed() {#getPrecisionAsDisplayed--}
```
public boolean getPrecisionAsDisplayed()
```


Vero se i calcoli in questa cartella di lavoro verranno eseguiti utilizzando solo la precisione dei numeri così come vengono visualizzati

**Returns:**
boolean
### getPreservePaddingSpaces() {#getPreservePaddingSpaces--}
```
public boolean getPreservePaddingSpaces()
```


Indica se preservare quegli spazi e interruzioni di riga che sono inseriti tra i token della formula durante il recupero e l'impostazione delle formule. Il valore predefinito è false.

**Remarks**

In generale quegli spazi e interruzioni di riga servono solo a scopo visivo; preservarli o meno non influisce sul risultato calcolato. Per motivi di prestazioni, se non vi è alcuna esigenza speciale, è preferibile non preservarli durante l'elaborazione delle formule.

**Returns:**
boolean
### getReCalculateOnOpen() {#getReCalculateOnOpen--}
```
public boolean getReCalculateOnOpen()
```


Ottiene se ricalcolare tutte le formule all'apertura del file.

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


Imposta se verificare il formato numerico personalizzato quando si imposta Style.Custom.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setCreateCalcChain(boolean value) {#setCreateCalcChain-boolean-}
```
public void setCreateCalcChain(boolean value)
```


Imposta se creare una catena di formule calcolate. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setDate1904(boolean value) {#setDate1904-boolean-}
```
public void setDate1904(boolean value)
```


Imposta il valore che indica se la cartella di lavoro utilizza il sistema di data 1904.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEnableMacros(boolean value) {#setEnableMacros-boolean-}
```
public void setEnableMacros(boolean value)
```


Imposta se abilitare le macro; ora funziona solo quando si copia un foglio di lavoro in un altro foglio all'interno di una cartella di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setForceFullCalculate(boolean value) {#setForceFullCalculate-boolean-}
```
public void setForceFullCalculate(boolean value)
```


Imposta se calcola completamente ogni volta quando viene avviato un calcolo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setIteration(boolean value) {#setIteration-boolean-}
```
public void setIteration(boolean value)
```


Imposta se utilizzare l'iterazione per risolvere riferimenti circolari.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setMaxIteration(int value) {#setMaxIteration-int-}
```
public void setMaxIteration(int value)
```


Imposta il numero massimo di iterazioni per risolvere un riferimento circolare, il valore predefinito è 100.

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

### setPreservePaddingSpaces(boolean value) {#setPreservePaddingSpaces-boolean-}
```
public void setPreservePaddingSpaces(boolean value)
```


Indica se preservare quegli spazi e interruzioni di riga che sono inseriti tra i token della formula durante il recupero e l'impostazione delle formule. Il valore predefinito è false.

**Remarks**

In generale quegli spazi e interruzioni di riga servono solo a scopo visivo; preservarli o meno non influisce sul risultato calcolato. Per motivi di prestazioni, se non vi è alcuna esigenza speciale, è preferibile non preservarli durante l'elaborazione delle formule.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setReCalculateOnOpen(boolean value) {#setReCalculateOnOpen-boolean-}
```
public void setReCalculateOnOpen(boolean value)
```


Imposta se ricalcolare tutte le formule all'apertura del file.

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

