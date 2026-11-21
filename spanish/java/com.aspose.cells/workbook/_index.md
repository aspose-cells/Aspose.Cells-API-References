---
title: "Workbook"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa un objeto raíz para crear una hoja de cálculo de Excel."
type: docs
url: /es/java/com.aspose.cells/workbook/
---

**Inheritance:**
java.lang.Object
```
public class Workbook
```

Representa un objeto raíz para crear una hoja de cálculo de Excel.

**Remarks**

La clase Workbook representa una hoja de cálculo de Excel. Cada hoja de cálculo puede contener múltiples hojas de trabajo. La característica básica de la clase es abrir y guardar archivos Excel nativos. La clase tiene algunas funciones avanzadas, como copiar datos de otros Workbooks, combinar dos Workbooks, convertir Excel a PDF, renderizar Excel a imagen y proteger la hoja de cálculo de Excel.

**Example**

El siguiente ejemplo carga un Workbook desde un archivo Excel llamado designer.xls y hace que las barras de desplazamiento horizontales y verticales sean invisibles. Luego reemplaza dos valores de cadena con un valor entero y un valor de cadena respectivamente dentro de la hoja de cálculo y finalmente guarda el libro de trabajo como archivo Excel xlsx.

```
         //Open a designer file
         String designerFile = "designer.xls";
         Workbook workbook = new Workbook(designerFile);
 
         //Set scroll bars
         workbook.getSettings().setHScrollBarVisible(false);
         workbook.getSettings().setVScrollBarVisible(false);
 
         //Replace the placeholder string with new values
         int newInt = 100;
         workbook.replace("OldInt", newInt);
 
         String newString = "Hello!";
         workbook.replace("OldString", newString);
         workbook.save("result.xlsx");
```
## Constructores

