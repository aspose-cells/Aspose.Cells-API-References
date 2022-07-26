---
title: Workbook
second_title: Referencia de API de Aspose.Cells para .NET
description: Representa un objeto raíz para crear una hoja de cálculo de Excel.
type: docs
weight: 6480
url: /es/net/aspose.cells/workbook/
---
## Workbook class

Representa un objeto raíz para crear una hoja de cálculo de Excel.

```csharp
public class Workbook : IDisposable
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [Workbook](workbook#constructor)() | Inicializa una nueva instancia del[`Workbook`](../workbook) clase. |
| [Workbook](workbook#constructor_1)(FileFormatType) | Inicializa una nueva instancia del[`Workbook`](../workbook) clase. |
| [Workbook](workbook#constructor_2)(Stream) | Inicializa una nueva instancia del[`Workbook`](../workbook) class y abre un stream. |
| [Workbook](workbook#constructor_4)(string) | Inicializa una nueva instancia del[`Workbook`](../workbook) clase y abra un archivo. |
| [Workbook](workbook#constructor_3)(Stream, LoadOptions) | Inicializa una nueva instancia del[`Workbook`](../workbook) clase y flujo abierto. |
| [Workbook](workbook#constructor_5)(string, LoadOptions) | Inicializa una nueva instancia del[`Workbook`](../workbook) clase y abra un archivo. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AbsolutePath](../../aspose.cells/workbook/absolutepath) { get; set; } | Obtiene y establece la ruta absoluta del archivo. |
| [BuiltInDocumentProperties](../../aspose.cells/workbook/builtindocumentproperties) { get; } | Devuelve un[`DocumentProperty`](../../aspose.cells.properties/documentproperty)colección que representa todas las propiedades de documento integradas de la hoja de cálculo. |
| [CellsDataTableFactory](../../aspose.cells/workbook/cellsdatatablefactory) { get; } | Obtiene la fábrica para construir ICellsDataTable a partir de objetos personalizados |
| [Colors](../../aspose.cells/workbook/colors) { get; } | Devuelve los colores de la paleta de la hoja de cálculo. |
| [ContentTypeProperties](../../aspose.cells/workbook/contenttypeproperties) { get; } | Obtiene la lista de[`ContentTypeProperty`](../../aspose.cells.properties/contenttypeproperty) objetos en el libro de trabajo. |
| [CountOfStylesInPool](../../aspose.cells/workbook/countofstylesinpool) { get; } | Obtiene el número de estilos en el grupo de estilos. |
| [CustomDocumentProperties](../../aspose.cells/workbook/customdocumentproperties) { get; } | Devuelve un[`DocumentProperty`](../../aspose.cells.properties/documentproperty) colección que representa todas las propiedades del documento personalizado de la hoja de cálculo. |
| [CustomXmlParts](../../aspose.cells/workbook/customxmlparts) { get; } | Representa una parte de almacenamiento de datos XML personalizados (datos XML personalizados dentro de un paquete). |
| [DataConnections](../../aspose.cells/workbook/dataconnections) { get; } | Obtiene el[`ExternalConnection`](../../aspose.cells.externalconnections/externalconnection) colección. |
| [DataMashup](../../aspose.cells/workbook/datamashup) { get; } | Obtiene datos de mashup. |
| [DataSorter](../../aspose.cells/workbook/datasorter) { get; } | Obtiene un objeto DataSorter para ordenar datos. |
| [DefaultStyle](../../aspose.cells/workbook/defaultstyle) { get; set; } | Obtiene o establece el valor predeterminado[`Style`](../style) objeto del libro. |
| [FileFormat](../../aspose.cells/workbook/fileformat) { get; set; } | Obtiene y establece el formato del archivo. |
| [FileName](../../aspose.cells/workbook/filename) { get; set; } | Obtiene y establece el nombre del archivo actual. |
| [HasMacro](../../aspose.cells/workbook/hasmacro) { get; } | Indica si esta hoja de cálculo contiene macro/VBA. |
| [HasRevisions](../../aspose.cells/workbook/hasrevisions) { get; } | Obtiene si el libro de trabajo tiene cambios rastreados |
| [InterruptMonitor](../../aspose.cells/workbook/interruptmonitor) { get; set; } | Obtiene y establece el monitor de interrupción. |
| [IsDigitallySigned](../../aspose.cells/workbook/isdigitallysigned) { get; } | Indica si esta hoja de cálculo está firmada digitalmente. |
| [IsLicensed](../../aspose.cells/workbook/islicensed) { get; } | Indica si la licencia está configurada. |
| [IsWorkbookProtectedWithPassword](../../aspose.cells/workbook/isworkbookprotectedwithpassword) { get; } | Indica si la estructura o ventana está protegida con contraseña. |
| [RibbonXml](../../aspose.cells/workbook/ribbonxml) { get; set; } | Obtiene y establece el archivo XML que define la interfaz de usuario de Ribbon. |
| [Settings](../../aspose.cells/workbook/settings) { get; } | Representa la configuración del libro. |
| [Theme](../../aspose.cells/workbook/theme) { get; } | Obtiene el nombre del tema. |
| [VbaProject](../../aspose.cells/workbook/vbaproject) { get; } | Obtiene el[`VbaProject`](./vbaproject) en una hoja de cálculo. |
| [Worksheets](../../aspose.cells/workbook/worksheets) { get; } | Obtiene el[`WorksheetCollection`](../worksheetcollection) colección en la hoja de cálculo. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AcceptAllRevisions](../../aspose.cells/workbook/acceptallrevisions)() | Acepta todos los cambios registrados en el libro de trabajo. |
| [AddDigitalSignature](../../aspose.cells/workbook/adddigitalsignature)(DigitalSignatureCollection) | Agrega una firma digital a un archivo de hoja de cálculo OOXML (Excel 2007 y posterior). |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula#calculateformula)() | Calcula el resultado de fórmulas. |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula#calculateformula_2)(bool) | Calcula el resultado de fórmulas. |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula#calculateformula_1)(CalculationOptions) | Cálculo de fórmulas en este libro. |
| [ChangePalette](../../aspose.cells/workbook/changepalette)(Color, int) | Cambia la paleta de la hoja de cálculo en el índice especificado. |
| [CloseAccessCache](../../aspose.cells/workbook/closeaccesscache)(AccessCacheOptions) | Cierra la sesión que usa cachés para acceder a los datos. |
| [Combine](../../aspose.cells/workbook/combine)(Workbook) | Combina otro objeto Workbook. |
| [Copy](../../aspose.cells/workbook/copy#copy)(Workbook) | Copia datos de un objeto de libro de trabajo de origen. |
| [Copy](../../aspose.cells/workbook/copy#copy_1)(Workbook, CopyOptions) | Copia datos de un objeto de libro de trabajo de origen. |
| [CopyTheme](../../aspose.cells/workbook/copytheme)(Workbook) | Copia el tema de otro libro. |
| [CreateBuiltinStyle](../../aspose.cells/workbook/createbuiltinstyle)(BuiltinStyleType) | Crea un estilo incorporado por tipo dado. |
| [CreateCellsColor](../../aspose.cells/workbook/createcellscolor)() | Crea un[`CellsColor`](../cellscolor) objeto. |
| [CreateStyle](../../aspose.cells/workbook/createstyle)() | Crea un nuevo estilo. |
| [CustomTheme](../../aspose.cells/workbook/customtheme)(string, Color[]) | Personaliza el tema. |
| [Dispose](../../aspose.cells/workbook/dispose)() | Realiza tareas definidas por la aplicación asociadas con la liberación, liberación o restablecimiento de recursos no administrados. |
| [ExportXml](../../aspose.cells/workbook/exportxml#exportxml)(string, Stream) | Exportar datos XML. |
| [ExportXml](../../aspose.cells/workbook/exportxml#exportxml_1)(string, string) | Exportar datos XML vinculados por el mapa XML especificado. |
| [GetDigitalSignature](../../aspose.cells/workbook/getdigitalsignature)() | Obtiene la firma digital del archivo. |
| [GetFonts](../../aspose.cells/workbook/getfonts)() | Obtiene todas las fuentes en el grupo de estilos. |
| [GetMatchingColor](../../aspose.cells/workbook/getmatchingcolor)(Color) | Encuentra el mejor color coincidente en la paleta actual. |
| [GetNamedStyle](../../aspose.cells/workbook/getnamedstyle)(string) | Obtiene el estilo con nombre en el grupo de estilos. |
| [GetStyleInPool](../../aspose.cells/workbook/getstyleinpool)(int) | Obtiene el estilo en el grupo de estilos. Todos los estilos del libro de trabajo se reunirán en un grupo. Solo hay un índice de referencia simple en las celdas. |
| [GetThemeColor](../../aspose.cells/workbook/getthemecolor)(ThemeColorType) | Obtiene el color del tema. |
| [ImportXml](../../aspose.cells/workbook/importxml#importxml)(Stream, string, int, int) | Importa/Actualiza un archivo de datos XML en el libro de trabajo. |
| [ImportXml](../../aspose.cells/workbook/importxml#importxml_1)(string, string, int, int) | Importa/Actualiza un archivo de datos XML en el libro de trabajo. |
| [IsColorInPalette](../../aspose.cells/workbook/iscolorinpalette)(Color) | Comprueba si un color está en la paleta de la hoja de cálculo. |
| [ParseFormulas](../../aspose.cells/workbook/parseformulas)(bool) | Analiza todas las fórmulas que no se analizaron cuando se cargaron desde un archivo de plantilla o se establecieron en una celda. |
| [Protect](../../aspose.cells/workbook/protect)(ProtectionType, string) | Protege un libro de trabajo. |
| [ProtectSharedWorkbook](../../aspose.cells/workbook/protectsharedworkbook)(string) | Protege un libro de trabajo compartido. |
| [RefreshDynamicArrayFormulas](../../aspose.cells/workbook/refreshdynamicarrayformulas)(bool) | Actualiza las fórmulas de matrices dinámicas (se derrama en un nuevo rango de celdas vecinas según los datos actuales) |
| [RemoveDigitalSignature](../../aspose.cells/workbook/removedigitalsignature)() | Elimina la firma digital de esta hoja de cálculo. |
| [RemoveMacro](../../aspose.cells/workbook/removemacro)() | Elimina VBA/macro de esta hoja de cálculo. |
| [RemovePersonalInformation](../../aspose.cells/workbook/removepersonalinformation)() | Elimina información personal. |
| [RemoveUnusedStyles](../../aspose.cells/workbook/removeunusedstyles)() | Eliminar todos los estilos no utilizados. |
| [Replace](../../aspose.cells/workbook/replace#replace)(bool, object) | Reemplaza los valores de las celdas con nuevos datos. |
| [Replace](../../aspose.cells/workbook/replace#replace_1)(int, object) | Reemplaza los valores de las celdas con nuevos datos. |
| [Replace](../../aspose.cells/workbook/replace#replace_6)(string, DataTable) | Reemplaza los valores de las celdas con datos de unDataTable . |
| [Replace](../../aspose.cells/workbook/replace#replace_2)(string, double) | Reemplaza el valor de una celda con un nuevo doble. |
| [Replace](../../aspose.cells/workbook/replace#replace_4)(string, int) | Reemplaza el valor de una celda con un nuevo entero. |
| [Replace](../../aspose.cells/workbook/replace#replace_7)(string, string) | Reemplaza el valor de una celda con una nueva cadena. |
| [Replace](../../aspose.cells/workbook/replace#replace_3)(string, double[], bool) | Reemplaza los valores de las celdas con una matriz doble. |
| [Replace](../../aspose.cells/workbook/replace#replace_5)(string, int[], bool) | Reemplaza los valores de las celdas con una matriz de enteros. |
| [Replace](../../aspose.cells/workbook/replace#replace_8)(string, string, ReplaceOptions) | Reemplaza el valor de una celda con una nueva cadena. |
| [Replace](../../aspose.cells/workbook/replace#replace_9)(string, string[], bool) | Reemplaza el valor de una celda con una nueva matriz de cadenas. |
| [Save](../../aspose.cells/workbook/save#save_2)(string) | Guarde el libro de trabajo en el disco. |
| [Save](../../aspose.cells/workbook/save#save)(Stream, SaveFormat) | Guarda el libro de trabajo en la secuencia. |
| [Save](../../aspose.cells/workbook/save#save_1)(Stream, SaveOptions) | Guarda el libro de trabajo en la secuencia. |
| [Save](../../aspose.cells/workbook/save#save_3)(string, SaveFormat) | Guarda el libro de trabajo en el disco. |
| [Save](../../aspose.cells/workbook/save#save_4)(string, SaveOptions) | Guarda el libro de trabajo en el disco. |
| [Save](../../aspose.cells/workbook/save#save_5)(HttpResponse, string, ContentDisposition, SaveOptions) | Crea la hoja de cálculo de resultados y la transfiere al cliente y luego la abre en el navegador o en MS Workbook. |
| [Save](../../aspose.cells/workbook/save#save_6)(HttpResponse, string, ContentDisposition, SaveOptions, bool) | Crea la hoja de cálculo de resultados y la transfiere al cliente y luego la abre en el navegador o en MS Workbook. |
| [SaveToStream](../../aspose.cells/workbook/savetostream)() | Guarda el archivo de Excel en un objeto MemoryStream y lo devuelve. |
| [SetDigitalSignature](../../aspose.cells/workbook/setdigitalsignature)(DigitalSignatureCollection) | Establece la firma digital en un archivo de hoja de cálculo (Excel 2007 y posterior). |
| [SetEncryptionOptions](../../aspose.cells/workbook/setencryptionoptions)(EncryptionType, int) | Establecer opciones de cifrado. |
| [SetThemeColor](../../aspose.cells/workbook/setthemecolor)(ThemeColorType, Color) | Establece el color del tema |
| [StartAccessCache](../../aspose.cells/workbook/startaccesscache)(AccessCacheOptions) | Inicia la sesión que utiliza cachés para acceder a los datos. |
| [Unprotect](../../aspose.cells/workbook/unprotect)(string) | Desprotege un libro. |
| [UnprotectSharedWorkbook](../../aspose.cells/workbook/unprotectsharedworkbook)(string) | Desprotege un libro de trabajo compartido. |
| [UpdateLinkedDataSource](../../aspose.cells/workbook/updatelinkeddatasource)(Workbook[]) | Si este libro de trabajo contiene enlaces externos a otra fuente de datos, Aspose.Cells intentará recuperar los datos más recientes. |

### Observaciones

La clase Workbook denota una hoja de cálculo de Excel. Cada hoja de cálculo puede contener varias hojas de trabajo. La función básica de la clase es abrir y guardar archivos nativos de Excel. La clase tiene algunas funciones avanzadas, como copiar datos de otros libros de trabajo, combinar dos libros de trabajo y proteger la hoja de cálculo de Excel.

### Ejemplos

El siguiente ejemplo carga un libro de trabajo desde un archivo llamado designer.xls y hace que las barras de desplazamiento horizontal y vertical sean invisibles para el libro de trabajo. Luego reemplaza dos valores de cadena con un valor entero y un valor de cadena respectivamente dentro de la hoja de cálculo y finalmente envía el archivo actualizado al navegador del cliente.

```csharp
[C#]

//Abrir un archivo de diseñador
string designerFile = "designer.xls";
Workbook workbook = new Workbook(designerFile);

//Establecer barras de desplazamiento
workbook.Settings.IsHScrollBarVisible = false;
workbook.Settings.IsVScrollBarVisible = false;

//Reemplazar la cadena de marcador de posición con nuevos valores
int newInt = 100;
workbook.Replace("OldInt", newInt);

string newString = "Hello!";
workbook.Replace("OldString", newString);
workbook.Save("result.xls");

[Visual Basic]

'Abrir un archivo de diseñador
Dim designerFile as String = "\designer.xls"
Dim workbook as Workbook = new Workbook(designerFile)

'Establecer barras de desplazamiento
workbook.IsHScrollBarVisible = False
workbook.IsVScrollBarVisible = False

'Reemplace la cadena de marcador de posición con nuevos valores
Dim newInt as Integer = 100
workbook.Replace("OldInt", newInt)

Dim newString as String = "Hello!"
workbook.Replace("OldString", newString)
workbook.Save("result.xls")    
```

### Ver también

* espacio de nombres [Aspose.Cells](../../aspose.cells)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
