---
title: "Clase DbfSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Saving.DbfSaveOptions. Representa las opciones de guardado del archivo dbf"
type: docs
url: /es/net/aspose.cells.saving/dbfsaveoptions/
---
## DbfSaveOptions class

Representa las opciones de guardar el archivo dbf

```csharp
public class DbfSaveOptions : SaveOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [DbfSaveOptions](dbfsaveoptions/)() | Las opciones de guardado del archivo .dbf. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | La carpeta para archivos temporales que pueden usarse como caché de datos. (Hereditado de [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Si se verifica la restricción del archivo excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, excel no permite ingresar un valor de cadena mayor a 32K. Cuando se ingresa un valor mayor a 32K, se truncará. (Hereditado de [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Deja el libro de trabajo vacío después de guardar el archivo. (Hereditado de [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Si es true y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo. (Hereditado de [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indica si se encriptan las propiedades del documento al guardar como archivo .xls. El valor predeterminado es true. (Heredado de [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ExportAsString](../../aspose.cells.saving/dbfsaveoptions/exportasstring/) { get; set; } | Indica si se exporta como valor de cadena |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indica si se fusionan las áreas de formato condicional y validación antes de guardar el archivo.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indica si se almacena en caché los datos más recientes del gráfico.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Obtiene el formato de archivo guardado.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indica si se ordenan los nombres definidos externos antes de guardar el archivo.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indica si se ordenan los nombres definidos antes de guardar el archivo.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indica si se actualiza la configuración de smart art. El valor predeterminado es false.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indica si se validan las celdas combinadas antes de guardar el archivo.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Obtiene o establece la devolución de llamada de advertencia.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class SavingClassDbfSaveOptionsDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Crear una instancia de DbfSaveOptions
            DbfSaveOptions saveOptions = new DbfSaveOptions();
            
            // Establecer la propiedad ExportAsString
            saveOptions.ExportAsString = true;

            // Guardar el libro de trabajo con opciones de guardado DBF
            workbook.Save("output.dbf", saveOptions);

            Console.WriteLine("Workbook saved as DBF with ExportAsString set to true.");
        }
    }
}
```

### Ver también

* class [SaveOptions](../../aspose.cells/saveoptions/)
* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


