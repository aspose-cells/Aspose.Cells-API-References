---
title: "Clase GridJsWorkbook"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.GridJs.GridJsWorkbook. Representa la clase principal de entrada para GridJs"
type: docs
url: /es/net/aspose.cells.gridjs/gridjsworkbook/
---
## GridJsWorkbook class

Representa la clase principal de entrada para GridJs

```csharp
public class GridJsWorkbook
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [GridJsWorkbook](gridjsworkbook/)() | Crea una nueva instancia de GridJsWorkbook. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CacheDirectory](../../aspose.cells.gridjs/gridjsworkbook/cachedirectory/) { get; set; } | Obtiene/Establece el directorio de caché para almacenar archivos de hoja de cálculo. Si no se establece, usaremos la propiedad estática de [`FileCacheDirectory`](../config/filecachedirectory/) o [`CacheImp`](./cacheimp/). |
| [Settings](../../aspose.cells.gridjs/gridjsworkbook/settings/) { get; set; } | Representa la configuración del libro de trabajo. |
| [WarningCallback](../../aspose.cells.gridjs/gridjsworkbook/warningcallback/) { get; set; } | Obtiene o establece la devolución de llamada de advertencia para la importación de archivo. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [BurnRedactionFile](../../aspose.cells.gridjs/gridjsworkbook/burnredactionfile/)(string, string) | Ejecuta (aplica) todas las operaciones de redacción en el libro de trabajo eliminando las formas de redacción y sus formas objetivo o borrando el contenido del rango de celdas objetivo. |
| [CheckInCacheForCollaborative](../../aspose.cells.gridjs/gridjsworkbook/checkincacheforcollaborative/)(string) | Comprueba si la instancia del libro de trabajo está en la caché de memoria. este método se aplica solo para el modo colaborativo. |
| [ClearAllJsonCache](../../aspose.cells.gridjs/gridjsworkbook/clearalljsoncache/)() | Borrar toda la caché JSON |
| [ClearJsonCacheForUid](../../aspose.cells.gridjs/gridjsworkbook/clearjsoncacheforuid/)(string) | Borrar la caché JSON según uid (para escenarios como UpdateCell que solo tienen uid) |
| [CopyImageOrShape](../../aspose.cells.gridjs/gridjsworkbook/copyimageorshape/)(string, string) | Copia imagen o forma. |
| [Dispose](../../aspose.cells.gridjs/gridjsworkbook/dispose/)() | Ejecuta tareas definidas por la aplicación asociadas con liberar, liberar o restablecer recursos no administrados. |
| [ErrorJson](../../aspose.cells.gridjs/gridjsworkbook/errorjson/)(string) | Obtiene la cadena del mensaje de error en formato JSON. |
| [ExportToJson](../../aspose.cells.gridjs/gridjsworkbook/exporttojson/#exporttojson)() | Obtiene la cadena JSON de los datos en memoria, el nombre de archivo predeterminado en el JSON es: book1. |
| [ExportToJson](../../aspose.cells.gridjs/gridjsworkbook/exporttojson/#exporttojson_1)(string) | Obtiene la cadena JSON de los datos en memoria, establece el nombre de archivo de salida en el JSON. |
| [ExportToJsonStringBuilder](../../aspose.cells.gridjs/gridjsworkbook/exporttojsonstringbuilder/)(string, string) | Obtiene la cadena JSON de los datos en memoria, establece el nombre de archivo de salida en el JSON. |
| [GetJsonByUid](../../aspose.cells.gridjs/gridjsworkbook/getjsonbyuid/)(string, string) | Obtiene la cadena JSON del archivo desde la caché usando el ID único especificado, establece el nombre de archivo de salida en el JSON. |
| [GetOle](../../aspose.cells.gridjs/gridjsworkbook/getole/)(string, string, int, out string) | Obtiene los datos del arreglo de bytes del objeto OLE incrustado. |
| [GetSheetJsonWithCache](../../aspose.cells.gridjs/gridjsworkbook/getsheetjsonwithcache/)(string, string, string) | Obtener el JSON de la hoja especificada (con caché) |
| [GetWorkbookJsonWithCache](../../aspose.cells.gridjs/gridjsworkbook/getworkbookjsonwithcache/)(string, string) | Obtener el JSON de todo el libro de trabajo (con caché) |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_3)(string) | Importa el archivo Excel desde la ruta del archivo. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile)(Workbook) | Importa el archivo Excel desde el objeto Workbook. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_1)(Stream, GridLoadFormat) | Importa el archivo Excel desde un flujo de archivo con formato de carga. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_7)(string, string) | Importa el archivo Excel desde la ruta del archivo. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_4)(string, Workbook) | Importa el archivo Excel desde el objeto Workbook. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_2)(Stream, GridLoadFormat, string) | Importa el archivo Excel desde un flujo de archivo con formato de carga y contraseña de apertura. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_5)(string, Stream, GridLoadFormat) | Importa el archivo Excel desde un flujo de archivo. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_8)(string, string, string) | Importa el archivo Excel desde la ruta del archivo y contraseña de apertura. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_6)(string, Stream, GridLoadFormat, string) | Importa el archivo Excel desde un flujo de archivo con formato de carga y contraseña de apertura. |
| [ImportExcelFileFromJson](../../aspose.cells.gridjs/gridjsworkbook/importexcelfilefromjson/)(string) | Importa el archivo Excel desde una cadena en formato JSON. |
| [InsertImage](../../aspose.cells.gridjs/gridjsworkbook/insertimage/)(string, string, Stream, string) | Inserta una imagen en la hoja de cálculo desde un flujo de archivo o la URL (se debe proporcionar el flujo de archivo o la URL), o inserta una forma cuando p.type es uno de AutoShapeType |
| [JsonToStream](../../aspose.cells.gridjs/gridjsworkbook/jsontostream/)(Stream, string, string) | Genera JSON a partir del Workbook en memoria y lo escribe en el flujo especificado. Opcionalmente almacena en caché el JSON generado para una recuperación posterior más rápida. Diferencias clave con JsonToStreamByUid: - Este método usa el estado actual del Workbook en memoria (campo wb) - JsonToStreamByUid recarga el Workbook desde los archivos de caché .cells en disco - Usa este método cuando deseas exportar el estado actual del libro después de modificaciones - Usa JsonToStreamByUid cuando necesitas regenerar JSON a partir de un estado de archivo previamente almacenado en caché. Comportamiento de caché (cuando se proporciona uid): - Verifica la caché de JSON antes de generar (memoria L1 + disco L2) - Si hay una falta de caché, genera JSON desde el workbook en memoria - Almacena el JSON generado en la caché para futuras solicitudes |
| [JsonToStreamByUid](../../aspose.cells.gridjs/gridjsworkbook/jsontostreambyuid/)(Stream, string, string) | Recupera la cadena JSON del archivo desde la caché usando el id único especificado, establece el nombre de archivo de salida en el JSON y lo escribe en el flujo. |
| [LazyLoadingJson](../../aspose.cells.gridjs/gridjsworkbook/lazyloadingjson/)(string, string) | Obtiene la cadena JSON de la hoja especificada en el archivo desde la caché usando el ID único especificado. |
| [LazyLoadingStream](../../aspose.cells.gridjs/gridjsworkbook/lazyloadingstream/)(Stream, string, string) | Recupera la cadena JSON de la hoja especificada en el archivo desde la caché usando el id único especificado, y lo escribe en el flujo. |
| [MergeExcelFileFromJson](../../aspose.cells.gridjs/gridjsworkbook/mergeexcelfilefromjson/)(string, string) | Aplica una actualización por lotes a los datos en memoria. |
| [RedactFile](../../aspose.cells.gridjs/gridjsworkbook/redactfile/)(string, string, string[]) | Realiza una redacción en un archivo Excel basada en una matriz de operaciones JSON. |
| [SaveToCacheWithFileName](../../aspose.cells.gridjs/gridjsworkbook/savetocachewithfilename/)(string, string, string) | Guarda los datos en memoria en el archivo de caché con el nombre de archivo especificado y también establece la contraseña de apertura; el formato de guardado se basa en la extensión del nombre de archivo. |
| [SaveToExcelFile](../../aspose.cells.gridjs/gridjsworkbook/savetoexcelfile/#savetoexcelfile)(Stream) | Guarda los datos en memoria en el flujo, basándose en el formato original del archivo. |
| [SaveToExcelFile](../../aspose.cells.gridjs/gridjsworkbook/savetoexcelfile/#savetoexcelfile_1)(string) | Guarda los datos en memoria en la ruta del archivo; si el archivo tiene extensión, el formato de guardado se basa en la extensión del archivo. |
| [SaveToHtml](../../aspose.cells.gridjs/gridjsworkbook/savetohtml/#savetohtml)(Stream) | Guarda los datos en memoria en el flujo, el formato de guardado es html |
| [SaveToHtml](../../aspose.cells.gridjs/gridjsworkbook/savetohtml/#savetohtml_1)(string) | Guarda los datos en memoria en la ruta del archivo, el formato de guardado es html. |
| [SaveToPdf](../../aspose.cells.gridjs/gridjsworkbook/savetopdf/#savetopdf)(Stream) | Guarda los datos en memoria en el flujo, el formato de guardado es pdf. |
| [SaveToPdf](../../aspose.cells.gridjs/gridjsworkbook/savetopdf/#savetopdf_1)(string) | Guarda los datos en memoria en la ruta del archivo, el formato de guardado es pdf. |
| [SaveToXlsx](../../aspose.cells.gridjs/gridjsworkbook/savetoxlsx/#savetoxlsx)(Stream) | Guarda los datos en memoria en el flujo, el formato de guardado es xlsx. |
| [SaveToXlsx](../../aspose.cells.gridjs/gridjsworkbook/savetoxlsx/#savetoxlsx_1)(string) | Guarda los datos en memoria en la ruta del archivo, el formato de guardado es xlsx. |
| [SetInterruptMonitorForLoad](../../aspose.cells.gridjs/gridjsworkbook/setinterruptmonitorforload/)(GridInterruptMonitor, int) | Establece InterruptMonitor para la operación de carga. |
| [SetInterruptMonitorForSave](../../aspose.cells.gridjs/gridjsworkbook/setinterruptmonitorforsave/)(GridInterruptMonitor) | Establece InterruptMonitor para la operación de guardado. |
| [SetTransParentView](../../aspose.cells.gridjs/gridjsworkbook/settransparentview/)(string, string, bool) | Establece la transparencia de las formas de redacción en el libro de trabajo. |
| [TranslateSheetAsync](../../aspose.cells.gridjs/gridjsworkbook/translatesheetasync/)(string, string, ITextTranslator, string) | Traduce todos los valores de cadena al idioma objetivo en la hoja de cálculo |
| [UpdateCell](../../aspose.cells.gridjs/gridjsworkbook/updatecell/)(string, string) | Aplica la operación de actualización. |
| static [GetGridLoadFormat](../../aspose.cells.gridjs/gridjsworkbook/getgridloadformat/)(string) | Obtiene el formato de carga según la extensión del archivo |
| static [GetImageStream](../../aspose.cells.gridjs/gridjsworkbook/getimagestream/)(string, string, string) | Obtener flujo de imagen. |
| static [GetImageUrl](../../aspose.cells.gridjs/gridjsworkbook/getimageurl/)(string, string, string) | Obtiene la URL de la imagen. |
| static [GetUidForFile](../../aspose.cells.gridjs/gridjsworkbook/getuidforfile/)(string) | Genera un nuevo identificador único para la caché de archivos usando el nombre de archivo proporcionado. |
| static [SetImageUrlBase](../../aspose.cells.gridjs/gridjsworkbook/setimageurlbase/)(string) | Establece la URL de la acción de obtención de la imagen base desde el controlador. |

## Campos

| Nombre | Descripción |
| --- | --- |
| static [CacheImp](../../aspose.cells.gridjs/gridjsworkbook/cacheimp/) | Implementación personalizada para el almacenamiento en caché; si deseas almacenar la caché de forma secuencial, debes configurarla e implementarla. |
| static [CalculateEngine](../../aspose.cells.gridjs/gridjsworkbook/calculateengine/) | Implementación personalizada para el motor de cálculo; si deseas realizar cálculos personalizados, debes configurarlo e implementarlo. |
| const [pictureType](../../aspose.cells.gridjs/gridjsworkbook/picturetype/) | valor constante para el tipo de la imagen |
| static [UpdateMonitor](../../aspose.cells.gridjs/gridjsworkbook/updatemonitor/) | Obtiene/Establece el monitor de actualización para rastrear la operación de actualización |

### Ver también

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


