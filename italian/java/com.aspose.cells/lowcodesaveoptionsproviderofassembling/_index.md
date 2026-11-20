---
title: "LowCodeSaveOptionsProviderOfAssembling"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Implementazione per fornire opzioni di salvataggio che salvano le parti suddivise in file e il percorso del file risultante è denominato come può contenere directory SheetIndex o SheetName SplitPartIndex."
type: docs
url: /it/java/com.aspose.cells/lowcodesaveoptionsproviderofassembling/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider)
```
public class LowCodeSaveOptionsProviderOfAssembling extends AbstractLowCodeSaveOptionsProvider
```

Implementazione per fornire opzioni di salvataggio che salvano le parti suddivise in file e il percorso del file risultante è denominato come (può contenere directory): [getPathHeader()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getPathHeader--)+[getSheetPrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSheetPrefix--)+SheetIndex(or SheetName) +[getSplitPartPrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSplitPartPrefix--)+SplitPartIndex+[getPathTail()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getPathTail--).
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [LowCodeSaveOptionsProviderOfAssembling()](#LowCodeSaveOptionsProviderOfAssembling--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finish(LowCodeSaveOptions part)](#finish-com.aspose.cells.LowCodeSaveOptions-) | Rilascia le risorse dopo l'elaborazione della parte divisa corrente. |
| [getBuildPathWithSheetAlways()](#getBuildPathWithSheetAlways--) | Indica se aggiungere sempre l'indice o il nome del foglio al percorso del file. |
| [getBuildPathWithSplitPartAlways()](#getBuildPathWithSplitPartAlways--) | Indica se aggiungere sempre l'indice della parte suddivisa al percorso del file. |
| [getClass()](#getClass--) |  |
| [getPathHeader()](#getPathHeader--) | Parte di intestazione (prima del contenuto aggiunto del foglio e della parte suddivisa) del percorso del file. |
| [getPathTail()](#getPathTail--) | Parte finale (dopo i numeri di sequenza) del percorso del file. |
| [getSaveOptions(SplitPartInfo part)](#getSaveOptions-com.aspose.cells.SplitPartInfo-) | Ottiene le opzioni di salvataggio da cui ricavare le impostazioni di output per la parte divisa corrente. |
| [getSaveOptionsTemplate()](#getSaveOptionsTemplate--) | Il modello per creare un'istanza di opzioni di salvataggio in [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSaveOptions-SplitPartInfo-). |
| [getSheetIndexOffset()](#getSheetIndexOffset--) | Scostamento dell'indice del foglio tra quello usato nel percorso del file e il suo valore reale ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)). |
| [getSheetPrefix()](#getSheetPrefix--) | Prefisso per l'indice del foglio di lavoro. |
| [getSplitPartIndexOffset()](#getSplitPartIndexOffset--) | Scostamento dell'indice della parte divisa tra quello usato nel percorso file e il suo valore reale ([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)). |
| [getSplitPartPrefix()](#getSplitPartPrefix--) | Prefisso per l'indice della parte divisa. |
| [getUseSheetName()](#getUseSheetName--) | Indica se costruire il percorso file con il nome del foglio invece dell'indice del foglio. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBuildPathWithSheetAlways(boolean value)](#setBuildPathWithSheetAlways-boolean-) | Indica se aggiungere sempre l'indice o il nome del foglio al percorso del file. |
| [setBuildPathWithSplitPartAlways(boolean value)](#setBuildPathWithSplitPartAlways-boolean-) | Indica se aggiungere sempre l'indice della parte suddivisa al percorso del file. |
| [setPathHeader(String value)](#setPathHeader-java.lang.String-) | Parte di intestazione (prima del contenuto aggiunto del foglio e della parte suddivisa) del percorso del file. |
| [setPathTail(String value)](#setPathTail-java.lang.String-) | Parte finale (dopo i numeri di sequenza) del percorso del file. |
| [setSaveOptionsTemplate(LowCodeSaveOptions value)](#setSaveOptionsTemplate-com.aspose.cells.LowCodeSaveOptions-) | Il modello per creare un'istanza di opzioni di salvataggio in [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSaveOptions-SplitPartInfo-). |
| [setSheetIndexOffset(int value)](#setSheetIndexOffset-int-) | Scostamento dell'indice del foglio tra quello usato nel percorso del file e il suo valore reale ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)). |
| [setSheetPrefix(String value)](#setSheetPrefix-java.lang.String-) | Prefisso per l'indice del foglio di lavoro. |
| [setSplitPartIndexOffset(int value)](#setSplitPartIndexOffset-int-) | Scostamento dell'indice della parte divisa tra quello usato nel percorso file e il suo valore reale ([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)). |
| [setSplitPartPrefix(String value)](#setSplitPartPrefix-java.lang.String-) | Prefisso per l'indice della parte divisa. |
| [setUseSheetName(boolean value)](#setUseSheetName-boolean-) | Indica se costruire il percorso file con il nome del foglio invece dell'indice del foglio. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeSaveOptionsProviderOfAssembling() {#LowCodeSaveOptionsProviderOfAssembling--}
```
public LowCodeSaveOptionsProviderOfAssembling()
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


Indica se aggiungere sempre l'indice o il nome del foglio al percorso file. Il valore predefinito è false, cioè quando c'è un solo foglio, l'indice (o il nome) del foglio e il prefisso corrispondente non verranno aggiunti al percorso file.

**Returns:**
boolean
### getBuildPathWithSplitPartAlways() {#getBuildPathWithSplitPartAlways--}
```
public boolean getBuildPathWithSplitPartAlways()
```


Indica se aggiungere sempre l'indice della parte divisa al percorso file. Il valore predefinito è false, cioè quando c'è una sola parte divisa, l'indice della parte divisa e il prefisso corrispondente non verranno aggiunti al percorso file.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getPathHeader() {#getPathHeader--}
```
public String getPathHeader()
```


Parte di intestazione (prima del contenuto aggiunto del foglio e della parte suddivisa) del percorso del file.

**Returns:**
java.lang.String
### getPathTail() {#getPathTail--}
```
public String getPathTail()
```


Parte finale (dopo i numeri di sequenza) del percorso file. Deve includere l'estensione del nome file.

**Returns:**
java.lang.String
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


Il modello per creare un'istanza di opzioni di salvataggio in [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSaveOptions-SplitPartInfo-).

**Remarks**

Se è stato specificato il modello, l'istanza creata copierà tutte le impostazioni da esso e aggiornerà il file di output di conseguenza.

**Returns:**
[LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
### getSheetIndexOffset() {#getSheetIndexOffset--}
```
public int getSheetIndexOffset()
```


Scostamento dell'indice del foglio tra quello usato nel percorso del file e il suo valore reale ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)).

**Remarks**

Ha effetto solo quando [getUseSheetName()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getUseSheetName--) è false.

**Returns:**
int
### getSheetPrefix() {#getSheetPrefix--}
```
public String getSheetPrefix()
```


Prefisso per l'indice del foglio di lavoro.

**Remarks**

Se c'è un solo foglio di lavoro e [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSheetAlways--) è false, allora questo prefisso e l'indice (o il nome) del foglio non verranno aggiunti al percorso file risultante.

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

Se c'è una sola parte divisa e [getBuildPathWithSplitPartAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSplitPartAlways--) è false, allora questo prefisso e l'indice della parte divisa (0) non verranno aggiunti al percorso file risultante.

**Returns:**
java.lang.String
### getUseSheetName() {#getUseSheetName--}
```
public boolean getUseSheetName()
```


Indica se costruire il percorso file con il nome del foglio invece dell'indice del foglio. Il valore predefinito è false.

**Remarks**

Il nome del foglio non verrà mai ricostruito automaticamente. Quindi, quando lo si imposta su true, assicurarsi che non ci siano nomi di foglio speciali che possano causare percorsi o nomi di file non validi.

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




### setBuildPathWithSheetAlways(boolean value) {#setBuildPathWithSheetAlways-boolean-}
```
public void setBuildPathWithSheetAlways(boolean value)
```


Indica se aggiungere sempre l'indice o il nome del foglio al percorso file. Il valore predefinito è false, cioè quando c'è un solo foglio, l'indice (o il nome) del foglio e il prefisso corrispondente non verranno aggiunti al percorso file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setBuildPathWithSplitPartAlways(boolean value) {#setBuildPathWithSplitPartAlways-boolean-}
```
public void setBuildPathWithSplitPartAlways(boolean value)
```


Indica se aggiungere sempre l'indice della parte divisa al percorso file. Il valore predefinito è false, cioè quando c'è una sola parte divisa, l'indice della parte divisa e il prefisso corrispondente non verranno aggiunti al percorso file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setPathHeader(String value) {#setPathHeader-java.lang.String-}
```
public void setPathHeader(String value)
```


Parte di intestazione (prima del contenuto aggiunto del foglio e della parte suddivisa) del percorso del file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setPathTail(String value) {#setPathTail-java.lang.String-}
```
public void setPathTail(String value)
```


Parte finale (dopo i numeri di sequenza) del percorso file. Deve includere l'estensione del nome file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setSaveOptionsTemplate(LowCodeSaveOptions value) {#setSaveOptionsTemplate-com.aspose.cells.LowCodeSaveOptions-}
```
public void setSaveOptionsTemplate(LowCodeSaveOptions value)
```


Il modello per creare un'istanza di opzioni di salvataggio in [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSaveOptions-SplitPartInfo-).

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

**Remarks**

Ha effetto solo quando [getUseSheetName()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getUseSheetName--) è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setSheetPrefix(String value) {#setSheetPrefix-java.lang.String-}
```
public void setSheetPrefix(String value)
```


Prefisso per l'indice del foglio di lavoro.

**Remarks**

Se c'è un solo foglio di lavoro e [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSheetAlways--) è false, allora questo prefisso e l'indice (o il nome) del foglio non verranno aggiunti al percorso file risultante.

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

Se c'è una sola parte divisa e [getBuildPathWithSplitPartAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSplitPartAlways--) è false, allora questo prefisso e l'indice della parte divisa (0) non verranno aggiunti al percorso file risultante.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setUseSheetName(boolean value) {#setUseSheetName-boolean-}
```
public void setUseSheetName(boolean value)
```


Indica se costruire il percorso file con il nome del foglio invece dell'indice del foglio. Il valore predefinito è false.

**Remarks**

Il nome del foglio non verrà mai ricostruito automaticamente. Quindi, quando lo si imposta su true, assicurarsi che non ci siano nomi di foglio speciali che possano causare percorsi o nomi di file non validi.

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

