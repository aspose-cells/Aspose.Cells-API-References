---
title: "GridJsWorkbook"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa la clase principal de entrada para GridJs"
type: docs
url: /es/java/com.aspose.gridjs/gridjsworkbook/
---

**Inheritance:**
java.lang.Object
```
public class GridJsWorkbook
```

Representa la clase principal de entrada para GridJs
## Constructores

| Constructor | Descripción |
| --- | --- |
| [GridJsWorkbook()](#GridJsWorkbook--) | Crea una nueva instancia de GridJsWorkbook. |
## Campos

| Campo | Descripción |
| --- | --- |
| [CacheImp](#CacheImp) | Implementación personalizada para el almacenamiento en caché, si deseas almacenar la caché de forma continua, necesitas configurarla e implementarla. |
| [CalculateEngine](#CalculateEngine) | Implementación personalizada para el motor de cálculo, si deseas realizar cálculos personalizados, debes configurarlo e implementarlo. |
| [PICTURE_TYPE](#PICTURE-TYPE) | valor constante para el tipo de la imagen |
| [UpdateMonitor](#UpdateMonitor) | Obtiene/Establece el monitor de actualización para rastrear la operación de actualización |
## Métodos

| Método | Descripción |
| --- | --- |
| [burnRedactionFile(String excelFilePath, String uid)](#burnRedactionFile-java.lang.String-java.lang.String-) | Aplica (applies) todas las operaciones de redacción en el libro de trabajo eliminando las formas de redacción y sus formas objetivo o borrando el contenido del rango de celdas objetivo. |
| [checkInCacheForCollaborative(String uid)](#checkInCacheForCollaborative-java.lang.String-) | Verifica si la instancia del libro de trabajo está en la caché de memoria. Este método se aplica solo al modo colaborativo. |
| [clearAllJsonCache()](#clearAllJsonCache--) | \\u5a13\\u5474\\u6ace\\u93b5\\u20ac\\u93c8? |
| [clearJsonCacheForUid(String uid)](#clearJsonCacheForUid-java.lang.String-) | \\u93cd\\u89c4\\u5d41 uid \\u5a13\\u5474\\u6ace JSON \\u7f02\\u64b3\\u74e8\\u951b\\u5822\\u6564\\u6d5c? |
| [copyImageOrShape(String uid, String p)](#copyImageOrShape-java.lang.String-java.lang.String-) | Copia la imagen o la forma. |
| [dispose()](#dispose--) | Ejecuta tareas definidas por la aplicación asociadas con la liberación, el lanzamiento o el restablecimiento de recursos no administrados. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [errorJson(String msg)](#errorJson-java.lang.String-) | Obtiene la cadena del mensaje de error en formato JSON. |
| [exportToJson()](#exportToJson--) | Obtiene la cadena JSON de los datos en memoria, el nombre de archivo predeterminado en el JSON es: book1. |
| [exportToJson(String filename)](#exportToJson-java.lang.String-) | Obtiene la cadena JSON de los datos en memoria,establezca el nombre de archivo de salida en el JSON. |
| [exportToJsonStringBuilder(String filename)](#exportToJsonStringBuilder-java.lang.String-) | Obtiene la cadena JSON de los datos en memoria,establezca el nombre de archivo de salida en el JSON. |
| [exportToJsonStringBuilder(String filename, String uid)](#exportToJsonStringBuilder-java.lang.String-java.lang.String-) |  |
| [getCacheDirectory()](#getCacheDirectory--) | Obtiene el directorio de caché para almacenar el archivo de hoja de cálculo. |
| [getClass()](#getClass--) |  |
| [getGridLoadFormat(String extension)](#getGridLoadFormat-java.lang.String-) | Obtiene el formato de carga según la extensión del archivo |
| [getImageStream(String uid, String picid, String cachedir)](#getImageStream-java.lang.String-java.lang.String-java.lang.String-) | Obtener flujo de imagen. |
| [getImageUrl(String uid, String picid, String delimiter)](#getImageUrl-java.lang.String-java.lang.String-java.lang.String-) | Obtiene la URL de la imagen. |
| [getJsonByUid(String uid, String filename)](#getJsonByUid-java.lang.String-java.lang.String-) | Obtiene la cadena JSON del archivo desde la caché usando el id único especificado, establece el nombre de archivo de salida en el JSON. |
| [getOle(String uid, String sheetname, int oleid, String label)](#getOle-java.lang.String-java.lang.String-int-java.lang.String-) | Obtiene los datos del arreglo de bytes del objeto ole incrustado. |
| [getSettings()](#getSettings--) | Representa la configuración del libro de trabajo. |
| [getSheetJsonWithCache(String uid, String sheetName, String fileName)](#getSheetJsonWithCache-java.lang.String-java.lang.String-java.lang.String-) | \\u947e\\u5cf0\\u5f47\\u93b8\\u56e7\\u757e hoja \\u9428? |
| [getUidForFile(String fileName)](#getUidForFile-java.lang.String-) | Genera un nuevo id único para la caché de archivos usando el nombre de archivo proporcionado. |
| [getWorkbookJsonWithCache(String uid, String fileName)](#getWorkbookJsonWithCache-java.lang.String-java.lang.String-) | \\u947e\\u5cf0\\u5f47\\u93c1\\u7fe0\\u91dc\\u5bb8\\u30e4\\u7d94\\u7ee8\\u8de8\\u6b91 JSON\\u951b\\u581d\\u752b\\u7f02\\u64b3\\u74e8\\u951b? |
| [hashCode()](#hashCode--) |  |
| [importExcelFile(InputStream filestream, int format)](#importExcelFile-java.io.InputStream-int-) | Importa el archivo Excel desde el flujo de archivo con formato de carga. |
| [importExcelFile(InputStream filestream, int format, String password)](#importExcelFile-java.io.InputStream-int-java.lang.String-) | Importa el archivo Excel desde el flujo de archivo con formato de carga y contraseña de apertura. |
| [importExcelFile(String fileName)](#importExcelFile-java.lang.String-) | Importa el archivo Excel desde la ruta del archivo. |
| [importExcelFile(String uid, InputStream filestream, int format)](#importExcelFile-java.lang.String-java.io.InputStream-int-) | Importa el archivo Excel desde el flujo de archivo. |
| [importExcelFile(String uid, InputStream filestream, int format, String password)](#importExcelFile-java.lang.String-java.io.InputStream-int-java.lang.String-) | Importa el archivo Excel desde el flujo de archivo con formato de carga y contraseña de apertura. |
| [importExcelFile(String uid, String fileName)](#importExcelFile-java.lang.String-java.lang.String-) | Importa el archivo Excel desde la ruta del archivo. |
| [importExcelFile(String uid, String fileName, String password)](#importExcelFile-java.lang.String-java.lang.String-java.lang.String-) | Importa el archivo Excel desde la ruta del archivo y contraseña de apertura. |
| [importExcelFileFromJson(String json)](#importExcelFileFromJson-java.lang.String-) | Importa el archivo Excel desde una cadena en formato JSON. |
| [insertImage(String uid, String p, InputStream s, String imageUrl)](#insertImage-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-) | Inserta una imagen en la hoja de cálculo desde el flujo de archivo o la URL, (se debe proporcionar el flujo de archivo o la URL) o inserta una forma, cuando p.type es uno de AutoShapeType |
| [jsonToStream(OutputStream stream, String filename)](#jsonToStream-java.io.OutputStream-java.lang.String-) | Genera JSON a partir del Workbook en memoria y lo escribe en el flujo especificado. |
| [jsonToStream(OutputStream stream, String filename, String uid)](#jsonToStream-java.io.OutputStream-java.lang.String-java.lang.String-) |  |
| [jsonToStreamByUid(OutputStream stream, String uid, String filename)](#jsonToStreamByUid-java.io.OutputStream-java.lang.String-java.lang.String-) | Recupera la cadena JSON del archivo de la caché usando el id único especificado,establezca el nombre de archivo de salida en el JSON,y escríbalo en el flujo. |
| [lazyLoadingJson(String uid, String sheetName)](#lazyLoadingJson-java.lang.String-java.lang.String-) | Obtiene la cadena JSON de la hoja especificada en el archivo desde la caché usando el ID único especificado. |
| [lazyLoadingStream(OutputStream stream, String uid, String sheetName)](#lazyLoadingStream-java.io.OutputStream-java.lang.String-java.lang.String-) | Recupera la cadena JSON de la hoja especificada en el archivo de la caché usando el id único especificado, y escríbala en el flujo. |
| [mergeExcelFileFromJson(String uid, String json)](#mergeExcelFileFromJson-java.lang.String-java.lang.String-) | Aplica una actualización por lotes a los datos en memoria. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [redactFile(String excelFilePath, String uid, String[] arrayOfRedactionOpr)](#redactFile-java.lang.String-java.lang.String-java.lang.String---) | Realiza una redacción en un archivo Excel basado en una matriz de operaciones JSON. |
| [saveToCacheWithFileName(String uid, String filename, String password)](#saveToCacheWithFileName-java.lang.String-java.lang.String-java.lang.String-) | Guarda los datos en memoria en el archivo de caché con el nombre de archivo especificado y también establece la contraseña de apertura, el formato de guardado se basa en la extensión del archivo del nombre de archivo. |
| [saveToExcelFile(OutputStream stream)](#saveToExcelFile-java.io.OutputStream-) | Guarda los datos en memoria en el flujo, basado en el formato de archivo original. |
| [saveToExcelFile(String path)](#saveToExcelFile-java.lang.String-) | Guarda los datos en memoria en la ruta del archivo, si el archivo tiene extensión, el formato de guardado se basa en la extensión del archivo. |
| [saveToHtml(OutputStream stream)](#saveToHtml-java.io.OutputStream-) | Guarda los datos en memoria en el flujo, el formato de guardado es html |
| [saveToHtml(String path)](#saveToHtml-java.lang.String-) | Guarda los datos en memoria en la ruta del archivo, el formato de guardado es html. |
| [saveToPdf(OutputStream stream)](#saveToPdf-java.io.OutputStream-) | Guarda los datos en memoria en el flujo, el formato de guardado es pdf. |
| [saveToPdf(String path)](#saveToPdf-java.lang.String-) | Guarda los datos de memoria en la ruta del archivo, el formato de guardado es pdf. |
| [saveToXlsx(OutputStream stream)](#saveToXlsx-java.io.OutputStream-) | Guarda los datos de memoria en el flujo, el formato de guardado es xlsx. |
| [saveToXlsx(String path)](#saveToXlsx-java.lang.String-) | Guarda los datos de memoria en la ruta del archivo, el formato de guardado es xlsx. |
| [setCacheDirectory(String value)](#setCacheDirectory-java.lang.String-) | Establece el directorio de caché para almacenar el archivo de hoja de cálculo. |
| [setImageUrlBase(String baseImageURL)](#setImageUrlBase-java.lang.String-) | Establece la URL de acción de obtención de la imagen base desde el controlador. |
| [setInterruptMonitorForLoad(GridInterruptMonitor monitor, int calculateTimeoutMilliseconds)](#setInterruptMonitorForLoad-com.aspose.gridjs.GridInterruptMonitor-int-) | Establece InterruptMonitor para la operación de carga. |
| [setInterruptMonitorForSave(GridInterruptMonitor monitor)](#setInterruptMonitorForSave-com.aspose.gridjs.GridInterruptMonitor-) | Establece InterruptMonitor para la operación de guardado. |
| [setSettings(GridWorkbookSettings value)](#setSettings-com.aspose.gridjs.GridWorkbookSettings-) | Representa la configuración del libro de trabajo. |
| [setTransParentView(String excelFilePath, String uid, boolean isTransparent)](#setTransParentView-java.lang.String-java.lang.String-boolean-) | Establece la transparencia de las formas de redacción en el libro de trabajo. |
| [toString()](#toString--) |  |
| [translateSheetAsync(String uid, String sheetName, ITextTranslator translator, String targetLanguage)](#translateSheetAsync-java.lang.String-java.lang.String-com.aspose.gridjs.ITextTranslator-java.lang.String-) | Traduce todos los valores de cadena al idioma objetivo en la hoja de cálculo. |
| [updateCell(String p, String uid)](#updateCell-java.lang.String-java.lang.String-) | Aplica la operación de actualización. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridJsWorkbook() {#GridJsWorkbook--}
```
public GridJsWorkbook()
```


Crea una nueva instancia de GridJsWorkbook.

### CacheImp {#CacheImp}
```
public static GridCacheForStream CacheImp
```


Implementación personalizada para el almacenamiento en caché, si deseas almacenar la caché de forma continua, necesitas configurarla e implementarla.

### CalculateEngine {#CalculateEngine}
```
public static GridAbstractCalculationEngine CalculateEngine
```


Implementación personalizada para el motor de cálculo, si deseas realizar cálculos personalizados, debes configurarlo e implementarlo.

### PICTURE_TYPE {#PICTURE-TYPE}
```
public static final String PICTURE_TYPE
```


valor constante para el tipo de la imagen

### UpdateMonitor {#UpdateMonitor}
```
public static GridUpdateMonitor UpdateMonitor
```


Obtiene/Establece el monitor de actualización para rastrear la operación de actualización

### burnRedactionFile(String excelFilePath, String uid) {#burnRedactionFile-java.lang.String-java.lang.String-}
```
public void burnRedactionFile(String excelFilePath, String uid)
```


Aplica (applies) todas las operaciones de redacción en el libro de trabajo eliminando las formas de redacción y sus formas objetivo o borrando el contenido del rango de celdas objetivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| excelFilePath | java.lang.String | La ruta del archivo Excel. |
| uid | java.lang.String | El identificador único del libro de trabajo. Si es nulo o vacío, se generará un nuevo uid basado en la ruta del archivo. |

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


\\u5a13\\u5474\\u6ace\\u93b5\\u20ac\\u93c8?JSON \\u7f02\\u64b3\\u74e8

### clearJsonCacheForUid(String uid) {#clearJsonCacheForUid-java.lang.String-}
```
public void clearJsonCacheForUid(String uid)
```


\\u93cd\\u89c4\\u5d41 uid \\u5a13\\u5474\\u6ace JSON \\u7f02\\u64b3\\u74e8\\u951b\\u5822\\u6564\\u6d5c?UpdateCell \\u7edb\\u590a\\u5f67\\u93c8?uid \\u9428\\u52eb\\u6e80\\u93c5\\ue224\\u7d1a

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| uid | java.lang.String | \\u93c2\\u56e6\\u6b22\\u9428\\u52eb\\u656e\\u6d93\\u20ac\\u93cd\\u56ea\\u7611 |

### copyImageOrShape(String uid, String p) {#copyImageOrShape-java.lang.String-java.lang.String-}
```
public String copyImageOrShape(String uid, String p)
```


Copia la imagen o la forma.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| uid | java.lang.String | El id único para la caché de archivos. |
| p | java.lang.String | La cadena JSON para la operación que especifica la ubicación de la celda, contiene el nombre de la hoja, fila superior izquierda, columna superior izquierda para la imagen o forma\\u951b\\u5b94tc \{name:'sheet1',ri:1,ci:1,srcid:2,srcname:'sheet2',isshape:true\} |

**Returns:**
java.lang.String - La cadena JSON de la nueva imagen copiada
### dispose() {#dispose--}
```
public void dispose()
```


Ejecuta tareas definidas por la aplicación asociadas con la liberación, el lanzamiento o el restablecimiento de recursos no administrados.

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
### errorJson(String msg) {#errorJson-java.lang.String-}
```
public String errorJson(String msg)
```


Obtiene la cadena del mensaje de error en formato JSON.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| msg | java.lang.String | El mensaje de error. |

**Returns:**
java.lang.String - La cadena JSON.
### exportToJson() {#exportToJson--}
```
public String exportToJson()
```


Obtiene la cadena JSON de los datos en memoria, el nombre de archivo predeterminado en el JSON es: book1.

**Returns:**
java.lang.String - La cadena JSON.
### exportToJson(String filename) {#exportToJson-java.lang.String-}
```
public String exportToJson(String filename)
```


Obtiene la cadena JSON de los datos en memoria,establezca el nombre de archivo de salida en el JSON.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre de archivo | java.lang.String | Especifica el nombre de archivo en el JSON. Si se establece en nulo, el nombre de archivo predeterminado es: book1.. |

**Returns:**
java.lang.String - La cadena JSON.
### exportToJsonStringBuilder(String filename) {#exportToJsonStringBuilder-java.lang.String-}
```
public StringBuilder exportToJsonStringBuilder(String filename)
```


Obtiene la cadena JSON de los datos en memoria,establezca el nombre de archivo de salida en el JSON.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre de archivo | java.lang.String | Especifica el nombre de archivo en el JSON. Si se establece en nulo, el nombre de archivo predeterminado es: book1.. |

**Returns:**
java.lang.StringBuilder - El StringBuilder JSON.
### exportToJsonStringBuilder(String filename, String uid) {#exportToJsonStringBuilder-java.lang.String-java.lang.String-}
```
public StringBuilder exportToJsonStringBuilder(String filename, String uid)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre de archivo | java.lang.String |  |
| uid | java.lang.String |  |

**Returns:**
java.lang.StringBuilder
### getCacheDirectory() {#getCacheDirectory--}
```
public String getCacheDirectory()
```


Obtiene el directorio de caché para almacenar archivos de hoja de cálculo. Si no está configurado, utilizaremos la propiedad estática de [Config.getFileCacheDirectory()](../../com.aspose.gridjs/config\#getFileCacheDirectory--) o [CacheImp](../../com.aspose.gridjs/gridjsworkbook\#CacheImp).

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getGridLoadFormat(String extension) {#getGridLoadFormat-java.lang.String-}
```
public static int getGridLoadFormat(String extension)
```


Obtiene el formato de carga según la extensión del archivo

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| extension | java.lang.String | La extensión del archivo, usualmente comienza con '.' . |

**Returns:**
int - [GridLoadFormat](../../com.aspose.gridjs/gridloadformat).
### getImageStream(String uid, String picid, String cachedir) {#getImageStream-java.lang.String-java.lang.String-java.lang.String-}
```
public static InputStream getImageStream(String uid, String picid, String cachedir)
```


Obtener flujo de imagen.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| uid | java.lang.String | El id único para la caché de archivos. |
| picid | java.lang.String | El id de la imagen. |
| cachedir | java.lang.String |  |

**Returns:**
java.io.InputStream - El flujo de la imagen
### getImageUrl(String uid, String picid, String delimiter) {#getImageUrl-java.lang.String-java.lang.String-java.lang.String-}
```
public static String getImageUrl(String uid, String picid, String delimiter)
```


Obtiene la URL de la imagen.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| uid | java.lang.String | El id único para la caché de archivos. |
| picid | java.lang.String | El id de la imagen. |
| delimiter | java.lang.String | El delimitador de cadena. |

**Returns:**
java.lang.String -
### getJsonByUid(String uid, String filename) {#getJsonByUid-java.lang.String-java.lang.String-}
```
public StringBuilder getJsonByUid(String uid, String filename)
```


Obtiene la cadena JSON del archivo desde la caché usando el id único especificado, establece el nombre de archivo de salida en el JSON.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| uid | java.lang.String | El id único para la caché de archivos. |
| nombre de archivo | java.lang.String | Especifica el nombre de archivo en el JSON. Si se establece en null, el nombre de archivo predeterminado es: book1. |

**Returns:**
java.lang.StringBuilder - El StringBuilder de cadena JSON
### getOle(String uid, String sheetname, int oleid, String label) {#getOle-java.lang.String-java.lang.String-int-java.lang.String-}
```
public byte[] getOle(String uid, String sheetname, int oleid, String label)
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
### getSettings() {#getSettings--}
```
public GridWorkbookSettings getSettings()
```


Representa la configuración del libro de trabajo.

**Returns:**
[GridWorkbookSettings](../../com.aspose.gridjs/gridworkbooksettings)
### getSheetJsonWithCache(String uid, String sheetName, String fileName) {#getSheetJsonWithCache-java.lang.String-java.lang.String-java.lang.String-}
```
public String getSheetJsonWithCache(String uid, String sheetName, String fileName)
```


\\u947e\\u5cf0\\u5f47\\u93b8\\u56e7\\u757e hoja \\u9428?JSON\\u951b\\u581d\\u752b\\u7f02\\u64b3\\u74e8\\u951b?\*

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| uid | java.lang.String | \\u93c2\\u56e6\\u6b22\\u9428\\u52eb\\u656e\\u6d93\\u20ac\\u93cd\\u56ea\\u7611 |
| sheetName | java.lang.String | \\u5bb8\\u30e4\\u7d94\\u741b\\u3125\\u6095\\u7ec9?\* @param fileName \\u9358\\u71b7\\ue750\\u93c2\\u56e6\\u6b22\\u935a?\* @return JSON \\u701b\\u6943\\ue0c1\\u6d93? |
| fileName | java.lang.String |  |

**Returns:**
java.lang.String
### getUidForFile(String fileName) {#getUidForFile-java.lang.String-}
```
public static String getUidForFile(String fileName)
```


Genera un nuevo id único para la caché de archivos usando el nombre de archivo proporcionado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | java.lang.String | El nombre del archivo. |

**Returns:**
java.lang.String -
### getWorkbookJsonWithCache(String uid, String fileName) {#getWorkbookJsonWithCache-java.lang.String-java.lang.String-}
```
public String getWorkbookJsonWithCache(String uid, String fileName)
```


\\u947e\\u5cf0\\u5f47\\u93c1\\u7fe0\\u91dc\\u5bb8\\u30e4\\u7d94\\u7ee8\\u8de8\\u6b91 JSON\\u951b\\u581d\\u752b\\u7f02\\u64b3\\u74e8\\u951b?\*

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| uid | java.lang.String | \\u93c2\\u56e6\\u6b22\\u9428\\u52eb\\u656e\\u6d93\\u20ac\\u93cd\\u56ea\\u7611 |
| fileName | java.lang.String | \\u9358\\u71b7\\ue750\\u93c2\\u56e6\\u6b22\\u935a?\* @return JSON \\u701b\\u6943\\ue0c1\\u6d93? |

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### importExcelFile(InputStream filestream, int format) {#importExcelFile-java.io.InputStream-int-}
```
public void importExcelFile(InputStream filestream, int format)
```


Importa el archivo Excel desde el flujo de archivo con formato de carga.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| filestream | java.io.InputStream | El flujo del archivo Excel. |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat). El LoadFormat del archivo Excel. |

### importExcelFile(InputStream filestream, int format, String password) {#importExcelFile-java.io.InputStream-int-java.lang.String-}
```
public void importExcelFile(InputStream filestream, int format, String password)
```


Importa el archivo Excel desde el flujo de archivo con formato de carga y contraseña de apertura.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| filestream | java.io.InputStream | El flujo del archivo Excel. |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat). El LoadFormat del archivo Excel. |
| password | java.lang.String | La contraseña de apertura del archivo Excel. El valor puede ser nulo si no se establece una contraseña. |

### importExcelFile(String fileName) {#importExcelFile-java.lang.String-}
```
public void importExcelFile(String fileName)
```


Importa el archivo Excel desde la ruta del archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | java.lang.String | La ruta completa del archivo. |

### importExcelFile(String uid, InputStream filestream, int format) {#importExcelFile-java.lang.String-java.io.InputStream-int-}
```
public void importExcelFile(String uid, InputStream filestream, int format)
```


Importa el archivo Excel desde el flujo de archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| uid | java.lang.String | El id único para la caché de archivos, si se establece en nulo, se generará automáticamente. |
| filestream | java.io.InputStream | El flujo del archivo Excel. |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat). El LoadFormat del archivo Excel. |

### importExcelFile(String uid, InputStream filestream, int format, String password) {#importExcelFile-java.lang.String-java.io.InputStream-int-java.lang.String-}
```
public void importExcelFile(String uid, InputStream filestream, int format, String password)
```


Importa el archivo Excel desde el flujo de archivo con formato de carga y contraseña de apertura.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| uid | java.lang.String | El id único para la caché de archivos, si se establece en nulo, se generará automáticamente. |
| filestream | java.io.InputStream | El flujo del archivo Excel. |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat). El LoadFormat del archivo Excel. |
| password | java.lang.String | La contraseña de apertura del archivo Excel. El valor puede ser nulo si no se establece una contraseña |

### importExcelFile(String uid, String fileName) {#importExcelFile-java.lang.String-java.lang.String-}
```
public void importExcelFile(String uid, String fileName)
```


Importa el archivo Excel desde la ruta del archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| uid | java.lang.String | El id único para la caché de archivos, si se establece en nulo, se generará automáticamente. |
| fileName | java.lang.String | La ruta completa del archivo. |

### importExcelFile(String uid, String fileName, String password) {#importExcelFile-java.lang.String-java.lang.String-java.lang.String-}
```
public void importExcelFile(String uid, String fileName, String password)
```


Importa el archivo Excel desde la ruta del archivo y contraseña de apertura.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| uid | java.lang.String | El id único para la caché de archivos, si se establece en nulo, se generará automáticamente. |
| fileName | java.lang.String | La ruta completa del archivo. |
| password | java.lang.String | La contraseña de apertura del archivo Excel. El valor puede ser nulo si no se establece una contraseña. |

### importExcelFileFromJson(String json) {#importExcelFileFromJson-java.lang.String-}
```
public void importExcelFileFromJson(String json)
```


Importa el archivo Excel desde una cadena en formato JSON.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| json | java.lang.String | La cadena con formato JSON. |

### insertImage(String uid, String p, InputStream s, String imageUrl) {#insertImage-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-}
```
public String insertImage(String uid, String p, InputStream s, String imageUrl)
```


Inserta una imagen en la hoja de cálculo desde el flujo de archivo o la URL, (se debe proporcionar el flujo de archivo o la URL) o inserta una forma, cuando p.type es uno de AutoShapeType

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| uid | java.lang.String | El id único para la caché de archivos |
| p | java.lang.String | La cadena con formato JSON para la operación que especifica la ubicación de la celda, el nombre de la hoja, la fila superior izquierda y la columna superior izquierda para la imagen\\u951b\\u5b94tc \{name:'sheet1',ri:1,ci:1\} |
| s | java.io.InputStream | El flujo de archivo de la imagen |
| imageUrl | java.lang.String | La URL del archivo de imagen |

**Returns:**
java.lang.String - La cadena con formato JSON de la imagen insertada
### jsonToStream(OutputStream stream, String filename) {#jsonToStream-java.io.OutputStream-java.lang.String-}
```
public void jsonToStream(OutputStream stream, String filename)
```


Genera JSON a partir del Workbook en memoria y lo escribe en el flujo especificado. Opcionalmente almacena en caché el JSON generado para una recuperación posterior más rápida. Diferencias clave con JsonToStreamByUid: - Este método usa el estado actual del Workbook en memoria (campo wb) - JsonToStreamByUid recarga el Workbook desde los archivos de caché .cells en disco - Usa este método cuando deseas exportar el estado actual del workbook después de modificaciones - Usa JsonToStreamByUid cuando necesitas regenerar JSON a partir de un estado de archivo previamente almacenado en caché. Comportamiento de caché (cuando se proporciona uid): - Verifica la caché de JSON antes de generar (memoria L1 + disco L2) - Si hay una falta de caché, genera JSON desde el workbook en memoria - Almacena el JSON generado en caché para futuras solicitudes

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.OutputStream | El flujo de salida donde escribir los datos JSON |
| nombre de archivo | java.lang.String | Especifica el nombre de archivo en el JSON. Si se establece en null, el nombre de archivo predeterminado es: book1. |

### jsonToStream(OutputStream stream, String filename, String uid) {#jsonToStream-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public void jsonToStream(OutputStream stream, String filename, String uid)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.OutputStream |  |
| nombre de archivo | java.lang.String |  |
| uid | java.lang.String |  |

### jsonToStreamByUid(OutputStream stream, String uid, String filename) {#jsonToStreamByUid-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public boolean jsonToStreamByUid(OutputStream stream, String uid, String filename)
```


Recupera la cadena JSON del archivo de la caché usando el id único especificado,establezca el nombre de archivo de salida en el JSON,y escríbalo en el flujo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.OutputStream | El flujo que se escribirá |
| uid | java.lang.String | El id único para la caché de archivos. |
| nombre de archivo | java.lang.String | Especifica el nombre de archivo en el JSON. Si se establece en null, el nombre de archivo predeterminado es: book1. |

**Returns:**
boolean
### lazyLoadingJson(String uid, String sheetName) {#lazyLoadingJson-java.lang.String-java.lang.String-}
```
public StringBuilder lazyLoadingJson(String uid, String sheetName)
```


Obtiene la cadena JSON de la hoja especificada en el archivo desde la caché usando el ID único especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| uid | java.lang.String | El id único para la caché de archivos. |
| sheetName | java.lang.String | el nombre de la hoja. |

**Returns:**
java.lang.StringBuilder - El StringBuilder de cadena JSON
### lazyLoadingStream(OutputStream stream, String uid, String sheetName) {#lazyLoadingStream-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public void lazyLoadingStream(OutputStream stream, String uid, String sheetName)
```


Recupera la cadena JSON de la hoja especificada en el archivo de la caché usando el id único especificado, y escríbala en el flujo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.OutputStream | El flujo que se escribirá |
| uid | java.lang.String | El id único para la caché de archivos. |
| sheetName | java.lang.String | el nombre de la hoja. |

### mergeExcelFileFromJson(String uid, String json) {#mergeExcelFileFromJson-java.lang.String-java.lang.String-}
```
public void mergeExcelFileFromJson(String uid, String json)
```


Aplica una actualización por lotes a los datos en memoria.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| uid | java.lang.String | El id único para la caché de archivos. |
| json | java.lang.String | La cadena con formato JSON de actualización. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### redactFile(String excelFilePath, String uid, String[] arrayOfRedactionOpr) {#redactFile-java.lang.String-java.lang.String-java.lang.String---}
```
public void redactFile(String excelFilePath, String uid, String[] arrayOfRedactionOpr)
```


Realiza una redacción en un archivo Excel basado en una matriz de operaciones JSON.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| excelFilePath | java.lang.String | La ruta del archivo Excel que será redactado. |
| uid | java.lang.String | El identificador único del libro de trabajo. Si es nulo o vacío, se generará un nuevo uid basado en la ruta del archivo. |
| arrayOfRedactionOpr | java.lang.String[] | Una matriz de cadenas JSON que representan las operaciones de redacción a aplicar. |

### saveToCacheWithFileName(String uid, String filename, String password) {#saveToCacheWithFileName-java.lang.String-java.lang.String-java.lang.String-}
```
public void saveToCacheWithFileName(String uid, String filename, String password)
```


Guarda los datos en memoria en el archivo de caché con el nombre de archivo especificado y también establece la contraseña de apertura, el formato de guardado se basa en la extensión del archivo del nombre de archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| uid | java.lang.String | El id único para la caché de archivos. |
| nombre de archivo | java.lang.String | El nombre de archivo para guardar. |
| password | java.lang.String | La contraseña de apertura del archivo Excel. El valor puede ser nulo si no se establece ninguna contraseña. |

### saveToExcelFile(OutputStream stream) {#saveToExcelFile-java.io.OutputStream-}
```
public void saveToExcelFile(OutputStream stream)
```


Guarda los datos en memoria en el flujo, basado en el formato de archivo original.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.OutputStream | El flujo para guardar. |

### saveToExcelFile(String path) {#saveToExcelFile-java.lang.String-}
```
public void saveToExcelFile(String path)
```


Guarda los datos en memoria en la ruta del archivo, si el archivo tiene extensión, el formato de guardado se basa en la extensión del archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ruta | java.lang.String | La ruta del archivo para guardar. |

### saveToHtml(OutputStream stream) {#saveToHtml-java.io.OutputStream-}
```
public void saveToHtml(OutputStream stream)
```


Guarda los datos en memoria en el flujo, el formato de guardado es html

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.OutputStream | El flujo para guardar. |

### saveToHtml(String path) {#saveToHtml-java.lang.String-}
```
public void saveToHtml(String path)
```


Guarda los datos en memoria en la ruta del archivo, el formato de guardado es html.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ruta | java.lang.String | La ruta del archivo para guardar. |

### saveToPdf(OutputStream stream) {#saveToPdf-java.io.OutputStream-}
```
public void saveToPdf(OutputStream stream)
```


Guarda los datos en memoria en el flujo, el formato de guardado es pdf.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.OutputStream | El flujo para guardar. |

### saveToPdf(String path) {#saveToPdf-java.lang.String-}
```
public void saveToPdf(String path)
```


Guarda los datos de memoria en la ruta del archivo, el formato de guardado es pdf.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ruta | java.lang.String | La ruta del archivo para guardar. |

### saveToXlsx(OutputStream stream) {#saveToXlsx-java.io.OutputStream-}
```
public void saveToXlsx(OutputStream stream)
```


Guarda los datos de memoria en el flujo, el formato de guardado es xlsx.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.OutputStream | El flujo para guardar. |

### saveToXlsx(String path) {#saveToXlsx-java.lang.String-}
```
public void saveToXlsx(String path)
```


Guarda los datos de memoria en la ruta del archivo, el formato de guardado es xlsx.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ruta | java.lang.String | La ruta del archivo para guardar. |

### setCacheDirectory(String value) {#setCacheDirectory-java.lang.String-}
```
public void setCacheDirectory(String value)
```


Establece el directorio de caché para almacenar el archivo de hoja de cálculo. Si no se establece, usaremos la propiedad estática de [Config.getFileCacheDirectory()](../../com.aspose.gridjs/config\#getFileCacheDirectory--) o [CacheImp](../../com.aspose.gridjs/gridjsworkbook\#CacheImp).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setImageUrlBase(String baseImageURL) {#setImageUrlBase-java.lang.String-}
```
public static void setImageUrlBase(String baseImageURL)
```


Establece la URL de acción de obtención de la imagen base desde el controlador.

**Remarks**

Cuando CacheImp es nulo, necesitamos establecer esto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| baseImageURL | java.lang.String | La URL de la acción de obtención de la imagen base. |

### setInterruptMonitorForLoad(GridInterruptMonitor monitor, int calculateTimeoutMilliseconds) {#setInterruptMonitorForLoad-com.aspose.gridjs.GridInterruptMonitor-int-}
```
public void setInterruptMonitorForLoad(GridInterruptMonitor monitor, int calculateTimeoutMilliseconds)
```


Establece InterruptMonitor para la operación de carga.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| monitor | [GridInterruptMonitor](../../com.aspose.gridjs/gridinterruptmonitor) | La instancia de InterruptMonitor. |
| calculateTimeoutMilliseconds | int | El tiempo de espera en milisegundos para cargar el archivo. |

### setInterruptMonitorForSave(GridInterruptMonitor monitor) {#setInterruptMonitorForSave-com.aspose.gridjs.GridInterruptMonitor-}
```
public void setInterruptMonitorForSave(GridInterruptMonitor monitor)
```


Establece InterruptMonitor para la operación de guardado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| monitor | [GridInterruptMonitor](../../com.aspose.gridjs/gridinterruptmonitor) | La instancia de InterruptMonitor. |

### setSettings(GridWorkbookSettings value) {#setSettings-com.aspose.gridjs.GridWorkbookSettings-}
```
public void setSettings(GridWorkbookSettings value)
```


Representa la configuración del libro de trabajo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [GridWorkbookSettings](../../com.aspose.gridjs/gridworkbooksettings) |  |

### setTransParentView(String excelFilePath, String uid, boolean isTransparent) {#setTransParentView-java.lang.String-java.lang.String-boolean-}
```
public void setTransParentView(String excelFilePath, String uid, boolean isTransparent)
```


Establece la transparencia de las formas de redacción en el libro de trabajo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| excelFilePath | java.lang.String | La ruta del archivo Excel. |
| uid | java.lang.String | El identificador único del libro de trabajo. Si es nulo o vacío, se generará un nuevo uid basado en la ruta del archivo. |
| isTransparent | boolean | Si es verdadero, establece la transparencia a 0.89 (semi-transparente); si es falso, establece la transparencia a 1 (completamente opaco/invisible). |

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
java.lang.String - La cadena en formato JSON del resultado de la actualización.
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