| Constructor | Descripción |
| --- | --- |
| [Workbook()](#Workbook--) | Inicializa una nueva instancia de la clase [Workbook](../../com.aspose.cells/workbook). |
| [Workbook(int fileFormatType)](#Workbook-int-) | Inicializa una nueva instancia de la clase [Workbook](../../com.aspose.cells/workbook). |
| [Workbook(LoadOptions loadOptions)](#Workbook-com.aspose.cells.LoadOptions-) | Inicializa una nueva instancia vacía de la clase [Workbook](../../com.aspose.cells/workbook) con opciones |
| [Workbook(String file)](#Workbook-java.lang.String-) | Inicializa una nueva instancia de la clase [Workbook](../../com.aspose.cells/workbook) y abre un archivo. |
| [Workbook(InputStream stream)](#Workbook-java.io.InputStream-) | Inicializa una nueva instancia de la clase [Workbook](../../com.aspose.cells/workbook) y abre un flujo. |
| [Workbook(String file, LoadOptions loadOptions)](#Workbook-java.lang.String-com.aspose.cells.LoadOptions-) | Inicializa una nueva instancia de la clase [Workbook](../../com.aspose.cells/workbook) y abre un archivo. |
| [Workbook(InputStream stream, LoadOptions loadOptions)](#Workbook-java.io.InputStream-com.aspose.cells.LoadOptions-) | Inicializa una nueva instancia de la clase [Workbook](../../com.aspose.cells/workbook) y abre el flujo. |
## Métodos

| Método | Descripción |
| --- | --- |
| [acceptAllRevisions()](#acceptAllRevisions--) | Acepta todos los cambios rastreados en el libro de trabajo. |
| [addDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)](#addDigitalSignature-com.aspose.cells.DigitalSignatureCollection-) | Agrega una firma digital a un archivo de hoja de cálculo OOXML (Excel2007 y posteriores). |
| [calculateFormula()](#calculateFormula--) | Calcula el resultado de las fórmulas. |
| [calculateFormula(boolean ignoreError)](#calculateFormula-boolean-) | Calcula el resultado de las fórmulas. |
| [calculateFormula(CalculationOptions options)](#calculateFormula-com.aspose.cells.CalculationOptions-) | Calculando fórmulas en este libro de trabajo. |
| [changePalette(Color color, int index)](#changePalette-com.aspose.cells.Color-int-) | Cambia la paleta de la hoja de cálculo en el índice especificado. |
| [closeAccessCache(int opts)](#closeAccessCache-int-) | Cierra la sesión que usa cachés para acceder a los datos. |
| [combine(Workbook secondWorkbook)](#combine-com.aspose.cells.Workbook-) | Combina otro objeto Workbook. |
| [copy(Workbook source)](#copy-com.aspose.cells.Workbook-) | Copia datos de un objeto Workbook fuente. |
| [copy(Workbook source, CopyOptions copyOptions)](#copy-com.aspose.cells.Workbook-com.aspose.cells.CopyOptions-) | Copia otro objeto Workbook. |
| [copyTheme(Workbook source)](#copyTheme-com.aspose.cells.Workbook-) | Copia el tema de otro libro de trabajo. |
| [createBuiltinStyle(int type)](#createBuiltinStyle-int-) | Crea un estilo incorporado según el tipo dado. |
| [createCellsColor()](#createCellsColor--) | Crea un objeto [CellsColor](../../com.aspose.cells/cellscolor). |
| [createStyle()](#createStyle--) | Crea un nuevo estilo. |
| [createStyle(boolean cloneDefaultStyle)](#createStyle-boolean-) | Crea un nuevo estilo. |
| [customTheme(String themeName, Color[] colors)](#customTheme-java.lang.String-com.aspose.cells.Color---) | Personaliza el tema. |
| [dispose()](#dispose--) | Ejecuta tareas definidas por la aplicación asociadas con la liberación, el lanzamiento o el restablecimiento de recursos no administrados. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportXml(String mapName, OutputStream stream)](#exportXml-java.lang.String-java.io.OutputStream-) | Exporta datos XML vinculados mediante el mapa XML especificado. |
| [exportXml(String mapName, String path)](#exportXml-java.lang.String-java.lang.String-) | Exporta datos XML vinculados mediante el mapa XML especificado. |
| [getAbsolutePath()](#getAbsolutePath--) | Obtiene la ruta absoluta del archivo. |
| [getBuiltInDocumentProperties()](#getBuiltInDocumentProperties--) | Devuelve una colección de [DocumentProperty](../../com.aspose.cells/documentproperty) que representa todas las propiedades de documento incorporadas de la hoja de cálculo. |
| [getCellsDataTableFactory()](#getCellsDataTableFactory--) | Obtiene la fábrica para crear ICellsDataTable a partir de objetos personalizados |
| [getClass()](#getClass--) |  |
| [getColors()](#getColors--) | Devuelve los colores de la paleta de la hoja de cálculo. |
| [getContentTypeProperties()](#getContentTypeProperties--) | Obtiene la lista de objetos [ContentTypeProperty](../../com.aspose.cells/contenttypeproperty) en el libro de trabajo. |
| [getCountOfStylesInPool()](#getCountOfStylesInPool--) | Obtiene el número de estilos en el grupo de estilos. |
| [getCustomDocumentProperties()](#getCustomDocumentProperties--) | Devuelve una colección de [DocumentProperty](../../com.aspose.cells/documentproperty) que representa todas las propiedades de documento personalizadas de la hoja de cálculo. |
| [getCustomXmlParts()](#getCustomXmlParts--) | Representa una parte de almacenamiento de datos XML personalizada (datos XML personalizados dentro de un paquete). |
| [getDataConnections()](#getDataConnections--) | Obtiene la colección [ExternalConnection](../../com.aspose.cells/externalconnection). |
| [getDataMashup()](#getDataMashup--) | Obtiene datos mashup. |
| [getDataModel()](#getDataModel--) | Obtiene el modelo de datos en el libro de trabajo. |
| [getDataSorter()](#getDataSorter--) | Obtiene un objeto DataSorter para ordenar datos. |
| [getDefaultStyle()](#getDefaultStyle--) | Obtiene el objeto [Style](../../com.aspose.cells/style) predeterminado del libro de trabajo. |
| [getDigitalSignature()](#getDigitalSignature--) | Obtiene la firma digital del archivo. |
| [getFileFormat()](#getFileFormat--) | Obtiene el formato de archivo. |
| [getFileName()](#getFileName--) | Obtiene el nombre de archivo actual. |
| [getFonts()](#getFonts--) | Obtiene todas las fuentes en el grupo de estilos. |
| [getInterruptMonitor()](#getInterruptMonitor--) | Obtiene el monitor de interrupciones. |
| [getMatchingColor(Color rawColor)](#getMatchingColor-com.aspose.cells.Color-) | Encuentra el color que mejor coincide en la paleta actual. |
| [getNamedStyle(String name)](#getNamedStyle-java.lang.String-) | Obtiene el estilo con nombre en el grupo de estilos. |
| [getRibbonXml()](#getRibbonXml--) | Obtiene el archivo XML que define la interfaz Ribbon. |
| [getSettings()](#getSettings--) | Representa la configuración del libro de trabajo. |
| [getStyleInPool(int index)](#getStyleInPool-int-) | Obtiene el estilo en el grupo de estilos. |
| [getTheme()](#getTheme--) | Obtiene el nombre del tema. |
| [getThemeColor(int type)](#getThemeColor-int-) | Obtiene el color del tema. |
| [getVbaProject()](#getVbaProject--) | Obtiene el [getVbaProject()](../../com.aspose.cells/workbook\#getVbaProject--) en una hoja de cálculo. |
| [getWorksheets()](#getWorksheets--) | Obtiene la colección [WorksheetCollection](../../com.aspose.cells/worksheetcollection) en la hoja de cálculo. |
| [hasCustomFunction()](#hasCustomFunction--) | Detecta si hay una función personalizada utilizada en este libro de trabajo, como en la fórmula de una celda, en nombres definidos... |
| [hasExernalLinks()](#hasExernalLinks--) | Indica si este libro de trabajo contiene enlaces externos a otras fuentes de datos. |
| [hasMacro()](#hasMacro--) | Indica si esta hoja de cálculo contiene macro/VBA. |
| [hasRevisions()](#hasRevisions--) | Obtiene si el libro de trabajo tiene cambios rastreados |
| [hashCode()](#hashCode--) |  |
| [importXml(InputStream stream, String sheetName, int row, int col)](#importXml-java.io.InputStream-java.lang.String-int-int-) | Importa/Actualiza un archivo de datos XML en el libro de trabajo. |
| [importXml(String url, String sheetName, int row, int col)](#importXml-java.lang.String-java.lang.String-int-int-) | Importa/Actualiza un archivo de datos XML en el libro de trabajo. |
| [isColorInPalette(Color color)](#isColorInPalette-com.aspose.cells.Color-) | Comprueba si un color está en la paleta de la hoja de cálculo. |
| [isDigitallySigned()](#isDigitallySigned--) | Indica si esta hoja de cálculo está firmada digitalmente. |
| [isLicensed()](#isLicensed--) | Indica si la licencia está establecida. |
| [isWorkbookProtectedWithPassword()](#isWorkbookProtectedWithPassword--) | Indica si la estructura o la ventana están protegidas con contraseña. |
| [mergeNamedStyles(Workbook source)](#mergeNamedStyles-com.aspose.cells.Workbook-) | Fusiona estilos con nombre del otro archivo Excel. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [parseFormulas(boolean ignoreError)](#parseFormulas-boolean-) | Analiza todas las fórmulas que no se han analizado cuando se cargaron desde un archivo de plantilla o se asignaron a una celda. |
| [protect(int protectionType, String password)](#protect-int-java.lang.String-) | Protege un libro de trabajo. |
| [protectSharedWorkbook(String password)](#protectSharedWorkbook-java.lang.String-) | Protege un libro de trabajo compartido. |
| [refreshAll()](#refreshAll--) | Actualizar las formas vinculadas, todas las tablas dinámicas y los gráficos con la fuente de tabla dinámica. |
| [refreshDynamicArrayFormulas(boolean calculate)](#refreshDynamicArrayFormulas-boolean-) | Actualiza las fórmulas de matrices dinámicas (desbordan a un nuevo rango de celdas vecinas según los datos actuales) Otras fórmulas en el libro de trabajo no se calcularán recursivamente incluso si fueron usadas por fórmulas de matrices dinámicas. |
| [refreshDynamicArrayFormulas(boolean calculate, CalculationOptions copts)](#refreshDynamicArrayFormulas-boolean-com.aspose.cells.CalculationOptions-) | Actualiza las fórmulas de matrices dinámicas (desbordan a un nuevo rango de celdas vecinas según los datos actuales) |
| [removeDigitalSignature()](#removeDigitalSignature--) | Elimina la firma digital de esta hoja de cálculo. |
| [removeExternalLinks()](#removeExternalLinks--) | Elimina todos los enlaces externos en el libro de trabajo. |
| [removeMacro()](#removeMacro--) | Elimina VBA/macros de esta hoja de cálculo. |
| [removePersonalInformation()](#removePersonalInformation--) | Elimina información personal. |
| [removeUnusedStyles()](#removeUnusedStyles--) | Eliminar todos los estilos no utilizados. |
| [replace(boolean boolValue, Object newValue)](#replace-boolean-java.lang.Object-) | Reemplaza los valores de las celdas con datos nuevos. |
| [replace(int intValue, Object newValue)](#replace-int-java.lang.Object-) | Reemplaza los valores de las celdas con datos nuevos. |
| [replace(String placeHolder, double newValue)](#replace-java.lang.String-double-) | Reemplaza el valor de una celda con un nuevo doble. |
| [replace(String placeHolder, double[] newValues, boolean isVertical)](#replace-java.lang.String-double---boolean-) | Reemplaza los valores de las celdas con una matriz de dobles. |
| [replace(String placeHolder, int newValue)](#replace-java.lang.String-int-) | Reemplaza el valor de una celda con un nuevo entero. |
| [replace(String placeHolder, int[] newValues, boolean isVertical)](#replace-java.lang.String-int---boolean-) | Reemplaza los valores de las celdas con una matriz de enteros. |
| [replace(String placeHolder, String newValue)](#replace-java.lang.String-java.lang.String-) | Reemplaza el valor de una celda con una cadena nueva. |
| [replace(String placeHolder, String newValue, ReplaceOptions options)](#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-) | Reemplaza el valor de una celda con una cadena nueva. |
| [replace(String placeHolder, String[] newValues, boolean isVertical)](#replace-java.lang.String-java.lang.String---boolean-) | Reemplaza el valor de una celda con una nueva matriz de cadenas. |
| [save(OutputStream stream, SaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.cells.SaveOptions-) | Guardar el libro de trabajo en el flujo. |
| [save(OutputStream stream, int saveFormat)](#save-java.io.OutputStream-int-) | Guardar el libro de trabajo en el flujo. |
| [save(String fileName)](#save-java.lang.String-) | Guardar el libro de trabajo en el disco. |
| [save(String fileName, SaveOptions saveOptions)](#save-java.lang.String-com.aspose.cells.SaveOptions-) | Guarda el libro de trabajo en el disco. |
| [save(String fileName, int saveFormat)](#save-java.lang.String-int-) | Guarda el libro de trabajo en el disco. |
| [setAbsolutePath(String value)](#setAbsolutePath-java.lang.String-) | Establece la ruta absoluta del archivo. |
| [setDefaultStyle(Style value)](#setDefaultStyle-com.aspose.cells.Style-) | Establece el objeto [Style](../../com.aspose.cells/style) predeterminado del libro de trabajo. |
| [setDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)](#setDigitalSignature-com.aspose.cells.DigitalSignatureCollection-) | Establece la firma digital en un archivo de hoja de cálculo (Excel2007 y posteriores). |
| [setEncryptionOptions(int encryptionType, int keyLength)](#setEncryptionOptions-int-int-) | Establecer opciones de cifrado. |
| [setFileFormat(int value)](#setFileFormat-int-) | Establece el formato del archivo. |
| [setFileName(String value)](#setFileName-java.lang.String-) | Establece el nombre actual del archivo. |
| [setInterruptMonitor(AbstractInterruptMonitor value)](#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-) | Establece el monitor de interrupciones. |
| [setRibbonXml(String value)](#setRibbonXml-java.lang.String-) | Establece el archivo XML que define la interfaz de cinta (Ribbon UI). |
| [setThemeColor(int type, Color color)](#setThemeColor-int-com.aspose.cells.Color-) | Establece el color del tema |
| [startAccessCache(int opts)](#startAccessCache-int-) | Inicia la sesión que usa cachés para acceder a los datos. |
| [toString()](#toString--) |  |
| [unprotect(String password)](#unprotect-java.lang.String-) | Desprotege un libro de trabajo. |
| [unprotectSharedWorkbook(String password)](#unprotectSharedWorkbook-java.lang.String-) | Desprotege un libro de trabajo compartido. |
| [updateCustomFunctionDefinition(CustomFunctionDefinition definition)](#updateCustomFunctionDefinition-com.aspose.cells.CustomFunctionDefinition-) | Actualiza la definición de funciones personalizadas. |
| [updateLinkedDataSource(Workbook[] externalWorkbooks)](#updateLinkedDataSource-com.aspose.cells.Workbook---) | Si este libro de trabajo contiene enlaces externos a otras fuentes de datos, Aspose.Cells intentará recuperar los datos más recientes de las fuentes dadas. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Workbook() {#Workbook--}
```
public Workbook()
```


Inicializa una nueva instancia de la clase [Workbook](../../com.aspose.cells/workbook).

**Remarks**

El tipo de formato de archivo predeterminado es Xlsx. Si desea crear otros tipos de archivos, utilice Workbook(FileFormatType).

**Example**

El siguiente código muestra cómo usar el constructor Workbook para crear e inicializar una nueva instancia de la clase.

```
         Workbook workbook = new Workbook();
```

### Workbook(int fileFormatType) {#Workbook-int-}
```
public Workbook(int fileFormatType)
```


Inicializa una nueva instancia de la clase [Workbook](../../com.aspose.cells/workbook).

**Remarks**

El tipo de formato de archivo predeterminado es Excel97To2003.

**Example**

El siguiente código muestra cómo usar el constructor Workbook para crear e inicializar una nueva instancia de la clase con varios tipos de formato de archivo.

```
         Workbook workbook = new Workbook(FileFormatType.XLSX);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileFormatType | int | [FileFormatType](../../com.aspose.cells/fileformattype). El nuevo formato de archivo. |

### Workbook(LoadOptions loadOptions) {#Workbook-com.aspose.cells.LoadOptions-}
```
public Workbook(LoadOptions loadOptions)
```


Inicializa una nueva instancia vacía de la clase [Workbook](../../com.aspose.cells/workbook) con opciones

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| loadOptions | [LoadOptions](../../com.aspose.cells/loadoptions) | Las opciones. |

### Workbook(String file) {#Workbook-java.lang.String-}
```
public Workbook(String file)
```


Inicializa una nueva instancia de la clase [Workbook](../../com.aspose.cells/workbook) y abre un archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| archivo | java.lang.String | El nombre del archivo. |

### Workbook(InputStream stream) {#Workbook-java.io.InputStream-}
```
public Workbook(InputStream stream)
```


Inicializa una nueva instancia de la clase [Workbook](../../com.aspose.cells/workbook) y abre un flujo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.InputStream | El flujo. |

### Workbook(String file, LoadOptions loadOptions) {#Workbook-java.lang.String-com.aspose.cells.LoadOptions-}
```
public Workbook(String file, LoadOptions loadOptions)
```


Inicializa una nueva instancia de la clase [Workbook](../../com.aspose.cells/workbook) y abre un archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| archivo | java.lang.String | El nombre del archivo. |
| loadOptions | [LoadOptions](../../com.aspose.cells/loadoptions) | Las opciones de carga |

### Workbook(InputStream stream, LoadOptions loadOptions) {#Workbook-java.io.InputStream-com.aspose.cells.LoadOptions-}
```
public Workbook(InputStream stream, LoadOptions loadOptions)
```


Inicializa una nueva instancia de la clase [Workbook](../../com.aspose.cells/workbook) y abre el flujo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.InputStream | El flujo. |
| loadOptions | [LoadOptions](../../com.aspose.cells/loadoptions) | Las opciones de carga |

### acceptAllRevisions() {#acceptAllRevisions--}
```
public void acceptAllRevisions()
```


Acepta todos los cambios rastreados en el libro de trabajo.

### addDigitalSignature(DigitalSignatureCollection digitalSignatureCollection) {#addDigitalSignature-com.aspose.cells.DigitalSignatureCollection-}
```
public void addDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```


Agrega una firma digital a un archivo de hoja de cálculo OOXML (Excel2007 y posteriores).

**Remarks**

Solo se admite agregar la firma digital Xmldsig a un archivo de hoja de cálculo OOXML

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| digitalSignatureCollection | [DigitalSignatureCollection](../../com.aspose.cells/digitalsignaturecollection) |  |

### calculateFormula() {#calculateFormula--}
```
public void calculateFormula()
```


Calcula el resultado de las fórmulas.

**Remarks**

Para todas las fórmulas compatibles, consulte la lista en https://docs.aspose.com/display/cellsnet/Supported+Formula+Functions

### calculateFormula(boolean ignoreError) {#calculateFormula-boolean-}
```
public void calculateFormula(boolean ignoreError)
```


Calcula el resultado de las fórmulas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ignoreError | boolean | Indica si se oculta el error al calcular fórmulas. El error puede ser una función no compatible, enlaces externos, etc. |

### calculateFormula(CalculationOptions options) {#calculateFormula-com.aspose.cells.CalculationOptions-}
```
public void calculateFormula(CalculationOptions options)
```


Calculando fórmulas en este libro de trabajo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| options | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Opciones de cálculo |

### changePalette(Color color, int index) {#changePalette-com.aspose.cells.Color-int-}
```
public void changePalette(Color color, int index)
```


Cambia la paleta de la hoja de cálculo en el índice especificado.

**Remarks**

La paleta tiene 56 entradas, cada una representada por un valor RGB.

Si establece un color que no está en la paleta, no tendrá efecto.

Por lo tanto, si desea establecer un color personalizado, cambie la paleta primero.

La siguiente es la paleta de colores estándar.

| Color | Rojo | Verde | Azul |
| ------- | --- | ----- | ---- |
| Negro | 0 | 0 | 0 |
| Blanco | 255 | 255 | 255 |
| Rojo | 255 | 0 | 0 |
| Lima | 0 | 255 | 0 |
| Azul | 0 | 0 | 255 |
| Amarillo | 255 | 255 | 0 |
| Magenta | 255 | 0 | 255 |
| Cian | 0 | 255 | 255 |
| Marrón | 128 | 0 | 0 |
| Verde | 0 | 128 | 0 |
| Azul marino | 0 | 0 | 128 |
| Oliva | 128 | 128 | 0 |
| Morado | 128 | 0 | 128 |
| Verde azulado | 0 | 128 | 128 |
| Plateado | 192 | 192 | 192 |
| Gris | 128 | 128 | 128 |
| Color17 | 153 | 153 | 255 |
| Color18 | 153 | 51 | 102 |
| Color19 | 255 | 255 | 204 |
| Color20 | 204 | 255 | 255 |
| Color21 | 102 | 0 | 102 |
| Color22 | 255 | 128 | 128 |
| Color23 | 0 | 102 | 204 |
| Color24 | 204 | 204 | 255 |
| Color25 | 0 | 0 | 128 |
| Color26 | 255 | 0 | 255 |
| Color27 | 255 | 255 | 0 |
| Color28 | 0 | 255 | 255 |
| Color29 | 128 | 0 | 128 |
| Color30 | 128 | 0 | 0 |
| Color31 | 0 | 128 | 128 |
| Color32 | 0 | 0 | 255 |
| Color33 | 0 | 204 | 255 |
| Color34 | 204 | 255 | 255 |
| Color35 | 204 | 255 | 204 |
| Color36 | 255 | 255 | 153 |
| Color37 | 153 | 204 | 255 |
| Color38 | 255 | 153 | 204 |
| Color39 | 204 | 153 | 255 |
| Color40 | 255 | 204 | 153 |
| Color41 | 51 | 102 | 255 |
| Color42 | 51 | 204 | 204 |
| Color43 | 153 | 204 | 0 |
| Color44 | 255 | 204 | 0 |
| Color45 | 255 | 153 | 0 |
| Color46 | 255 | 102 | 0 |
| Color47 | 102 | 102 | 153 |
| Color48 | 150 | 150 | 150 |
| Color49 | 0 | 51 | 102 |
| Color50 | 51 | 153 | 102 |
| Color51 | 0 | 51 | 0 |
| Color52 | 51 | 51 | 0 |
| Color53 | 153 | 51 | 0 |
| Color54 | 153 | 51 | 102 |
| Color55 | 51 | 51 | 153 |
| Color56 | 51 | 51 | 51 |

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Estructura de color. |
| índice | int | Índice de paleta, 0 - 55. |

### closeAccessCache(int opts) {#closeAccessCache-int-}
```
public void closeAccessCache(int opts)
```


Cierra la sesión que usa cachés para acceder a los datos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| opts | int | [AccessCacheOptions](../../com.aspose.cells/accesscacheoptions). opciones de acceso a datos |

### combine(Workbook secondWorkbook) {#combine-com.aspose.cells.Workbook-}
```
public void combine(Workbook secondWorkbook)
```


Combina otro objeto Workbook.

**Remarks**

Combina Excel, ODS, CSV y otros archivos en un solo archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| secondWorkbook | [Workbook](../../com.aspose.cells/workbook) | Otro objeto Workbook. |

### copy(Workbook source) {#copy-com.aspose.cells.Workbook-}
```
public void copy(Workbook source)
```


Copia datos de un objeto Workbook fuente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| source | [Workbook](../../com.aspose.cells/workbook) | Objeto Workbook de origen. |

### copy(Workbook source, CopyOptions copyOptions) {#copy-com.aspose.cells.Workbook-com.aspose.cells.CopyOptions-}
```
public void copy(Workbook source, CopyOptions copyOptions)
```


Copia otro objeto Workbook.

**Remarks**

Es muy sencillo clonar un archivo Excel.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| source | [Workbook](../../com.aspose.cells/workbook) | Objeto Workbook de origen. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | Las opciones de copiar otro workbook. |

### copyTheme(Workbook source) {#copyTheme-com.aspose.cells.Workbook-}
```
public void copyTheme(Workbook source)
```


Copia el tema de otro libro de trabajo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| source | [Workbook](../../com.aspose.cells/workbook) | Workbook de origen. |

### createBuiltinStyle(int type) {#createBuiltinStyle-int-}
```
public Style createBuiltinStyle(int type)
```


Crea un estilo incorporado según el tipo dado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [BuiltinStyleType](../../com.aspose.cells/builtinstyletype). El estilo incorporado. |

**Returns:**
[Style](../../com.aspose.cells/style) - [Style](../../com.aspose.cells/style) object
### createCellsColor() {#createCellsColor--}
```
public CellsColor createCellsColor()
```


Crea un objeto [CellsColor](../../com.aspose.cells/cellscolor).

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor) - Returns a [CellsColor](../../com.aspose.cells/cellscolor) object.
### createStyle() {#createStyle--}
```
public Style createStyle()
```


Crea un nuevo estilo.

**Returns:**
[Style](../../com.aspose.cells/style) - Returns a style object.
### createStyle(boolean cloneDefaultStyle) {#createStyle-boolean-}
```
public Style createStyle(boolean cloneDefaultStyle)
```


Crea un nuevo estilo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cloneDefaultStyle | boolean | Indica si clona el estilo predeterminado |

**Returns:**
[Style](../../com.aspose.cells/style) - Returns a style object.
### customTheme(String themeName, Color[] colors) {#customTheme-java.lang.String-com.aspose.cells.Color---}
```
public void customTheme(String themeName, Color[] colors)
```


Personaliza el tema.

**Remarks**

La longitud de los colores debe ser 12.

| Índice de matriz | Tipo de tema |
| ----------- | ------------------ |
| 0 | Backgournd1 |
| 1 | Text1 |
| 2 | Backgournd2 |
| 3 | Text2 |
| 4 | Accent1 |
| 5 | Accent2 |
| 6 | Accent3 |
| 7 | Accent4 |
| 8 | Accent5 |
| 9 | Accent6 |
| 10 | Hipervínculo |
| 11 | Hipervínculo seguido |

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| themeName | java.lang.String | El nombre del tema |
| colors | [Color\[\]](../../com.aspose.cells/color) | Los colores del tema |

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
### exportXml(String mapName, OutputStream stream) {#exportXml-java.lang.String-java.io.OutputStream-}
```
public void exportXml(String mapName, OutputStream stream)
```


Exporta datos XML vinculados mediante el mapa XML especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| mapName | java.lang.String | nombre del mapa XML que necesita ser exportado |
| stream | java.io.OutputStream | el flujo de exportación |

### exportXml(String mapName, String path) {#exportXml-java.lang.String-java.lang.String-}
```
public void exportXml(String mapName, String path)
```


Exporta datos XML vinculados mediante el mapa XML especificado.

**Example**

El siguiente código exportó los datos vinculados por el primer XmlMap.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         //Make sure that the source xlsx file contains a XmlMap.
         XmlMap xmlMap = wb.getWorksheets().getXmlMaps().get(0);
 
         wb.exportXml(xmlMap.getName(), "output.xml");
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| mapName | java.lang.String | nombre del mapa XML que necesita ser exportado |
| ruta | java.lang.String | la ruta de exportación |

### getAbsolutePath() {#getAbsolutePath--}
```
public String getAbsolutePath()
```


Obtiene la ruta absoluta del archivo.

**Remarks**

Solo se usa para enlaces externos.

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
         DocumentProperty doc = workbook.getBuiltInDocumentProperties().get("Author");
         doc.setValue("John Smith");
```

**Returns:**
[BuiltInDocumentPropertyCollection](../../com.aspose.cells/builtindocumentpropertycollection)
### getCellsDataTableFactory() {#getCellsDataTableFactory--}
```
public CellsDataTableFactory getCellsDataTableFactory()
```


Obtiene la fábrica para crear ICellsDataTable a partir de objetos personalizados

**Returns:**
[CellsDataTableFactory](../../com.aspose.cells/cellsdatatablefactory)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColors() {#getColors--}
```
public Color[] getColors()
```


Devuelve los colores de la paleta de la hoja de cálculo.

**Remarks**

La paleta tiene 56 entradas, cada una representada por un valor RGB.

**Returns:**
com.aspose.cells.Color[]
### getContentTypeProperties() {#getContentTypeProperties--}
```
public ContentTypePropertyCollection getContentTypeProperties()
```


Obtiene la lista de objetos [ContentTypeProperty](../../com.aspose.cells/contenttypeproperty) en el libro de trabajo.

**Returns:**
[ContentTypePropertyCollection](../../com.aspose.cells/contenttypepropertycollection)
### getCountOfStylesInPool() {#getCountOfStylesInPool--}
```
public int getCountOfStylesInPool()
```


Obtiene el número de estilos en el grupo de estilos.

**Returns:**
int
### getCustomDocumentProperties() {#getCustomDocumentProperties--}
```
public CustomDocumentPropertyCollection getCustomDocumentProperties()
```


Devuelve una colección de [DocumentProperty](../../com.aspose.cells/documentproperty) que representa todas las propiedades de documento personalizadas de la hoja de cálculo.

**Example**

```
         Workbook excel = new Workbook();
         excel.getCustomDocumentProperties().add("Checked by", "Jane");
```

**Returns:**
[CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection)
### getCustomXmlParts() {#getCustomXmlParts--}
```
public CustomXmlPartCollection getCustomXmlParts()
```


Representa una parte de almacenamiento de datos XML personalizada (datos XML personalizados dentro de un paquete).

**Returns:**
[CustomXmlPartCollection](../../com.aspose.cells/customxmlpartcollection)
### getDataConnections() {#getDataConnections--}
```
public ExternalConnectionCollection getDataConnections()
```


Obtiene la colección [ExternalConnection](../../com.aspose.cells/externalconnection).

**Returns:**
[ExternalConnectionCollection](../../com.aspose.cells/externalconnectioncollection)
### getDataMashup() {#getDataMashup--}
```
public DataMashup getDataMashup()
```


Obtiene datos mashup.

**Returns:**
[DataMashup](../../com.aspose.cells/datamashup)
### getDataModel() {#getDataModel--}
```
public DataModel getDataModel()
```


Obtiene el modelo de datos en el libro de trabajo.

**Returns:**
[DataModel](../../com.aspose.cells/datamodel)
### getDataSorter() {#getDataSorter--}
```
public DataSorter getDataSorter()
```


Obtiene un objeto DataSorter para ordenar datos.

**Returns:**
[DataSorter](../../com.aspose.cells/datasorter)
### getDefaultStyle() {#getDefaultStyle--}
```
public Style getDefaultStyle()
```


Obtiene el objeto [Style](../../com.aspose.cells/style) predeterminado del libro de trabajo.

**Remarks**

La propiedad DefaultStyle es útil para implementar un Style para todo el Workbook.

**Example**

El siguiente código crea e instancia un nuevo Workbook y establece un [Style](../../com.aspose.cells/style) predeterminado.

```
         Workbook workbook = new Workbook();
         Style defaultStyle = workbook.getDefaultStyle();
         defaultStyle.getFont().setName("Tahoma");
         workbook.setDefaultStyle(defaultStyle);
```

**Returns:**
[Style](../../com.aspose.cells/style)
### getDigitalSignature() {#getDigitalSignature--}
```
public DigitalSignatureCollection getDigitalSignature()
```


Obtiene la firma digital del archivo.

**Returns:**
[DigitalSignatureCollection](../../com.aspose.cells/digitalsignaturecollection)
### getFileFormat() {#getFileFormat--}
```
public int getFileFormat()
```


Obtiene el formato de archivo.

Ver [FileFormatType](../../com.aspose.cells/fileformattype).

**Returns:**
int
### getFileName() {#getFileName--}
```
public String getFileName()
```


Obtiene el nombre de archivo actual.

**Remarks**

Si el archivo se abre mediante flujo y existen algunas referencias de fórmula externas, por favor establezca el nombre del archivo.

**Returns:**
java.lang.String
### getFonts() {#getFonts--}
```
public Font[] getFonts()
```


Obtiene todas las fuentes en el grupo de estilos.

**Returns:**
com.aspose.cells.Font[]
### getInterruptMonitor() {#getInterruptMonitor--}
```
public AbstractInterruptMonitor getInterruptMonitor()
```


Obtiene el monitor de interrupciones.

**Returns:**
[AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor)
### getMatchingColor(Color rawColor) {#getMatchingColor-com.aspose.cells.Color-}
```
public Color getMatchingColor(Color rawColor)
```


Encuentra el color que mejor coincide en la paleta actual.

**Remarks**

Solo hay 56 colores en la paleta de colores de Excel 97-2003. Si el color no está en la paleta, se establecerá el color más similar.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rawColor | [Color](../../com.aspose.cells/color) | Color sin procesar. |

**Returns:**
[Color](../../com.aspose.cells/color) - Best matching color.
### getNamedStyle(String name) {#getNamedStyle-java.lang.String-}
```
public Style getNamedStyle(String name)
```


Obtiene el estilo con nombre en el grupo de estilos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | nombre del estilo |

**Returns:**
[Style](../../com.aspose.cells/style) - named style, maybe null.
### getRibbonXml() {#getRibbonXml--}
```
public String getRibbonXml()
```


Obtiene el archivo XML que define la interfaz Ribbon.

**Returns:**
java.lang.String
### getSettings() {#getSettings--}
```
public WorkbookSettings getSettings()
```


Representa la configuración del libro de trabajo.

**Returns:**
[WorkbookSettings](../../com.aspose.cells/workbooksettings)
### getStyleInPool(int index) {#getStyleInPool-int-}
```
public Style getStyleInPool(int index)
```


Obtiene el estilo en el pool de estilos. Todos los estilos en el workbook se recopilarán en un pool. Solo hay un índice de referencia simple en las celdas.

**Remarks**

Si el estilo devuelto se modifica, el estilo de todas las celdas (que hacen referencia a este estilo) se cambiará.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice. |

**Returns:**
[Style](../../com.aspose.cells/style) - The style in the pool corresponds to given index, may be null.
### getTheme() {#getTheme--}
```
public String getTheme()
```


Obtiene el nombre del tema.

**Returns:**
java.lang.String
### getThemeColor(int type) {#getThemeColor-int-}
```
public Color getThemeColor(int type)
```


Obtiene el color del tema.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [ThemeColorType](../../com.aspose.cells/themecolortype). El tipo de color del tema. |

**Returns:**
[Color](../../com.aspose.cells/color) - The theme color.
### getVbaProject() {#getVbaProject--}
```
public VbaProject getVbaProject()
```


Obtiene el [getVbaProject()](../../com.aspose.cells/workbook\#getVbaProject--) en una hoja de cálculo.

**Returns:**
[VbaProject](../../com.aspose.cells/vbaproject)
### getWorksheets() {#getWorksheets--}
```
public WorksheetCollection getWorksheets()
```


Obtiene la colección [WorksheetCollection](../../com.aspose.cells/worksheetcollection) en la hoja de cálculo.

**Returns:**
[WorksheetCollection](../../com.aspose.cells/worksheetcollection) - [WorksheetCollection](../../com.aspose.cells/worksheetcollection) collection
### hasCustomFunction() {#hasCustomFunction--}
```
public boolean hasCustomFunction()
```


Detecta si hay una función personalizada utilizada en este libro de trabajo, como en la fórmula de una celda, en nombres definidos...

**Returns:**
boolean
### hasExernalLinks() {#hasExernalLinks--}
```
public boolean hasExernalLinks()
```


Indica si este libro de trabajo contiene enlaces externos a otras fuentes de datos.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use ExternalLinkCollection.Count para comprobar si hay enlaces externos en este workbook. Este método será eliminado 12 meses después, a partir de diciembre de 2021. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
boolean - Indica si este workbook contiene enlaces externos a otras fuentes de datos.
### hasMacro() {#hasMacro--}
```
public boolean hasMacro()
```


Indica si esta hoja de cálculo contiene macro/VBA.

**Returns:**
boolean
### hasRevisions() {#hasRevisions--}
```
public boolean hasRevisions()
```


Obtiene si el libro de trabajo tiene cambios rastreados

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### importXml(InputStream stream, String sheetName, int row, int col) {#importXml-java.io.InputStream-java.lang.String-int-int-}
```
public void importXml(InputStream stream, String sheetName, int row, int col)
```


Importa/Actualiza un archivo de datos XML en el libro de trabajo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.InputStream | el flujo del archivo xml. |
| sheetName | java.lang.String | el nombre de la hoja de destino. |
| fila | int | la fila de destino. |
| col | int | la columna de destino. |

### importXml(String url, String sheetName, int row, int col) {#importXml-java.lang.String-java.lang.String-int-int-}
```
public void importXml(String url, String sheetName, int row, int col)
```


Importa/Actualiza un archivo de datos XML en el libro de trabajo.

**Example**

El siguiente código importa datos xml a la hoja de cálculo 'Sheet 1' en la celda A1.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         wb.importXml("xml.xml", "Sheet1", 0, 0);
 
         wb.save("output.xlsx");
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| url | java.lang.String | la url/ruta del archivo xml. |
| sheetName | java.lang.String | el nombre de la hoja de destino. |
| fila | int | la fila de destino |
| col | int | la columna de destino |

### isColorInPalette(Color color) {#isColorInPalette-com.aspose.cells.Color-}
```
public boolean isColorInPalette(Color color)
```


Comprueba si un color está en la paleta de la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Estructura de color. |

**Returns:**
booleano - Devuelve true si este color está en la paleta. De lo contrario, devuelve false
### isDigitallySigned() {#isDigitallySigned--}
```
public boolean isDigitallySigned()
```


Indica si esta hoja de cálculo está firmada digitalmente.

**Returns:**
boolean
### isLicensed() {#isLicensed--}
```
public boolean isLicensed()
```


Indica si la licencia está establecida.

**Returns:**
boolean
### isWorkbookProtectedWithPassword() {#isWorkbookProtectedWithPassword--}
```
public boolean isWorkbookProtectedWithPassword()
```


Indica si la estructura o la ventana están protegidas con contraseña.

**Returns:**
boolean
### mergeNamedStyles(Workbook source) {#mergeNamedStyles-com.aspose.cells.Workbook-}
```
public void mergeNamedStyles(Workbook source)
```


Fusiona estilos con nombre del otro archivo Excel.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| source | [Workbook](../../com.aspose.cells/workbook) | El otro archivo |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### parseFormulas(boolean ignoreError) {#parseFormulas-boolean-}
```
public void parseFormulas(boolean ignoreError)
```


Analiza todas las fórmulas que no se han analizado cuando se cargaron desde un archivo de plantilla o se asignaron a una celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ignoreError | boolean | Indica si se ignora el error para una fórmula inválida. Para una fórmula inválida, si se ignora el error, esa fórmula será omitida y el proceso continuará analizando otras fórmulas; de lo contrario se lanzará una excepción. |

### protect(int protectionType, String password) {#protect-int-java.lang.String-}
```
public void protect(int protectionType, String password)
```


Protege un libro de trabajo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| protectionType | int | [ProtectionType](../../com.aspose.cells/protectiontype). Tipo de protección. |
| password | java.lang.String | Contraseña para proteger el libro de trabajo. |

### protectSharedWorkbook(String password) {#protectSharedWorkbook-java.lang.String-}
```
public void protectSharedWorkbook(String password)
```


Protege un libro de trabajo compartido.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| password | java.lang.String | Contraseña para proteger el libro de trabajo. |

### refreshAll() {#refreshAll--}
```
public void refreshAll()
```


Actualizar las formas vinculadas, todas las tablas dinámicas y los gráficos con la fuente de tabla dinámica.

### refreshDynamicArrayFormulas(boolean calculate) {#refreshDynamicArrayFormulas-boolean-}
```
public void refreshDynamicArrayFormulas(boolean calculate)
```


Actualiza las fórmulas de matrices dinámicas (desbordan a un nuevo rango de celdas vecinas según los datos actuales) Otras fórmulas en el libro de trabajo no se calcularán recursivamente incluso si fueron usadas por fórmulas de matrices dinámicas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| calcular | boolean | Indica si calcula y actualiza los valores de celda para esas fórmulas de matrices dinámicas |

### refreshDynamicArrayFormulas(boolean calculate, CalculationOptions copts) {#refreshDynamicArrayFormulas-boolean-com.aspose.cells.CalculationOptions-}
```
public void refreshDynamicArrayFormulas(boolean calculate, CalculationOptions copts)
```


Actualiza las fórmulas de matrices dinámicas (desbordan a un nuevo rango de celdas vecinas según los datos actuales)

**Remarks**

Por consideraciones de rendimiento, no actualizamos automáticamente todas las fórmulas de matrices dinámicas cuando la propia fórmula o los datos a los que hace referencia cambian. Por lo tanto, el usuario debe llamar a este método manualmente después de esas operaciones que puedan influir en las fórmulas de matrices dinámicas, como importar/establecer valores de celda, insertar/eliminar filas/columnas/rangos, etc.

Para la mayoría de las fórmulas con funciones, calcular el rango de desbordamiento también requiere calcular la fórmula, por lo que en general se prefiere el valor true para la bandera "calculate". Si la fórmula es simple, como una referencia de rango o una matriz (por ejemplo "=C1:E5", "=\{1,2;3,4\}", ...), una función simple sobre un rango o matriz (por ejemplo "=ABS(C1:E5)", "=1+\{1,2;3,4\}", ...), y todas las fórmulas se calcularán más tarde (por ejemplo mediante [calculateFormula(CalculationOptions)](../../com.aspose.cells/workbook\\#calculateFormula-CalculationOptions-)), entonces usar el valor false para la bandera "calculate" puede evitar el cálculo duplicado en beneficio del rendimiento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| calcular | boolean | Indica si calcula y actualiza los valores de celda para esas fórmulas de matrices dinámicas |
| copts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Las opciones para calcular fórmulas |

### removeDigitalSignature() {#removeDigitalSignature--}
```
public void removeDigitalSignature()
```


Elimina la firma digital de esta hoja de cálculo.

### removeExternalLinks() {#removeExternalLinks--}
```
public void removeExternalLinks()
```


Elimina todos los enlaces externos en el libro de trabajo.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice el método ExternalLinkCollection.Clear(). Este método será eliminado 12 meses después, desde diciembre de 2021. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### removeMacro() {#removeMacro--}
```
public void removeMacro()
```


Elimina VBA/macros de esta hoja de cálculo.

### removePersonalInformation() {#removePersonalInformation--}
```
public void removePersonalInformation()
```


Elimina información personal.

### removeUnusedStyles() {#removeUnusedStyles--}
```
public void removeUnusedStyles()
```


Eliminar todos los estilos no utilizados.

### replace(boolean boolValue, Object newValue) {#replace-boolean-java.lang.Object-}
```
public int replace(boolean boolValue, Object newValue)
```


Reemplaza los valores de las celdas con datos nuevos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| boolValue | boolean | El valor booleano a reemplazar. |
| newValue | java.lang.Object | Nuevo valor. Puede ser una cadena, entero, doble o valor DateTime. |

**Returns:**
int
### replace(int intValue, Object newValue) {#replace-int-java.lang.Object-}
```
public int replace(int intValue, Object newValue)
```


Reemplaza los valores de las celdas con datos nuevos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| intValue | int | El valor entero a reemplazar. |
| newValue | java.lang.Object | Nuevo valor. Puede ser una cadena, entero, doble o valor DateTime. |

**Returns:**
int
### replace(String placeHolder, double newValue) {#replace-java.lang.String-double-}
```
public int replace(String placeHolder, double newValue)
```


Reemplaza el valor de una celda con un nuevo doble.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         double newValue = 100.0;
         workbook.replace("AnOldValue", newValue);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| placeHolder | java.lang.String | Marcador de posición de celda |
| newValue | double | Valor double a reemplazar |

**Returns:**
int
### replace(String placeHolder, double[] newValues, boolean isVertical) {#replace-java.lang.String-double---boolean-}
```
public int replace(String placeHolder, double[] newValues, boolean isVertical)
```


Reemplaza los valores de las celdas con una matriz de dobles.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         double[] newValues = new double[]{1.23, 2.56, 3.14159};
         workbook.replace("AnOldValue", newValues, true);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| placeHolder | java.lang.String | Marcador de posición de celda |
| newValues | double[] | Arreglo Double para reemplazar |
| isVertical | boolean | Verdadero - Vertical, Falso - Horizontal |

**Returns:**
int
### replace(String placeHolder, int newValue) {#replace-java.lang.String-int-}
```
public int replace(String placeHolder, int newValue)
```


Reemplaza el valor de una celda con un nuevo entero.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         int newValue = 100;
         workbook.replace("AnOldValue", newValue);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| placeHolder | java.lang.String | Marcador de posición de celda |
| newValue | int | Valor entero para reemplazar |

**Returns:**
int
### replace(String placeHolder, int[] newValues, boolean isVertical) {#replace-java.lang.String-int---boolean-}
```
public int replace(String placeHolder, int[] newValues, boolean isVertical)
```


Reemplaza los valores de las celdas con una matriz de enteros.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         int[] newValues = new int[]{1, 2, 3};
         workbook.replace("AnOldValue", newValues, true);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| placeHolder | java.lang.String | Marcador de posición de celda |
| newValues | int[] | Arreglo entero para reemplazar |
| isVertical | boolean | Verdadero - Vertical, Falso - Horizontal |

**Returns:**
int
### replace(String placeHolder, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public int replace(String placeHolder, String newValue)
```


Reemplaza el valor de una celda con una cadena nueva.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         workbook.replace("AnOldValue", "NewValue");
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| placeHolder | java.lang.String | Marcador de posición de celda |
| newValue | java.lang.String | Valor de cadena para reemplazar |

**Returns:**
int
### replace(String placeHolder, String newValue, ReplaceOptions options) {#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-}
```
public int replace(String placeHolder, String newValue, ReplaceOptions options)
```


Reemplaza el valor de una celda con una cadena nueva.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| placeHolder | java.lang.String | Marcador de posición de celda |
| newValue | java.lang.String | Valor de cadena para reemplazar |
| options | [ReplaceOptions](../../com.aspose.cells/replaceoptions) | Las opciones de reemplazo |

**Returns:**
int
### replace(String placeHolder, String[] newValues, boolean isVertical) {#replace-java.lang.String-java.lang.String---boolean-}
```
public int replace(String placeHolder, String[] newValues, boolean isVertical)
```


Reemplaza el valor de una celda con una nueva matriz de cadenas.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         String[] newValues = new String[]{"Tom", "Alice", "Jerry"};
         workbook.replace("AnOldValue", newValues, true);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| placeHolder | java.lang.String | Marcador de posición de celda |
| newValues | java.lang.String[] | Arreglo de cadena para reemplazar |
| isVertical | boolean | Verdadero - Vertical, Falso - Horizontal |

**Returns:**
int
### save(OutputStream stream, SaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.cells.SaveOptions-}
```
public void save(OutputStream stream, SaveOptions saveOptions)
```


Guardar el libro de trabajo en el flujo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.OutputStream | El flujo de archivo. |
| saveOptions | [SaveOptions](../../com.aspose.cells/saveoptions) | Las opciones de guardado. |

### save(OutputStream stream, int saveFormat) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int saveFormat)
```


Guardar el libro de trabajo en el flujo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.OutputStream | El flujo de archivo. |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). El tipo de formato de archivo guardado. |

### save(String fileName) {#save-java.lang.String-}
```
public void save(String fileName)
```


Guardar el libro de trabajo en el disco.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | java.lang.String |  |

### save(String fileName, SaveOptions saveOptions) {#save-java.lang.String-com.aspose.cells.SaveOptions-}
```
public void save(String fileName, SaveOptions saveOptions)
```


Guarda el libro de trabajo en el disco.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | java.lang.String | El nombre del archivo. |
| saveOptions | [SaveOptions](../../com.aspose.cells/saveoptions) | Las opciones de guardado. |

### save(String fileName, int saveFormat) {#save-java.lang.String-int-}
```
public void save(String fileName, int saveFormat)
```


Guarda el libro de trabajo en el disco.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | java.lang.String | El nombre del archivo. |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). El tipo de formato de guardado. |

### setAbsolutePath(String value) {#setAbsolutePath-java.lang.String-}
```
public void setAbsolutePath(String value)
```


Establece la ruta absoluta del archivo.

**Remarks**

Solo se usa para enlaces externos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setDefaultStyle(Style value) {#setDefaultStyle-com.aspose.cells.Style-}
```
public void setDefaultStyle(Style value)
```


Establece el objeto [Style](../../com.aspose.cells/style) predeterminado del libro de trabajo.

**Remarks**

La propiedad DefaultStyle es útil para implementar un Style para todo el Workbook.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setDigitalSignature(DigitalSignatureCollection digitalSignatureCollection) {#setDigitalSignature-com.aspose.cells.DigitalSignatureCollection-}
```
public void setDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```


Establece la firma digital en un archivo de hoja de cálculo (Excel2007 y posteriores).

**Remarks**

Solo se admite agregar Xmldsig Digital Signature

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| digitalSignatureCollection | [DigitalSignatureCollection](../../com.aspose.cells/digitalsignaturecollection) |  |

### setEncryptionOptions(int encryptionType, int keyLength) {#setEncryptionOptions-int-int-}
```
public void setEncryptionOptions(int encryptionType, int keyLength)
```


Establecer opciones de cifrado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| encryptionType | int | [EncryptionType](../../com.aspose.cells/encryptiontype). El tipo de cifrado. |
| keyLength | int | La longitud de la clave. |

### setFileFormat(int value) {#setFileFormat-int-}
```
public void setFileFormat(int value)
```


Establece el formato del archivo.

Ver [FileFormatType](../../com.aspose.cells/fileformattype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setFileName(String value) {#setFileName-java.lang.String-}
```
public void setFileName(String value)
```


Establece el nombre actual del archivo.

**Remarks**

Si el archivo se abre mediante flujo y existen algunas referencias de fórmula externas, por favor establezca el nombre del archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setInterruptMonitor(AbstractInterruptMonitor value) {#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-}
```
public void setInterruptMonitor(AbstractInterruptMonitor value)
```


Establece el monitor de interrupciones.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor) |  |

### setRibbonXml(String value) {#setRibbonXml-java.lang.String-}
```
public void setRibbonXml(String value)
```


Establece el archivo XML que define la interfaz de cinta (Ribbon UI).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setThemeColor(int type, Color color) {#setThemeColor-int-com.aspose.cells.Color-}
```
public void setThemeColor(int type, Color color)
```


Establece el color del tema

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [ThemeColorType](../../com.aspose.cells/themecolortype). El tipo de color del tema. |
| color | [Color](../../com.aspose.cells/color) | el color del tema |

### startAccessCache(int opts) {#startAccessCache-int-}
```
public void startAccessCache(int opts)
```


Inicia la sesión que usa cachés para acceder a los datos.

**Remarks**

Si la caché del acceso a datos especificado requiere que algunos modelos de datos en la hoja de cálculo sean "read-only", entonces los modelos de datos correspondientes en cada hoja de cálculo de este libro se considerarán "read-only" y el usuario no debe modificar ninguno de ellos.

Después de terminar el acceso a los datos, [closeAccessCache(int)](../../com.aspose.cells/workbook\#closeAccessCache-int-) debe invocarse con las mismas opciones para borrar todas las cachés y recuperar el modo de acceso normal.



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| opts | int | [AccessCacheOptions](../../com.aspose.cells/accesscacheoptions). opciones de acceso a datos |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### unprotect(String password) {#unprotect-java.lang.String-}
```
public void unprotect(String password)
```


Desprotege un libro de trabajo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| password | java.lang.String | Contraseña para desproteger el libro. |

### unprotectSharedWorkbook(String password) {#unprotectSharedWorkbook-java.lang.String-}
```
public void unprotectSharedWorkbook(String password)
```


Desprotege un libro de trabajo compartido.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| password | java.lang.String | Contraseña para desproteger el libro. |

### updateCustomFunctionDefinition(CustomFunctionDefinition definition) {#updateCustomFunctionDefinition-com.aspose.cells.CustomFunctionDefinition-}
```
public void updateCustomFunctionDefinition(CustomFunctionDefinition definition)
```


Actualiza la definición de funciones personalizadas.

**Remarks**

Este método puede usarse en algunos escenarios especiales. Por ejemplo, si el usuario necesita que algunos parámetros de funciones personalizadas se calculen en modo de matriz, entonces el usuario puede proporcionar su propia definición con la implementación de [CustomFunctionDefinition.getArrayModeParameters(String)](../../com.aspose.cells/customfunctiondefinition\#getArrayModeParameters-String-) para esas funciones. Después de que los datos de las fórmulas se actualicen, esos parámetros especificados se calcularán automáticamente en modo de matriz al calcular las funciones personalizadas correspondientes.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| definition | [CustomFunctionDefinition](../../com.aspose.cells/customfunctiondefinition) | Definición especial de funciones personalizadas para el requisito especial del usuario. |

### updateLinkedDataSource(Workbook[] externalWorkbooks) {#updateLinkedDataSource-com.aspose.cells.Workbook---}
```
public void updateLinkedDataSource(Workbook[] externalWorkbooks)
```


Si este libro de trabajo contiene enlaces externos a otras fuentes de datos, Aspose.Cells intentará recuperar los datos más recientes de las fuentes dadas.

**Remarks**

Si no se encuentra el enlace externo correspondiente para un libro, entonces ese libro será ignorado. Por lo tanto, cuando establezca una fórmula más tarde con un nuevo enlace externo que pretende vincular al libro ignorado, el enlace no se podrá realizar hasta que vuelva a llamar a este método con esos libros.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| externalWorkbooks | [Workbook\[\]](../../com.aspose.cells/workbook) | Libros que se usarán para actualizar los datos de los enlaces externos referenciados por este libro. La coincidencia de esos libros con los enlaces externos se determina mediante [getFileName()](../../com.aspose.cells/workbook\#getFileName--) y [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--). Por lo tanto, asegúrese de que [getFileName()](../../com.aspose.cells/workbook\#getFileName--) haya sido especificado con el valor correcto para cada libro, de modo que puedan enlazarse al enlace externo correspondiente. |

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

