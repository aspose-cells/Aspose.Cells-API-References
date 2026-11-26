---
title: "Clase Workbook"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Workbook. Representa un objeto raíz para crear una hoja de cálculo de Excel"
type: docs
url: /es/net/aspose.cells/workbook/
---
## Workbook class

Representa un objeto raíz para crear una hoja de cálculo Excel.

```csharp
public class Workbook : IDisposable
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [Workbook](workbook/#constructor)() | Inicializa una nueva instancia de la clase `Workbook`. |
| [Workbook](workbook/#constructor_1)(FileFormatType) | Inicializa una nueva instancia de la clase `Workbook`. |
| [Workbook](workbook/#constructor_2)(LoadOptions) | Inicializa una nueva instancia vacía de la clase `Workbook` con opciones |
| [Workbook](workbook/#constructor_3)(Stream) | Inicializa una nueva instancia de la clase `Workbook` y abre un flujo. |
| [Workbook](workbook/#constructor_5)(string) | Inicializa una nueva instancia de la clase `Workbook` y abre un archivo. |
| [Workbook](workbook/#constructor_4)(Stream, LoadOptions) | Inicializa una nueva instancia de la clase `Workbook` y abre el flujo. |
| [Workbook](workbook/#constructor_6)(string, LoadOptions) | Inicializa una nueva instancia de la clase `Workbook` y abre un archivo. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AbsolutePath](../../aspose.cells/workbook/absolutepath/) { get; set; } | Obtiene y establece la ruta absoluta del archivo. |
| [BuiltInDocumentProperties](../../aspose.cells/workbook/builtindocumentproperties/) { get; } | Devuelve una colección de [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) que representa todas las propiedades de documento incorporadas de la hoja de cálculo. |
| [CellsDataTableFactory](../../aspose.cells/workbook/cellsdatatablefactory/) { get; } | Obtiene la fábrica para crear ICellsDataTable a partir de objetos personalizados |
| [Colors](../../aspose.cells/workbook/colors/) { get; } | Devuelve los colores de la paleta para la hoja de cálculo. |
| [ContentTypeProperties](../../aspose.cells/workbook/contenttypeproperties/) { get; } | Obtiene la lista de objetos [`ContentTypeProperty`](../../aspose.cells.properties/contenttypeproperty/) en el libro de trabajo. |
| [CountOfStylesInPool](../../aspose.cells/workbook/countofstylesinpool/) { get; } | Obtiene el número de estilos en el conjunto de estilos. |
| [CustomDocumentProperties](../../aspose.cells/workbook/customdocumentproperties/) { get; } | Devuelve una colección de [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) que representa todas las propiedades de documento personalizadas de la hoja de cálculo. |
| [CustomXmlParts](../../aspose.cells/workbook/customxmlparts/) { get; } | Representa una parte de almacenamiento de datos XML personalizada (datos XML personalizados dentro de un paquete). |
| [DataConnections](../../aspose.cells/workbook/dataconnections/) { get; } | Obtiene la colección [`ExternalConnection`](../../aspose.cells.externalconnections/externalconnection/). |
| [DataMashup](../../aspose.cells/workbook/datamashup/) { get; } | Obtiene los datos mashup. |
| [DataModel](../../aspose.cells/workbook/datamodel/) { get; } | Obtiene el modelo de datos en el libro de trabajo. |
| [DataSorter](../../aspose.cells/workbook/datasorter/) { get; } | Obtiene un objeto DataSorter para ordenar datos. |
| [DefaultStyle](../../aspose.cells/workbook/defaultstyle/) { get; set; } | Obtiene o establece el objeto [`Style`](../style/) predeterminado del libro de trabajo. |
| [FileFormat](../../aspose.cells/workbook/fileformat/) { get; set; } | Obtiene y establece el formato del archivo. |
| [FileName](../../aspose.cells/workbook/filename/) { get; set; } | Obtiene y establece el nombre actual del archivo. |
| [HasCustomFunction](../../aspose.cells/workbook/hascustomfunction/) { get; } | Detecta si hay una función personalizada utilizada en este libro de trabajo, como en la fórmula de una celda, en nombres definidos... |
| [HasMacro](../../aspose.cells/workbook/hasmacro/) { get; } | Indica si esta hoja de cálculo contiene macro/VBA. |
| [HasRevisions](../../aspose.cells/workbook/hasrevisions/) { get; } | Obtiene si el libro de trabajo tiene cambios rastreados |
| [InterruptMonitor](../../aspose.cells/workbook/interruptmonitor/) { get; set; } | Obtiene y establece el monitor de interrupción. |
| [IsDigitallySigned](../../aspose.cells/workbook/isdigitallysigned/) { get; } | Indica si esta hoja de cálculo está firmada digitalmente. |
| [IsLicensed](../../aspose.cells/workbook/islicensed/) { get; } | Indica si la licencia está establecida. |
| [IsWorkbookProtectedWithPassword](../../aspose.cells/workbook/isworkbookprotectedwithpassword/) { get; } | Indica si la estructura o la ventana están protegidas con contraseña. |
| [RibbonXml](../../aspose.cells/workbook/ribbonxml/) { get; set; } | Obtiene y establece el archivo XML que define la interfaz Ribbon UI. |
| [Settings](../../aspose.cells/workbook/settings/) { get; } | Representa la configuración del libro de trabajo. |
| [Theme](../../aspose.cells/workbook/theme/) { get; } | Obtiene el nombre del tema. |
| [VbaProject](../../aspose.cells/workbook/vbaproject/) { get; } | Obtiene el [`VbaProject`](./vbaproject/) en una hoja de cálculo. |
| [Worksheets](../../aspose.cells/workbook/worksheets/) { get; } | Obtiene la colección [`WorksheetCollection`](../worksheetcollection/) en la hoja de cálculo. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AcceptAllRevisions](../../aspose.cells/workbook/acceptallrevisions/)() | Acepta todos los cambios rastreados en el libro de trabajo. |
| [AddDigitalSignature](../../aspose.cells/workbook/adddigitalsignature/)(DigitalSignatureCollection) | Agrega una firma digital a un archivo de hoja de cálculo OOXML (Excel2007 y posteriores). |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula/#calculateformula)() | Calcula el resultado de las fórmulas. |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula/#calculateformula_2)(bool) | Calcula el resultado de las fórmulas. |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula/#calculateformula_1)(CalculationOptions) | Calculando fórmulas en este libro de trabajo. |
| [ChangePalette](../../aspose.cells/workbook/changepalette/)(Color, int) | Cambia la paleta de la hoja de cálculo en el índice especificado. |
| [CloseAccessCache](../../aspose.cells/workbook/closeaccesscache/)(AccessCacheOptions) | Cierra la sesión que utiliza cachés para acceder a los datos. |
| [Combine](../../aspose.cells/workbook/combine/)(Workbook) | Combina otro objeto Workbook. |
| [Copy](../../aspose.cells/workbook/copy/#copy)(Workbook) | Copia datos de un objeto Workbook fuente. |
| [Copy](../../aspose.cells/workbook/copy/#copy_1)(Workbook, CopyOptions) | Copia otro objeto Workbook. |
| [CopyTheme](../../aspose.cells/workbook/copytheme/)(Workbook) | Copia el tema de otro libro de trabajo. |
| [CreateBuiltinStyle](../../aspose.cells/workbook/createbuiltinstyle/)(BuiltinStyleType) | Crea un estilo incorporado según el tipo dado. |
| [CreateCellsColor](../../aspose.cells/workbook/createcellscolor/)() | Crea un objeto [`CellsColor`](../cellscolor/). |
| [CreateStyle](../../aspose.cells/workbook/createstyle/#createstyle)() | Crea un nuevo estilo. |
| [CreateStyle](../../aspose.cells/workbook/createstyle/#createstyle_1)(bool) | Crea un nuevo estilo. |
| [CustomTheme](../../aspose.cells/workbook/customtheme/)(string, Color[]) | Personaliza el tema. |
| [Dispose](../../aspose.cells/workbook/dispose/)() | Ejecuta tareas definidas por la aplicación asociadas con liberar, liberar o restablecer recursos no administrados. |
| [ExportXml](../../aspose.cells/workbook/exportxml/#exportxml)(string, Stream) | Exporta datos XML. |
| [ExportXml](../../aspose.cells/workbook/exportxml/#exportxml_1)(string, string) | Exporta datos XML vinculados mediante el mapa XML especificado. |
| [GetDigitalSignature](../../aspose.cells/workbook/getdigitalsignature/)() | Obtiene la firma digital del archivo. |
| [GetFonts](../../aspose.cells/workbook/getfonts/)() | Obtiene todas las fuentes en el grupo de estilos. |
| [GetMatchingColor](../../aspose.cells/workbook/getmatchingcolor/)(Color) | Encuentra el Color que mejor coincide en la paleta actual. |
| [GetNamedStyle](../../aspose.cells/workbook/getnamedstyle/)(string) | Obtiene el estilo nombrado en el grupo de estilos. |
| [GetStyleInPool](../../aspose.cells/workbook/getstyleinpool/)(int) | Obtiene el estilo en el grupo de estilos. Todos los estilos del libro de trabajo se recopilarán en un grupo. Sólo hay un índice de referencia simple en las celdas. |
| [GetThemeColor](../../aspose.cells/workbook/getthemecolor/)(ThemeColorType) | Obtiene el color del tema. |
| [HasExernalLinks](../../aspose.cells/workbook/hasexernallinks/)() | (**Obsolete.**) Indica si este libro de trabajo contiene enlaces externos a otras fuentes de datos. |
| [ImportXml](../../aspose.cells/workbook/importxml/#importxml)(Stream, string, int, int) | Importa/Actualiza un archivo de datos XML en el libro de trabajo. |
| [ImportXml](../../aspose.cells/workbook/importxml/#importxml_1)(string, string, int, int) | Importa/Actualiza un archivo de datos XML en el libro de trabajo. |
| [IsColorInPalette](../../aspose.cells/workbook/iscolorinpalette/)(Color) | Comprueba si un color está en la paleta de la hoja de cálculo. |
| [MergeNamedStyles](../../aspose.cells/workbook/mergenamedstyles/)(Workbook) | Fusiona estilos nombrados del otro archivo Excel. |
| [ParseFormulas](../../aspose.cells/workbook/parseformulas/)(bool) | Analiza todas las fórmulas que no se han analizado cuando se cargaron desde el archivo de plantilla o se establecieron en una celda. |
| [Protect](../../aspose.cells/workbook/protect/)(ProtectionType, string) | Protege un libro de trabajo. |
| [ProtectSharedWorkbook](../../aspose.cells/workbook/protectsharedworkbook/)(string) | Protege un libro de trabajo compartido. |
| [RefreshAll](../../aspose.cells/workbook/refreshall/)() | Actualiza las formas vinculadas, todas las tablas dinámicas y los gráficos con origen dinámico. |
| [RefreshDynamicArrayFormulas](../../aspose.cells/workbook/refreshdynamicarrayformulas/#refreshdynamicarrayformulas)(bool) | Actualiza las fórmulas de matrices dinámicas (desbordan en un nuevo rango de celdas vecinas según los datos actuales). Otras fórmulas en el libro de trabajo no se calcularán de forma recursiva aunque hayan sido utilizadas por fórmulas de matrices dinámicas. |
| [RefreshDynamicArrayFormulas](../../aspose.cells/workbook/refreshdynamicarrayformulas/#refreshdynamicarrayformulas_1)(bool, CalculationOptions) | Actualiza las fórmulas de matrices dinámicas (desbordan en un nuevo rango de celdas vecinas según los datos actuales). |
| [RemoveDigitalSignature](../../aspose.cells/workbook/removedigitalsignature/)() | Elimina la firma digital de esta hoja de cálculo. |
| [RemoveExternalLinks](../../aspose.cells/workbook/removeexternallinks/)() | (**Obsoleto.**) Elimina todos los enlaces externos en el libro de trabajo. |
| [RemoveMacro](../../aspose.cells/workbook/removemacro/)() | Elimina VBA/macros de esta hoja de cálculo. |
| [RemovePersonalInformation](../../aspose.cells/workbook/removepersonalinformation/)() | Elimina información personal. |
| [RemoveUnusedStyles](../../aspose.cells/workbook/removeunusedstyles/)() | Elimina todos los estilos no utilizados. |
| [Replace](../../aspose.cells/workbook/replace/#replace)(bool, object) | Reemplaza los valores de las celdas con datos nuevos. |
| [Replace](../../aspose.cells/workbook/replace/#replace_1)(int, object) | Reemplaza los valores de las celdas con datos nuevos. |
| [Replace](../../aspose.cells/workbook/replace/#replace_6)(string, DataTable) | Reemplaza los valores de las celdas con datos de una DataTable. |
| [Replace](../../aspose.cells/workbook/replace/#replace_2)(string, double) | Reemplaza el valor de una celda con un double nuevo. |
| [Replace](../../aspose.cells/workbook/replace/#replace_4)(string, int) | Reemplaza el valor de una celda con un entero nuevo. |
| [Replace](../../aspose.cells/workbook/replace/#replace_7)(string, string) | Reemplaza el valor de una celda con una cadena nueva. |
| [Replace](../../aspose.cells/workbook/replace/#replace_3)(string, double[], bool) | Reemplaza los valores de las celdas con una matriz de double. |
| [Replace](../../aspose.cells/workbook/replace/#replace_5)(string, int[], bool) | Reemplaza los valores de las celdas con una matriz de integer. |
| [Replace](../../aspose.cells/workbook/replace/#replace_8)(string, string, ReplaceOptions) | Reemplaza el valor de una celda con una cadena nueva. |
| [Replace](../../aspose.cells/workbook/replace/#replace_9)(string, string[], bool) | Reemplaza el valor de una celda con una nueva matriz de string. |
| [Save](../../aspose.cells/workbook/save/#save_2)(string) | Guarda el libro de trabajo en el disco. |
| [Save](../../aspose.cells/workbook/save/#save)(Stream, SaveFormat) | Guarda el libro de trabajo en el flujo. |
| [Save](../../aspose.cells/workbook/save/#save_1)(Stream, SaveOptions) | Guarda el libro de trabajo en el flujo. |
| [Save](../../aspose.cells/workbook/save/#save_3)(string, SaveFormat) | Guarda el libro de trabajo en el disco. |
| [Save](../../aspose.cells/workbook/save/#save_4)(string, SaveOptions) | Guarda el libro de trabajo en el disco. |
| [Save](../../aspose.cells/workbook/save/#save_5)(HttpResponse, string, ContentDisposition, SaveOptions) | Crea la hoja de cálculo resultante y la transfiere al cliente, luego la abre en el navegador o en MS Workbook. |
| [Save](../../aspose.cells/workbook/save/#save_6)(HttpResponse, string, ContentDisposition, SaveOptions, bool) | Crea la hoja de cálculo resultante y la transfiere al cliente, luego la abre en el navegador o en MS Workbook. |
| [SaveToStream](../../aspose.cells/workbook/savetostream/)() | Guarda el archivo Excel en un objeto MemoryStream como un archivo xls de Excel97-2003 y lo devuelve. |
| [SetDigitalSignature](../../aspose.cells/workbook/setdigitalsignature/)(DigitalSignatureCollection) | Establece una firma digital en un archivo de hoja de cálculo (Excel2007 y posteriores). |
| [SetEncryptionOptions](../../aspose.cells/workbook/setencryptionoptions/)(EncryptionType, int) | Establecer opciones de cifrado. |
| [SetThemeColor](../../aspose.cells/workbook/setthemecolor/)(ThemeColorType, Color) | Establece el color del tema |
| [StartAccessCache](../../aspose.cells/workbook/startaccesscache/)(AccessCacheOptions) | Inicia la sesión que usa cachés para acceder a los datos. |
| [Unprotect](../../aspose.cells/workbook/unprotect/)(string) | Desprotege un libro de trabajo. |
| [UnprotectSharedWorkbook](../../aspose.cells/workbook/unprotectsharedworkbook/)(string) | Desprotege un libro de trabajo compartido. |
| [UpdateCustomFunctionDefinition](../../aspose.cells/workbook/updatecustomfunctiondefinition/)(CustomFunctionDefinition) | Actualiza la definición de funciones personalizadas. |
| [UpdateLinkedDataSource](../../aspose.cells/workbook/updatelinkeddatasource/)(Workbook[]) | Si este libro de trabajo contiene enlaces externos a otras fuentes de datos, Aspose.Cells intentará recuperar los datos más recientes de las fuentes dadas. |

### Observaciones

La clase Workbook denota una hoja de cálculo de Excel. Cada hoja de cálculo puede contener múltiples hojas de trabajo. La característica básica de la clase es abrir y guardar archivos Excel nativos. La clase tiene algunas características avanzadas como copiar datos de otros Workbooks, combinar dos Workbooks, convertir Excel a PDF, renderizar Excel a imagen y proteger la hoja de cálculo de Excel.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookDemo
    {
        public static void WorkbookExample()
        {
            // Crear una nueva instancia de Workbook
            Workbook workbook = new Workbook();

            // Acceder a la hoja de trabajo predeterminada
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer algunas propiedades del libro de trabajo
            workbook.FileName = "ExampleWorkbook.xlsx";
            workbook.DefaultStyle.Font.Name = "Tahoma";

            // Agregar una nueva hoja de trabajo
            int newSheetIndex = workbook.Worksheets.Add();
            Worksheet newWorksheet = workbook.Worksheets[newSheetIndex];
            newWorksheet.Name = "NewSheet";

            // Agregar algunos datos a la nueva hoja de trabajo
            newWorksheet.Cells["A1"].PutValue("Hello, Aspose.Cells!");

            // Establecer algunas propiedades del documento
            workbook.BuiltInDocumentProperties["Author"].Value = "John Smith";
            workbook.CustomDocumentProperties.Add("Checked by", "Jane");

            // Guardar el libro de trabajo en un archivo
            workbook.Save("WorkbookExample.xlsx");

            // Mostrar algunas propiedades
            Console.WriteLine("Workbook File Name: " + workbook.FileName);
            Console.WriteLine("Default Font: " + workbook.DefaultStyle.Font.Name);
            Console.WriteLine("Author: " + workbook.BuiltInDocumentProperties["Author"].Value);
            Console.WriteLine("Custom Property 'Checked by': " + workbook.CustomDocumentProperties["Checked by"].Value);

            // Verificar si el libro de trabajo está licenciado
            Console.WriteLine("Is Licensed: " + workbook.IsLicensed);

            // Verificar si el libro de trabajo está firmado digitalmente
            Console.WriteLine("Is Digitally Signed: " + workbook.IsDigitallySigned);

            // Verificar si el libro de trabajo contiene macros
            Console.WriteLine("Has Macros: " + workbook.HasMacro);

            // Verificar si el libro de trabajo tiene cambios rastreados
            Console.WriteLine("Has Revisions: " + workbook.HasRevisions);

            // Verificar el número de estilos en el conjunto de estilos
            Console.WriteLine("Number of Styles in Pool: " + workbook.CountOfStylesInPool);

            // Verificar el nombre del tema
            Console.WriteLine("Theme: " + workbook.Theme);

            // Verificar si el libro de trabajo está protegido con una contraseña
            Console.WriteLine("Is Workbook Protected With Password: " + workbook.IsWorkbookProtectedWithPassword);

            // Verificar si el libro de trabajo contiene enlaces externos
            Console.WriteLine("Has External Links: " + (workbook.Worksheets.ExternalLinks.Count > 0));

            // Liberar el libro de trabajo
            workbook.Dispose();
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


