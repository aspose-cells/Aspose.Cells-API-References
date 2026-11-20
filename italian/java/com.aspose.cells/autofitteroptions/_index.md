---
title: "AutoFitterOptions"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta tutte le opzioni di adattamento automatico."
type: docs
url: /it/java/com.aspose.cells/autofitteroptions/
---

**Inheritance:**
java.lang.Object
```
public class AutoFitterOptions
```

Rappresenta tutte le opzioni di adattamento automatico.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [AutoFitterOptions()](#AutoFitterOptions--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFitMergedCells()](#getAutoFitMergedCells--) | Indica se adattare automaticamente l'altezza della riga quando le celle sono unite in una riga. |
| [getAutoFitMergedCellsType()](#getAutoFitMergedCellsType--) | Restituisce il tipo di adattamento automatico dell'altezza della riga per le celle unite. |
| [getAutoFitWrappedTextType()](#getAutoFitWrappedTextType--) | Restituisce il tipo di adattamento automatico del testo a capo. |
| [getClass()](#getClass--) |  |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | Restituisce la lingua di modifica predefinita. |
| [getForRendering()](#getForRendering--) | Indica se adattare per scopi di rendering. |
| [getFormatStrategy()](#getFormatStrategy--) | Restituisce la strategia di formattazione. |
| [getIgnoreHidden()](#getIgnoreHidden--) | Ignora le righe/colonne nascoste. |
| [getMaxRowHeight()](#getMaxRowHeight--) | Restituisce l'altezza massima della riga (in unità di Point) durante l'adattamento automatico delle righe. |
| [getOnlyAuto()](#getOnlyAuto--) | Indica se adattare solo le righe la cui altezza non è personalizzata. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFitMergedCells(boolean value)](#setAutoFitMergedCells-boolean-) | Indica se adattare automaticamente l'altezza della riga quando le celle sono unite in una riga. |
| [setAutoFitMergedCellsType(int value)](#setAutoFitMergedCellsType-int-) | Imposta il tipo di adattamento automatico dell'altezza delle righe delle celle unite. |
| [setAutoFitWrappedTextType(int value)](#setAutoFitWrappedTextType-int-) | Imposta il tipo di adattamento automatico del testo a capo. |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) | Imposta la lingua di modifica predefinita. |
| [setForRendering(boolean value)](#setForRendering-boolean-) | Indica se adattare per scopi di rendering. |
| [setFormatStrategy(int value)](#setFormatStrategy-int-) | Imposta la strategia di formattazione. |
| [setIgnoreHidden(boolean value)](#setIgnoreHidden-boolean-) | Ignora le righe/colonne nascoste. |
| [setMaxRowHeight(double value)](#setMaxRowHeight-double-) | Imposta l'altezza massima della riga (in unità di Point) durante l'adattamento automatico delle righe. |
| [setOnlyAuto(boolean value)](#setOnlyAuto-boolean-) | Indica se adattare solo le righe la cui altezza non è personalizzata. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AutoFitterOptions() {#AutoFitterOptions--}
```
public AutoFitterOptions()
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
### getAutoFitMergedCells() {#getAutoFitMergedCells--}
```
public boolean getAutoFitMergedCells()
```


Indica se adattare automaticamente l'altezza della riga quando le celle sono unite in una riga. Il valore predefinito è false.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà AutoFitterOptions.AutoFitMergedCellsType. Questa proprietà sarà rimossa 12 mesi dopo, a partire da dicembre 2018. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Returns:**
boolean
### getAutoFitMergedCellsType() {#getAutoFitMergedCellsType--}
```
public int getAutoFitMergedCellsType()
```


Restituisce il tipo di adattamento automatico dell'altezza della riga per le celle unite.

Vedi [AutoFitMergedCellsType](../../com.aspose.cells/autofitmergedcellstype).

**Remarks**

Excel ignora per impostazione predefinita le celle unite quando adatta l'altezza della riga, quindi Aspose.Cells funziona come il valore predefinito di MS Excel. Si prega di impostare questo tipo per modificare il modo di adattamento automatico dell'altezza delle righe delle celle unite.

**Returns:**
int
### getAutoFitWrappedTextType() {#getAutoFitWrappedTextType--}
```
public int getAutoFitWrappedTextType()
```


Restituisce il tipo di adattamento automatico del testo a capo.

Vedi [AutoFitWrappedTextType](../../com.aspose.cells/autofitwrappedtexttype).

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDefaultEditLanguage() {#getDefaultEditLanguage--}
```
public int getDefaultEditLanguage()
```


Restituisce la lingua di modifica predefinita.

Vedi [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

Può visualizzare/renderizzare layout diversi per i paragrafi di testo quando sono impostate lingue di modifica differenti. Il valore predefinito è [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO).

**Returns:**
int
### getForRendering() {#getForRendering--}
```
public boolean getForRendering()
```


Indica se adattare per scopi di rendering.

**Returns:**
boolean
### getFormatStrategy() {#getFormatStrategy--}
```
public int getFormatStrategy()
```


Restituisce la strategia di formattazione.

Vedi [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Remarks**

Il valore predefinito è CellStyle per le prestazioni.

**Returns:**
int
### getIgnoreHidden() {#getIgnoreHidden--}
```
public boolean getIgnoreHidden()
```


Ignora le righe/colonne nascoste.

**Returns:**
boolean
### getMaxRowHeight() {#getMaxRowHeight--}
```
public double getMaxRowHeight()
```


Restituisce l'altezza massima della riga (in unità di Point) durante l'adattamento automatico delle righe.

**Returns:**
double
### getOnlyAuto() {#getOnlyAuto--}
```
public boolean getOnlyAuto()
```


Indica se adattare solo le righe la cui altezza non è personalizzata.

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




### setAutoFitMergedCells(boolean value) {#setAutoFitMergedCells-boolean-}
```
public void setAutoFitMergedCells(boolean value)
```


Indica se adattare automaticamente l'altezza della riga quando le celle sono unite in una riga. Il valore predefinito è false.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà AutoFitterOptions.AutoFitMergedCellsType. Questa proprietà sarà rimossa 12 mesi dopo, a partire da dicembre 2018. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAutoFitMergedCellsType(int value) {#setAutoFitMergedCellsType-int-}
```
public void setAutoFitMergedCellsType(int value)
```


Imposta il tipo di adattamento automatico dell'altezza delle righe delle celle unite.

Vedi [AutoFitMergedCellsType](../../com.aspose.cells/autofitmergedcellstype).

**Remarks**

Excel ignora per impostazione predefinita le celle unite quando adatta l'altezza della riga, quindi Aspose.Cells funziona come il valore predefinito di MS Excel. Si prega di impostare questo tipo per modificare il modo di adattamento automatico dell'altezza delle righe delle celle unite.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setAutoFitWrappedTextType(int value) {#setAutoFitWrappedTextType-int-}
```
public void setAutoFitWrappedTextType(int value)
```


Imposta il tipo di adattamento automatico del testo a capo.

Vedi [AutoFitWrappedTextType](../../com.aspose.cells/autofitwrappedtexttype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setDefaultEditLanguage(int value) {#setDefaultEditLanguage-int-}
```
public void setDefaultEditLanguage(int value)
```


Imposta la lingua di modifica predefinita.

Vedi [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

Può visualizzare/renderizzare layout diversi per i paragrafi di testo quando sono impostate lingue di modifica differenti. Il valore predefinito è [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setForRendering(boolean value) {#setForRendering-boolean-}
```
public void setForRendering(boolean value)
```


Indica se adattare per scopi di rendering.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setFormatStrategy(int value) {#setFormatStrategy-int-}
```
public void setFormatStrategy(int value)
```


Imposta la strategia di formattazione.

Vedi [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Remarks**

Il valore predefinito è CellStyle per le prestazioni.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setIgnoreHidden(boolean value) {#setIgnoreHidden-boolean-}
```
public void setIgnoreHidden(boolean value)
```


Ignora le righe/colonne nascoste.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setMaxRowHeight(double value) {#setMaxRowHeight-double-}
```
public void setMaxRowHeight(double value)
```


Imposta l'altezza massima della riga (in unità di Point) durante l'adattamento automatico delle righe.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setOnlyAuto(boolean value) {#setOnlyAuto-boolean-}
```
public void setOnlyAuto(boolean value)
```


Indica se adattare solo le righe la cui altezza non è personalizzata.

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

