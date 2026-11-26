---
title: "Clase OoxmlSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.OoxmlSaveOptions class. Representa las opciones de guardado del archivo Office Open XML."
type: docs
url: /es/net/aspose.cells/ooxmlsaveoptions/
---
## OoxmlSaveOptions class

Representa las opciones de guardado de archivos Office Open XML.

```csharp
public class OoxmlSaveOptions : SaveOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [OoxmlSaveOptions](ooxmlsaveoptions/#constructor)() | Crea las opciones para guardar el archivo Office Open XML. |
| [OoxmlSaveOptions](ooxmlsaveoptions/#constructor_1)(SaveFormat) | Crea las opciones para guardar el archivo Office Open XML. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AsFlatOpc](../../aspose.cells/ooxmlsaveoptions/asflatopc/) { get; set; } | Indica si se guarda como un archivo OPC plano que puede ser generado por el SDK de Open XML. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | La carpeta para archivos temporales que pueden usarse como caché de datos.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, Excel no permite ingresar un valor de cadena más largo que 32K. Cuando se ingresa un valor más largo que 32K, se truncará.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Dejar el libro de trabajo vacío después de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [CompressionType](../../aspose.cells/ooxmlsaveoptions/compressiontype/) { get; set; } | Obtiene y establece el tipo de compresión para el archivo ooxml. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [EmbedOoxmlAsOleObject](../../aspose.cells/ooxmlsaveoptions/embedooxmlasoleobject/) { get; set; } | Indica si se incrustan archivos Ooxml de OleObject como objeto ole. |
| [EnableZip64](../../aspose.cells/ooxmlsaveoptions/enablezip64/) { get; set; } | Usar extensiones ZIP64 al escribir archivos zip, según sea necesario. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indica si se encriptan las propiedades del documento al guardar como archivo .xls. El valor predeterminado es verdadero.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [ExportCellName](../../aspose.cells/ooxmlsaveoptions/exportcellname/) { get; set; } | Indica si se exporta el nombre de la celda a un archivo Excel2007 .xlsx (.xlsm, .xltx, .xltm). Si el archivo de salida puede ser accedido por SQL Server DTS, este valor debe ser verdadero. Configurar el valor a falso aumentará considerablemente el rendimiento y reducirá el tamaño del archivo al crear archivos grandes. El valor predeterminado es verdadero. |
| [LightCellsDataProvider](../../aspose.cells/ooxmlsaveoptions/lightcellsdataprovider/) { get; set; } | El proveedor de datos para guardar el libro de trabajo en modo ligero. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indica si se fusionan las áreas de formato condicional y validación antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indica si se almacena en caché los datos más recientes del gráfico.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Obtiene el formato de archivo guardado.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indica si se ordenan los nombres definidos externos antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indica si se ordenan los nombres definidos antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indica si se actualiza la configuración de SmartArt. El valor predeterminado es falso.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [UpdateZoom](../../aspose.cells/ooxmlsaveoptions/updatezoom/) { get; set; } | Indica si se actualiza el factor de escala antes de guardar el archivo cuando las propiedades PageSetup.FitToPagesWide y PageSetup.FitToPagesTall controlan cómo se escala la hoja de cálculo. |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indica si se validan las celdas combinadas antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Obtiene o establece la devolución de llamada de advertencia. (Hereda de [`SaveOptions`](../saveoptions/).) |
| [WpsCompatibility](../../aspose.cells/ooxmlsaveoptions/wpscompatibility/) { get; set; } | (**Obsolete.**) Indica si hacer el xls más compatible con WPS. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OoxmlSaveOptionsDemo
    {
        public static void OoxmlSaveOptionsExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rellenar algunos datos en la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // Crear una instancia de OoxmlSaveOptions
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();

            // Estableciendo propiedades
            saveOptions.ExportCellName = true;
            saveOptions.UpdateZoom = true;
            saveOptions.EnableZip64 = false;
            saveOptions.EmbedOoxmlAsOleObject = false;
            saveOptions.CompressionType = OoxmlCompressionType.Level6;
            saveOptions.ClearData = false;
            saveOptions.CachedFileFolder = "C:\\Temp";
            saveOptions.ValidateMergedAreas = true;
            saveOptions.MergeAreas = false;
            saveOptions.SortNames = true;
            saveOptions.SortExternalNames = false;
            saveOptions.RefreshChartCache = true;
            saveOptions.UpdateSmartArt = false;

            // Guardar el libro de trabajo con las opciones especificadas
            workbook.Save("OoxmlSaveOptionsExample.xlsx", saveOptions);

            return;
        }
    }
}
```

### Ver también

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


