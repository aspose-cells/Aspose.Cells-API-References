---
title: "GridJsOptions"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa todas las opciones de carga para GridJs"
type: docs
url: /es/java/com.aspose.gridjs/gridjsoptions/
---

**Inheritance:**
java.lang.Object
```
public class GridJsOptions
```

Representa todas las opciones de carga para GridJs
## Constructores

| Constructor | Descripción |
| --- | --- |
| [GridJsOptions()](#GridJsOptions--) |  |
## Campos

| Campo | Descripción |
| --- | --- |
| [CacheImp](#CacheImp) | Implementación personalizada para el almacenamiento en caché, si deseas almacenar la caché de forma continua, necesitas configurarla e implementarla. |
| [RedactionUseClientGenerateId](#RedactionUseClientGenerateId) | Indica si se usa el ID generado por el cliente en lugar del ID real de la forma en operaciones relacionadas con la redacción |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFitColumnsOnLoad()](#getAutoFitColumnsOnLoad--) | Indica si se ajusta automáticamente el ancho de las columnas al cargar el archivo, el valor predeterminado es false. |
| [getAutoFitRowsHeightOnLoad()](#getAutoFitRowsHeightOnLoad--) | Indica si se ajusta automáticamente la altura de las filas al cargar el archivo, el valor predeterminado es false. |
| [getAutoOptimizeForLargeCells()](#getAutoOptimizeForLargeCells--) | Obtiene si se debe optimizar automáticamente el rendimiento de carga para la hoja de cálculo con celdas grandes. |
| [getBaseRouteName()](#getBaseRouteName--) | Obtiene el nombre base de la URL de ruta para el controlador GridJs, el valor predeterminado es GridJs2. |
| [getClass()](#getClass--) |  |
| [getEmptySheetMaxCol()](#getEmptySheetMaxCol--) | Obtiene la columna máxima predeterminada para una hoja de cálculo vacía. |
| [getEmptySheetMaxRow()](#getEmptySheetMaxRow--) | Obtiene la fila máxima predeterminada para una hoja de cálculo vacía. |
| [getEnableChartClientRendering()](#getEnableChartClientRendering--) | Obtiene si se debe habilitar la renderización de gráficos del lado del cliente. |
| [getFileCacheDirectory()](#getFileCacheDirectory--) | Obtiene el directorio de caché para almacenar el archivo de hoja de cálculo. |
| [getFontFolders()](#getFontFolders--) | Obtiene las carpetas de fuentes para las fuentes en las imágenes/formas renderizadas. |
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
| [setAutoFitColumnsOnLoad(boolean value)](#setAutoFitColumnsOnLoad-boolean-) | Indica si se ajusta automáticamente el ancho de las columnas al cargar el archivo, el valor predeterminado es false. |
| [setAutoFitRowsHeightOnLoad(boolean value)](#setAutoFitRowsHeightOnLoad-boolean-) | Indica si se ajusta automáticamente la altura de las filas al cargar el archivo, el valor predeterminado es false. |
| [setAutoOptimizeForLargeCells(boolean value)](#setAutoOptimizeForLargeCells-boolean-) | Establece si se debe optimizar automáticamente el rendimiento de carga para hojas de cálculo con celdas grandes. |
| [setBaseRouteName(String value)](#setBaseRouteName-java.lang.String-) | Establece el nombre base de la URL de ruta para el controlador GridJs. el valor predeterminado es GridJs2 |
| [setCollaborative(boolean value)](#setCollaborative-boolean-) | Establece si se admite la edición colaborativa, el valor predeterminado es false. |
| [setEmptySheetMaxCol(int value)](#setEmptySheetMaxCol-int-) | Establece la columna máxima predeterminada para una hoja de cálculo vacía. |
| [setEmptySheetMaxRow(int value)](#setEmptySheetMaxRow-int-) | Establece la fila máxima predeterminada para una hoja de cálculo vacía. |
| [setEnableChartClientRendering(boolean value)](#setEnableChartClientRendering-boolean-) | Establece si se debe habilitar la renderización de gráficos del lado del cliente. |
| [setFileCacheDirectory(String value)](#setFileCacheDirectory-java.lang.String-) | Establece el directorio de caché para almacenar el archivo de hoja de cálculo. |
| [setFontFolders(String[] value)](#setFontFolders-java.lang.String---) | Establece las carpetas de fuentes para las fuentes en las imágenes/formas renderizadas |
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
### GridJsOptions() {#GridJsOptions--}
```
public GridJsOptions()
```


### CacheImp {#CacheImp}
```
public GridCacheForStream CacheImp
```


Implementación personalizada para el almacenamiento en caché. Si desea almacenar la caché de forma de flujo, necesita configurarla e implementarla. Un host WebAssembly (IsWasm = true) debe configurarla, porque no hay disco local para la caché de archivos predeterminada.

### RedactionUseClientGenerateId {#RedactionUseClientGenerateId}
```
public boolean RedactionUseClientGenerateId
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
public boolean getAutoFitColumnsOnLoad()
```


Indica si se ajusta automáticamente el ancho de las columnas al cargar el archivo, el valor predeterminado es false.

**Returns:**
boolean
### getAutoFitRowsHeightOnLoad() {#getAutoFitRowsHeightOnLoad--}
```
public boolean getAutoFitRowsHeightOnLoad()
```


Indica si se ajusta automáticamente la altura de las filas al cargar el archivo, el valor predeterminado es false.

**Returns:**
boolean
### getAutoOptimizeForLargeCells() {#getAutoOptimizeForLargeCells--}
```
public boolean getAutoOptimizeForLargeCells()
```


Obtiene si se optimiza automáticamente el rendimiento de carga para hojas de cálculo con celdas grandes. Ignorará algunos estilos /bordes para reducir el tiempo de carga. El valor predeterminado es true.

**Returns:**
boolean
### getBaseRouteName() {#getBaseRouteName--}
```
public String getBaseRouteName()
```


Obtiene el nombre base de la URL de ruta para el controlador GridJs, el valor predeterminado es GridJs2.

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
public int getEmptySheetMaxCol()
```


Obtiene la columna máxima predeterminada para una hoja de cálculo vacía. El valor predeterminado es 15.

**Returns:**
int
### getEmptySheetMaxRow() {#getEmptySheetMaxRow--}
```
public int getEmptySheetMaxRow()
```


Obtiene la fila máxima predeterminada para una hoja de cálculo vacía. El valor predeterminado es 12.

**Returns:**
int
### getEnableChartClientRendering() {#getEnableChartClientRendering--}
```
public boolean getEnableChartClientRendering()
```


Obtiene si se habilita la renderización de gráficos del lado del cliente. Si se establece en false, GridJs solo emitirá imágenes/formas de gráficos y no requerirá la renderización del lado del cliente. El valor predeterminado es true.

**Returns:**
boolean
### getFileCacheDirectory() {#getFileCacheDirectory--}
```
public String getFileCacheDirectory()
```


Obtiene el directorio de caché para almacenar el archivo de hoja de cálculo. Necesitamos configurarlo en una ruta específica antes de usar GridJs.

**Returns:**
java.lang.String
### getFontFolders() {#getFontFolders--}
```
public String[] getFontFolders()
```


Obtiene las carpetas de fuentes para las fuentes en las imágenes/formas renderizadas.

**Returns:**
java.lang.String[]
### getIgnoreEmptyContent() {#getIgnoreEmptyContent--}
```
public boolean getIgnoreEmptyContent()
```


Obtiene si se muestra el rango máximo que incluye datos, estilo, celdas combinadas y formas. Si la última fila o columna contiene celdas sin valor ni fórmula pero con estilo personalizado, entonces no mostraremos esa fila/columna cuando este valor sea true\\u9286?\\* el valor predeterminado es true.

**Returns:**
boolean
### getIslimitShapeOrImage() {#getIslimitShapeOrImage--}
```
public boolean getIslimitShapeOrImage()
```


Obtiene si se debe limitar el recuento total de formas/imagenes mostradas en una hoja de cálculo; si se establece en true, GridJs limitará el recuento total de formas o imágenes mostradas en una hoja de cálculo a MaxShapeOrImageCount, el valor predeterminado es true.

**Returns:**
boolean
### getJsonCache() {#getJsonCache--}
```
public JsonCacheOptions getJsonCache()
```


Obtiene las opciones de configuración de caché JSON. Controla tanto el comportamiento de la caché en memoria (L1) como en disco (L2) para el JSON del libro de trabajo generado.

**Returns:**
[JsonCacheOptions](../../com.aspose.gridjs/jsoncacheoptions)
### getLazyLoading() {#getLazyLoading--}
```
public boolean getLazyLoading()
```


Obtiene si se debe cargar solo la hoja de cálculo activa, el valor predeterminado es false.

**Returns:**
boolean
### getMaxPdfSaveSeconds() {#getMaxPdfSaveSeconds--}
```
public int getMaxPdfSaveSeconds()
```


Obtiene el número máximo de segundos de tiempo de espera al guardar en PDF. El valor predeterminado es 10.

**Returns:**
int
### getMaxShapeOrImageCount() {#getMaxShapeOrImageCount--}
```
public int getMaxShapeOrImageCount()
```


Obtiene el recuento total de las formas o imágenes mostradas en la hoja activa, tiene efecto cuando IslimitShapeOrImage=true. El valor predeterminado es 100.

**Returns:**
int
### getMaxShapeOrImageWidthOrHeight() {#getMaxShapeOrImageWidthOrHeight--}
```
public int getMaxShapeOrImageWidthOrHeight()
```


Obtiene el ancho o alto máximo para una forma o una imagen, GridJs ignorará la forma o imagen con un ancho o alto mayor que este valor, tiene efecto cuando IslimitShapeOrImage=true. El valor predeterminado es 10000.

**Returns:**
int
### getMaxTotalShapeOrImageCount() {#getMaxTotalShapeOrImageCount--}
```
public int getMaxTotalShapeOrImageCount()
```


Obtiene el recuento total de las formas o imágenes mostradas en el libro de trabajo, tiene efecto cuando IslimitShapeOrImage=true. El valor predeterminado es 300.

**Returns:**
int
### getMessageTopic() {#getMessageTopic--}
```
public String getMessageTopic()
```


Obtiene los destinos de websocket con el prefijo "/topic". El valor predeterminado es "/topic/opr". Se usa solo en modo colaborativo.

**Returns:**
java.lang.String
### getPictureCacheDirectory() {#getPictureCacheDirectory--}
```
public String getPictureCacheDirectory()
```


Obtiene el directorio de caché para imágenes. (esto tiene efecto cuando GridJsWorkbook.CacheImp es null) la ruta predeterminada será "\\_piccache" dentro de FileCacheDirectory.

**Returns:**
java.lang.String
### getSameImageDetecting() {#getSameImageDetecting--}
```
public boolean getSameImageDetecting()
```


Obtiene si se debe comprobar si las imágenes tienen la misma fuente, el valor predeterminado es true.

**Returns:**
boolean
### getSaveHtmlAsZip() {#getSaveHtmlAsZip--}
```
public boolean getSaveHtmlAsZip()
```


Obtiene si se debe guardar el archivo HTML como archivo zip, el valor predeterminado es false.

**Returns:**
boolean
### getShowChartSheet() {#getShowChartSheet--}
```
public boolean getShowChartSheet()
```


Obtiene si se muestra la hoja de gráficos. El valor predeterminado es false.

**Returns:**
boolean
### getSkipInvisibleShapes() {#getSkipInvisibleShapes--}
```
public boolean getSkipInvisibleShapes()
```


Obtiene si se deben omitir las formas que son invisibles para la UI, el valor predeterminado es true.

**Returns:**
boolean
### getUsePrintArea() {#getUsePrintArea--}
```
public boolean getUsePrintArea()
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
public boolean isCollaborative()
```


Obtiene si se admite la edición colaborativa, el valor predeterminado es false.

**Returns:**
boolean
### isWasm() {#isWasm--}
```
public boolean isWasm()
```


Obtiene si GridJs se ejecuta dentro de un host WebAssembly del navegador en lugar de un proceso del servidor. Cuando es true, no se utiliza FileCacheDirectory / disco / ruta de subproceso de interrupción, y la caché de archivos debe provenir de CacheImp, porque un host de navegador no tiene disco local. Selecciona rutas de código en tiempo de ejecución, por lo que un Aspose.Cells.GridJs.dll sirve a ambos hosts. El valor predeterminado es false.

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
public void setAutoFitColumnsOnLoad(boolean value)
```


Indica si se ajusta automáticamente el ancho de las columnas al cargar el archivo, el valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAutoFitRowsHeightOnLoad(boolean value) {#setAutoFitRowsHeightOnLoad-boolean-}
```
public void setAutoFitRowsHeightOnLoad(boolean value)
```


Indica si se ajusta automáticamente la altura de las filas al cargar el archivo, el valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setAutoOptimizeForLargeCells(boolean value) {#setAutoOptimizeForLargeCells-boolean-}
```
public void setAutoOptimizeForLargeCells(boolean value)
```


Establece si se optimiza automáticamente el rendimiento de carga para hojas de cálculo con celdas grandes. Ignorará algunos estilos /bordes para reducir el tiempo de carga. El valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setBaseRouteName(String value) {#setBaseRouteName-java.lang.String-}
```
public void setBaseRouteName(String value)
```


Establece el nombre base de la URL de ruta para el controlador GridJs. el valor predeterminado es GridJs2

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setCollaborative(boolean value) {#setCollaborative-boolean-}
```
public void setCollaborative(boolean value)
```


Establece si se admite la edición colaborativa, el valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEmptySheetMaxCol(int value) {#setEmptySheetMaxCol-int-}
```
public void setEmptySheetMaxCol(int value)
```


Establece la columna máxima predeterminada para una hoja de cálculo vacía. El valor predeterminado es 15.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setEmptySheetMaxRow(int value) {#setEmptySheetMaxRow-int-}
```
public void setEmptySheetMaxRow(int value)
```


Establece la fila máxima predeterminada para una hoja de cálculo vacía. El valor predeterminado es 12.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setEnableChartClientRendering(boolean value) {#setEnableChartClientRendering-boolean-}
```
public void setEnableChartClientRendering(boolean value)
```


Establece si se habilita la renderización de gráficos del lado del cliente. Si se establece en false, GridJs solo emitirá imágenes/formas de gráficos y no requerirá la renderización del lado del cliente. El valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setFileCacheDirectory(String value) {#setFileCacheDirectory-java.lang.String-}
```
public void setFileCacheDirectory(String value)
```


Establece el directorio de caché para almacenar el archivo de hoja de cálculo. Necesitamos configurarlo en una ruta específica antes de usar GridJs.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setFontFolders(String[] value) {#setFontFolders-java.lang.String---}
```
public void setFontFolders(String[] value)
```


Establece las carpetas de fuentes para las fuentes en las imágenes/formas renderizadas

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String[] |  |

### setIgnoreEmptyContent(boolean value) {#setIgnoreEmptyContent-boolean-}
```
public void setIgnoreEmptyContent(boolean value)
```


Establece si se muestra el rango máximo que incluye datos, estilo, celdas combinadas y formas. Si la última fila o columna contiene celdas sin valor ni fórmula pero con estilo personalizado, entonces no mostraremos esa fila/columna cuando este valor sea true\\u9286?\\* el valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setIslimitShapeOrImage(boolean value) {#setIslimitShapeOrImage-boolean-}
```
public void setIslimitShapeOrImage(boolean value)
```


Establece si se debe limitar el recuento total de formas/imagenes mostradas en una hoja de cálculo, si se establece en true, GridJs limitará el recuento total de formas o imágenes mostradas en una hoja de cálculo a MaxShapeOrImageCount, el valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setJsonCache(JsonCacheOptions value) {#setJsonCache-com.aspose.gridjs.JsonCacheOptions-}
```
public void setJsonCache(JsonCacheOptions value)
```


Establece opciones de configuración de caché JSON. Controla tanto el comportamiento de la caché en memoria (L1) como en disco (L2) para el JSON del libro de trabajo generado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [JsonCacheOptions](../../com.aspose.gridjs/jsoncacheoptions) |  |

### setLazyLoading(boolean value) {#setLazyLoading-boolean-}
```
public void setLazyLoading(boolean value)
```


Establece si se debe cargar solo la hoja de cálculo activa, el valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setMaxPdfSaveSeconds(int value) {#setMaxPdfSaveSeconds-int-}
```
public void setMaxPdfSaveSeconds(int value)
```


Establece el número máximo de segundos de tiempo de espera al guardar en PDF. el valor predeterminado es 10.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setMaxShapeOrImageCount(int value) {#setMaxShapeOrImageCount-int-}
```
public void setMaxShapeOrImageCount(int value)
```


Establece el recuento total de formas o imágenes mostradas en la hoja activa, tiene efecto cuando IslimitShapeOrImage=true. el valor predeterminado es 100.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setMaxShapeOrImageWidthOrHeight(int value) {#setMaxShapeOrImageWidthOrHeight-int-}
```
public void setMaxShapeOrImageWidthOrHeight(int value)
```


Establece el ancho o alto máximo para una forma o una imagen, GridJs ignorará la forma o imagen cuyo ancho o alto sea mayor que este valor, tiene efecto cuando IslimitShapeOrImage=true. el valor predeterminado es 10000.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setMaxTotalShapeOrImageCount(int value) {#setMaxTotalShapeOrImageCount-int-}
```
public void setMaxTotalShapeOrImageCount(int value)
```


Establece el recuento total de formas o imágenes mostradas en el libro de trabajo, tiene efecto cuando IslimitShapeOrImage=true. el valor predeterminado es 300.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setMessageTopic(String value) {#setMessageTopic-java.lang.String-}
```
public void setMessageTopic(String value)
```


Establece los destinos de websocket con el prefijo "/topic". el valor predeterminado es "/topic/opr". usado solo en modo colaborativo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setPictureCacheDirectory(String value) {#setPictureCacheDirectory-java.lang.String-}
```
public void setPictureCacheDirectory(String value)
```


Establece el directorio de caché para imágenes. (esto tiene efecto cuando GridJsWorkbook.CacheImp es nulo) la ruta predeterminada será "\\_piccache" dentro de FileCacheDirectory.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setSameImageDetecting(boolean value) {#setSameImageDetecting-boolean-}
```
public void setSameImageDetecting(boolean value)
```


Establece si se debe comprobar si las imágenes tienen la misma fuente, el valor predeterminado es true el valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSaveHtmlAsZip(boolean value) {#setSaveHtmlAsZip-boolean-}
```
public void setSaveHtmlAsZip(boolean value)
```


Establece si se debe guardar el archivo html como archivo zip, el valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowChartSheet(boolean value) {#setShowChartSheet-boolean-}
```
public void setShowChartSheet(boolean value)
```


Establece si se muestra la hoja de gráfico. el valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSkipInvisibleShapes(boolean value) {#setSkipInvisibleShapes-boolean-}
```
public void setSkipInvisibleShapes(boolean value)
```


Establece si se omiten las formas que son invisibles para la UI, el valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setUsePrintArea(boolean value) {#setUsePrintArea-boolean-}
```
public void setUsePrintArea(boolean value)
```


Establece si se usa PageSetup.PrintArea para el rango de visualización de la UI cuando la hoja tiene la configuración PageSetup para PrintArea. el valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setWasm(boolean value) {#setWasm-boolean-}
```
public void setWasm(boolean value)
```


Establece si GridJs se ejecuta dentro de un host WebAssembly en el navegador en lugar de un proceso de servidor. Cuando es true, no se utiliza FileCacheDirectory / disco / ruta de hilo de interrupción, y la caché de archivos debe provenir de CacheImp, porque un host de navegador no tiene disco local. Selecciona rutas de código en tiempo de ejecución, por lo que un Aspose.Cells.GridJs.dll sirve a ambos hosts. el valor predeterminado es false.

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

