---
title: "DeleteBlankOptions"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta l'impostazione di eliminazione di celle/righe/colonne vuote."
type: docs
url: /it/java/com.aspose.cells/deleteblankoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.DeleteOptions](../../com.aspose.cells/deleteoptions)
```
public class DeleteBlankOptions extends DeleteOptions
```

Rappresenta l'impostazione di eliminazione di celle/righe/colonne vuote.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [DeleteBlankOptions()](#DeleteBlankOptions--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDrawingsAsBlank()](#getDrawingsAsBlank--) | Indica se gli oggetti correlati al disegno, come immagine, forma, grafico..., saranno considerati vuoti. |
| [getEmptyFormulaValueAsBlank()](#getEmptyFormulaValueAsBlank--) | Indica se una cella verrà considerata vuota quando è una formula e il risultato calcolato è null o una stringa vuota. |
| [getEmptyStringAsBlank()](#getEmptyStringAsBlank--) | Indica se una cella verrà considerata vuota quando il suo valore è una stringa vuota. |
| [getEndIndex()](#getEndIndex--) | Specifica l'indice di riga/colonna finale (inclusivo) dell'intervallo da controllare e da cui eliminare righe/colonne vuote. |
| [getFormulaChangeMonitor()](#getFormulaChangeMonitor--) | Ottiene il monitor per tracciare le modifiche causate dall'eliminazione. |
| [getMergedCellsShrinkType()](#getMergedCellsShrinkType--) | Indica come elaborare le celle unite durante l'eliminazione di righe/colonne vuote. |
| [getStartIndex()](#getStartIndex--) | Specifica l'indice di riga/colonna iniziale dell'intervallo da controllare e da cui eliminare righe/colonne vuote. |
| [getUpdateReference()](#getUpdateReference--) | Indica se aggiornare i riferimenti in altri fogli di lavoro. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDrawingsAsBlank(boolean value)](#setDrawingsAsBlank-boolean-) | Indica se gli oggetti correlati al disegno, come immagine, forma, grafico..., saranno considerati vuoti. |
| [setEmptyFormulaValueAsBlank(boolean value)](#setEmptyFormulaValueAsBlank-boolean-) | Indica se una cella verrà considerata vuota quando è una formula e il risultato calcolato è null o una stringa vuota. |
| [setEmptyStringAsBlank(boolean value)](#setEmptyStringAsBlank-boolean-) | Indica se una cella verrà considerata vuota quando il suo valore è una stringa vuota. |
| [setEndIndex(int value)](#setEndIndex-int-) | Specifica l'indice di riga/colonna finale (inclusivo) dell'intervallo da controllare e da cui eliminare righe/colonne vuote. |
| [setFormulaChangeMonitor(AbstractFormulaChangeMonitor value)](#setFormulaChangeMonitor-com.aspose.cells.AbstractFormulaChangeMonitor-) | Imposta il monitor per tracciare le modifiche causate dall'eliminazione. |
| [setMergedCellsShrinkType(int value)](#setMergedCellsShrinkType-int-) | Indica come elaborare le celle unite durante l'eliminazione di righe/colonne vuote. |
| [setStartIndex(int value)](#setStartIndex-int-) | Specifica l'indice di riga/colonna iniziale dell'intervallo da controllare e da cui eliminare righe/colonne vuote. |
| [setUpdateReference(boolean value)](#setUpdateReference-boolean-) | Indica se aggiornare i riferimenti in altri fogli di lavoro. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DeleteBlankOptions() {#DeleteBlankOptions--}
```
public DeleteBlankOptions()
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDrawingsAsBlank() {#getDrawingsAsBlank--}
```
public boolean getDrawingsAsBlank()
```


Indica se gli oggetti correlati al disegno, come immagine, forma, grafico..., saranno considerati vuoti. Il valore predefinito è true.

**Remarks**

Impostando questa proprietà su false, tutte le righe/colonne coperte da oggetti di disegno non saranno considerate vuote e non verranno eliminate.

**Returns:**
boolean
### getEmptyFormulaValueAsBlank() {#getEmptyFormulaValueAsBlank--}
```
public boolean getEmptyFormulaValueAsBlank()
```


Se una cella verrà considerata vuota quando è una formula e il risultato calcolato è nullo o una stringa vuota. Il valore predefinito è false.

**Remarks**

In generale l'utente dovrebbe assicurarsi che le formule siano state calcolate prima dell'operazione di eliminazione con questa proprietà impostata su true. Altrimenti tutte le formule appena create tramite le API normali, come [Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--), saranno considerate vuote e potrebbero essere eliminate perché, prima del calcolo, i loro risultati calcolati sono tutti null.

**Returns:**
boolean
### getEmptyStringAsBlank() {#getEmptyStringAsBlank--}
```
public boolean getEmptyStringAsBlank()
```


Indica se una cella verrà considerata vuota quando il suo valore è una stringa vuota. Il valore predefinito è true.

**Returns:**
boolean
### getEndIndex() {#getEndIndex--}
```
public int getEndIndex()
```


Specifica l'indice finale di riga/colonna (inclusivo) dell'intervallo da controllare ed eliminare righe/colonne vuote. Il valore predefinito è -1 e -1 indica l'intervallo massimo di tutti gli oggetti (celle, disegni, ...) che devono essere controllati.

**Returns:**
int
### getFormulaChangeMonitor() {#getFormulaChangeMonitor--}
```
public AbstractFormulaChangeMonitor getFormulaChangeMonitor()
```


Ottiene il monitor per tracciare le modifiche causate dall'eliminazione.

**Returns:**
[AbstractFormulaChangeMonitor](../../com.aspose.cells/abstractformulachangemonitor)
### getMergedCellsShrinkType() {#getMergedCellsShrinkType--}
```
public int getMergedCellsShrinkType()
```


Indica come elaborare le celle unite durante l'eliminazione di righe/colonne vuote.

Vedi [MergedCellsShrinkType](../../com.aspose.cells/mergedcellsshrinktype).

**Remarks**

Per [MergedCellsShrinkType.KEEP\_HEADER\_ONLY](../../com.aspose.cells/mergedcellsshrinktype\#KEEP-HEADER-ONLY), tutte le celle in esso saranno considerate vuote eccetto la cella in alto a sinistra non vuota. È il valore predefinito di questa proprietà.

Per [MergedCellsShrinkType.NONE](../../com.aspose.cells/mergedcellsshrinktype\#NONE), tutte le celle in esso saranno considerate non vuote.

Per [MergedCellsShrinkType.SHRINK\_TO\_FIT](../../com.aspose.cells/mergedcellsshrinktype\#SHRINK-TO-FIT), tutte le celle al di fuori dell'area di visualizzazione del contenuto saranno considerate vuote.



**Returns:**
int
### getStartIndex() {#getStartIndex--}
```
public int getStartIndex()
```


Specifica l'indice di riga/colonna iniziale dell'intervallo da controllare e da cui eliminare righe/colonne vuote.

**Returns:**
int
### getUpdateReference() {#getUpdateReference--}
```
public boolean getUpdateReference()
```


Indica se aggiornare i riferimenti in altri fogli di lavoro.

**Remarks**

A partire dalla versione 26.7 impostiamo il valore predefinito di questa proprietà su true.

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




### setDrawingsAsBlank(boolean value) {#setDrawingsAsBlank-boolean-}
```
public void setDrawingsAsBlank(boolean value)
```


Indica se gli oggetti correlati al disegno, come immagine, forma, grafico..., saranno considerati vuoti. Il valore predefinito è true.

**Remarks**

Impostando questa proprietà su false, tutte le righe/colonne coperte da oggetti di disegno non saranno considerate vuote e non verranno eliminate.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEmptyFormulaValueAsBlank(boolean value) {#setEmptyFormulaValueAsBlank-boolean-}
```
public void setEmptyFormulaValueAsBlank(boolean value)
```


Se una cella verrà considerata vuota quando è una formula e il risultato calcolato è nullo o una stringa vuota. Il valore predefinito è false.

**Remarks**

In generale l'utente dovrebbe assicurarsi che le formule siano state calcolate prima dell'operazione di eliminazione con questa proprietà impostata su true. Altrimenti tutte le formule appena create tramite le API normali, come [Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--), saranno considerate vuote e potrebbero essere eliminate perché, prima del calcolo, i loro risultati calcolati sono tutti null.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEmptyStringAsBlank(boolean value) {#setEmptyStringAsBlank-boolean-}
```
public void setEmptyStringAsBlank(boolean value)
```


Indica se una cella verrà considerata vuota quando il suo valore è una stringa vuota. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEndIndex(int value) {#setEndIndex-int-}
```
public void setEndIndex(int value)
```


Specifica l'indice finale di riga/colonna (inclusivo) dell'intervallo da controllare ed eliminare righe/colonne vuote. Il valore predefinito è -1 e -1 indica l'intervallo massimo di tutti gli oggetti (celle, disegni, ...) che devono essere controllati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setFormulaChangeMonitor(AbstractFormulaChangeMonitor value) {#setFormulaChangeMonitor-com.aspose.cells.AbstractFormulaChangeMonitor-}
```
public void setFormulaChangeMonitor(AbstractFormulaChangeMonitor value)
```


Imposta il monitor per tracciare le modifiche causate dall'eliminazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [AbstractFormulaChangeMonitor](../../com.aspose.cells/abstractformulachangemonitor) |  |

### setMergedCellsShrinkType(int value) {#setMergedCellsShrinkType-int-}
```
public void setMergedCellsShrinkType(int value)
```


Indica come elaborare le celle unite durante l'eliminazione di righe/colonne vuote.

Vedi [MergedCellsShrinkType](../../com.aspose.cells/mergedcellsshrinktype).

**Remarks**

Per [MergedCellsShrinkType.KEEP\_HEADER\_ONLY](../../com.aspose.cells/mergedcellsshrinktype\#KEEP-HEADER-ONLY), tutte le celle in esso saranno considerate vuote eccetto la cella in alto a sinistra non vuota. È il valore predefinito di questa proprietà.

Per [MergedCellsShrinkType.NONE](../../com.aspose.cells/mergedcellsshrinktype\#NONE), tutte le celle in esso saranno considerate non vuote.

Per [MergedCellsShrinkType.SHRINK\_TO\_FIT](../../com.aspose.cells/mergedcellsshrinktype\#SHRINK-TO-FIT), tutte le celle al di fuori dell'area di visualizzazione del contenuto saranno considerate vuote.



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setStartIndex(int value) {#setStartIndex-int-}
```
public void setStartIndex(int value)
```


Specifica l'indice di riga/colonna iniziale dell'intervallo da controllare e da cui eliminare righe/colonne vuote.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setUpdateReference(boolean value) {#setUpdateReference-boolean-}
```
public void setUpdateReference(boolean value)
```


Indica se aggiornare i riferimenti in altri fogli di lavoro.

**Remarks**

A partire dalla versione 26.7 impostiamo il valore predefinito di questa proprietà su true.

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

