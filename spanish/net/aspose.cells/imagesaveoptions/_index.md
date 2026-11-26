---
title: "Clase ImageSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.ImageSaveOptions. Representa opciones de guardado de imagen. Para uso avanzado, por favor use WorkbookRender o SheetRender"
type: docs
url: /es/net/aspose.cells/imagesaveoptions/
---
## ImageSaveOptions class

Representa opciones de guardado de imagen. Para uso avanzado, por favor use [`WorkbookRender`](../../aspose.cells.rendering/workbookrender/) o [`SheetRender`](../../aspose.cells.rendering/sheetrender/).

```csharp
public class ImageSaveOptions : SaveOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [ImageSaveOptions](imagesaveoptions/#constructor)() | Crea las opciones para guardar el archivo de imagen. |
| [ImageSaveOptions](imagesaveoptions/#constructor_1)(SaveFormat) | Crea las opciones para guardar el archivo de imagen. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | La carpeta para archivos temporales que pueden usarse como caché de datos.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, Excel no permite ingresar un valor de cadena más largo que 32K. Cuando se ingresa un valor más largo que 32K, se truncará.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Dejar el libro de trabajo vacío después de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indica si se encriptan las propiedades del documento al guardar como archivo .xls. El valor predeterminado es verdadero.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [ImageOrPrintOptions](../../aspose.cells/imagesaveoptions/imageorprintoptions/) { get; } | Opciones adicionales de creación de imagen. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indica si se fusionan las áreas de formato condicional y validación antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indica si se almacena en caché los datos más recientes del gráfico.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Obtiene el formato de archivo guardado.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indica si se ordenan los nombres definidos externos antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indica si se ordenan los nombres definidos antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [StreamProvider](../../aspose.cells/imagesaveoptions/streamprovider/) { get; set; } | Obtiene o establece el IStreamProvider para exportar objetos. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indica si se actualiza la configuración de SmartArt. El valor predeterminado es falso.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indica si se validan las celdas combinadas antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Obtiene o establece la devolución de llamada de advertencia. (Hereda de [`SaveOptions`](../saveoptions/).) |

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassImageSaveOptionsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Image Export");

            // Establecer la ruta de destino
            string destPath = "output.png";

            // Crear opciones de guardado de imagen
            ImageSaveOptions saveOptions = new ImageSaveOptions(SaveFormat.Png);
            
            // Personalizar opciones de guardado
            saveOptions.ImageOrPrintOptions.OnePagePerSheet = true;
            saveOptions.ImageOrPrintOptions.OnlyArea = true;

            // Guardar el libro de trabajo con opciones de imagen
            workbook.Save(destPath, saveOptions);

            Console.WriteLine("Image saved successfully to: " + destPath);
        }
    }
}
```

### Ver también

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


