---
title: "GridCacheForStream"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Questa classe contiene le operazioni di cache per GridJs."
type: docs
url: /it/java/com.aspose.gridjs/gridcacheforstream/
---

**Inheritance:**
java.lang.Object
```
public abstract class GridCacheForStream
```

Questa classe contiene le operazioni di cache per GridJs. L'utente dovrà implementare la propria logica di business per l'archiviazione basandosi su di essa.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [GridCacheForStream()](#GridCacheForStream--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFileUrl(String uid)](#getFileUrl-java.lang.String-) | Implementa questo metodo per ottenere l'url del file dalla cache. |
| [hashCode()](#hashCode--) |  |
| [isExisted(String uid)](#isExisted-java.lang.String-) | Verifica se la cache con uid esiste |
| [loadStream(String uid)](#loadStream-java.lang.String-) | Implementa questo metodo per caricare la cache con la chiave uid e restituire lo stream dalla cache. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [saveStream(InputStream s, String uid)](#saveStream-java.io.InputStream-java.lang.String-) | Implementa questo metodo per salvare la cache, salvando lo stream nella cache con la chiave uid. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridCacheForStream() {#GridCacheForStream--}
```
public GridCacheForStream()
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
### getFileUrl(String uid) {#getFileUrl-java.lang.String-}
```
public abstract String getFileUrl(String uid)
```


Implementa questo metodo per ottenere l'url del file dalla cache.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | java.lang.String | L'id univoco per la cache del file. |

**Returns:**
java.lang.String - L'URL del file
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isExisted(String uid) {#isExisted-java.lang.String-}
```
public abstract boolean isExisted(String uid)
```


Verifica se la cache con uid esiste

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | java.lang.String | L'id univoco per la cache del file. |

**Returns:**
boolean - Il valore booleano
### loadStream(String uid) {#loadStream-java.lang.String-}
```
public abstract InputStream loadStream(String uid)
```


Implementa questo metodo per caricare la cache con la chiave uid e restituire lo stream dalla cache.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | java.lang.String |  |

**Returns:**
java.io.InputStream
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### saveStream(InputStream s, String uid) {#saveStream-java.io.InputStream-java.lang.String-}
```
public abstract void saveStream(InputStream s, String uid)
```


Implementa questo metodo per salvare la cache, salvando lo stream nella cache con la chiave uid.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| s | java.io.InputStream |  |
| uid | java.lang.String |  |

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

