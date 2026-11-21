---
title: "WorksheetCollection"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Encapsula una colección de objetos."
type: docs
url: /es/java/com.aspose.cells/worksheetcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class WorksheetCollection extends CollectionBase
```

Encapsula una colección de objetos [Worksheet](../../com.aspose.cells/worksheet).

**Example**

```
         Workbook workbook = new Workbook();
 
         WorksheetCollection sheets = workbook.getWorksheets();
 
         //Add a worksheet
         sheets.add();
 
         //Change the name of a worksheet
         sheets.get(0).setName("First Sheet");
 
         //Set the active sheet to the second worksheet
         sheets.setActiveSheetIndex(1);
```
## Métodos

| Método | Descripción |
| --- | --- |
| [add()](#add--) | Agrega una hoja de cálculo a la colección. |
| [add(int type)](#add-int-) | Agrega una hoja de cálculo a la colección. |
| [add(Object o)](#add-java.lang.Object-) | Agrega un elemento a la instancia de CollectionBase. |
| [add(String sheetName)](#add-java.lang.String-) | Agrega una hoja de cálculo a la colección. |
| [addCopy(Worksheet[] source, String[] destSheetNames)](#addCopy-com.aspose.cells.Worksheet---java.lang.String---) | Copia un grupo de hojas de cálculo. |
| [addCopy(int sheetIndex)](#addCopy-int-) | Agrega una hoja de cálculo a la colección y copia datos de una hoja de cálculo existente. |
| [addCopy(String sheetName)](#addCopy-java.lang.String-) | Agrega una hoja de cálculo a la colección y copia datos de una hoja de cálculo existente. |
| [clear()](#clear--) | Borra todas las hojas de cálculo. |
| [clearPivottables()](#clearPivottables--) | Elimina tablas dinámicas de la hoja de cálculo. |
| [contains(Object o)](#contains-java.lang.Object-) | Devuelve si la instancia contiene este objeto |
| [createRange(String address, int sheetIndex)](#createRange-java.lang.String-int-) | Crea un objeto [Range](../../com.aspose.cells/range) a partir de una dirección del rango. |
| [createUnionRange(String address, int sheetIndex)](#createUnionRange-java.lang.String-int-) | Crea un objeto [Range](../../com.aspose.cells/range) a partir de una dirección del rango. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtiene el elemento [Worksheet](../../com.aspose.cells/worksheet) en el índice especificado. |
| [get(String sheetName)](#get-java.lang.String-) | Obtiene el elemento [Worksheet](../../com.aspose.cells/worksheet) con el nombre especificado. |
| [getActiveSheetIndex()](#getActiveSheetIndex--) | Representa el índice de la hoja de cálculo activa cuando se abre la hoja de cálculo. |
| [getActiveSheetName()](#getActiveSheetName--) | Representa el nombre de la hoja de cálculo activa cuando se abre la hoja de cálculo. |
| [getBuiltInDocumentProperties()](#getBuiltInDocumentProperties--) | Devuelve una colección de [DocumentProperty](../../com.aspose.cells/documentproperty) que representa todas las propiedades de documento incorporadas de la hoja de cálculo. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtiene el número de elementos contenidos en la instancia de CollectionBase. |
| [getCustomDocumentProperties()](#getCustomDocumentProperties--) | Devuelve una colección de [DocumentProperty](../../com.aspose.cells/documentproperty) que representa todas las propiedades de documento personalizadas de la hoja de cálculo. |
| [getDxfs()](#getDxfs--) | Obtiene los registros maestros de formato diferencial. |
| [getExternalLinks()](#getExternalLinks--) | Representa enlaces externos en un libro de trabajo. |
| [getNamedRanges()](#getNamedRanges--) | Obtiene todos los rangos con nombre predefinidos en la hoja de cálculo. |
| [getNamedRangesAndTables()](#getNamedRangesAndTables--) | Obtiene todos los rangos con nombre predefinidos en la hoja de cálculo. |
| [getNames()](#getNames--) | Obtiene la colección de todos los objetos Name en la hoja de cálculo. |
| [getOleSize()](#getOleSize--) | Obtiene el tamaño mostrado cuando el archivo Workbook se usa como un objeto Ole. |
| [getPivotCaches()](#getPivotCaches--) | Obtiene todos los [PivotCache](../../com.aspose.cells/pivotcache). |
| [getRangeByName(String rangeName)](#getRangeByName-java.lang.String-) | Obtiene el objeto Range por nombre predefinido. |
| [getRangeByName(String rangeName, int currentSheetIndex, boolean includeTable)](#getRangeByName-java.lang.String-int-boolean-) | Obtiene [Range](../../com.aspose.cells/range) por nombre predefinido o nombre de tabla. |
| [getRevisionLogs()](#getRevisionLogs--) | Representa los registros de revisiones. |
| [getSensitivityLabels()](#getSensitivityLabels--) | Representa todas las etiquetas de sensibilidad. |
| [getSheetByCodeName(String codeName)](#getSheetByCodeName-java.lang.String-) | Obtiene la hoja de cálculo por el nombre de código. |
| [getTableStyles()](#getTableStyles--) | Obtiene el objeto [getTableStyles()](../../com.aspose.cells/worksheetcollection\#getTableStyles--). |
| [getThreadedCommentAuthors()](#getThreadedCommentAuthors--) | Obtiene la lista de autores de comentarios en hilo. |
| [getWebExtensionTaskPanes()](#getWebExtensionTaskPanes--) | Obtiene la lista de paneles de tareas. |
| [getWebExtensions()](#getWebExtensions--) | Obtiene la lista de paneles de tareas. |
| [getXmlMaps()](#getXmlMaps--) | Obtiene los mapas XML en el libro de trabajo. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determina el índice de un elemento específico en la instancia de CollectionBase. |
| [insert(int index, int sheetType)](#insert-int-int-) | Insertar una hoja de cálculo. |
| [insert(int index, int sheetType, String sheetName)](#insert-int-int-java.lang.String-) | Insertar una hoja de cálculo. |
| [isRefreshAllConnections()](#isRefreshAllConnections--) | Indica si se actualizan todas las conexiones al abrir el archivo en MS Excel. |
| [iterator()](#iterator--) | Devuelve un enumerador que recorre la instancia de CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshAll()](#refreshAll--) | Actualiza todas las tablas dinámicas y gráficos con la fuente dinámica. |
| [refreshPivotTables()](#refreshPivotTables--) | Actualiza todas las tablas dinámicas en el archivo de Excel. |
| [refreshPivotTables(PivotTableRefreshOption option)](#refreshPivotTables-com.aspose.cells.PivotTableRefreshOption-) | Actualiza todas las tablas dinámicas en el archivo de Excel. |
| [registerAddInFunction(int id, String functionName)](#registerAddInFunction-int-java.lang.String-) | Agrega la función del complemento al libro de trabajo |
| [registerAddInFunction(String addInFile, String functionName, boolean lib)](#registerAddInFunction-java.lang.String-java.lang.String-boolean-) | Agrega la función del complemento al libro de trabajo |
| [removeAt(int index)](#removeAt-int-) | Elimina el elemento en un índice especificado. |
| [removeAt(String name)](#removeAt-java.lang.String-) | Elimina el elemento con un nombre especificado. |
| [setActiveSheetIndex(int value)](#setActiveSheetIndex-int-) | Representa el índice de la hoja de cálculo activa cuando se abre la hoja de cálculo. |
| [setActiveSheetName(String value)](#setActiveSheetName-java.lang.String-) | Representa el nombre de la hoja de cálculo activa cuando se abre la hoja de cálculo. |
| [setOleSize(int startRow, int endRow, int startColumn, int endColumn)](#setOleSize-int-int-int-int-) | Establece el tamaño mostrado cuando el archivo de libro de trabajo se usa como objeto Ole. |
| [setOleSize(Object value)](#setOleSize-java.lang.Object-) | Establece el tamaño mostrado cuando el archivo de libro de trabajo se usa como objeto Ole. |
| [setRefreshAllConnections(boolean value)](#setRefreshAllConnections-boolean-) | Indica si se actualizan todas las conexiones al abrir el archivo en MS Excel. |
| [setXmlMaps(XmlMapCollection value)](#setXmlMaps-com.aspose.cells.XmlMapCollection-) | Establece los mapas XML en el libro de trabajo. |
| [sortNames()](#sortNames--) | Ordena los nombres definidos. |
| [swapSheet(int sheetIndex1, int sheetIndex2)](#swapSheet-int-int-) | Intercambia las dos hojas. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add() {#add--}
```
public int add()
```


Agrega una hoja de cálculo a la colección.

**Returns:**
int - [Worksheet](../../com.aspose.cells/worksheet) índice del objeto.
### add(int type) {#add-int-}
```
public int add(int type)
```


Agrega una hoja de cálculo a la colección.

**Example**

```
         Workbook workbook = new Workbook();
         workbook.getWorksheets().add(SheetType.CHART);
         	Cells cells = workbook.getWorksheets().get(0).getCells();
         	cells.get("c2").putValue(5000);
         	cells.get("c3").putValue(3000);
         	cells.get("c4").putValue(4000);
         	cells.get("c5").putValue(5000);
         	cells.get("c6").putValue(6000);
         	ChartCollection charts = workbook.getWorksheets().get(1).getCharts();
         	int chartIndex = charts.add(ChartType.COLUMN, 10,10,20,20);
         	Chart chart = charts.get(chartIndex);
         	chart.getNSeries().add("Sheet1!C2:C6", true);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [SheetType](../../com.aspose.cells/sheettype). Tipo de hoja de cálculo. |

