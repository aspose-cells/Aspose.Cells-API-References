---
title: "StreamProviderOptions"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa las opciones de flujo."
type: docs
url: /es/java/com.aspose.cells/streamprovideroptions/
---

**Inheritance:**
java.lang.Object
```
public class StreamProviderOptions
```

Representa las opciones de flujo.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [StreamProviderOptions(int loadingType, String defaultPath)](#StreamProviderOptions-int-java.lang.String-) | Inicializa una nueva instancia de la clase [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions). |
| [StreamProviderOptions()](#StreamProviderOptions--) | Inicializa una nueva instancia de la clase [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions). |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCustomPath()](#getCustomPath--) | La ruta personalizada del usuario (URL) guardada en el archivo HTML generado para la fuente referida. |
| [getDefaultPath()](#getDefaultPath--) | La ruta predeterminada (URL) guardada en el archivo HTML generado para la fuente referida. |
| [getInputStream()](#getInputStream--) | Obtiene el flujo de entrada para obtener datos. |
| [getResourceLoadingType()](#getResourceLoadingType--) | Obtiene el tipo de recurso de carga. |
| [getStream()](#getStream--) | Obtiene el flujo de salida para escribir los datos guardados. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCustomPath(String value)](#setCustomPath-java.lang.String-) | La ruta personalizada del usuario (URL) guardada en el archivo HTML generado para la fuente referida. |
| [setInputStream(InputStream value)](#setInputStream-java.io.InputStream-) | Establece el flujo de entrada para obtener datos. |
| [setResourceLoadingType(int value)](#setResourceLoadingType-int-) | Establece el tipo de recurso de carga. |
| [setStream(OutputStream value)](#setStream-java.io.OutputStream-) | Establece el flujo de salida para escribir los datos guardados. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### StreamProviderOptions(int loadingType, String defaultPath) {#StreamProviderOptions-int-java.lang.String-}
```
public StreamProviderOptions(int loadingType, String defaultPath)
```


Inicializa una nueva instancia de la clase [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| loadingType | int | [ResourceLoadingType](../../com.aspose.cells/resourceloadingtype). El tipo para cargar el recurso vinculado. |
| defaultPath | java.lang.String | La ruta predeterminada. |

### StreamProviderOptions() {#StreamProviderOptions--}
```
public StreamProviderOptions()
```


Inicializa una nueva instancia de la clase [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions).

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
### getCustomPath() {#getCustomPath--}
```
public String getCustomPath()
```


La ruta personalizada del usuario (URL) guardada en el archivo HTML generado para la fuente referida. Si no es definida por el usuario, se utilizará DefaultPath. Por ejemplo, los datos de la hoja serán guardados por el usuario en d:/sheet001.htm, la URL utilizada en el archivo HTML principal debería ser "d:/sheet001.htm" o cualquier otra ruta relativa válida que pueda ser accedida por el archivo HTML principal.

**Returns:**
java.lang.String
### getDefaultPath() {#getDefaultPath--}
```
public String getDefaultPath()
```


La ruta predeterminada (URL) guardada en el archivo HTML generado para la fuente referida. Por ejemplo, los datos de la hoja guardados en xxx\_files/sheet001.htm, la URL utilizada en el archivo HTML principal debería ser como "src=\"xxx\_files/sheet001.htm\""

**Returns:**
java.lang.String
### getInputStream() {#getInputStream--}
```
public InputStream getInputStream()
```


Obtiene el flujo de entrada para obtener datos.

**Returns:**
java.io.InputStream
### getResourceLoadingType() {#getResourceLoadingType--}
```
public int getResourceLoadingType()
```


Obtiene el tipo de recurso de carga.

Ver [ResourceLoadingType](../../com.aspose.cells/resourceloadingtype).

**Returns:**
int
### getStream() {#getStream--}
```
public OutputStream getStream()
```


Obtiene el flujo de salida para escribir los datos guardados.

**Returns:**
java.io.OutputStream
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




### setCustomPath(String value) {#setCustomPath-java.lang.String-}
```
public void setCustomPath(String value)
```


La ruta personalizada del usuario (URL) guardada en el archivo HTML generado para la fuente referida. Si no es definida por el usuario, se utilizará DefaultPath. Por ejemplo, los datos de la hoja serán guardados por el usuario en d:/sheet001.htm, la URL utilizada en el archivo HTML principal debería ser "d:/sheet001.htm" o cualquier otra ruta relativa válida que pueda ser accedida por el archivo HTML principal.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setInputStream(InputStream value) {#setInputStream-java.io.InputStream-}
```
public void setInputStream(InputStream value)
```


Establece el flujo de entrada para obtener datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.io.InputStream |  |

### setResourceLoadingType(int value) {#setResourceLoadingType-int-}
```
public void setResourceLoadingType(int value)
```


Establece el tipo de recurso de carga.

Ver [ResourceLoadingType](../../com.aspose.cells/resourceloadingtype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setStream(OutputStream value) {#setStream-java.io.OutputStream-}
```
public void setStream(OutputStream value)
```


Establece el flujo de salida para escribir los datos guardados.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.io.OutputStream |  |

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

