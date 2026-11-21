---
title: "GridCacheForStream"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Esta clase contiene las operaciones de caché para GridJs."
type: docs
url: /es/java/com.aspose.gridjs/gridcacheforstream/
---

**Inheritance:**
java.lang.Object
```
public abstract class GridCacheForStream
```

Esta clase contiene las operaciones de caché para GridJs. El usuario debe implementar su propia lógica de negocio para el almacenamiento basada en ella.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [GridCacheForStream()](#GridCacheForStream--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFileUrl(String uid)](#getFileUrl-java.lang.String-) | Implementa este método para obtener la URL del archivo de la caché. |
| [hashCode()](#hashCode--) |  |
| [isExisted(String uid)](#isExisted-java.lang.String-) | Comprueba si la caché con uid existe |
| [loadStream(String uid)](#loadStream-java.lang.String-) | Implementa este método para cargar la caché con la clave uid, y devolver el flujo de la caché. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [saveStream(InputStream s, String uid)](#saveStream-java.io.InputStream-java.lang.String-) | Implementa este método para guardar la caché, guardar el flujo en la caché con la clave uid. |
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
| Parámetro | Tipo | Descripción |
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


Implementa este método para obtener la URL del archivo de la caché.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| uid | java.lang.String | El id único para la caché de archivos. |

**Returns:**
java.lang.String - La URL del archivo
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


Comprueba si la caché con uid existe

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| uid | java.lang.String | El id único para la caché de archivos. |

**Returns:**
boolean - El valor booleano
### loadStream(String uid) {#loadStream-java.lang.String-}
```
public abstract InputStream loadStream(String uid)
```


Implementa este método para cargar la caché con la clave uid, y devolver el flujo de la caché.

**Parameters:**
| Parámetro | Tipo | Descripción |
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


Implementa este método para guardar la caché, guardar el flujo en la caché con la clave uid.

**Parameters:**
| Parámetro | Tipo | Descripción |
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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