**Returns:**
int - [Worksheet](../../com.aspose.cells/worksheet) índice del objeto.
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Agrega un elemento a la instancia de CollectionBase.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| o | java.lang.Object | El objeto a agregar a la instancia de CollectionBase. |

**Returns:**
int - La posición en la que se insertó el nuevo elemento.
### add(String sheetName) {#add-java.lang.String-}
```
public Worksheet add(String sheetName)
```


Agrega una hoja de cálculo a la colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetName | java.lang.String | Nombre de la hoja de cálculo |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - [Worksheet](../../com.aspose.cells/worksheet) object.
### addCopy(Worksheet[] source, String[] destSheetNames) {#addCopy-com.aspose.cells.Worksheet---java.lang.String---}
```
public void addCopy(Worksheet[] source, String[] destSheetNames)
```


Copia un grupo de hojas de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| source | [Worksheet\[\]](../../com.aspose.cells/worksheet) | Las hojas de cálculo origen. |
| destSheetNames | java.lang.String[] | Los nombres de las hojas copiadas. |

### addCopy(int sheetIndex) {#addCopy-int-}
```
public int addCopy(int sheetIndex)
```


Agrega una hoja de cálculo a la colección y copia datos de una hoja de cálculo existente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetIndex | int | Índice de la hoja de cálculo origen. |

