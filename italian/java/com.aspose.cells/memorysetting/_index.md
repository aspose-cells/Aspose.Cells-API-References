---
title: "MemorySetting"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Modalità di utilizzo della memoria per il modello dati delle celle."
type: docs
url: /it/java/com.aspose.cells/memorysetting/
---

**Inheritance:**
java.lang.Object
```
public final class MemorySetting
```

Modalità di utilizzo della memoria per il modello dati delle celle.
## Campi

| Campo | Descrizione |
| --- | --- |
| [FILE_CACHE](#FILE-CACHE) | Preferibile la prestazione della memoria e l'uso di file invece della memoria per mantenere i dati delle celle. |
| [MEMORY_PREFERENCE](#MEMORY-PREFERENCE) | Prestazione della memoria preferibile. |
| [NORMAL](#NORMAL) | Modalità predefinita per il modello di celle. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### FILE_CACHE {#FILE-CACHE}
```
public static final int FILE_CACHE
```


Preferibile la prestazione della memoria e l'uso di file invece della memoria per mantenere i dati delle celle.

**Remarks**

Con questa modalità i dati delle celle verranno mantenuti in formato compatto e la parte principale dei dati sarà mantenuta in un file temporaneo invece della memoria. Quindi, confrontandola con la modalità [MEMORY\_PREFERENCE](../../com.aspose.cells/memorysetting\#MEMORY-PREFERENCE), questa modalità può ridurre ulteriormente il consumo di memoria, ma le operazioni di I/O per accedere ai dati delle celle comporteranno anche un costo temporale più elevato.

Questa opzione è disponibile dalla versione v25.7.0.

| Alcuni limiti notevoli e operazioni consigliate quando si utilizza questa modalità: |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Quando questa modalità è usata per qualsiasi foglio di lavoro in una cartella di lavoro, [Workbook.dispose()](../../com.aspose.cells/workbook\#dispose--) dovrebbe essere chiamato alla fine del lavoro per rilasciare tutte le risorse, come i file temporanei. |
| L'accesso casuale alle celle comporta scarse prestazioni perché i dati devono essere letti in modo casuale e ripetuto (quindi il puntatore nel file verrà modificato di conseguenza e le operazioni di I/O saranno richieste ripetutamente). Se possibile, accedi sempre ai dati in modo sequenziale (riga per riga). |
| Quando i dati di una riga/cella vengono modificati, i dati delle altre celle/righe possono essere influenzati (ad esempio i dati vengono spostati in altre posizioni per allocare spazio sufficiente per i dati modificati). Pertanto ogni modifica di qualsiasi dato richiede la sincronizzazione degli altri oggetti esistenti (come l'oggetto Row o Cell). Per ottenere migliori prestazioni, evita di mantenere più righe/celle contemporaneamente. Elaborarle una alla volta ridurrà la sincronizzazione dei dati, migliorando le prestazioni. |

### MEMORY_PREFERENCE {#MEMORY-PREFERENCE}
```
public static final int MEMORY_PREFERENCE
```


Prestazione della memoria preferibile.

**Remarks**

Con questa modalità i dati delle celle verranno mantenuti in formato compatto per ridurre il consumo di memoria. D'altra parte, i dati compatti possono anche comportare un costo temporale più elevato, soprattutto durante l'aggiornamento dei dati delle celle o l'accesso casuale.

Questa opzione è disponibile dalla versione v8.0.0.

### NORMAL {#NORMAL}
```
public static final int NORMAL
```


Modalità predefinita per il modello di celle.

**Remarks**

Questa modalità è applicata a tutte le versioni.

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

