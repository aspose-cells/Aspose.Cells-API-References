---
title: GridJsWorkbook
second_title: Referencia de API de Aspose.Cells para .NET
description: Representa la clase de entrada principal para GridJs
type: docs
weight: 80
url: /es/net/aspose.cells.gridjs/gridjsworkbook/
---
## GridJsWorkbook class

Representa la clase de entrada principal para GridJs

```csharp
public class GridJsWorkbook
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [GridJsWorkbook](gridjsworkbook)() | Constructor predeterminado |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Settings](../../aspose.cells.gridjs/gridjsworkbook/settings) { get; set; } | Representa la configuración del libro. |
| [WarningCallback](../../aspose.cells.gridjs/gridjsworkbook/warningcallback) { get; set; } | Obtiene o establece una devolución de llamada de advertencia para el archivo de importación. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [CopyImageOrShape](../../aspose.cells.gridjs/gridjsworkbook/copyimageorshape)(string, string) | copiar imagen o forma en la hoja de trabajo |
| [ErrorJson](../../aspose.cells.gridjs/gridjsworkbook/errorjson)(string) | devolver mensaje de error |
| [ExportToJson](../../aspose.cells.gridjs/gridjsworkbook/exporttojson#exporttojson)() | Obtener json de workbook |
| [ExportToJson](../../aspose.cells.gridjs/gridjsworkbook/exporttojson#exporttojson_1)(string) | Obtener json de workbook |
| [ExportToJsonStringBuilder](../../aspose.cells.gridjs/gridjsworkbook/exporttojsonstringbuilder)(string) | Obtener json de workbook |
| [GetJsonByUid](../../aspose.cells.gridjs/gridjsworkbook/getjsonbyuid)(string, string) | obtener el json del caché por uid |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_3)(string) | Importaciones desde un archivo excel. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile)(Workbook) | Importaciones desde Workbook. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_1)(Stream, GridLoadFormat) | Importaciones desde un archivo de Excel stream. Debe proporcionar formato de carga y puede configurar GridJsWorkbook.CacheImp para implementar stream cache |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_7)(string, string) | Importaciones desde un archivo excel. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_4)(string, Workbook) | Importaciones desde un archivo excel. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_2)(Stream, GridLoadFormat, string) | Importaciones desde un archivo de Excel stream. Debe proporcionar formato de carga y puede configurar GridJsWorkbook.CacheImp para implementar stream cache |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_5)(string, Stream, GridLoadFormat) | Importaciones desde un archivo de Excel stream. Debe proporcionar formato de carga y puede configurar GridJsWorkbook.CacheImp para implementar stream cache |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_8)(string, string, string) | Importaciones desde un archivo excel. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_6)(string, Stream, GridLoadFormat, string) | Importaciones desde un archivo de Excel stream. Debe proporcionar formato de carga y puede configurar GridJsWorkbook.CacheImp para implementar stream cache |
| [ImportExcelFileFromJson](../../aspose.cells.gridjs/gridjsworkbook/importexcelfilefromjson)(string) | Importar archivo desde json |
| [InsertImage](../../aspose.cells.gridjs/gridjsworkbook/insertimage)(string, string, Stream, string) | insertar imagen en la hoja de cálculo |
| [MergeExcelFileFromJson](../../aspose.cells.gridjs/gridjsworkbook/mergeexcelfilefromjson)(string, string) | Aplicar actualización de estilo al archivo de caché |
| [SaveToCacheWithFileName](../../aspose.cells.gridjs/gridjsworkbook/savetocachewithfilename)(string, string, string) | Guarda las hojas de trabajo en la caché, el formato de guardado se basa en la extensión de archivo del nombre de archivo . |
| [SaveToExcelFile](../../aspose.cells.gridjs/gridjsworkbook/savetoexcelfile#savetoexcelfile)(Stream) | Guarda las hojas de trabajo en el flujo, según el formato de archivo de origen . |
| [SaveToExcelFile](../../aspose.cells.gridjs/gridjsworkbook/savetoexcelfile#savetoexcelfile_1)(string) | Guarda las hojas de trabajo en la ruta del archivo, si el archivo tiene extensión, el formato de guardado se basa en la extensión de archivo . |
| [SaveToHtml](../../aspose.cells.gridjs/gridjsworkbook/savetohtml#savetohtml)(Stream) | Guarda las hojas de trabajo en el sream, el formato de guardado es html |
| [SaveToHtml](../../aspose.cells.gridjs/gridjsworkbook/savetohtml#savetohtml_1)(string) | Guarda las hojas de trabajo en la ruta del archivo, el formato de guardado es html |
| [SaveToPdf](../../aspose.cells.gridjs/gridjsworkbook/savetopdf#savetopdf)(Stream) | Guarda las hojas de trabajo en el sream, el formato de guardado es pdf |
| [SaveToPdf](../../aspose.cells.gridjs/gridjsworkbook/savetopdf#savetopdf_1)(string) | Guarda las hojas de trabajo en la ruta del archivo, el formato de guardado es pdf |
| [SaveToXlsx](../../aspose.cells.gridjs/gridjsworkbook/savetoxlsx#savetoxlsx)(Stream) | Guarda las hojas de trabajo en el flujo, el formato de guardado es xlsx |
| [SaveToXlsx](../../aspose.cells.gridjs/gridjsworkbook/savetoxlsx#savetoxlsx_1)(string) | Guarda las hojas de trabajo en la ruta del archivo, el formato de guardado es xlsx |
| [SetInterruptMonitorForLoad](../../aspose.cells.gridjs/gridjsworkbook/setinterruptmonitorforload)(GridInterruptMonitor, int) | establecer InterruptMonitor para la operación de carga para el libro de trabajo |
| [SetInterruptMonitorForSave](../../aspose.cells.gridjs/gridjsworkbook/setinterruptmonitorforsave)(GridInterruptMonitor) | establecer InterruptMonitor para guardar la operación para el libro de trabajo |
| [UpdateCell](../../aspose.cells.gridjs/gridjsworkbook/updatecell)(string, string) | Actualizar operación |
| static [GetGridLoadFormat](../../aspose.cells.gridjs/gridjsworkbook/getgridloadformat)(string) | Obtener GridLoadFormat por extensión de archivo |
| static [GetImageStream](../../aspose.cells.gridjs/gridjsworkbook/getimagestream)(string, string) | Obtener flujo de imagen de workbook |
| static [GetImageUrl](../../aspose.cells.gridjs/gridjsworkbook/getimageurl)(string, string, string) | Obtener la URL de la imagen |
| static [GetUidForFile](../../aspose.cells.gridjs/gridjsworkbook/getuidforfile)(string) | Generar el uid para el archivo |

## Campos

| Nombre | Descripción |
| --- | --- |
| static [CacheImp](../../aspose.cells.gridjs/gridjsworkbook/cacheimp) | Implementación personalizada para el almacenamiento de caché, si desea almacenar el caché de forma continua, debe configurarlo e implementarlo |
| static [CalculateEngine](../../aspose.cells.gridjs/gridjsworkbook/calculateengine) | Implementación personalizada para el motor de cálculo, si desea realizar un cálculo personalizado, debe configurarlo e implementarlo |

### Ver también

* espacio de nombres [Aspose.Cells.GridJs](../../aspose.cells.gridjs)
* asamblea [Aspose.Cells.GridJs](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridJs.dll -->