**Returns:**
int - [Worksheet](../../com.aspose.cells/worksheet) índice del objeto.
### addCopy(String sheetName) {#addCopy-java.lang.String-}
```
public int addCopy(String sheetName)
```


Agrega una hoja de cálculo a la colección y copia datos de una hoja de cálculo existente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetName | java.lang.String | Nombre de la hoja de cálculo origen. |

**Returns:**
int - [Worksheet](../../com.aspose.cells/worksheet) índice del objeto.
### clear() {#clear--}
```
public void clear()
```


Borra todas las hojas de cálculo.

**Remarks**

Un libro de trabajo debe contener una hoja de cálculo.

### clearPivottables() {#clearPivottables--}
```
public void clearPivottables()
```


Elimina tablas dinámicas de la hoja de cálculo.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Devuelve si la instancia contiene este objeto

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| o | java.lang.Object | objeto de prueba |

**Returns:**
boolean - Si la instancia contiene este objeto
### createRange(String address, int sheetIndex) {#createRange-java.lang.String-int-}
```
public Range createRange(String address, int sheetIndex)
```


Crea un objeto [Range](../../com.aspose.cells/range) a partir de una dirección del rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dirección | java.lang.String | La dirección del rango. |
| sheetIndex | int | El índice de la hoja. |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### createUnionRange(String address, int sheetIndex) {#createUnionRange-java.lang.String-int-}
```
public UnionRange createUnionRange(String address, int sheetIndex)
```


