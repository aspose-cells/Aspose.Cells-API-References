---
title: "GridCacheForStream"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Diese Klasse enthält die Cache-Operationen für GridJs."
type: docs
url: /de/java/com.aspose.gridjs/gridcacheforstream/
---

**Inheritance:**
java.lang.Object
```
public abstract class GridCacheForStream
```

Diese Klasse enthält die Cache-Operationen für GridJs. Der Benutzer soll basierend darauf seine eigene Geschäftslogik für die Speicherung implementieren.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [GridCacheForStream()](#GridCacheForStream--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFileUrl(String uid)](#getFileUrl-java.lang.String-) | Implementiert diese Methode, um die Datei‑URL aus dem Cache zu erhalten. |
| [hashCode()](#hashCode--) |  |
| [isExisted(String uid)](#isExisted-java.lang.String-) | Überprüft, ob der Cache mit uid existiert. |
| [loadStream(String uid)](#loadStream-java.lang.String-) | Implementiert diese Methode, um den Cache mit dem Schlüssel uid zu laden, und gibt den Stream aus dem Cache zurück. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [saveStream(InputStream s, String uid)](#saveStream-java.io.InputStream-java.lang.String-) | Implementiert diese Methode, um den Cache zu speichern, und speichert den Stream im Cache mit dem Schlüssel uid. |
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
| Parameter | Typ | Beschreibung |
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


Implementiert diese Methode, um die Datei‑URL aus dem Cache zu erhalten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uid | java.lang.String | Die eindeutige ID für den Dateicache. |

**Returns:**
java.lang.String - Die URL der Datei
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


Überprüft, ob der Cache mit uid existiert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uid | java.lang.String | Die eindeutige ID für den Dateicache. |

**Returns:**
boolean - Der boolesche Wert
### loadStream(String uid) {#loadStream-java.lang.String-}
```
public abstract InputStream loadStream(String uid)
```


Implementiert diese Methode, um den Cache mit dem Schlüssel uid zu laden, und gibt den Stream aus dem Cache zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
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


Implementiert diese Methode, um den Cache zu speichern, und speichert den Stream im Cache mit dem Schlüssel uid.

**Parameters:**
| Parameter | Typ | Beschreibung |
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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

