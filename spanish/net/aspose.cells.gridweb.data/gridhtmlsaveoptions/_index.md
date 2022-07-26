---
title: GridHtmlSaveOptions
second_title: Referencia de API de Aspose.Cells para .NET
description: Representa las opciones para guardar el archivo html.
type: docs
weight: 250
url: /es/net/aspose.cells.gridweb.data/gridhtmlsaveoptions/
---
## GridHtmlSaveOptions class

Representa las opciones para guardar el archivo html.

```csharp
public class GridHtmlSaveOptions : GridSaveOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [GridHtmlSaveOptions](gridhtmlsaveoptions#constructor)() | Crea opciones para guardar el archivo html. |
| [GridHtmlSaveOptions](gridhtmlsaveoptions#constructor_1)(GridSaveFormat) | Crea opciones para guardar el archivo htm. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AttachedFilesDirectory](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/attachedfilesdirectory) { get; set; } | El directorio en el que se guardarán los archivos adjuntos. Solo para guardar en flujo html. |
| [AttachedFilesUrlPrefix](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/attachedfilesurlprefix) { get; set; } | Especifique el prefijo de URL de los archivos adjuntos, como la imagen en el archivo html. Solo para guardar en flujo html. |
| [CachedFileFolder](../../aspose.cells.gridweb.data/gridsaveoptions/cachedfilefolder) { get; set; } | La carpeta de archivos en caché se utiliza para almacenar algunos datos de gran tamaño. |
| [ClearData](../../aspose.cells.gridweb.data/gridsaveoptions/cleardata) { get; set; } | Vacía el libro de trabajo después de guardar el archivo. |
| [CreateDirectory](../../aspose.cells.gridweb.data/gridsaveoptions/createdirectory) { get; set; } | Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo. |
| [DefaultFontName](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/defaultfontname) { get; set; } | Especifique el nombre de la fuente predeterminada para exportar html, la fuente predeterminada se usará cuando la fuente del estilo no exista, Si esta propiedad es nula, Aspose.Cells usará la fuente universal que tiene la misma familia que la fuente original, el valor predeterminado es nulo. |
| [Encoding](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/encoding) { get; set; } | Si no se establece, use Codificación.UTF8 como tipo de codificación predeterminado. |
| [ExportActiveWorksheetOnly](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportactiveworksheetonly) { get; set; } | Indica si se exporta todo el libro de trabajo a un archivo html. |
| [ExportArea](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportarea) { get; set; } | Obtiene o establece el área de celda de exportación de la hoja de trabajo activa actual. Si establece este atributo, se omitirá el área de impresión de la hoja de trabajo activa actual. Solo se exportará el área especificada al guardar el archivo en html. |
| [ExportGridLines](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportgridlines) { get; set; } | Indicando si se están exportando las cuadrículas. El valor por defecto es falso. |
| [ExportHeadings](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportheadings) { get; set; } | Indica si se exportan encabezados al guardar el archivo en html. El valor predeterminado es falso. Si desea importar el archivo html a Excel, mantenga el valor predeterminado. |
| [ExportHiddenWorksheet](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exporthiddenworksheet) { get; set; } | Indica si se está exportando el contenido oculto de la hoja de cálculo. El valor predeterminado es verdadero. |
| [ExportImagesAsBase64](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportimagesasbase64) { get; set; } | Especifica si las imágenes se guardan en formato Base64 en HTML, MHTML o EPUB. |
| [ExportPrintAreaOnly](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportprintareaonly) { get; set; } | Indica si solo se exporta el área de impresión a archivo html. El valor predeterminado es falso. |
| [ExportSingleTab](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportsingletab) { get; set; } | Indica si exportar la pestaña única cuando el archivo solo tiene una hoja de trabajo. El valor predeterminado es falso. |
| [IsExportComments](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/isexportcomments) { get; set; } | Indica si al exportar comentarios al guardar el archivo en html, el valor predeterminado es falso. |
| [IsFullPathLink](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/isfullpathlink) { get; set; } | Indica si se usa el enlace de ruta completa en sheet00x.htm,filelist.xml y tabstrip.htm. El valor predeterminado es false. |
| [MergeAreas](../../aspose.cells.gridweb.data/gridsaveoptions/mergeareas) { get; set; } | Indica si fusionar las áreas de formato condicional y validación antes de guardar el archivo. |
| [PageTitle](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/pagetitle) { get; set; } | El título de la página html. Solo para guardar en flujo html. |
| [ParseHtmlTagInCell](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/parsehtmltagincell) { get; set; } | Analizar la etiqueta html en la celda, como ,como valor de celda o como etiqueta html, el valor predeterminado es true |
| [PresentationPreference](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/presentationpreference) { get; set; } | Indica si el archivo html o mht es la preferencia de presentación. El valor predeterminado es falso. Si desea obtener una presentación más hermosa, establezca el valor en verdadero. |
| [RefreshChartCache](../../aspose.cells.gridweb.data/gridsaveoptions/refreshchartcache) { get; set; } | Indica si se están actualizando los datos de la memoria caché del gráfico |
| [SaveFormat](../../aspose.cells.gridweb.data/gridsaveoptions/saveformat) { get; } | Obtiene el formato de archivo guardado. |
| [SortNames](../../aspose.cells.gridweb.data/gridsaveoptions/sortnames) { get; set; } | Indica si ordenar los nombres definidos antes de guardar el archivo. |
| [ValidateMergedAreas](../../aspose.cells.gridweb.data/gridsaveoptions/validatemergedareas) { get; set; } | Indica si validar las celdas combinadas antes de guardar el archivo. |

### Ver también

* class [GridSaveOptions](../gridsaveoptions)
* espacio de nombres [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data)
* asamblea [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