Crea un objeto [Range](../../com.aspose.cells/range) a partir de una dirección del rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dirección | java.lang.String | La dirección del rango. |
| sheetIndex | int | El índice de la hoja. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - A [Range](../../com.aspose.cells/range) object
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
### get(int index) {#get-int-}
```
public Worksheet get(int index)
```


Obtiene el elemento [Worksheet](../../com.aspose.cells/worksheet) en el índice especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice basado en cero del elemento. |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - The element at the specified index.
### get(String sheetName) {#get-java.lang.String-}
```
public Worksheet get(String sheetName)
```


Obtiene el elemento [Worksheet](../../com.aspose.cells/worksheet) con el nombre especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetName | java.lang.String | Nombre de la hoja de cálculo |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - The element with the specified name.
### getActiveSheetIndex() {#getActiveSheetIndex--}
```
public int getActiveSheetIndex()
```


Representa el índice de la hoja de cálculo activa cuando se abre la hoja de cálculo.

**Remarks**

El índice de la hoja comienza en cero.

**Returns:**
int
### getActiveSheetName() {#getActiveSheetName--}
```
public String getActiveSheetName()
```


Representa el nombre de la hoja de cálculo activa cuando se abre la hoja de cálculo.

**Returns:**
java.lang.String
### getBuiltInDocumentProperties() {#getBuiltInDocumentProperties--}
```
public BuiltInDocumentPropertyCollection getBuiltInDocumentProperties()
```


Devuelve una colección de [DocumentProperty](../../com.aspose.cells/documentproperty) que representa todas las propiedades de documento incorporadas de la hoja de cálculo.

**Remarks**

No se puede agregar una nueva propiedad a la lista de propiedades de documento incorporadas. Solo puede obtener una propiedad incorporada y cambiar su valor. La siguiente es la lista de nombres de propiedades incorporadas:

Title

Asunto

Autor

Palabras clave

Comentarios

Plantilla

Último autor

Número de revisión

Nombre de la aplicación

Fecha de última impresión

Fecha de creación

Hora de última guardado

Tiempo total de edición

Número de páginas

Número de palabras

Número de caracteres

Seguridad

Categoría

Formato

Administrador

Empresa

Número de bytes

Número de líneas

Número de párrafos

Número de diapositivas

Número de notas

Número de diapositivas ocultas

Número de clips multimedia

**Example**

```
         Workbook workbook = new Workbook();
         DocumentProperty doc = workbook.getWorksheets().getBuiltInDocumentProperties().get("Author");
         doc.setValue("John Smith");
```

**Returns:**
[BuiltInDocumentPropertyCollection](../../com.aspose.cells/builtindocumentpropertycollection)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


Obtiene el número de elementos contenidos en la instancia de CollectionBase.

**Returns:**
int - El número de elementos contenidos en la instancia de CollectionBase.
### getCustomDocumentProperties() {#getCustomDocumentProperties--}
```
public CustomDocumentPropertyCollection getCustomDocumentProperties()
```


Devuelve una colección de [DocumentProperty](../../com.aspose.cells/documentproperty) que representa todas las propiedades de documento personalizadas de la hoja de cálculo.

**Example**

```
         Workbook workbook = new Workbook();
         workbook.getWorksheets().getCustomDocumentProperties().add("Checked by", "Jane");
```

