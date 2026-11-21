---
title: "JsonCacheOptions"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Opciones de configuración para el almacenamiento en caché JSON en GridJs."
type: docs
url: /es/java/com.aspose.gridjs/jsoncacheoptions/
---

**Inheritance:**
java.lang.Object
```
public class JsonCacheOptions
```

Opciones de configuración para la caché JSON en GridJs. Controla tanto la caché en memoria (L1) como en disco (L2).
## Constructores

| Constructor | Descripción |
| --- | --- |
| [JsonCacheOptions()](#JsonCacheOptions--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCompressDisk()](#getCompressDisk--) | Obtiene si comprimir la caché de disco usando Gzip (predeterminado: true). |
| [getDiskPath()](#getDiskPath--) | Obtiene la ruta del directorio de caché de disco. |
| [getDiskTtl()](#getDiskTtl--) | Obtiene el TTL para la caché de disco, en minutos (predeterminado: 1440). |
| [getEnable()](#getEnable--) | Obtiene si habilitar la caché JSON para una respuesta más rápida. |
| [getEnableDisk()](#getEnableDisk--) | Obtiene si habilitar la caché de disco (predeterminado: true). |
| [getImplementation()](#getImplementation--) | Obtiene la implementación personalizada de caché JSON. |
| [getMaxDiskSizeMB()](#getMaxDiskSizeMB--) | Obtiene el tamaño máximo de la caché de disco en MB (predeterminado: 500 MB). |
| [getMaxMemoryEntries()](#getMaxMemoryEntries--) | Obtiene el número máximo de entradas en la caché en memoria (predeterminado: 1000). |
| [getMemoryTtl()](#getMemoryTtl--) | Obtiene el TTL para la caché en memoria, en minutos (predeterminado: 60). |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCompressDisk(boolean value)](#setCompressDisk-boolean-) | Establece si comprimir la caché de disco usando Gzip (predeterminado: true). |
| [setDiskPath(String value)](#setDiskPath-java.lang.String-) | Establece la ruta del directorio de caché de disco. |
| [setDiskTtl(long value)](#setDiskTtl-long-) | Establece el TTL para la caché de disco, en minutos (predeterminado: 1440). |
| [setEnable(boolean value)](#setEnable-boolean-) | Establece si habilitar la caché JSON para una respuesta más rápida. |
| [setEnableDisk(boolean value)](#setEnableDisk-boolean-) | Establece si habilitar la caché de disco (predeterminado: true). |
| [setImplementation(IGridJsJsonCache value)](#setImplementation-com.aspose.gridjs.IGridJsJsonCache-) | Establece la implementación personalizada de caché JSON. |
| [setMaxDiskSizeMB(long value)](#setMaxDiskSizeMB-long-) | Establece el tamaño máximo de la caché en disco en MB (predeterminado: 500 MB). |
| [setMaxMemoryEntries(int value)](#setMaxMemoryEntries-int-) | Establece el número máximo de entradas en la caché en memoria (predeterminado: 1000). |
| [setMemoryTtl(long value)](#setMemoryTtl-long-) | Establece el TTL para la caché en memoria, en minutos (predeterminado: 60). |
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
### getCompressDisk() {#getCompressDisk--}
```
public boolean getCompressDisk()
```


Obtiene si se debe comprimir la caché en disco usando Gzip (predeterminado: true). Tiene efecto cuando Enable = true y se usa la caché predeterminada.

**Returns:**
boolean
### getDiskPath() {#getDiskPath--}
```
public String getDiskPath()
```


Obtiene la ruta del directorio de la caché en disco. Tiene efecto cuando Enable = true y se usa la caché predeterminada. Predeterminado: [FileCacheDirectory]/json\_cache

**Returns:**
java.lang.String
### getDiskTtl() {#getDiskTtl--}
```
public long getDiskTtl()
```


Obtiene el TTL para la caché en disco, en minutos (predeterminado: 1440). Tiene efecto cuando Enable = true y se usa la caché predeterminada.

**Returns:**
long
### getEnable() {#getEnable--}
```
public boolean getEnable()
```


Obtiene si se habilita el almacenamiento en caché de JSON para una respuesta más rápida. Cuando está habilitado, GridJs almacenará en caché el JSON generado y lo reutilizará para solicitudes posteriores. El valor predeterminado es false. Nota: Necesita establecer Implementation para usar un almacenamiento de caché personalizado.

**Returns:**
boolean
### getEnableDisk() {#getEnableDisk--}
```
public boolean getEnableDisk()
```


Obtiene si se habilita la caché en disco (predeterminado: true). Tiene efecto cuando Enable = true y se usa la caché predeterminada.

**Returns:**
boolean
### getImplementation() {#getImplementation--}
```
public IGridJsJsonCache getImplementation()
```


Obtiene la implementación personalizada de caché JSON. Si no se establece, GridJs usará la caché predeterminada de memoria + disco.

**Returns:**
[IGridJsJsonCache](../../com.aspose.gridjs/igridjsjsoncache)
### getMaxDiskSizeMB() {#getMaxDiskSizeMB--}
```
public long getMaxDiskSizeMB()
```


Obtiene el tamaño máximo de la caché en disco en MB (predeterminado: 500 MB). Tiene efecto cuando Enable = true y se usa la caché predeterminada.

**Returns:**
long
### getMaxMemoryEntries() {#getMaxMemoryEntries--}
```
public int getMaxMemoryEntries()
```


Obtiene el número máximo de entradas en la caché en memoria (predeterminado: 1000). Tiene efecto cuando Enable = true y se usa la caché predeterminada.

**Returns:**
int
### getMemoryTtl() {#getMemoryTtl--}
```
public long getMemoryTtl()
```


Obtiene el TTL para la caché en memoria, en minutos (predeterminado: 60). Tiene efecto cuando Enable = true y se usa la caché predeterminada.

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


Establece si se debe comprimir la caché en disco usando Gzip (predeterminado: true). Tiene efecto cuando Enable = true y se usa la caché predeterminada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setDiskPath(String value) {#setDiskPath-java.lang.String-}
```
public void setDiskPath(String value)
```


Establece la ruta del directorio de la caché en disco. Tiene efecto cuando Enable = true y se usa la caché predeterminada. Predeterminado: [FileCacheDirectory]/json\_cache

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setDiskTtl(long value) {#setDiskTtl-long-}
```
public void setDiskTtl(long value)
```


Establece el TTL para la caché en disco, en minutos (predeterminado: 1440). Tiene efecto cuando Enable = true y se usa la caché predeterminada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | long |  |

### setEnable(boolean value) {#setEnable-boolean-}
```
public void setEnable(boolean value)
```


Establece si se habilita el almacenamiento en caché de JSON para una respuesta más rápida. Cuando está habilitado, GridJs almacenará en caché el JSON generado y lo reutilizará para solicitudes posteriores. El valor predeterminado es false. Nota: Necesita establecer Implementation para usar un almacenamiento de caché personalizado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEnableDisk(boolean value) {#setEnableDisk-boolean-}
```
public void setEnableDisk(boolean value)
```


Establece si se habilita la caché en disco (predeterminado: true). Tiene efecto cuando Enable = true y se usa la caché predeterminada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setImplementation(IGridJsJsonCache value) {#setImplementation-com.aspose.gridjs.IGridJsJsonCache-}
```
public void setImplementation(IGridJsJsonCache value)
```


Establece la implementación personalizada de caché JSON. Si no se establece, GridJs usará la caché predeterminada de memoria + disco.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [IGridJsJsonCache](../../com.aspose.gridjs/igridjsjsoncache) |  |

### setMaxDiskSizeMB(long value) {#setMaxDiskSizeMB-long-}
```
public void setMaxDiskSizeMB(long value)
```


Establece el tamaño máximo de la caché en disco en MB (predeterminado: 500 MB). Tiene efecto cuando Enable = true y se usa la caché predeterminada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | long |  |

### setMaxMemoryEntries(int value) {#setMaxMemoryEntries-int-}
```
public void setMaxMemoryEntries(int value)
```


Establece el número máximo de entradas en la caché en memoria (predeterminado: 1000). Tiene efecto cuando Enable = true y se usa la caché predeterminada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setMemoryTtl(long value) {#setMemoryTtl-long-}
```
public void setMemoryTtl(long value)
```


Establece el TTL para la caché en memoria, en minutos (predeterminado: 60). Tiene efecto cuando Enable = true y se usa la caché predeterminada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | long |  |

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

