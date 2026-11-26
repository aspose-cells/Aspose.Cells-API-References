---
title: "Clase XlsSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.XlsSaveOptions class. Representa las opciones de guardado para el formato de archivo Excel 972003 xls y xlt"
type: docs
url: /es/net/aspose.cells/xlssaveoptions/
---
## XlsSaveOptions class

Representa las opciones de guardado para el formato de archivo Excel 97-2003: xls y xlt.

```csharp
public class XlsSaveOptions : SaveOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [XlsSaveOptions](xlssaveoptions/#constructor)() | Crea opciones para guardar el archivo Excel 97-2003 xls. |
| [XlsSaveOptions](xlssaveoptions/#constructor_1)(SaveFormat) | Crea opciones para guardar el archivo Excel 97-2003 xls/xlt. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | La carpeta para archivos temporales que pueden usarse como caché de datos.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, Excel no permite ingresar un valor de cadena más largo que 32K. Cuando se ingresa un valor más largo que 32K, se truncará.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Dejar el libro de trabajo vacío después de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indica si se encriptan las propiedades del documento al guardar como archivo .xls. El valor predeterminado es verdadero.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [IsTemplate](../../aspose.cells/xlssaveoptions/istemplate/) { get; set; } | (**Obsolete.**) Indica si se está guardando un archivo de plantilla. |
| [LightCellsDataProvider](../../aspose.cells/xlssaveoptions/lightcellsdataprovider/) { get; set; } | El proveedor de datos para guardar el libro de trabajo en modo ligero. |
| [MatchColor](../../aspose.cells/xlssaveoptions/matchcolor/) { get; set; } | Indica si coincidir el color de fuente porque hay 56 colores en la paleta de colores estándar. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indica si se fusionan las áreas de formato condicional y validación antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indica si se almacena en caché los datos más recientes del gráfico.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Obtiene el formato de archivo guardado.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indica si se ordenan los nombres definidos externos antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indica si se ordenan los nombres definidos antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indica si se actualiza la configuración de SmartArt. El valor predeterminado es falso.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indica si se validan las celdas combinadas antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Obtiene o establece la devolución de llamada de advertencia. (Hereda de [`SaveOptions`](../saveoptions/).) |
| [WpsCompatibility](../../aspose.cells/xlssaveoptions/wpscompatibility/) { get; set; } | (**Obsolete.**) Indica si hacer el xls más compatible con WPS. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XlsSaveOptionsDemo
    {
        public static void XlsSaveOptionsExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rellenar algunos datos en la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(25);

            // Crear una instancia de XlsSaveOptions
            XlsSaveOptions saveOptions = new XlsSaveOptions();

            // Estableciendo propiedades
            saveOptions.MatchColor = true;
            saveOptions.ClearData = false;
            saveOptions.ValidateMergedAreas = true;
            saveOptions.MergeAreas = true;
            saveOptions.SortNames = true;
            saveOptions.SortExternalNames = false;
            saveOptions.RefreshChartCache = true;
            saveOptions.UpdateSmartArt = false;

            // Guarde el libro de trabajo con las opciones de guardado especificadas
            workbook.Save("XlsSaveOptionsExample.xlsx", saveOptions);

            return;
        }
    }
}
```

### Ver también

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


