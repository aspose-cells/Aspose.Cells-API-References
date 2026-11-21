---
title: "GridCacheForStream"
second_title: "Aspose.Cells för Java API-referens"
description: "Denna klass innehåller cacheoperationerna för GridJs."
type: docs
url: /sv/java/com.aspose.gridjs/gridcacheforstream/
---

**Inheritance:**
java.lang.Object
```
public abstract class GridCacheForStream
```

Denna klass innehåller cacheoperationerna för GridJs. Användaren ska implementera sin egen affärslogik för lagring baserat på den.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [GridCacheForStream()](#GridCacheForStream--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFileUrl(String uid)](#getFileUrl-java.lang.String-) | Implementerar denna metod för att hämta fil-url från cachen. |
| [hashCode()](#hashCode--) |  |
| [isExisted(String uid)](#isExisted-java.lang.String-) | Kontrollerar om cachen med uid finns. |
| [loadStream(String uid)](#loadStream-java.lang.String-) | Implementerar denna metod för att ladda cache med nyckeln uid, returnera strömmen från cachen. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [saveStream(InputStream s, String uid)](#saveStream-java.io.InputStream-java.lang.String-) | Implementerar denna metod för att spara cache, spara strömmen till cachen med nyckeln uid. |
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
| Parameter | Typ | Beskrivning |
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


Implementerar denna metod för att hämta fil-url från cachen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uid | java.lang.String | Det unika id-et för filcachen. |

**Returns:**
java.lang.String - Filens URL
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


Kontrollerar om cachen med uid finns.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uid | java.lang.String | Det unika id-et för filcachen. |

**Returns:**
boolean - Det boolska värdet
### loadStream(String uid) {#loadStream-java.lang.String-}
```
public abstract InputStream loadStream(String uid)
```


Implementerar denna metod för att ladda cache med nyckeln uid, returnera strömmen från cachen.

**Parameters:**
| Parameter | Typ | Beskrivning |
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


Implementerar denna metod för att spara cache, spara strömmen till cachen med nyckeln uid.

**Parameters:**
| Parameter | Typ | Beskrivning |
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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

