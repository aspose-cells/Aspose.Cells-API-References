---
title: "Clase GridHtmlSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.GridWeb.Data.GridHtmlSaveOptions. Representa las opciones para guardar un archivo html"
type: docs
url: /es/net/aspose.cells.gridweb.data/gridhtmlsaveoptions/
---
## GridHtmlSaveOptions class

Representa las opciones para guardar un archivo html.

```csharp
public class GridHtmlSaveOptions : GridSaveOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [GridHtmlSaveOptions](gridhtmlsaveoptions/#constructor)() | Crea opciones para guardar un archivo html. |
| [GridHtmlSaveOptions](gridhtmlsaveoptions/#constructor_1)(GridSaveFormat) | Crea opciones para guardar un archivo htm. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AttachedFilesDirectory](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/attachedfilesdirectory/) { get; set; } | El directorio donde se guardarán los archivos adjuntos. Solo para guardar en un flujo html. |
| [AttachedFilesUrlPrefix](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/attachedfilesurlprefix/) { get; set; } | Especifique el prefijo Url de los archivos adjuntos, como imágenes, en el archivo html. Solo para guardar en un flujo html. |
| [CachedFileFolder](../../aspose.cells.gridweb.data/gridsaveoptions/cachedfilefolder/) { get; set; } | La carpeta de archivos en caché se utiliza para almacenar algunos datos grandes. (Heredado de [`GridSaveOptions`](../gridsaveoptions/).) |
| [ClearData](../../aspose.cells.gridweb.data/gridsaveoptions/cleardata/) { get; set; } | Deja el libro de trabajo vacío después de guardar el archivo. (Heredado de [`GridSaveOptions`](../gridsaveoptions/).) |
| [CreateDirectory](../../aspose.cells.gridweb.data/gridsaveoptions/createdirectory/) { get; set; } | Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo. (Heredado de [`GridSaveOptions`](../gridsaveoptions/).) |
| [DefaultFontName](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/defaultfontname/) { get; set; } | Especifique el nombre de fuente predeterminado para exportar html; la fuente predeterminada se usará cuando la fuente del estilo no exista. Si esta propiedad es null, Aspose.Cells utilizará una fuente universal que tenga la misma familia que la fuente original. El valor predeterminado es null. |
| [Encoding](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/encoding/) { get; set; } | Si no se establece, use Encoding.UTF8 como tipo de codificación predeterminado. |
| [ExportActiveWorksheetOnly](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportactiveworksheetonly/) { get; set; } | Indica si se exporta todo el libro de trabajo a un archivo html. |
| [ExportArea](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportarea/) { get; set; } | Obtiene o establece el área de celdas que se exporta de la hoja de cálculo activa actual. Si establece este atributo, el área de impresión de la hoja activa se omitirá. Solo el área especificada se exportará al guardar el archivo en html. |
| [ExportGridLines](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportgridlines/) { get; set; } | Indica si se exportan las líneas de cuadrícula. El valor predeterminado es false. |
| [ExportHeadings](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportheadings/) { get; set; } | Indica si se exportan los encabezados al guardar el archivo en html. El valor predeterminado es false. Si desea importar el archivo html a Excel, mantenga el valor predeterminado. |
| [ExportHiddenWorksheet](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exporthiddenworksheet/) { get; set; } | Indica si se exporta el contenido oculto de la hoja de cálculo. El valor predeterminado es true. |
| [ExportImagesAsBase64](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportimagesasbase64/) { get; set; } | Especifica si las imágenes se guardan en formato Base64 en HTML, MHTML o EPUB. |
| [ExportPrintAreaOnly](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportprintareaonly/) { get; set; } | Indica si solo se exporta el área de impresión al archivo html. El valor predeterminado es false. |
| [ExportSingleTab](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportsingletab/) { get; set; } | Indica si se exporta la pestaña única cuando el archivo tiene solo una hoja de cálculo. El valor predeterminado es false. |
| [IsExportComments](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/isexportcomments/) { get; set; } | Indica si se exportan los comentarios al guardar el archivo en HTML, el valor predeterminado es false. |
| [IsFullPathLink](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/isfullpathlink/) { get; set; } | Indica si se utiliza una ruta completa en los enlaces de sheet00x.htm, filelist.xml y tabstrip.htm. El valor predeterminado es false. |
| [MergeAreas](../../aspose.cells.gridweb.data/gridsaveoptions/mergeareas/) { get; set; } | Indica si se deben combinar las áreas de formato condicional y validación antes de guardar el archivo. (Heredado de [`GridSaveOptions`](../gridsaveoptions/).) |
| [PageTitle](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/pagetitle/) { get; set; } | El título de la página HTML. Solo para guardar en flujo HTML. |
| [ParseHtmlTagInCell](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/parsehtmltagincell/) { get; set; } | Analiza la etiqueta html en la celda, como valor de celda, o como etiqueta html, el valor predeterminado es true. |
| [PresentationPreference](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/presentationpreference/) { get; set; } | Indica si el archivo html o mht es la preferencia de presentación. El valor predeterminado es false. Si desea obtener una presentación más atractiva, establezca el valor en true. |
| [RefreshChartCache](../../aspose.cells.gridweb.data/gridsaveoptions/refreshchartcache/) { get; set; } | Indica si se actualizan los datos de caché del gráfico (Heredado de [`GridSaveOptions`](../gridsaveoptions/).) |
| [SaveFormat](../../aspose.cells.gridweb.data/gridsaveoptions/saveformat/) { get; } | Obtiene el formato de archivo guardado. (Heredado de [`GridSaveOptions`](../gridsaveoptions/).) |
| [SortNames](../../aspose.cells.gridweb.data/gridsaveoptions/sortnames/) { get; set; } | Indica si se ordenan los nombres definidos antes de guardar el archivo. (Heredado de [`GridSaveOptions`](../gridsaveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells.gridweb.data/gridsaveoptions/validatemergedareas/) { get; set; } | Indica si se validan las celdas combinadas antes de guardar el archivo. (Heredado de [`GridSaveOptions`](../gridsaveoptions/).) |

### Ver también

* class [GridSaveOptions](../gridsaveoptions/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


