---
title: PdfSaveOptions
second_title: Referencia de API de Aspose.Cells para .NET
description: Representa las opciones para guardar el archivo pdf.
type: docs
weight: 4500
url: /es/net/aspose.cells/pdfsaveoptions/
---
## PdfSaveOptions class

Representa las opciones para guardar el archivo pdf.

```csharp
public class PdfSaveOptions : SaveOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions#constructor)() | Crea las opciones para guardar el archivo pdf. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells/pdfsaveoptions/allcolumnsinonepagepersheet) { get; set; } | Si AllColumnsInOnePagePerSheet es verdadero, todo el contenido de la columna de una hoja se generará en una sola página como resultado. Se ignorará el ancho del tamaño del papel de la configuración de la página, y las demás configuraciones de la configuración de la página seguirán teniendo efecto. |
| [Bookmark](../../aspose.cells/pdfsaveoptions/bookmark) { get; set; } | Obtiene y establece el[`PdfMarcadorEntrada`](../../aspose.cells.rendering/pdfbookmarkentry) objeto. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder) { get; set; } | La carpeta de archivos en caché se utiliza para almacenar algunos datos de gran tamaño. |
| [CalculateFormula](../../aspose.cells/pdfsaveoptions/calculateformula) { get; set; } | Indica si calcular fórmulas antes de guardar el archivo pdf. |
| [CheckFontCompatibility](../../aspose.cells/pdfsaveoptions/checkfontcompatibility) { get; set; } | Indica si se debe comprobar la compatibilidad de fuentes para cada carácter del texto. |
| [CheckWorkbookDefaultFont](../../aspose.cells/pdfsaveoptions/checkworkbookdefaultfont) { get; set; } | Cuando los caracteres en Excel son Unicode y no están configurados con la fuente correcta en el estilo de celda, Pueden aparecer como bloque en pdf,imagen. Establezca esto en verdadero para intentar usar la fuente predeterminada del libro de trabajo para mostrar estos caracteres primero. |
| [ClearData](../../aspose.cells/saveoptions/cleardata) { get; set; } | Vacía el libro de trabajo después de guardar el archivo. |
| [Compliance](../../aspose.cells/pdfsaveoptions/compliance) { get; set; } | El libro de trabajo se convierte a pdf de acuerdo con PdfCompliance en esta propiedad. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory) { get; set; } | Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo. |
| [CreatedTime](../../aspose.cells/pdfsaveoptions/createdtime) { get; set; } | Obtiene y establece el tiempo de generación del documento pdf. |
| [CustomPropertiesExport](../../aspose.cells/pdfsaveoptions/custompropertiesexport) { get; set; } | Obtiene o establece un valor que determina el camino[`CustomDocumentPropertyCollection`](../../aspose.cells.properties/customdocumentpropertycollection) se exportan a un archivo PDF. El valor predeterminado es Ninguno. |
| [DefaultEditLanguage](../../aspose.cells/pdfsaveoptions/defaulteditlanguage) { get; set; } | Obtiene o establece el idioma de edición predeterminado. |
| [DefaultFont](../../aspose.cells/pdfsaveoptions/defaultfont) { get; set; } | Cuando los caracteres en Excel son Unicode y no están configurados con la fuente correcta en el estilo de celda, Pueden aparecer como bloque en pdf, imagen. Establezca la Fuente predeterminada como MingLiu o MS Gothic para mostrar estos caracteres. Si esta propiedad es no configurado, Aspose.Cells utilizará la fuente predeterminada del sistema para mostrar estos caracteres Unicode. |
| [DisplayDocTitle](../../aspose.cells/pdfsaveoptions/displaydoctitle) { get; set; } | Indica si la barra de título de la ventana debe mostrar el título del documento. |
| [DrawObjectEventHandler](../../aspose.cells/pdfsaveoptions/drawobjecteventhandler) { get; set; } | Implementa esta interfaz para obtener DrawObject y Bound al renderizar. |
| [EmbedStandardWindowsFonts](../../aspose.cells/pdfsaveoptions/embedstandardwindowsfonts) { get; set; } | True para incrustar fuentes de tipo verdadero. Afecta solo a los caracteres ASCII 32-127. Las fuentes para códigos de caracteres superiores a 127 siempre están incrustadas. Las fuentes siempre están incrustadas para PDF/A-1a, PDF/A-1b estándar. El valor predeterminado es verdadero. |
| [EmfRenderSetting](../../aspose.cells/pdfsaveoptions/emfrendersetting) { get; set; } | Configuración para representar el metarchivo Emf. |
| [ExportDocumentStructure](../../aspose.cells/pdfsaveoptions/exportdocumentstructure) { get; set; } | Indica si exportar la estructura del documento. |
| [FontEncoding](../../aspose.cells/pdfsaveoptions/fontencoding) { get; set; } | Obtiene o establece la codificación de fuente incrustada en pdf. |
| [GridlineType](../../aspose.cells/pdfsaveoptions/gridlinetype) { get; set; } | Obtiene o establece el tipo de línea de cuadrícula. |
| [IgnoreError](../../aspose.cells/pdfsaveoptions/ignoreerror) { get; set; } | Indica si necesita ocultar el error durante la representación. El error puede ser un error en la forma, la imagen, la representación del gráfico, etc. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells/pdfsaveoptions/isfontsubstitutionchargranularity) { get; set; } | Indica si solo se sustituye la fuente del carácter cuando la fuente de la celda no es compatible con él. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas) { get; set; } | Indica si fusionar las áreas de formato condicional y validación antes de guardar el archivo. |
| [OnePagePerSheet](../../aspose.cells/pdfsaveoptions/onepagepersheet) { get; set; } | Si OnePagePerSheet es verdadero, todo el contenido de una hoja se generará en una sola página como resultado. El tamaño de papel de la configuración de la página no será válido y las demás configuraciones de la configuración de la página seguirán teniendo efecto. |
| [OptimizationType](../../aspose.cells/pdfsaveoptions/optimizationtype) { get; set; } | Obtiene y establece el tipo de optimización de pdf. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells/pdfsaveoptions/outputblankpagewhennothingtoprint) { get; set; } | Indica si se imprime una página en blanco cuando no hay nada que imprimir. |
| [PageCount](../../aspose.cells/pdfsaveoptions/pagecount) { get; set; } | Obtiene o establece el número de páginas a guardar. |
| [PageIndex](../../aspose.cells/pdfsaveoptions/pageindex) { get; set; } | Obtiene o establece el índice basado en 0 de la primera página para guardar. |
| [PageSavingCallback](../../aspose.cells/pdfsaveoptions/pagesavingcallback) { get; set; } | Controlar/Indicar el progreso del proceso de guardado de página. |
| [PdfCompression](../../aspose.cells/pdfsaveoptions/pdfcompression) { get; set; } | Indica el algoritmo de compresión |
| [PrintingPageType](../../aspose.cells/pdfsaveoptions/printingpagetype) { get; set; } | Indica qué páginas no se imprimirán. |
| [Producer](../../aspose.cells/pdfsaveoptions/producer) { get; set; } | Obtiene y establece el productor del documento pdf generado. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache) { get; set; } | Indica si se están actualizando los datos de la memoria caché del gráfico |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat) { get; } | Obtiene el formato de archivo guardado. |
| [SecurityOptions](../../aspose.cells/pdfsaveoptions/securityoptions) { get; set; } | Configure estas opciones cuando se necesite seguridad en el resultado xls2pdf. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames) { get; set; } | Indica si ordenar los nombres definidos externos antes de guardar el archivo. |
| [SortNames](../../aspose.cells/saveoptions/sortnames) { get; set; } | Indica si ordenar los nombres definidos antes de guardar el archivo. |
| [TextCrossType](../../aspose.cells/pdfsaveoptions/textcrosstype) { get; set; } | Obtiene o establece el tipo de texto que se muestra cuando el ancho del texto es mayor que el ancho de la celda. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart) { get; set; } | Indica si se está actualizando la configuración de arte inteligente. El valor predeterminado es falso. |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas) { get; set; } | Indica si validar las celdas combinadas antes de guardar el archivo. |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback) { get; set; } | Obtiene o establece la devolución de llamada de advertencia. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [SetImageResample](../../aspose.cells/pdfsaveoptions/setimageresample)(int, int) | Establece los PPI (píxeles por pulgada) deseados de las imágenes de remuestreo y la calidad jpeg. Todas las imágenes se convertirán a JPEG con la configuración de calidad especificada, y las imágenes que superen los PPI (píxeles por pulgada) especificados se volverán a muestrear. |

### Ver también

* class [SaveOptions](../saveoptions)
* espacio de nombres [Aspose.Cells](../../aspose.cells)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
