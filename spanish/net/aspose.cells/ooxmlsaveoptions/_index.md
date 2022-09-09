---
title: OoxmlSaveOptions
second_title: Referencia de API de Aspose.Cells para .NET
description: Representa las opciones de guardar el archivo xml abierto de Office.
type: docs
weight: 4370
url: /es/net/aspose.cells/ooxmlsaveoptions/
---
## OoxmlSaveOptions class

Representa las opciones de guardar el archivo xml abierto de Office.

```csharp
public class OoxmlSaveOptions : SaveOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [OoxmlSaveOptions](ooxmlsaveoptions#constructor)() | Crea las opciones para guardar el archivo xml abierto de Office. |
| [OoxmlSaveOptions](ooxmlsaveoptions#constructor_1)(SaveFormat) | Crea las opciones para guardar el archivo xml abierto de Office. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder) { get; set; } | La carpeta de archivos en caché se utiliza para almacenar algunos datos de gran tamaño. |
| [ClearData](../../aspose.cells/saveoptions/cleardata) { get; set; } | Vacía el libro de trabajo después de guardar el archivo. |
| [CompressionType](../../aspose.cells/ooxmlsaveoptions/compressiontype) { get; set; } | Obtiene y establece el tipo de compresión para el archivo ooxml. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory) { get; set; } | Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo. |
| [EmbedOoxmlAsOleObject](../../aspose.cells/ooxmlsaveoptions/embedooxmlasoleobject) { get; set; } | Indica si incrustar archivos Ooxml de OleObject como objeto ole. |
| [EnableZip64](../../aspose.cells/ooxmlsaveoptions/enablezip64) { get; set; } | Siempre use extensiones ZIP64 cuando escriba archivos zip, incluso cuando no sea necesario. |
| [ExportCellName](../../aspose.cells/ooxmlsaveoptions/exportcellname) { get; set; } | Indica si exportar el nombre de la celda al archivo Excel2007 .xlsx (.xlsm, .xltx, .xltm). Si SQL Server DTS puede acceder al archivo de salida, este valor debe ser verdadero. Establecer el valor en falso aumentará considerablemente el rendimiento y reducirá el tamaño del archivo al crear un archivo grande. El valor predeterminado es verdadero. |
| [LightCellsDataProvider](../../aspose.cells/ooxmlsaveoptions/lightcellsdataprovider) { get; set; } | El proveedor de datos para proporcionar datos de celdas para guardar el libro de trabajo en modo ligero. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas) { get; set; } | Indica si fusionar las áreas de formato condicional y validación antes de guardar el archivo. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache) { get; set; } | Indica si se están actualizando los datos de la memoria caché del gráfico |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat) { get; } | Obtiene el formato de archivo guardado. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames) { get; set; } | Indica si ordenar los nombres definidos externos antes de guardar el archivo. |
| [SortNames](../../aspose.cells/saveoptions/sortnames) { get; set; } | Indica si ordenar los nombres definidos antes de guardar el archivo. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart) { get; set; } | Indica si se está actualizando la configuración de arte inteligente. El valor predeterminado es falso. |
| [UpdateZoom](../../aspose.cells/ooxmlsaveoptions/updatezoom) { get; set; } | Indica si actualizar el factor de escala antes de guardar el archivo si las propiedades PageSetup.FitToPagesWide y PageSetup.FitToPagesTall controlan cómo se escala la hoja de cálculo. |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas) { get; set; } | Indica si validar las celdas combinadas antes de guardar el archivo. |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback) { get; set; } | Obtiene o establece la devolución de llamada de advertencia. |

### Ver también

* class [SaveOptions](../saveoptions)
* espacio de nombres [Aspose.Cells](../../aspose.cells)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->