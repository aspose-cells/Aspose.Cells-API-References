---
title: "IGridJsService"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa la interfaz de APIs básicas de operación utilizadas en acciones de controlador."
type: docs
url: /es/java/com.aspose.gridjs/igridjsservice/
---
```
public interface IGridJsService
```

Representa la interfaz de APIs básicas de operación utilizadas en acciones de controlador.
## Métodos

| Método | Descripción |
| --- | --- |
| [addImage(String p, String uid, InputStream filestream)](#addImage-java.lang.String-java.lang.String-java.io.InputStream-) | Aplica la operación de agregar imagen desde un archivo local. |
| [addImageByURL(String p, String uid, InputStream filestream, String imageurl)](#addImageByURL-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-) | Aplica la operación de agregar imagen desde URL remota. |
| [checkInCacheForCollaborative(String uid)](#checkInCacheForCollaborative-java.lang.String-) | Verifica si la instancia del libro de trabajo está en la caché de memoria. Este método se aplica solo al modo colaborativo. |
| [clearAllJsonCache()](#clearAllJsonCache--) | Borra todas las entradas de caché JSON (memoria y disco). |
| [clearJsonCacheForUid(String uid)](#clearJsonCacheForUid-java.lang.String-) | Borra todas las entradas de caché JSON que pertenecen al ID único especificado. |
| [copyImage(String p, String uid)](#copyImage-java.lang.String-java.lang.String-) | Aplica la operación de copiar imagen. |
| [detailFileJsonWithUid(String filePath, String uid)](#detailFileJsonWithUid-java.lang.String-java.lang.String-) | Obtiene la cadena JSON del archivo mediante el ID único especificado. |
| [detailStreamJson(OutputStream stream, String filePath)](#detailStreamJson-java.io.OutputStream-java.lang.String-) | Escribe la cadena JSON del Libro de trabajo al flujo |
| [detailStreamJsonWithUid(OutputStream stream, String filePath, String uid)](#detailStreamJsonWithUid-java.io.OutputStream-java.lang.String-java.lang.String-) | Escribe la cadena JSON del archivo en el flujo mediante el ID único especificado. |
| [dispose()](#dispose--) |  |
| [download(String p, String uid, String filename)](#download-java.lang.String-java.lang.String-java.lang.String-) | Aplica la operación de descarga de archivo |
| [getFile(String fileid)](#getFile-java.lang.String-) | Obtener flujo de archivo |
| [image(String uid, String picid)](#image-java.lang.String-java.lang.String-) | Obtener flujo de imagen. |
| [imageUrl(String baseURL, String picid, String uid)](#imageUrl-java.lang.String-java.lang.String-java.lang.String-) | Obtiene la URL de la imagen. |
| [lazyLoadingJson(String sheetName, String uid)](#lazyLoadingJson-java.lang.String-java.lang.String-) | Obtiene la cadena JSON de la hoja especificada en el archivo desde la caché usando el ID único especificado. |
| [lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid)](#lazyLoadingStreamJson-java.io.OutputStream-java.lang.String-java.lang.String-) | Escribe la cadena JSON de la hoja especificada en el archivo desde la caché usando el id único especificado al flujo.. |
| [load(String uid, String filename)](#load-java.lang.String-java.lang.String-) | Obtiene la cadena JSON del archivo desde la caché usando el id único especificado, establece el nombre de archivo de salida en el JSON. |
| [ole(String uid, String sheetname, int oleid, String label)](#ole-java.lang.String-java.lang.String-int-java.lang.String-) | Obtiene los datos del arreglo de bytes del objeto ole incrustado. |
| [updateCell(String p, String uid)](#updateCell-java.lang.String-java.lang.String-) | Aplica la operación de actualización. |
### addImage(String p, String uid, InputStream filestream) {#addImage-java.lang.String-java.lang.String-java.io.InputStream-}
```
public abstract String addImage(String p, String uid, InputStream filestream)
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
public abstract String addImageByURL(String p, String uid, InputStream filestream, String imageurl)
```


Aplica la operación de agregar imagen desde URL remota.

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
public abstract boolean checkInCacheForCollaborative(String uid)
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
public abstract void clearAllJsonCache()
```


Borra todas las entradas de caché JSON (memoria y disco).

### clearJsonCacheForUid(String uid) {#clearJsonCacheForUid-java.lang.String-}
```
public abstract void clearJsonCacheForUid(String uid)
```


Borra todas las entradas de caché JSON que pertenecen al id único especificado. Llame a esto después de modificar el archivo fuente fuera de banda para que la siguiente solicitud regenere el JSON.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| uid | java.lang.String | El id único para la caché de archivos. |

### copyImage(String p, String uid) {#copyImage-java.lang.String-java.lang.String-}
```
public abstract String copyImage(String p, String uid)
```


Aplica la operación de copiar imagen.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| p | java.lang.String | El parámetro de cadena JSON |
| uid | java.lang.String | El id único para la caché de archivos. |

**Returns:**
java.lang.String - El resultado de cadena JSON
### detailFileJsonWithUid(String filePath, String uid) {#detailFileJsonWithUid-java.lang.String-java.lang.String-}
```
public abstract StringBuilder detailFileJsonWithUid(String filePath, String uid)
```


Obtiene la cadena JSON del archivo mediante el ID único especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| filePath | java.lang.String | La ruta del archivo |
| uid | java.lang.String | El id único para la caché de archivos. |

**Returns:**
java.lang.StringBuilder
### detailStreamJson(OutputStream stream, String filePath) {#detailStreamJson-java.io.OutputStream-java.lang.String-}
```
public abstract void detailStreamJson(OutputStream stream, String filePath)
```


Escribe la cadena JSON del Libro de trabajo al flujo

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.OutputStream | El flujo que se escribirá |
| filePath | java.lang.String | La ruta del archivo |

### detailStreamJsonWithUid(OutputStream stream, String filePath, String uid) {#detailStreamJsonWithUid-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public abstract void detailStreamJsonWithUid(OutputStream stream, String filePath, String uid)
```


Escribe la cadena JSON del archivo en el flujo mediante el ID único especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.OutputStream | El flujo que se escribirá |
| filePath | java.lang.String | La ruta del archivo |
| uid | java.lang.String | El id único para la caché de archivos. |

### dispose() {#dispose--}
```
public abstract void dispose()
```




### download(String p, String uid, String filename) {#download-java.lang.String-java.lang.String-java.lang.String-}
```
public abstract String download(String p, String uid, String filename)
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
### getFile(String fileid) {#getFile-java.lang.String-}
```
public abstract InputStream getFile(String fileid)
```


Obtener flujo de archivo

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileid | java.lang.String | el id del archivo |

**Returns:**
java.io.InputStream - El flujo del archivo
### image(String uid, String picid) {#image-java.lang.String-java.lang.String-}
```
public abstract InputStream image(String uid, String picid)
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
public abstract String imageUrl(String baseURL, String picid, String uid)
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
public abstract StringBuilder lazyLoadingJson(String sheetName, String uid)
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
public abstract void lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid)
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
public abstract String load(String uid, String filename)
```


Obtiene la cadena JSON del archivo desde la caché usando el id único especificado, establece el nombre de archivo de salida en el JSON.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| uid | java.lang.String | El id único para la caché de archivos. |
| nombre de archivo | java.lang.String | Especifica el nombre de archivo en el JSON. Si se establece en null, el nombre de archivo predeterminado es: book1. |

**Returns:**
java.lang.String - La cadena JSON
### ole(String uid, String sheetname, int oleid, String label) {#ole-java.lang.String-java.lang.String-int-java.lang.String-}
```
public abstract byte[] ole(String uid, String sheetname, int oleid, String label)
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
### updateCell(String p, String uid) {#updateCell-java.lang.String-java.lang.String-}
```
public abstract String updateCell(String p, String uid)
```


Aplica la operación de actualización.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| p | java.lang.String | La cadena de formato JSON de la operación de actualización. |
| uid | java.lang.String | El id único para la caché de archivos. |

**Returns:**
java.lang.String