**Returns:**
[CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection)
### getDxfs() {#getDxfs--}
```
public DxfCollection getDxfs()
```


Obtiene los registros maestros de formato diferencial.

**Returns:**
[DxfCollection](../../com.aspose.cells/dxfcollection)
### getExternalLinks() {#getExternalLinks--}
```
public ExternalLinkCollection getExternalLinks()
```


Representa enlaces externos en un libro de trabajo.

**Returns:**
[ExternalLinkCollection](../../com.aspose.cells/externallinkcollection)
### getNamedRanges() {#getNamedRanges--}
```
public Range[] getNamedRanges()
```


Obtiene todos los rangos con nombre predefinidos en la hoja de cálculo.

**Returns:**
com.aspose.cells.Range[] - Una matriz de objetos Range. Si la referencia del Name definido es externa o tiene múltiples rangos, no se devolverá ningún objeto Range para este Name.

Devuelve null si el rango nombrado no existe.
### getNamedRangesAndTables() {#getNamedRangesAndTables--}
```
public Range[] getNamedRangesAndTables()
```


Obtiene todos los rangos con nombre predefinidos en la hoja de cálculo.

**Returns:**
com.aspose.cells.Range[] - Una matriz de objetos Range.

Devuelve null si el rango nombrado no existe.
### getNames() {#getNames--}
```
public NameCollection getNames()
```


Obtiene la colección de todos los objetos Name en la hoja de cálculo.

**Returns:**
[NameCollection](../../com.aspose.cells/namecollection)
### getOleSize() {#getOleSize--}
```
public Object getOleSize()
```


Obtiene el tamaño mostrado cuando el archivo Workbook se usa como un objeto Ole.

**Remarks**

Null significa que no hay configuración de tamaño ole.

**Returns:**
java.lang.Object
### getPivotCaches() {#getPivotCaches--}
```
public PivotCacheCollection getPivotCaches()
```


Obtiene todos los [PivotCache](../../com.aspose.cells/pivotcache).

**Returns:**
[PivotCacheCollection](../../com.aspose.cells/pivotcachecollection)
### getRangeByName(String rangeName) {#getRangeByName-java.lang.String-}
```
public Range getRangeByName(String rangeName)
```


Obtiene el objeto Range por nombre predefinido.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rangeName | java.lang.String | Nombre del rango. |

**Returns:**
[Range](../../com.aspose.cells/range) - Range object.

Devuelve null si el rango nombrado no existe.
### getRangeByName(String rangeName, int currentSheetIndex, boolean includeTable) {#getRangeByName-java.lang.String-int-boolean-}
```
public Range getRangeByName(String rangeName, int currentSheetIndex, boolean includeTable)
```


Obtiene [Range](../../com.aspose.cells/range) por nombre predefinido o nombre de tabla.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rangeName | java.lang.String | Nombre del rango o nombre de la tabla. |
| currentSheetIndex | int | El índice de la hoja. -1 representa global . |
| includeTable | boolean | Indica si se están comprobando todas las tablas. |

**Returns:**
[Range](../../com.aspose.cells/range) - 
### getRevisionLogs() {#getRevisionLogs--}
```
public RevisionLogCollection getRevisionLogs()
```


Representa los registros de revisiones.

**Returns:**
[RevisionLogCollection](../../com.aspose.cells/revisionlogcollection)
### getSensitivityLabels() {#getSensitivityLabels--}
```
public SensitivityLabelCollection getSensitivityLabels()
```


Representa todas las etiquetas de sensibilidad.

**Returns:**
[SensitivityLabelCollection](../../com.aspose.cells/sensitivitylabelcollection)
### getSheetByCodeName(String codeName) {#getSheetByCodeName-java.lang.String-}
```
public Worksheet getSheetByCodeName(String codeName)
```


