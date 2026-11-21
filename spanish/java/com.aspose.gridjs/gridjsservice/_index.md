---
title: "GridJsService"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Proporciona las APIs básicas de operación utilizadas en acciones de controlador."
type: docs
url: /es/java/com.aspose.gridjs/gridjsservice/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.gridjs.IGridJsService](../../com.aspose.gridjs/igridjsservice)
```
public class GridJsService implements IGridJsService
```

Proporciona las APIs básicas de operación utilizadas en acciones de controlador.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [GridJsService(GridJsOptions options)](#GridJsService-com.aspose.gridjs.GridJsOptions-) | El constructor predeterminado para GridJsService |
## Métodos

| Método | Descripción |
| --- | --- |
| [addImage(String p, String uid, InputStream filestream)](#addImage-java.lang.String-java.lang.String-java.io.InputStream-) | Aplica la operación de agregar imagen desde un archivo local. |
| [addImageByURL(String p, String uid, InputStream filestream, String imageurl)](#addImageByURL-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-) | Aplica la operación de agregar imagen desde un archivo local. |
| [checkInCacheForCollaborative(String uid)](#checkInCacheForCollaborative-java.lang.String-) | Verifica si la instancia del libro de trabajo está en la caché de memoria. Este método se aplica solo al modo colaborativo. |
| [clearAllJsonCache()](#clearAllJsonCache--) | Borra todas las entradas de caché JSON (memoria y disco). |
| [clearJsonCacheForUid(String uid)](#clearJsonCacheForUid-java.lang.String-) | Borra todas las entradas de caché JSON que pertenecen al ID único especificado. |
| [copyImage(String p, String uid)](#copyImage-java.lang.String-java.lang.String-) | Aplica la operación de copiar imagen. |
| [destroy()](#destroy--) | Este método es solo para Java, implementa el método destroy en DisposableBean, que será llamado automáticamente por Spring al finalizar la solicitud; en realidad llamará al método Dispose. |
| [detailFileJsonWithUid(String filePath, String uid)](#detailFileJsonWithUid-java.lang.String-java.lang.String-) | Obtiene la cadena JSON del archivo mediante el ID único especificado. |
| [detailStreamJson(OutputStream stream, String filePath)](#detailStreamJson-java.io.OutputStream-java.lang.String-) | Escribe la cadena JSON del archivo en el flujo. |
| [detailStreamJsonWithUid(OutputStream stream, String filePath, String uid)](#detailStreamJsonWithUid-java.io.OutputStream-java.lang.String-java.lang.String-) | Escribe la cadena JSON del archivo en el flujo mediante el ID único especificado. |
| [dispose()](#dispose--) | Ejecuta tareas definidas por la aplicación asociadas con la liberación, el lanzamiento o el restablecimiento de recursos no administrados. |
| [download(String p, String uid, String filename)](#download-java.lang.String-java.lang.String-java.lang.String-) | Aplica la operación de descarga de archivo |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFile(String fileid)](#getFile-java.lang.String-) | Obtener flujo de archivo |
| [getSettings()](#getSettings--) | Representa la configuración del libro de trabajo. |
| [hashCode()](#hashCode--) |  |
| [image(String uid, String picid)](#image-java.lang.String-java.lang.String-) | Obtener flujo de imagen. |
| [imageUrl(String baseURL, String picid, String uid)](#imageUrl-java.lang.String-java.lang.String-java.lang.String-) | Obtiene la URL de la imagen. |
| [lazyLoadingJson(String sheetName, String uid)](#lazyLoadingJson-java.lang.String-java.lang.String-) | Obtiene la cadena JSON de la hoja especificada en el archivo desde la caché usando el ID único especificado. |
| [lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid)](#lazyLoadingStreamJson-java.io.OutputStream-java.lang.String-java.lang.String-) | Escribe la cadena JSON de la hoja especificada en el archivo desde la caché usando el id único especificado al flujo.. |
| [load(String uid, String filename)](#load-java.lang.String-java.lang.String-) | Obtiene la cadena JSON del archivo desde la caché usando el id único especificado, establece el nombre de archivo de salida en el JSON. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [ole(String uid, String sheetname, int oleid, String label)](#ole-java.lang.String-java.lang.String-int-java.lang.String-) | Obtiene los datos del arreglo de bytes del objeto ole incrustado. |
| [setSettings(GridWorkbookSettings value)](#setSettings-com.aspose.gridjs.GridWorkbookSettings-) | Representa la configuración del libro de trabajo. |
| [toString()](#toString--) |  |
| [translateSheetAsync(String uid, String sheetName, ITextTranslator translator, String targetLanguage)](#translateSheetAsync-java.lang.String-java.lang.String-com.aspose.gridjs.ITextTranslator-java.lang.String-) | Traduce todos los valores de cadena al idioma objetivo en la hoja de cálculo. |
| [updateCell(String p, String uid)](#updateCell-java.lang.String-java.lang.String-) | Aplica la operación de actualización. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridJsService(GridJsOptions options) {#GridJsService-com.aspose.gridjs.GridJsOptions-}
```
public GridJsService(GridJsOptions options)
```


El constructor predeterminado para GridJsService

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| options | [GridJsOptions](../../com.aspose.gridjs/gridjsoptions) |  |

### addImage(String p, String uid, InputStream filestream) {#addImage-java.lang.String-java.lang.String-java.io.InputStream-}
```
public String addImage(String p, String uid, InputStream filestream)
```


Aplica la operación de agregar imagen desde un archivo local.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| p | java.lang.String | El parámetro de cadena JSON |
| uid | java.lang.String | El id único para la caché de archivos. |
| filestream | java.io.InputStream | El flujo de archivo de la imagen |

**Returns:**
java.lang.String - El resultado de cadena JSON
### addImageByURL(String p, String uid, InputStream filestream, String imageurl) {#addImageByURL-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-}
```
public String addImageByURL(String p, String uid, InputStream filestream, String imageurl)
```


Aplica la operación de agregar imagen desde un archivo local.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| p | java.lang.String | El parámetro de cadena JSON |
| uid | java.lang.String | El id único para la caché de archivos. |
| filestream | java.io.InputStream | El flujo de archivo de la imagen |
| imageurl | java.lang.String | Especifique la URL de la imagen. |

**Returns:**
java.lang.String - El resultado de cadena JSON
### checkInCacheForCollaborative(String uid) {#checkInCacheForCollaborative-java.lang.String-}
```
public boolean checkInCacheForCollaborative(String uid)
```


Verifica si la instancia del libro de trabajo está en la caché de memoria. Este método se aplica solo al modo colaborativo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| uid | java.lang.String |  |

**Returns:**
boolean -
### clearAllJsonCache() {#clearAllJsonCache--}
```
public void clearAllJsonCache()
```


Borra todas las entradas de caché JSON (memoria y disco).

### clearJsonCacheForUid(String uid) {#clearJsonCacheForUid-java.lang.String-}
```
public void clearJsonCacheForUid(String uid)
```


Borra todas las entradas de caché JSON que pertenecen al id único especificado. Llame a esto después de modificar el archivo fuente fuera de banda para que la siguiente solicitud regenere el JSON.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| uid | java.lang.String | El id único para la caché de archivos. |

### copyImage(String p, String uid) {#copyImage-java.lang.String-java.lang.String-}
```
public String copyImage(String p, String uid)
```


Aplica la operación de copiar imagen.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| p | java.lang.String | El parámetro de cadena JSON |
| uid | java.lang.String | El id único para la caché de archivos. |

**Returns:**
java.lang.String - El resultado de cadena JSON
### destroy() {#destroy--}
```
public void destroy()
```


Este método es solo para Java, implementa el método destroy en DisposableBean, que será llamado automáticamente por Spring al finalizar la solicitud; en realidad llamará al método Dispose.

### detailFileJsonWithUid(String filePath, String uid) {#detailFileJsonWithUid-java.lang.String-java.lang.String-}
```
public StringBuilder detailFileJsonWithUid(String filePath, String uid)
```


Obtiene la cadena JSON del archivo mediante el ID único especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| filePath | java.lang.String | La ruta completa del archivo |
| uid | java.lang.String | El id único para la caché de archivos. |

**Returns:**
java.lang.StringBuilder
### detailStreamJson(OutputStream stream, String filePath) {#detailStreamJson-java.io.OutputStream-java.lang.String-}
```
public void detailStreamJson(OutputStream stream, String filePath)
```


Escribe la cadena JSON del archivo en el flujo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.OutputStream | El flujo que se escribirá |
| filePath | java.lang.String | La ruta completa del archivo |

### detailStreamJsonWithUid(OutputStream stream, String filePath, String uid) {#detailStreamJsonWithUid-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public void detailStreamJsonWithUid(OutputStream stream, String filePath, String uid)
```


Escribe la cadena JSON del archivo en el flujo mediante el ID único especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.OutputStream | El flujo que se escribirá |
| filePath | java.lang.String | La ruta completa del archivo |
| uid | java.lang.String | El id único para la caché de archivos. |

### dispose() {#dispose--}
```
public void dispose()
```


Ejecuta tareas definidas por la aplicación asociadas con la liberación, el lanzamiento o el restablecimiento de recursos no administrados.

### download(String p, String uid, String filename) {#download-java.lang.String-java.lang.String-java.lang.String-}
```
public String download(String p, String uid, String filename)
```


Aplica la operación de descarga de archivo

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| p | java.lang.String | El parámetro JSON |
| uid | java.lang.String | El id único para la caché de archivos. |
| nombre de archivo | java.lang.String | El nombre del archivo |

**Returns:**
java.lang.String - La URL del archivo
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
### getFile(String fileid) {#getFile-java.lang.String-}
```
public InputStream getFile(String fileid)
```


Obtener flujo de archivo

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileid | java.lang.String | el id del archivo |

**Returns:**
java.io.InputStream - El flujo del archivo
### getSettings() {#getSettings--}
```
public GridWorkbookSettings getSettings()
```


Representa la configuración del libro de trabajo.

**Returns:**
[GridWorkbookSettings](../../com.aspose.gridjs/gridworkbooksettings)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### image(String uid, String picid) {#image-java.lang.String-java.lang.String-}
```
public InputStream image(String uid, String picid)
```


Obtener flujo de imagen.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| uid | java.lang.String | El id único para la caché de archivos. |
| picid | java.lang.String | El id de la imagen. |

**Returns:**
java.io.InputStream - El flujo de la imagen
### imageUrl(String baseURL, String picid, String uid) {#imageUrl-java.lang.String-java.lang.String-java.lang.String-}
```
public String imageUrl(String baseURL, String picid, String uid)
```


Obtiene la URL de la imagen.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| baseURL | java.lang.String | La URL de acción base. |
| picid | java.lang.String | El id de la imagen. |
| uid | java.lang.String | El id único para la caché de archivos. |

**Returns:**
java.lang.String - La URL de la imagen
### lazyLoadingJson(String sheetName, String uid) {#lazyLoadingJson-java.lang.String-java.lang.String-}
```
public StringBuilder lazyLoadingJson(String sheetName, String uid)
```


Obtiene la cadena JSON de la hoja especificada en el archivo desde la caché usando el ID único especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetName | java.lang.String | el nombre de la hoja. |
| uid | java.lang.String | El id único para la caché de archivos. |

**Returns:**
java.lang.StringBuilder
### lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid) {#lazyLoadingStreamJson-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public void lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid)
```


Escribe la cadena JSON de la hoja especificada en el archivo desde la caché usando el id único especificado al flujo..

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.OutputStream | El flujo que se escribirá |
| sheetName | java.lang.String | El nombre de la hoja. |
| uid | java.lang.String | El id único para la caché de archivos. |

### load(String uid, String filename) {#load-java.lang.String-java.lang.String-}
```
public String load(String uid, String filename)
```


Obtiene la cadena JSON del archivo desde la caché usando el id único especificado, establece el nombre de archivo de salida en el JSON.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| uid | java.lang.String | El id único para la caché de archivos. |
| nombre de archivo | java.lang.String | Especifica el nombre de archivo en el JSON. Si se establece en null, el nombre de archivo predeterminado es: book1. |

**Returns:**
java.lang.String - La cadena JSON
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### ole(String uid, String sheetname, int oleid, String label) {#ole-java.lang.String-java.lang.String-int-java.lang.String-}
```
public byte[] ole(String uid, String sheetname, int oleid, String label)
```


Obtiene los datos del arreglo de bytes del objeto ole incrustado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| uid | java.lang.String | El id único para la caché de archivos. |
| sheetname | java.lang.String | El nombre de la hoja de cálculo. |
| oleid | int | El id del objeto ole incrustado. |
| label | java.lang.String | La etiqueta visible del objeto ole incrustado. |

**Returns:**
byte[] - Los datos del arreglo de bytes del objeto ole incrustado.
### setSettings(GridWorkbookSettings value) {#setSettings-com.aspose.gridjs.GridWorkbookSettings-}
```
public void setSettings(GridWorkbookSettings value)
```


Representa la configuración del libro de trabajo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [GridWorkbookSettings](../../com.aspose.gridjs/gridworkbooksettings) |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### translateSheetAsync(String uid, String sheetName, ITextTranslator translator, String targetLanguage) {#translateSheetAsync-java.lang.String-java.lang.String-com.aspose.gridjs.ITextTranslator-java.lang.String-}
```
public String translateSheetAsync(String uid, String sheetName, ITextTranslator translator, String targetLanguage)
```


Traduce todos los valores de cadena al idioma objetivo en la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| uid | java.lang.String | El id único para la caché de archivos. |
| sheetName | java.lang.String | El nombre de la hoja |
| translator | [ITextTranslator](../../com.aspose.gridjs/itexttranslator) | El traductor que implementa la función translate |
| idiomaObjetivo | java.lang.String | El idioma objetivo |

**Returns:**
java.lang.String -
### updateCell(String p, String uid) {#updateCell-java.lang.String-java.lang.String-}
```
public String updateCell(String p, String uid)
```


Aplica la operación de actualización.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| p | java.lang.String | La cadena de formato JSON de la operación de actualización. |
| uid | java.lang.String | El id único para la caché de archivos. |

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

