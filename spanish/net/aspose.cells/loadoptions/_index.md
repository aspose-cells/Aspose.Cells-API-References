---
title: "Clase LoadOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.LoadOptions. Representa las opciones de carga del archivo"
type: docs
url: /es/net/aspose.cells/loadoptions/
---
## LoadOptions class

Representa las opciones de carga del archivo.

```csharp
public class LoadOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [LoadOptions](loadoptions/#constructor)() | Crea una opción de carga del archivo. |
| [LoadOptions](loadoptions/#constructor_1)(LoadFormat) | Crea una opción de carga del archivo. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Indica si se filtra automáticamente los datos al cargar los archivos. |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Obtiene y establece las opciones del ajuste automático |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Verificar si los datos son válidos en el archivo de plantilla. |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, Excel no permite introducir un valor de cadena superior a 32 K. Cuando introduces un valor superior a 32 K, como mediante Cell.PutValue(string), si esta propiedad es verdadera, obtendrás una excepción. Si esta propiedad es falsa, aceptaremos la cadena introducida como el valor de la celda, de modo que posteriormente puedas exportar la cadena completa a otros formatos de archivo como CSV. Sin embargo, si has establecido un valor que no es válido para el formato de archivo Excel, no deberías guardar el libro posteriormente en formato Excel. De lo contrario, podría producirse un error inesperado en el archivo Excel generado. |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Obtiene o establece la configuración regional utilizada para el Workbook que se cargará. |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | Obtiene la configuración de estilo predeterminada para inicializar los estilos del libro de trabajo |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Obtiene y establece configuraciones de fuente individuales. Solo funciona para el [`Workbook`](../workbook/) que usa este `LoadOptions` para cargar. |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Ignora los datos que no se imprimen al imprimir directamente el archivo |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Indica si se ignoran formas inútiles. |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Obtiene y establece el monitor de interrupción. |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Indica si se mantiene los datos no analizados en memoria para el Workbook cuando se carga desde un archivo de plantilla. El valor predeterminado es true. |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Obtiene o establece el idioma de la interfaz de usuario de la versión del Workbook basado en CountryCode que ha guardado el archivo. |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | El controlador de datos para procesar los datos de celdas al leer el archivo de plantilla. |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | El filtro que indica cómo cargar los datos. |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Obtiene el formato de carga. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Obtiene o establece el modo de memoria para el libro de trabajo cargado. |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Indica si se analiza la fórmula al leer el archivo. |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Indica si se analizan los registros en caché de la tabla dinámica al cargar el archivo. El valor predeterminado es false. |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Obtiene y establece la contraseña del libro de trabajo. |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Indica si se conservan los espacios y saltos de línea que se insertan entre los tokens de la fórmula al obtener y establecer fórmulas. El valor predeterminado es false. |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Obtiene o establece la configuración regional utilizada para el Workbook que se cargará. |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsolete.**) Establece el nombre de fuente estándar predeterminado |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsolete.**) Establece el tamaño de fuente estándar predeterminado. |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback/) { get; set; } | Obtiene o establece la devolución de llamada de advertencia. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize/)(PaperSizeType) | Establece el tamaño de papel de impresión predeterminado a partir de la configuración de la impresora predeterminada. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Globalization;

    public class LoadOptionsDemo
    {
        public static void LoadOptionsExample()
        {
            // Crea una instancia de LoadOptions
            LoadOptions loadOptions = new LoadOptions();

            // Estableciendo propiedades
            loadOptions.Password = "password123";
            loadOptions.ParsingFormulaOnOpen = true;
            loadOptions.ParsingPivotCachedRecords = false;
            loadOptions.LanguageCode = CountryCode.USA;
            loadOptions.Region = CountryCode.USA;
            loadOptions.CultureInfo = new CultureInfo("en-US");
            loadOptions.IgnoreNotPrinted = true;
            loadOptions.CheckDataValid = true;
            loadOptions.CheckExcelRestriction = false;
            loadOptions.KeepUnparsedData = true;
            loadOptions.MemorySetting = MemorySetting.MemoryPreference;
            loadOptions.AutoFitterOptions = new AutoFitterOptions { AutoFitMergedCells = true };
            loadOptions.AutoFilter = true;
            loadOptions.IgnoreUselessShapes = true;
            loadOptions.PreservePaddingSpacesInFormula = false;

            // Cargue un libro de trabajo con los LoadOptions especificados
            Workbook workbook = new Workbook("LoadOptionsExample_original.xlsx", loadOptions);

            // Realiza operaciones en el libro de trabajo
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello, World!");

            // Guarda el libro de trabajo
            workbook.Save("LoadOptionsExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