Obtiene la hoja de cálculo por el nombre de código.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| codeName | java.lang.String | Nombre de código de la hoja de cálculo. |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - The element with the specified code name.
### getTableStyles() {#getTableStyles--}
```
public TableStyleCollection getTableStyles()
```


Obtiene el objeto [getTableStyles()](../../com.aspose.cells/worksheetcollection\#getTableStyles--).

**Returns:**
[TableStyleCollection](../../com.aspose.cells/tablestylecollection)
### getThreadedCommentAuthors() {#getThreadedCommentAuthors--}
```
public ThreadedCommentAuthorCollection getThreadedCommentAuthors()
```


Obtiene la lista de autores de comentarios en hilo.

**Returns:**
[ThreadedCommentAuthorCollection](../../com.aspose.cells/threadedcommentauthorcollection)
### getWebExtensionTaskPanes() {#getWebExtensionTaskPanes--}
```
public WebExtensionTaskPaneCollection getWebExtensionTaskPanes()
```


Obtiene la lista de paneles de tareas.

**Returns:**
[WebExtensionTaskPaneCollection](../../com.aspose.cells/webextensiontaskpanecollection)
### getWebExtensions() {#getWebExtensions--}
```
public WebExtensionCollection getWebExtensions()
```


Obtiene la lista de paneles de tareas.

**Returns:**
[WebExtensionCollection](../../com.aspose.cells/webextensioncollection)
### getXmlMaps() {#getXmlMaps--}
```
public XmlMapCollection getXmlMaps()
```


Obtiene los mapas XML en el libro de trabajo.

**Returns:**
[XmlMapCollection](../../com.aspose.cells/xmlmapcollection)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


Determina el índice de un elemento específico en la instancia de CollectionBase.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| o | java.lang.Object | Determina el índice de un elemento específico en la instancia de CollectionBase. |

**Returns:**
int - El índice del valor si se encuentra en la lista; de lo contrario, -1.
### insert(int index, int sheetType) {#insert-int-int-}
```
public Worksheet insert(int index, int sheetType)
```


Insertar una hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice de la hoja |
| sheetType | int | [SheetType](../../com.aspose.cells/sheettype). El tipo de hoja. |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - Returns an inserted worksheet.
### insert(int index, int sheetType, String sheetName) {#insert-int-int-java.lang.String-}
```
public Worksheet insert(int index, int sheetType, String sheetName)
```


Insertar una hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice de la hoja |
| sheetType | int | [SheetType](../../com.aspose.cells/sheettype). El tipo de hoja. |
| sheetName | java.lang.String | El nombre de la hoja. |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - Returns an inserted worksheet.
### isRefreshAllConnections() {#isRefreshAllConnections--}
```
public boolean isRefreshAllConnections()
```


Indica si se actualizan todas las conexiones al abrir el archivo en MS Excel.

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


Devuelve un enumerador que recorre la instancia de CollectionBase.

**Returns:**
java.util.Iterator - Un iterador para la instancia de CollectionBase.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refreshAll() {#refreshAll--}
```
public void refreshAll()
```


Actualiza todas las tablas dinámicas y gráficos con la fuente dinámica.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use el método Workbook.RefreshAll(). Este método será eliminado 12 meses después desde abril de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### refreshPivotTables() {#refreshPivotTables--}
```
public void refreshPivotTables()
```


Actualiza todas las tablas dinámicas en el archivo de Excel.

### refreshPivotTables(PivotTableRefreshOption option) {#refreshPivotTables-com.aspose.cells.PivotTableRefreshOption-}
```
public boolean refreshPivotTables(PivotTableRefreshOption option)
```


Actualiza todas las tablas dinámicas en el archivo de Excel.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) | La opción para actualizar la fuente de datos de las tablas dinámicas. |

**Returns:**
boolean
### registerAddInFunction(int id, String functionName) {#registerAddInFunction-int-java.lang.String-}
```
public String registerAddInFunction(int id, String functionName)
```


Agrega la función del complemento al libro de trabajo

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| id | int | ID de los datos que contienen funciones addin, se puede obtener mediante la primera llamada a [registerAddInFunction(String,String,boolean)](../../com.aspose.cells/worksheetcollection\#registerAddInFunction-String-String-boolean-) para el mismo archivo addin. |
| functionName | java.lang.String | el nombre de la función addin |

**Returns:**
java.lang.String - URL del archivo addin que contiene funciones addin
### registerAddInFunction(String addInFile, String functionName, boolean lib) {#registerAddInFunction-java.lang.String-java.lang.String-boolean-}
```
public int registerAddInFunction(String addInFile, String functionName, boolean lib)
```


Agrega la función del complemento al libro de trabajo

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| addInFile | java.lang.String | el archivo contiene las funciones addin |
| functionName | java.lang.String | el nombre de la función addin |
| lib | boolean | si el archivo addin dado está en el directorio o subdirectorio de la biblioteca Workbook Add-In. Esta bandera entra en vigor y marca la diferencia cuando el addInFile proporcionado es una ruta relativa: true indica que la ruta es relativa a la biblioteca Add-In y false indica que la ruta es relativa a este Workbook. |

**Returns:**
int - ID de los datos que contiene la función addin dada
### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Elimina el elemento en un índice especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El valor del índice del elemento a eliminar. |

### removeAt(String name) {#removeAt-java.lang.String-}
```
public void removeAt(String name)
```


Elimina el elemento con un nombre especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | El nombre del elemento a eliminar. |

### setActiveSheetIndex(int value) {#setActiveSheetIndex-int-}
```
public void setActiveSheetIndex(int value)
```


Representa el índice de la hoja de cálculo activa cuando se abre la hoja de cálculo.

**Remarks**

El índice de la hoja comienza en cero.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setActiveSheetName(String value) {#setActiveSheetName-java.lang.String-}
```
public void setActiveSheetName(String value)
```


Representa el nombre de la hoja de cálculo activa cuando se abre la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setOleSize(int startRow, int endRow, int startColumn, int endColumn) {#setOleSize-int-int-int-int-}
```
public void setOleSize(int startRow, int endRow, int startColumn, int endColumn)
```


Establece el tamaño mostrado cuando el archivo de libro de trabajo se usa como objeto Ole.

**Remarks**

Este método se usa generalmente para ajustar el tamaño de visualización en archivos ppt o doc.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | int | Índice de fila inicial. |
| endRow | int | Índice de fila final. |
| startColumn | int | Índice de columna inicial. |
| endColumn | int | Índice de columna final. |

### setOleSize(Object value) {#setOleSize-java.lang.Object-}
```
public void setOleSize(Object value)
```


Establece el tamaño mostrado cuando el archivo de libro de trabajo se usa como objeto Ole.

**Remarks**

Null significa que no hay configuración de tamaño ole.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.Object |  |

### setRefreshAllConnections(boolean value) {#setRefreshAllConnections-boolean-}
```
public void setRefreshAllConnections(boolean value)
```


Indica si se actualizan todas las conexiones al abrir el archivo en MS Excel.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setXmlMaps(XmlMapCollection value) {#setXmlMaps-com.aspose.cells.XmlMapCollection-}
```
public void setXmlMaps(XmlMapCollection value)
```


Establece los mapas XML en el libro de trabajo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [XmlMapCollection](../../com.aspose.cells/xmlmapcollection) |  |

### sortNames() {#sortNames--}
```
public void sortNames()
```


Ordena los nombres definidos.

**Remarks**

Si crea una gran cantidad de rangos con nombre en el archivo Excel, llame a este método después de que se hayan creado todos los rangos con nombre y antes de guardar.

### swapSheet(int sheetIndex1, int sheetIndex2) {#swapSheet-int-int-}
```
public void swapSheet(int sheetIndex1, int sheetIndex2)
```


Intercambia las dos hojas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetIndex1 | int | La primera hoja de cálculo. |
| sheetIndex2 | int | La segunda hoja de cálculo. |

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

