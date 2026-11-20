---
title: "LoadFilter"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta il filtro che fornisce opzioni per il caricamento dei dati quando si carica la cartella di lavoro da un modello."
type: docs
url: /it/java/com.aspose.cells/loadfilter/
---

**Inheritance:**
java.lang.Object
```
public class LoadFilter
```

Rappresenta il filtro che fornisce opzioni per il caricamento dei dati quando si carica la cartella di lavoro da un modello.

**Remarks**

L'utente può specificare le opzioni di filtro o implementare il proprio LoadFilter per indicare come caricare i dati.

**Example**

Il seguente esempio mostra come determinare le opzioni di filtro in base alle proprietà del foglio di lavoro.

```
         class LoadFilterSheet extends LoadFilter
         {
             public /*override*/ void startSheet(Worksheet sheet) 
             {
                 if ("Sheet1".equals(sheet.getName()))
                 {
                     setLoadDataFilterOptions(LoadDataFilterOptions.ALL);
                 }
                 else
                 {
                     setLoadDataFilterOptions(LoadDataFilterOptions.STRUCTURE);
                 }
             }
         }
         LoadOptions opts = new LoadOptions();
         opts.setLoadFilter(new LoadFilterSheet());
         Workbook wb = new Workbook("template.xlsx", opts);
         //Custom LoadFilter implementation
```
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [LoadFilter()](#LoadFilter--) | Crea un LoadFilter con le opzioni di filtro predefinite LoadDataFilterOptions.All. |
| [LoadFilter(int opts)](#LoadFilter-int-) | Crea un LoadFilter con le opzioni di filtro fornite. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getLoadDataFilterOptions()](#getLoadDataFilterOptions--) | Le opzioni di filtro per indicare quali dati devono essere caricati. |
| [getSheetsInLoadingOrder()](#getSheetsInLoadingOrder--) | Specifica i fogli (indici) e l'ordine da caricare. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setLoadDataFilterOptions(int value)](#setLoadDataFilterOptions-int-) | Le opzioni di filtro per indicare quali dati devono essere caricati. |
| [startSheet(Worksheet sheet)](#startSheet-com.aspose.cells.Worksheet-) | Prepara le opzioni di filtro prima di caricare il foglio di lavoro specificato. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LoadFilter() {#LoadFilter--}
```
public LoadFilter()
```


Crea un LoadFilter con le opzioni di filtro predefinite LoadDataFilterOptions.All.

### LoadFilter(int opts) {#LoadFilter-int-}
```
public LoadFilter(int opts)
```


Crea un LoadFilter con le opzioni di filtro fornite.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| opts | int | [LoadDataFilterOptions](../../com.aspose.cells/loaddatafilteroptions). le opzioni di filtro predefinite |

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
### getLoadDataFilterOptions() {#getLoadDataFilterOptions--}
```
public int getLoadDataFilterOptions()
```


Le opzioni di filtro per indicare quali dati devono essere caricati.

Vedi [LoadDataFilterOptions](../../com.aspose.cells/loaddatafilteroptions).

**Returns:**
int
### getSheetsInLoadingOrder() {#getSheetsInLoadingOrder--}
```
public int[] getSheetsInLoadingOrder()
```


Specifica i fogli (indici) e l'ordine da caricare. Il valore predefinito è null, il che indica di caricare tutti i fogli nell'ordine predefinito nel file modello. Se non è null e l'indice di qualche foglio non è presente nell'array restituito, quel foglio non verrà caricato.

**Returns:**
int[]
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




### setLoadDataFilterOptions(int value) {#setLoadDataFilterOptions-int-}
```
public void setLoadDataFilterOptions(int value)
```


Le opzioni di filtro per indicare quali dati devono essere caricati.

Vedi [LoadDataFilterOptions](../../com.aspose.cells/loaddatafilteroptions).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### startSheet(Worksheet sheet) {#startSheet-com.aspose.cells.Worksheet-}
```
public void startSheet(Worksheet sheet)
```


Prepara le opzioni di filtro prima di caricare il foglio di lavoro specificato. L'implementazione dell'utente di LoadFilter può modificare qui le LoadDataFilterOptions per indicare come caricare i dati per questo foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheet | [Worksheet](../../com.aspose.cells/worksheet) | Il foglio di lavoro da caricare. Qui sono disponibili solo poche proprietà per l'oggetto foglio di lavoro fornito, poiché la maggior parte dei dati e delle proprietà non è stata caricata. Le proprietà disponibili sono: Name, Index, VisibilityType |

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

