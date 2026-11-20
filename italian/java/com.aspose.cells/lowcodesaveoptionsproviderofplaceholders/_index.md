---
title: "LowCodeSaveOptionsProviderOfPlaceHolders"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Implementazione per fornire opzioni di salvataggio che salvano le parti suddivise in file e il percorso del file risultante è definito con segnaposti."
type: docs
url: /it/java/com.aspose.cells/lowcodesaveoptionsproviderofplaceholders/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider)
```
public class LowCodeSaveOptionsProviderOfPlaceHolders extends AbstractLowCodeSaveOptionsProvider
```

Implementazione per fornire opzioni di salvataggio che salvano le parti suddivise in file e il percorso del file risultante è definito con segnaposti.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [LowCodeSaveOptionsProviderOfPlaceHolders(String pathTemplate)](#LowCodeSaveOptionsProviderOfPlaceHolders-java.lang.String-) | Istanzia un'istanza per fornire le opzioni di salvataggio in base ai modelli specificati. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finish(LowCodeSaveOptions part)](#finish-com.aspose.cells.LowCodeSaveOptions-) | Rilascia le risorse dopo l'elaborazione della parte divisa corrente. |
| [getBuildPathWithSheetAlways()](#getBuildPathWithSheetAlways--) | Indica se aggiungere sempre l'indice o il nome del foglio al percorso del file. |
| [getBuildPathWithSplitPartAlways()](#getBuildPathWithSplitPartAlways--) | Indica se aggiungere sempre l'indice della parte suddivisa al percorso del file. |
| [getClass()](#getClass--) |  |
| [getSaveOptions(SplitPartInfo part)](#getSaveOptions-com.aspose.cells.SplitPartInfo-) | Ottiene le opzioni di salvataggio da cui ricavare le impostazioni di output per la parte divisa corrente. |
| [getSaveOptionsTemplate()](#getSaveOptionsTemplate--) | Il modello per creare un'istanza di opzioni di salvataggio in [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSaveOptions-SplitPartInfo-). |
| [getSheetIndexOffset()](#getSheetIndexOffset--) | Scostamento dell'indice del foglio tra quello usato nel percorso del file e il suo valore reale ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)). |
| [getSheetIndexPrefix()](#getSheetIndexPrefix--) | Prefisso per l'indice del foglio di lavoro. |
| [getSheetNamePrefix()](#getSheetNamePrefix--) | Prefisso per l'indice del foglio di lavoro. |
| [getSplitPartIndexOffset()](#getSplitPartIndexOffset--) | Scostamento dell'indice della parte divisa tra quello usato nel percorso file e il suo valore reale ([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)). |
| [getSplitPartPrefix()](#getSplitPartPrefix--) | Prefisso per l'indice della parte divisa. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBuildPathWithSheetAlways(boolean value)](#setBuildPathWithSheetAlways-boolean-) | Indica se aggiungere sempre l'indice o il nome del foglio al percorso del file. |
| [setBuildPathWithSplitPartAlways(boolean value)](#setBuildPathWithSplitPartAlways-boolean-) | Indica se aggiungere sempre l'indice della parte suddivisa al percorso del file. |
| [setSaveOptionsTemplate(LowCodeSaveOptions value)](#setSaveOptionsTemplate-com.aspose.cells.LowCodeSaveOptions-) | Il modello per creare un'istanza di opzioni di salvataggio in [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSaveOptions-SplitPartInfo-). |
| [setSheetIndexOffset(int value)](#setSheetIndexOffset-int-) | Scostamento dell'indice del foglio tra quello usato nel percorso del file e il suo valore reale ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)). |
| [setSheetIndexPrefix(String value)](#setSheetIndexPrefix-java.lang.String-) | Prefisso per l'indice del foglio di lavoro. |
| [setSheetNamePrefix(String value)](#setSheetNamePrefix-java.lang.String-) | Prefisso per l'indice del foglio di lavoro. |
| [setSplitPartIndexOffset(int value)](#setSplitPartIndexOffset-int-) | Scostamento dell'indice della parte divisa tra quello usato nel percorso file e il suo valore reale ([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)). |
| [setSplitPartPrefix(String value)](#setSplitPartPrefix-java.lang.String-) | Prefisso per l'indice della parte divisa. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeSaveOptionsProviderOfPlaceHolders(String pathTemplate) {#LowCodeSaveOptionsProviderOfPlaceHolders-java.lang.String-}
```
public LowCodeSaveOptionsProviderOfPlaceHolders(String pathTemplate)
```


Istanzia un'istanza per fornire le opzioni di salvataggio in base ai modelli specificati.

**Remarks**

I segnaposto supportati nel modello di percorso file:

 *  $\{SheetIndex\}: will be replaced by the sheet index of the split part
 *  $\{SheetName\}: will be replaced by the sheet name of the split part
 *  $\{SplitPartIndex\}: will be replaced by the index of the split part
 *  $\{SheetIndexPrefix\}: will be replaced by
 *  $\{SheetNamePrefix\}: will be replaced by
 *  $\{SplitPartPrefix\}: will be replaced by

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pathTemplate | java.lang.String | Il modello del percorso file risultante. |

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
### finish(LowCodeSaveOptions part) {#finish-com.aspose.cells.LowCodeSaveOptions-}
```
public void finish(LowCodeSaveOptions part)
```


Rilascia le risorse dopo l'elaborazione della parte divisa corrente.

**Remarks**

Per impostazione predefinita, questo metodo chiude semplicemente lo stream specificato da [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--) direttamente (se le opzioni di salvataggio hanno specificato uno Stream come destinazione). L'utente può sovrascrivere questo metodo per controllare come rilasciare le risorse in base alle proprie esigenze e all'implementazione di [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/abstractlowcodesaveoptionsprovider\#getSaveOptions-SplitPartInfo-).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| part | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | le opzioni di salvataggio utilizzate per la parte divisa corrente. |

### getBuildPathWithSheetAlways() {#getBuildPathWithSheetAlways--}
```
public boolean getBuildPathWithSheetAlways()
```


Indica se aggiungere sempre l'indice o il nome del foglio al percorso file. Il valore predefinito è false, cioè quando c'è un solo foglio, l'indice e il nome del foglio e il prefisso corrispondente ([getSheetNamePrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSheetNamePrefix--)) non verranno aggiunti al percorso file.

**Returns:**
boolean
### getBuildPathWithSplitPartAlways() {#getBuildPathWithSplitPartAlways--}
```
public boolean getBuildPathWithSplitPartAlways()
```


Indica se aggiungere sempre l'indice della parte di divisione al percorso file. Il valore predefinito è false, cioè quando c'è una sola parte di divisione, l'indice della parte di divisione e il prefisso corrispondente ([getSplitPartPrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSplitPartPrefix--)) non verranno aggiunti al percorso file.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getSaveOptions(SplitPartInfo part) {#getSaveOptions-com.aspose.cells.SplitPartInfo-}
```
public LowCodeSaveOptions getSaveOptions(SplitPartInfo part)
```


Ottiene le opzioni di salvataggio da cui ricavare le impostazioni di output per la parte divisa corrente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| part | [SplitPartInfo](../../com.aspose.cells/splitpartinfo) |  |

**Returns:**
[LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
### getSaveOptionsTemplate() {#getSaveOptionsTemplate--}
```
public LowCodeSaveOptions getSaveOptionsTemplate()
```


Il modello per creare un'istanza di opzioni di salvataggio in [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSaveOptions-SplitPartInfo-).

**Remarks**

Se è stato specificato il modello, l'istanza creata copierà tutte le impostazioni da esso e aggiornerà il file di output di conseguenza.

**Returns:**
[LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
### getSheetIndexOffset() {#getSheetIndexOffset--}
```
public int getSheetIndexOffset()
```


Scostamento dell'indice del foglio tra quello usato nel percorso del file e il suo valore reale ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)).

**Returns:**
int
### getSheetIndexPrefix() {#getSheetIndexPrefix--}
```
public String getSheetIndexPrefix()
```


Prefisso per l'indice del foglio di lavoro.

**Remarks**

Se c'è un solo foglio di lavoro e [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSheetAlways--) è false, allora questo prefisso e l'indice (o nome) del foglio non verranno aggiunti al percorso file risultante.

**Returns:**
java.lang.String
### getSheetNamePrefix() {#getSheetNamePrefix--}
```
public String getSheetNamePrefix()
```


Prefisso per l'indice del foglio di lavoro.

**Remarks**

Se c'è un solo foglio di lavoro e [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSheetAlways--) è false, allora questo prefisso e l'indice (o nome) del foglio non verranno aggiunti al percorso file risultante.

**Returns:**
java.lang.String
### getSplitPartIndexOffset() {#getSplitPartIndexOffset--}
```
public int getSplitPartIndexOffset()
```


Scostamento dell'indice della parte divisa tra quello usato nel percorso file e il suo valore reale ([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)).

**Returns:**
int
### getSplitPartPrefix() {#getSplitPartPrefix--}
```
public String getSplitPartPrefix()
```


Prefisso per l'indice della parte divisa.

**Remarks**

Se c'è una sola parte di divisione e [getBuildPathWithSplitPartAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSplitPartAlways--) è false, allora questo prefisso e l'indice della parte di divisione (0) non verranno aggiunti al percorso file risultante.

**Returns:**
java.lang.String
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




### setBuildPathWithSheetAlways(boolean value) {#setBuildPathWithSheetAlways-boolean-}
```
public void setBuildPathWithSheetAlways(boolean value)
```


Indica se aggiungere sempre l'indice o il nome del foglio al percorso file. Il valore predefinito è false, cioè quando c'è un solo foglio, l'indice e il nome del foglio e il prefisso corrispondente ([getSheetNamePrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSheetNamePrefix--)) non verranno aggiunti al percorso file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setBuildPathWithSplitPartAlways(boolean value) {#setBuildPathWithSplitPartAlways-boolean-}
```
public void setBuildPathWithSplitPartAlways(boolean value)
```


Indica se aggiungere sempre l'indice della parte di divisione al percorso file. Il valore predefinito è false, cioè quando c'è una sola parte di divisione, l'indice della parte di divisione e il prefisso corrispondente ([getSplitPartPrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSplitPartPrefix--)) non verranno aggiunti al percorso file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSaveOptionsTemplate(LowCodeSaveOptions value) {#setSaveOptionsTemplate-com.aspose.cells.LowCodeSaveOptions-}
```
public void setSaveOptionsTemplate(LowCodeSaveOptions value)
```


Il modello per creare un'istanza di opzioni di salvataggio in [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSaveOptions-SplitPartInfo-).

**Remarks**

Se è stato specificato il modello, l'istanza creata copierà tutte le impostazioni da esso e aggiornerà il file di output di conseguenza.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) |  |

### setSheetIndexOffset(int value) {#setSheetIndexOffset-int-}
```
public void setSheetIndexOffset(int value)
```


Scostamento dell'indice del foglio tra quello usato nel percorso del file e il suo valore reale ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setSheetIndexPrefix(String value) {#setSheetIndexPrefix-java.lang.String-}
```
public void setSheetIndexPrefix(String value)
```


Prefisso per l'indice del foglio di lavoro.

**Remarks**

Se c'è un solo foglio di lavoro e [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSheetAlways--) è false, allora questo prefisso e l'indice (o nome) del foglio non verranno aggiunti al percorso file risultante.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setSheetNamePrefix(String value) {#setSheetNamePrefix-java.lang.String-}
```
public void setSheetNamePrefix(String value)
```


Prefisso per l'indice del foglio di lavoro.

**Remarks**

Se c'è un solo foglio di lavoro e [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSheetAlways--) è false, allora questo prefisso e l'indice (o nome) del foglio non verranno aggiunti al percorso file risultante.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setSplitPartIndexOffset(int value) {#setSplitPartIndexOffset-int-}
```
public void setSplitPartIndexOffset(int value)
```


Scostamento dell'indice della parte divisa tra quello usato nel percorso file e il suo valore reale ([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setSplitPartPrefix(String value) {#setSplitPartPrefix-java.lang.String-}
```
public void setSplitPartPrefix(String value)
```


Prefisso per l'indice della parte divisa.

**Remarks**

Se c'è una sola parte di divisione e [getBuildPathWithSplitPartAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSplitPartAlways--) è false, allora questo prefisso e l'indice della parte di divisione (0) non verranno aggiunti al percorso file risultante.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

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

