---
title: "Configuración"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa todas las configuraciones estáticas para GridJs"
type: docs
url: /es/java/com.aspose.gridjs/config/
---

**Inheritance:**
java.lang.Object
```
public class Config
```

Representa todas las configuraciones estáticas para GridJs
## Constructores

| Constructor | Descripción |
| --- | --- |
| [Config()](#Config--) |  |
## Campos

| Campo | Descripción |
| --- | --- |
| [RedactionUseClientGenerateId](#RedactionUseClientGenerateId) | Indica si se usa el ID generado por el cliente en lugar del ID real de la forma en operaciones relacionadas con la redacción |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFitColumnsOnLoad()](#getAutoFitColumnsOnLoad--) | Indica si se ajustan automáticamente los anchos de columna durante la carga del archivo. |
| [getAutoFitRowsHeightOnLoad()](#getAutoFitRowsHeightOnLoad--) | Indica si se ajustan automáticamente las alturas de fila durante la carga del archivo. |
| [getAutoOptimizeForLargeCells()](#getAutoOptimizeForLargeCells--) | Obtiene si se debe optimizar automáticamente el rendimiento de carga para la hoja de cálculo con celdas grandes. |
| [getBaseRouteName()](#getBaseRouteName--) | Obtiene el nombre de ruta base para la URL del controlador GridJs. el valor predeterminado es "/GridJs2". |
| [getClass()](#getClass--) |  |
| [getEmptySheetMaxCol()](#getEmptySheetMaxCol--) | Obtiene la columna máxima predeterminada para una hoja de cálculo vacía. |
| [getEmptySheetMaxRow()](#getEmptySheetMaxRow--) | Obtiene la fila máxima predeterminada para una hoja de cálculo vacía. |
| [getEnableChartClientRendering()](#getEnableChartClientRendering--) | Obtiene si se debe habilitar la renderización de gráficos del lado del cliente. |
| [getFileCacheDirectory()](#getFileCacheDirectory--) | Obtiene el directorio de caché para almacenar el archivo de hoja de cálculo. |
| [getIgnoreEmptyContent()](#getIgnoreEmptyContent--) | Obtiene si se debe mostrar el rango máximo que incluye datos, estilo, celdas combinadas y formas. |
| [getIslimitShapeOrImage()](#getIslimitShapeOrImage--) | Obtiene si se debe limitar el recuento total de formas/imagenes mostradas en una hoja de cálculo; si se establece en true, GridJs limitará el recuento total de formas o imágenes mostradas en una hoja de cálculo a MaxShapeOrImageCount, el valor predeterminado es true. |
| [getJsonCache()](#getJsonCache--) | Obtiene las opciones de configuración de caché JSON. |
| [getLazyLoading()](#getLazyLoading--) | Obtiene si se debe cargar solo la hoja de cálculo activa, el valor predeterminado es false. |
| [getMaxPdfSaveSeconds()](#getMaxPdfSaveSeconds--) | Obtiene los segundos máximos de tiempo de espera al guardar en PDF. |
| [getMaxShapeOrImageCount()](#getMaxShapeOrImageCount--) | Obtiene el recuento total de formas o imágenes mostradas en la hoja activa, tiene efecto cuando IslimitShapeOrImage=true. |
| [getMaxShapeOrImageWidthOrHeight()](#getMaxShapeOrImageWidthOrHeight--) | Obtiene el ancho o altura máximos para una forma o una imagen, GridJs ignorará la forma o imagen con un ancho o altura mayor a este valor, tiene efecto cuando IslimitShapeOrImage=true. |
| [getMaxTotalShapeOrImageCount()](#getMaxTotalShapeOrImageCount--) | Obtiene el recuento total de formas o imágenes mostradas en el libro de trabajo, tiene efecto cuando IslimitShapeOrImage=true. |
| [getMessageTopic()](#getMessageTopic--) | Obtiene los destinos de websocket con el prefijo "/topic". El valor predeterminado es "/topic/opr". Se usa solo en modo colaborativo. |
| [getPictureCacheDirectory()](#getPictureCacheDirectory--) | Obtiene el directorio de caché para imágenes. |
| [getSameImageDetecting()](#getSameImageDetecting--) | Obtiene si se debe comprobar si las imágenes tienen la misma fuente, el valor predeterminado es true. |
| [getSaveHtmlAsZip()](#getSaveHtmlAsZip--) | Obtiene si se debe guardar el archivo HTML como archivo zip, el valor predeterminado es false. |
| [getShowChartSheet()](#getShowChartSheet--) | Obtiene si se debe mostrar la hoja de gráficos. |
| [getSkipInvisibleShapes()](#getSkipInvisibleShapes--) | Obtiene si se deben omitir las formas que son invisibles para la UI, el valor predeterminado es true. |
| [getUsePrintArea()](#getUsePrintArea--) | Obtiene si se debe usar PageSetup.PrintArea para el rango de visualización de la UI cuando la hoja de cálculo tiene la configuración PageSetup para PrintArea. |
| [hashCode()](#hashCode--) |  |
| [isCollaborative()](#isCollaborative--) | Obtiene si se admite la edición colaborativa, el valor predeterminado es false. |
| [isWasm()](#isWasm--) | Obtiene si GridJs se ejecuta dentro de un host WebAssembly del navegador en lugar de un proceso de servidor. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFitColumnsOnLoad(boolean value)](#setAutoFitColumnsOnLoad-boolean-) | Indica si se ajustan automáticamente los anchos de columna durante la carga del archivo. |
| [setAutoFitRowsHeightOnLoad(boolean value)](#setAutoFitRowsHeightOnLoad-boolean-) | Indica si se ajustan automáticamente las alturas de fila durante la carga del archivo. |
| [setAutoOptimizeForLargeCells(boolean value)](#setAutoOptimizeForLargeCells-boolean-) | Establece si se debe optimizar automáticamente el rendimiento de carga para hojas de cálculo con celdas grandes. |
| [setBaseRouteName(String value)](#setBaseRouteName-java.lang.String-) | Establece el nombre de ruta base para la URL del controlador GridJs. el valor predeterminado es "/GridJs2". |
| [setCollaborative(boolean value)](#setCollaborative-boolean-) | Establece si se admite la edición colaborativa, el valor predeterminado es false. |
| [setEmptySheetMaxCol(int value)](#setEmptySheetMaxCol-int-) | Establece la columna máxima predeterminada para una hoja de cálculo vacía. |
| [setEmptySheetMaxRow(int value)](#setEmptySheetMaxRow-int-) | Establece la fila máxima predeterminada para una hoja de cálculo vacía. |
| [setEnableChartClientRendering(boolean value)](#setEnableChartClientRendering-boolean-) | Establece si se debe habilitar la renderización de gráficos del lado del cliente. |
| [setFileCacheDirectory(String value)](#setFileCacheDirectory-java.lang.String-) | Establece el directorio de caché para almacenar el archivo de hoja de cálculo. |
| [setFontFolder(String fontFolder, boolean recursive)](#setFontFolder-java.lang.String-boolean-) | Establece la carpeta de fuentes |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Establece las carpetas de fuentes |
| [setIgnoreEmptyContent(boolean value)](#setIgnoreEmptyContent-boolean-) | Establece si se debe mostrar el rango máximo que incluye datos, estilo, celdas combinadas y formas. |
| [setIslimitShapeOrImage(boolean value)](#setIslimitShapeOrImage-boolean-) | Establece si se debe limitar el recuento total de formas/imagenes mostradas en una hoja de cálculo, si se establece en true, GridJs limitará el recuento total de formas o imágenes mostradas en una hoja de cálculo a MaxShapeOrImageCount, el valor predeterminado es true. |
| [setJsonCache(JsonCacheOptions value)](#setJsonCache-com.aspose.gridjs.JsonCacheOptions-) | Establece las opciones de configuración de caché JSON. |
| [setLazyLoading(boolean value)](#setLazyLoading-boolean-) | Establece si se debe cargar solo la hoja de cálculo activa, el valor predeterminado es false. |
| [setMaxPdfSaveSeconds(int value)](#setMaxPdfSaveSeconds-int-) | Establece los segundos máximos de tiempo de espera al guardar en PDF. |
| [setMaxShapeOrImageCount(int value)](#setMaxShapeOrImageCount-int-) | Establece el recuento total de formas o imágenes mostradas en la hoja activa, tiene efecto cuando IslimitShapeOrImage=true. |
| [setMaxShapeOrImageWidthOrHeight(int value)](#setMaxShapeOrImageWidthOrHeight-int-) | Establece el ancho o alto máximo para una forma o una imagen, GridJs ignorará la forma o imagen con un ancho o alto mayor que este, tiene efecto cuando IslimitShapeOrImage=true. |
| [setMaxTotalShapeOrImageCount(int value)](#setMaxTotalShapeOrImageCount-int-) | Establece el recuento total de formas o imágenes mostradas en el libro de trabajo, tiene efecto cuando IslimitShapeOrImage=true. |
| [setMessageTopic(String value)](#setMessageTopic-java.lang.String-) | Establece los destinos de websocket con el prefijo "/topic". el valor predeterminado es "/topic/opr". usado solo en modo colaborativo. |
| [setPictureCacheDirectory(String value)](#setPictureCacheDirectory-java.lang.String-) | Establece el directorio de caché para imágenes. |
| [setSameImageDetecting(boolean value)](#setSameImageDetecting-boolean-) | Establece si se debe comprobar si las imágenes tienen la misma fuente, el valor predeterminado es true el valor predeterminado es true. |
| [setSaveHtmlAsZip(boolean value)](#setSaveHtmlAsZip-boolean-) | Establece si se debe guardar el archivo html como archivo zip, el valor predeterminado es false. |
| [setShowChartSheet(boolean value)](#setShowChartSheet-boolean-) | Establece si se debe mostrar la hoja de gráficos. |
| [setSkipInvisibleShapes(boolean value)](#setSkipInvisibleShapes-boolean-) | Establece si se omiten las formas que son invisibles para la UI, el valor predeterminado es true. |
| [setUsePrintArea(boolean value)](#setUsePrintArea-boolean-) | Establece si se usa PageSetup.PrintArea para el rango de visualización de la UI cuando la hoja de cálculo tiene la configuración PageSetup para PrintArea. |
| [setWasm(boolean value)](#setWasm-boolean-) | Establece si GridJs se ejecuta dentro de un host WebAssembly del navegador en lugar de un proceso del servidor. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Config() {#Config--}
```
public Config()
```


### RedactionUseClientGenerateId {#RedactionUseClientGenerateId}
```
public static boolean RedactionUseClientGenerateId
```


Indica si se usa el ID generado por el cliente en lugar del ID real de la forma en operaciones relacionadas con la redacción

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
### getAutoFitColumnsOnLoad() {#getAutoFitColumnsOnLoad--}
```
public static boolean getAutoFitColumnsOnLoad()
```


Indica si se ajustan automáticamente los anchos de columna durante la carga del archivo. El valor predeterminado es `false`. Advertencia: Configurar esto a `true` realizará una operación de ajuste automático de todas las columnas después de la carga, lo que puede tener un impacto notable en el rendimiento.

**Returns:**
boolean
### getAutoFitRowsHeightOnLoad() {#getAutoFitRowsHeightOnLoad--}
```
public static boolean getAutoFitRowsHeightOnLoad()
```


Indica si se ajustan automáticamente las alturas de fila durante la carga del archivo. El valor predeterminado es `false`. Advertencia: Configurar esto a `true` realizará una operación de ajuste automático de todas las filas después de la carga, lo que puede tener un impacto notable en el rendimiento.

**Returns:**
boolean
### getAutoOptimizeForLargeCells() {#getAutoOptimizeForLargeCells--}
```
public static boolean getAutoOptimizeForLargeCells()
```


Obtiene si se optimiza automáticamente el rendimiento de carga para hojas de cálculo con celdas grandes. Ignorará algunos estilos /bordes para reducir el tiempo de carga. El valor predeterminado es true.

**Returns:**
boolean
### getBaseRouteName() {#getBaseRouteName--}
```
public static String getBaseRouteName()
```


Obtiene el nombre de ruta base para la URL del controlador GridJs. el valor predeterminado es "/GridJs2".

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEmptySheetMaxCol() {#getEmptySheetMaxCol--}
```
public static int getEmptySheetMaxCol()
```


Obtiene la columna máxima predeterminada para una hoja de cálculo vacía. El valor predeterminado es 15.

**Returns:**
int
### getEmptySheetMaxRow() {#getEmptySheetMaxRow--}
```
public static int getEmptySheetMaxRow()
```


Obtiene la fila máxima predeterminada para una hoja de cálculo vacía. El valor predeterminado es 12.

**Returns:**
int
### getEnableChartClientRendering() {#getEnableChartClientRendering--}
```
public static boolean getEnableChartClientRendering()
```


Obtiene si se habilita la renderización de gráficos del lado del cliente. Si se establece en false, GridJs recurrirá solo a imágenes/formas de gráficos generadas por el servidor. el valor predeterminado es true.

**Returns:**
boolean
### getFileCacheDirectory() {#getFileCacheDirectory--}
```
public static String getFileCacheDirectory()
```


Obtiene el directorio de caché para almacenar el archivo de hoja de cálculo. Necesitamos configurarlo en una ruta específica antes de usar GridJs.

**Returns:**
java.lang.String
### getIgnoreEmptyContent() {#getIgnoreEmptyContent--}
```
public static boolean getIgnoreEmptyContent()
```


Obtiene si se muestra el rango máximo que incluye datos, estilo, celdas combinadas y formas. Si la última fila o columna contiene celdas sin valor ni fórmula pero con estilo personalizado, entonces no mostraremos esa fila/columna cuando este valor sea true\\u9286?\\* el valor predeterminado es true.

**Returns:**
boolean
### getIslimitShapeOrImage() {#getIslimitShapeOrImage--}
```
public static boolean getIslimitShapeOrImage()
```


Obtiene si se debe limitar el recuento total de formas/imagenes mostradas en una hoja de cálculo; si se establece en true, GridJs limitará el recuento total de formas o imágenes mostradas en una hoja de cálculo a MaxShapeOrImageCount, el valor predeterminado es true.

**Returns:**
boolean
### getJsonCache() {#getJsonCache--}
```
public static JsonCacheOptions getJsonCache()
```


Obtiene las opciones de configuración de caché JSON. Controla tanto el comportamiento de la caché en memoria (L1) como en disco (L2) para el JSON del libro de trabajo generado.

**Returns:**
[JsonCacheOptions](../../com.aspose.gridjs/jsoncacheoptions)
### getLazyLoading() {#getLazyLoading--}
```
public static boolean getLazyLoading()
```


Obtiene si se debe cargar solo la hoja de cálculo activa, el valor predeterminado es false.

**Returns:**
boolean
### getMaxPdfSaveSeconds() {#getMaxPdfSaveSeconds--}
```
public static int getMaxPdfSaveSeconds()
```


Obtiene el número máximo de segundos de tiempo de espera al guardar en PDF. El valor predeterminado es 10.

**Returns:**
int
### getMaxShapeOrImageCount() {#getMaxShapeOrImageCount--}
```
public static int getMaxShapeOrImageCount()
```


Obtiene el recuento total de las formas o imágenes mostradas en la hoja activa, tiene efecto cuando IslimitShapeOrImage=true. El valor predeterminado es 100.

**Returns:**
int
### getMaxShapeOrImageWidthOrHeight() {#getMaxShapeOrImageWidthOrHeight--}
```
public static int getMaxShapeOrImageWidthOrHeight()
```


Obtiene el ancho o alto máximo para una forma o una imagen, GridJs ignorará la forma o imagen con un ancho o alto mayor que este valor, tiene efecto cuando IslimitShapeOrImage=true. El valor predeterminado es 10000.

**Returns:**
int
### getMaxTotalShapeOrImageCount() {#getMaxTotalShapeOrImageCount--}
```
public static int getMaxTotalShapeOrImageCount()
```


Obtiene el recuento total de las formas o imágenes mostradas en el libro de trabajo, tiene efecto cuando IslimitShapeOrImage=true. El valor predeterminado es 300.

**Returns:**
int
### getMessageTopic() {#getMessageTopic--}
```
public static String getMessageTopic()
```


Obtiene los destinos de websocket con el prefijo "/topic". El valor predeterminado es "/topic/opr". Se usa solo en modo colaborativo.

**Returns:**
java.lang.String
### getPictureCacheDirectory() {#getPictureCacheDirectory--}
```
public static String getPictureCacheDirectory()
```


Obtiene el directorio de caché para imágenes. (esto tiene efecto cuando GridJsWorkbook.CacheImp es null) la ruta predeterminada será "\\_piccache" dentro de FileCacheDirectory.

**Returns:**
java.lang.String
### getSameImageDetecting() {#getSameImageDetecting--}
```
public static boolean getSameImageDetecting()
```


Obtiene si se debe comprobar si las imágenes tienen la misma fuente, el valor predeterminado es true.

**Returns:**
boolean
### getSaveHtmlAsZip() {#getSaveHtmlAsZip--}
```
public static boolean getSaveHtmlAsZip()
```


Obtiene si se debe guardar el archivo HTML como archivo zip, el valor predeterminado es false.

**Returns:**
boolean
### getShowChartSheet() {#getShowChartSheet--}
```
public static boolean getShowChartSheet()
```


Obtiene si se muestra la hoja de gráficos. El valor predeterminado es false.

**Returns:**
boolean
### getSkipInvisibleShapes() {#getSkipInvisibleShapes--}
```
public static boolean getSkipInvisibleShapes()
```


Obtiene si se deben omitir las formas que son invisibles para la UI, el valor predeterminado es true.

**Returns:**
boolean
### getUsePrintArea() {#getUsePrintArea--}
```
public static boolean getUsePrintArea()
```


Obtiene si se usa PageSetup.PrintArea para el rango de visualización de la UI cuando la hoja de cálculo tiene la configuración PageSetup para PrintArea. El valor predeterminado es false.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCollaborative() {#isCollaborative--}
```
public static boolean isCollaborative()
```


Obtiene si se admite la edición colaborativa, el valor predeterminado es false.

**Returns:**
boolean
### isWasm() {#isWasm--}
```
public static boolean isWasm()
```


Obtiene si GridJs se ejecuta dentro de un host WebAssembly del navegador en lugar de un proceso de servidor. Cuando es true, no se utiliza la ruta FileCacheDirectory / disco / hilo de interrupción y la caché de archivos debe provenir de GridJsOptions.CacheImp. GridJsOptions.IsWasm establece esto cuando se construye el servicio GridJs, de modo que un solo Aspose.Cells.GridJs.dll sirve a ambos hosts. el valor predeterminado es false.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAutoFitColumnsOnLoad(boolean value) {#setAutoFitColumnsOnLoad-boolean-}
```
public static void setAutoFitColumnsOnLoad(boolean value)
```


Indica si se ajustan automáticamente los anchos de columna durante la carga del archivo. El valor predeterminado es `false`. Advertencia: Configurar esto a `true` realizará una operación de ajuste automático de todas las columnas después de la carga, lo que puede tener un impacto notable en el rendimiento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAutoFitRowsHeightOnLoad(boolean value) {#setAutoFitRowsHeightOnLoad-boolean-}
```
public static void setAutoFitRowsHeightOnLoad(boolean value)
```


Indica si se ajustan automáticamente las alturas de fila durante la carga del archivo. El valor predeterminado es `false`. Advertencia: Configurar esto a `true` realizará una operación de ajuste automático de todas las filas después de la carga, lo que puede tener un impacto notable en el rendimiento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAutoOptimizeForLargeCells(boolean value) {#setAutoOptimizeForLargeCells-boolean-}
```
public static void setAutoOptimizeForLargeCells(boolean value)
```


Establece si se optimiza automáticamente el rendimiento de carga para hojas de cálculo con celdas grandes. Ignorará algunos estilos /bordes para reducir el tiempo de carga. El valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setBaseRouteName(String value) {#setBaseRouteName-java.lang.String-}
```
public static void setBaseRouteName(String value)
```


Establece el nombre de ruta base para la URL del controlador GridJs. el valor predeterminado es "/GridJs2".

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setCollaborative(boolean value) {#setCollaborative-boolean-}
```
public static void setCollaborative(boolean value)
```


Establece si se admite la edición colaborativa, el valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEmptySheetMaxCol(int value) {#setEmptySheetMaxCol-int-}
```
public static void setEmptySheetMaxCol(int value)
```


Establece la columna máxima predeterminada para una hoja de cálculo vacía. El valor predeterminado es 15.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setEmptySheetMaxRow(int value) {#setEmptySheetMaxRow-int-}
```
public static void setEmptySheetMaxRow(int value)
```


Establece la fila máxima predeterminada para una hoja de cálculo vacía. El valor predeterminado es 12.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setEnableChartClientRendering(boolean value) {#setEnableChartClientRendering-boolean-}
```
public static void setEnableChartClientRendering(boolean value)
```


Establece si se habilita la renderización de gráficos del lado del cliente. Si se establece en false, GridJs recurrirá solo a imágenes/formas de gráficos generadas por el servidor. el valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setFileCacheDirectory(String value) {#setFileCacheDirectory-java.lang.String-}
```
public static void setFileCacheDirectory(String value)
```


Establece el directorio de caché para almacenar el archivo de hoja de cálculo. Necesitamos configurarlo en una ruta específica antes de usar GridJs.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setFontFolder(String fontFolder, boolean recursive) {#setFontFolder-java.lang.String-boolean-}
```
public static void setFontFolder(String fontFolder, boolean recursive)
```


Establece la carpeta de fuentes

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fontFolder | java.lang.String | La carpeta que contiene fuentes TrueType. |
| recursive | boolean | Determina si se deben escanear o no las subcarpetas. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public static void setFontFolders(String[] fontFolders, boolean recursive)
```


Establece las carpetas de fuentes

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fontFolders | java.lang.String[] | Las carpetas que contienen fuentes TrueType. |
| recursive | boolean | Determina si se deben escanear o no las subcarpetas. |

### setIgnoreEmptyContent(boolean value) {#setIgnoreEmptyContent-boolean-}
```
public static void setIgnoreEmptyContent(boolean value)
```


Establece si se muestra el rango máximo que incluye datos, estilo, celdas combinadas y formas. Si la última fila o columna contiene celdas sin valor ni fórmula pero con estilo personalizado, entonces no mostraremos esa fila/columna cuando este valor sea true\\u9286?\\* el valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setIslimitShapeOrImage(boolean value) {#setIslimitShapeOrImage-boolean-}
```
public static void setIslimitShapeOrImage(boolean value)
```


Establece si se debe limitar el recuento total de formas/imagenes mostradas en una hoja de cálculo, si se establece en true, GridJs limitará el recuento total de formas o imágenes mostradas en una hoja de cálculo a MaxShapeOrImageCount, el valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setJsonCache(JsonCacheOptions value) {#setJsonCache-com.aspose.gridjs.JsonCacheOptions-}
```
public static void setJsonCache(JsonCacheOptions value)
```


Establece opciones de configuración de caché JSON. Controla tanto el comportamiento de la caché en memoria (L1) como en disco (L2) para el JSON del libro de trabajo generado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [JsonCacheOptions](../../com.aspose.gridjs/jsoncacheoptions) |  |

### setLazyLoading(boolean value) {#setLazyLoading-boolean-}
```
public static void setLazyLoading(boolean value)
```


Establece si se debe cargar solo la hoja de cálculo activa, el valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setMaxPdfSaveSeconds(int value) {#setMaxPdfSaveSeconds-int-}
```
public static void setMaxPdfSaveSeconds(int value)
```


Establece el número máximo de segundos de tiempo de espera al guardar en PDF. el valor predeterminado es 10.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setMaxShapeOrImageCount(int value) {#setMaxShapeOrImageCount-int-}
```
public static void setMaxShapeOrImageCount(int value)
```


Establece el recuento total de formas o imágenes mostradas en la hoja activa, tiene efecto cuando IslimitShapeOrImage=true. el valor predeterminado es 100.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setMaxShapeOrImageWidthOrHeight(int value) {#setMaxShapeOrImageWidthOrHeight-int-}
```
public static void setMaxShapeOrImageWidthOrHeight(int value)
```


Establece el ancho o alto máximo para una forma o una imagen, GridJs ignorará la forma o imagen cuyo ancho o alto sea mayor que este valor, tiene efecto cuando IslimitShapeOrImage=true. el valor predeterminado es 10000.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setMaxTotalShapeOrImageCount(int value) {#setMaxTotalShapeOrImageCount-int-}
```
public static void setMaxTotalShapeOrImageCount(int value)
```


Establece el recuento total de formas o imágenes mostradas en el libro de trabajo, tiene efecto cuando IslimitShapeOrImage=true. el valor predeterminado es 300.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setMessageTopic(String value) {#setMessageTopic-java.lang.String-}
```
public static void setMessageTopic(String value)
```


Establece los destinos de websocket con el prefijo "/topic". el valor predeterminado es "/topic/opr". usado solo en modo colaborativo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setPictureCacheDirectory(String value) {#setPictureCacheDirectory-java.lang.String-}
```
public static void setPictureCacheDirectory(String value)
```


Establece el directorio de caché para imágenes. (esto tiene efecto cuando GridJsWorkbook.CacheImp es nulo) la ruta predeterminada será "\\_piccache" dentro de FileCacheDirectory.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setSameImageDetecting(boolean value) {#setSameImageDetecting-boolean-}
```
public static void setSameImageDetecting(boolean value)
```


Establece si se debe comprobar si las imágenes tienen la misma fuente, el valor predeterminado es true el valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSaveHtmlAsZip(boolean value) {#setSaveHtmlAsZip-boolean-}
```
public static void setSaveHtmlAsZip(boolean value)
```


Establece si se debe guardar el archivo html como archivo zip, el valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowChartSheet(boolean value) {#setShowChartSheet-boolean-}
```
public static void setShowChartSheet(boolean value)
```


Establece si se muestra la hoja de gráfico. el valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSkipInvisibleShapes(boolean value) {#setSkipInvisibleShapes-boolean-}
```
public static void setSkipInvisibleShapes(boolean value)
```


Establece si se omiten las formas que son invisibles para la UI, el valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setUsePrintArea(boolean value) {#setUsePrintArea-boolean-}
```
public static void setUsePrintArea(boolean value)
```


Establece si se usa PageSetup.PrintArea para el rango de visualización de la UI cuando la hoja tiene la configuración PageSetup para PrintArea. el valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setWasm(boolean value) {#setWasm-boolean-}
```
public static void setWasm(boolean value)
```


Establece si GridJs se ejecuta dentro de un host WebAssembly del navegador en lugar de un proceso de servidor. Cuando es true, no se utiliza la ruta FileCacheDirectory / disco / hilo de interrupción y la caché de archivos debe provenir de GridJsOptions.CacheImp. GridJsOptions.IsWasm establece esto cuando se construye el servicio GridJs, de modo que un solo Aspose.Cells.GridJs.dll sirve a ambos hosts. el valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

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

