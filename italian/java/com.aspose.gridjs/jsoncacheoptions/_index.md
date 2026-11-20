---
title: "JsonCacheOptions"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Opzioni di configurazione per la cache JSON in GridJs."
type: docs
url: /it/java/com.aspose.gridjs/jsoncacheoptions/
---

**Inheritance:**
java.lang.Object
```
public class JsonCacheOptions
```

Opzioni di configurazione per la cache JSON in GridJs. Controlla sia il comportamento della cache in memoria (L1) che su disco (L2).
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [JsonCacheOptions()](#JsonCacheOptions--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCompressDisk()](#getCompressDisk--) | Restituisce se comprimere la cache su disco usando Gzip (predefinito: true). |
| [getDiskPath()](#getDiskPath--) | Restituisce il percorso della directory della cache su disco. |
| [getDiskTtl()](#getDiskTtl--) | Restituisce il TTL per la cache su disco, in minuti (predefinito: 1440). |
| [getEnable()](#getEnable--) | Restituisce se abilitare la cache JSON per una risposta più veloce. |
| [getEnableDisk()](#getEnableDisk--) | Restituisce se abilitare la cache su disco (predefinito: true). |
| [getImplementation()](#getImplementation--) | Restituisce l'implementazione personalizzata della cache JSON. |
| [getMaxDiskSizeMB()](#getMaxDiskSizeMB--) | Restituisce la dimensione massima della cache su disco in MB (predefinito: 500 MB). |
| [getMaxMemoryEntries()](#getMaxMemoryEntries--) | Restituisce il numero massimo di voci nella cache in memoria (predefinito: 1000). |
| [getMemoryTtl()](#getMemoryTtl--) | Restituisce il TTL per la cache in memoria, in minuti (predefinito: 60). |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCompressDisk(boolean value)](#setCompressDisk-boolean-) | Imposta se comprimere la cache su disco usando Gzip (predefinito: true). |
| [setDiskPath(String value)](#setDiskPath-java.lang.String-) | Imposta il percorso della directory della cache su disco. |
| [setDiskTtl(long value)](#setDiskTtl-long-) | Imposta il TTL per la cache su disco, in minuti (predefinito: 1440). |
| [setEnable(boolean value)](#setEnable-boolean-) | Imposta se abilitare la cache JSON per una risposta più veloce. |
| [setEnableDisk(boolean value)](#setEnableDisk-boolean-) | Imposta se abilitare la cache su disco (predefinito: true). |
| [setImplementation(IGridJsJsonCache value)](#setImplementation-com.aspose.gridjs.IGridJsJsonCache-) | Imposta l'implementazione personalizzata della cache JSON. |
| [setMaxDiskSizeMB(long value)](#setMaxDiskSizeMB-long-) | Imposta la dimensione massima della cache su disco in MB (predefinito: 500 MB). |
| [setMaxMemoryEntries(int value)](#setMaxMemoryEntries-int-) | Imposta il numero massimo di voci nella cache in memoria (predefinito: 1000). |
| [setMemoryTtl(long value)](#setMemoryTtl-long-) | Imposta il TTL per la cache in memoria, in minuti (predefinito: 60). |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### JsonCacheOptions() {#JsonCacheOptions--}
```
public JsonCacheOptions()
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
### getCompressDisk() {#getCompressDisk--}
```
public boolean getCompressDisk()
```


Restituisce se comprimere la cache su disco usando Gzip (predefinito: true). Ha effetto quando Enable = true e si utilizza la cache predefinita.

**Returns:**
boolean
### getDiskPath() {#getDiskPath--}
```
public String getDiskPath()
```


Restituisce il percorso della directory della cache su disco. Ha effetto quando Enable = true e si utilizza la cache predefinita. Predefinito: [FileCacheDirectory]/json\_cache

**Returns:**
java.lang.String
### getDiskTtl() {#getDiskTtl--}
```
public long getDiskTtl()
```


Restituisce il TTL per la cache su disco, in minuti (predefinito: 1440). Ha effetto quando Enable = true e si utilizza la cache predefinita.

**Returns:**
long
### getEnable() {#getEnable--}
```
public boolean getEnable()
```


Restituisce se abilitare la cache JSON per una risposta più veloce. Quando abilitato, GridJs memorizzerà nella cache il JSON generato e lo riutilizzerà per le richieste successive. Il valore predefinito è false. Nota: è necessario impostare Implementation per utilizzare un'archiviazione cache personalizzata.

**Returns:**
boolean
### getEnableDisk() {#getEnableDisk--}
```
public boolean getEnableDisk()
```


Restituisce se abilitare la cache su disco (predefinito: true). Ha effetto quando Enable = true e si utilizza la cache predefinita.

**Returns:**
boolean
### getImplementation() {#getImplementation--}
```
public IGridJsJsonCache getImplementation()
```


Restituisce l'implementazione personalizzata della cache JSON. Se non impostata, GridJs utilizzerà la cache predefinita in memoria + su disco.

**Returns:**
[IGridJsJsonCache](../../com.aspose.gridjs/igridjsjsoncache)
### getMaxDiskSizeMB() {#getMaxDiskSizeMB--}
```
public long getMaxDiskSizeMB()
```


Restituisce la dimensione massima della cache su disco in MB (predefinito: 500 MB). Ha effetto quando Enable = true e si utilizza la cache predefinita.

**Returns:**
long
### getMaxMemoryEntries() {#getMaxMemoryEntries--}
```
public int getMaxMemoryEntries()
```


Restituisce il numero massimo di voci nella cache in memoria (predefinito: 1000). Ha effetto quando Enable = true e si utilizza la cache predefinita.

**Returns:**
int
### getMemoryTtl() {#getMemoryTtl--}
```
public long getMemoryTtl()
```


Restituisce il TTL per la cache in memoria, in minuti (predefinito: 60). Ha effetto quando Enable = true e si utilizza la cache predefinita.

**Returns:**
long
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




### setCompressDisk(boolean value) {#setCompressDisk-boolean-}
```
public void setCompressDisk(boolean value)
```


Imposta se comprimere la cache su disco usando Gzip (predefinito: true). Ha effetto quando Enable = true e si utilizza la cache predefinita.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setDiskPath(String value) {#setDiskPath-java.lang.String-}
```
public void setDiskPath(String value)
```


Imposta il percorso della directory della cache su disco. Ha effetto quando Enable = true e si utilizza la cache predefinita. Predefinito: [FileCacheDirectory]/json\_cache

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setDiskTtl(long value) {#setDiskTtl-long-}
```
public void setDiskTtl(long value)
```


Imposta il TTL per la cache su disco, in minuti (predefinito: 1440). Ha effetto quando Enable = true e si utilizza la cache predefinita.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | long |  |

### setEnable(boolean value) {#setEnable-boolean-}
```
public void setEnable(boolean value)
```


Imposta se abilitare la cache JSON per una risposta più veloce. Quando abilitato, GridJs memorizzerà nella cache il JSON generato e lo riutilizzerà per le richieste successive. Il valore predefinito è false. Nota: è necessario impostare Implementation per utilizzare un'archiviazione cache personalizzata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEnableDisk(boolean value) {#setEnableDisk-boolean-}
```
public void setEnableDisk(boolean value)
```


Imposta se abilitare la cache su disco (predefinito: true). Ha effetto quando Enable = true e si utilizza la cache predefinita.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setImplementation(IGridJsJsonCache value) {#setImplementation-com.aspose.gridjs.IGridJsJsonCache-}
```
public void setImplementation(IGridJsJsonCache value)
```


Imposta l'implementazione personalizzata della cache JSON. Se non impostata, GridJs utilizzerà la cache predefinita in memoria + su disco.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [IGridJsJsonCache](../../com.aspose.gridjs/igridjsjsoncache) |  |

### setMaxDiskSizeMB(long value) {#setMaxDiskSizeMB-long-}
```
public void setMaxDiskSizeMB(long value)
```


Imposta la dimensione massima della cache su disco in MB (predefinito: 500 MB). Ha effetto quando Enable = true e si utilizza la cache predefinita.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | long |  |

### setMaxMemoryEntries(int value) {#setMaxMemoryEntries-int-}
```
public void setMaxMemoryEntries(int value)
```


Imposta il numero massimo di voci nella cache in memoria (predefinito: 1000). Ha effetto quando Enable = true e si utilizza la cache predefinita.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setMemoryTtl(long value) {#setMemoryTtl-long-}
```
public void setMemoryTtl(long value)
```


Imposta il TTL per la cache in memoria, in minuti (predefinito: 60). Ha effetto quando Enable = true e si utilizza la cache predefinita.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | long |  |

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

