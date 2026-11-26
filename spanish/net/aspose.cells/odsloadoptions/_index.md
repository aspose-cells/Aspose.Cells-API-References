---
title: "Clase OdsLoadOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.OdsLoadOptions. Representa las opciones de carga del archivo ods"
type: docs
url: /es/net/aspose.cells/odsloadoptions/
---
## OdsLoadOptions class

Representa las opciones de carga de archivos ODS.

```csharp
public class OdsLoadOptions : LoadOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [OdsLoadOptions](odsloadoptions/#constructor)() | Representa las opciones de carga de archivos ODS. |
| [OdsLoadOptions](odsloadoptions/#constructor_1)(LoadFormat) | Representa las opciones de carga de archivos ODS. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ApplyExcelDefaultStyleToHyperlink](../../aspose.cells/odsloadoptions/applyexceldefaultstyletohyperlink/) { get; set; } | Indica si se aplica el estilo predeterminado de Excel al hipervínculo. |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Indica si se filtra automáticamente los datos al cargar los archivos.(Hereda de [`LoadOptions`](../loadoptions/).) |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Obtiene y establece las opciones de ajuste automático (Hereda de [`LoadOptions`](../loadoptions/).) |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Comprueba si los datos son válidos en el archivo de plantilla.(Hereda de [`LoadOptions`](../loadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, Excel no permite ingresar un valor de cadena mayor a 32 K. Cuando ingresas un valor mayor a 32 K, por ejemplo mediante Cell.PutValue(string), si esta propiedad es verdadera, obtendrás una excepción. Si es falsa, aceptaremos tu cadena de entrada como el valor de la celda, de modo que luego puedas exportar la cadena completa a otros formatos de archivo como CSV. Sin embargo, si has establecido un valor que es inválido para el formato de archivo Excel, no deberías guardar el libro de trabajo como formato Excel más adelante. De lo contrario, podría haber errores inesperados en el archivo Excel generado.(Hereda de [`LoadOptions`](../loadoptions/).) |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Obtiene o establece la configuración regional utilizada para el Workbook que se cargará.(Hereda de [`LoadOptions`](../loadoptions/).) |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | Obtiene la configuración de estilo predeterminada para inicializar los estilos del libro de trabajo (Hereda de [`LoadOptions`](../loadoptions/).) |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Obtiene y establece configuraciones de fuentes individuales. Solo funciona para el [`Workbook`](../workbook/) que usa este [`LoadOptions`](../loadoptions/) para cargar. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Ignora los datos que no se imprimen al imprimir directamente el archivo (Hereda de [`LoadOptions`](../loadoptions/).) |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Indica si se ignoran formas inútiles. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Obtiene y establece el monitor de interrupción. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [IsClassicPivotTable](../../aspose.cells/odsloadoptions/isclassicpivottable/) { get; set; } | Indica si la tabla dinámica es clásica. |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Indica si se mantiene los datos no analizados en memoria para el Workbook cuando se carga desde un archivo de plantilla. El valor predeterminado es true. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Obtiene o establece el idioma de la interfaz de usuario de la versión del Workbook basado en CountryCode que guardó el archivo. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | El manejador de datos para procesar los datos de celdas al leer el archivo de plantilla. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | El filtro que indica cómo cargar los datos. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Obtiene el formato de carga. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Obtiene o establece el modo de memoria para el libro de trabajo cargado. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Indica si se analiza la fórmula al leer el archivo. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Indica si se analizan los registros en caché de pivote al cargar el archivo. El valor predeterminado es false. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Obtiene y establece la contraseña del libro de trabajo. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Indica si se conservan esos espacios y saltos de línea que se rellenan entre los tokens de fórmula al obtener y establecer fórmulas. El valor predeterminado es false.(Heredado de [`LoadOptions`](../loadoptions/).) |
| [RefreshPivotTables](../../aspose.cells/odsloadoptions/refreshpivottables/) { get; set; } | Indica si se actualizan las tablas dinámicas al cargar el archivo. |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Obtiene o establece la configuración regional utilizada para el Workbook que se cargará.(Hereda de [`LoadOptions`](../loadoptions/).) |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsoleto.**) Establece el nombre de fuente estándar predeterminado(Heredado de [`LoadOptions`](../loadoptions/).) |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsoleto.**) Establece el tamaño de fuente estándar predeterminado.(Heredado de [`LoadOptions`](../loadoptions/).) |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback/) { get; set; } | Obtiene o establece la devolución de llamada de advertencia.(Heredado de [`LoadOptions`](../loadoptions/).) |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize/)(PaperSizeType) | Establece el tamaño de papel de impresión predeterminado a partir de la configuración de la impresora predeterminada.(Heredado de [`LoadOptions`](../loadoptions/).) |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OdsLoadOptionsDemo
    {
        public static void OdsLoadOptionsExample()
        {
            // Crea una instancia de OdsLoadOptions
            OdsLoadOptions loadOptions = new OdsLoadOptions();

            // Estableciendo propiedades
            loadOptions.ApplyExcelDefaultStyleToHyperlink = true;
            loadOptions.RefreshPivotTables = true;
            loadOptions.Password = "your_password";
            loadOptions.ParsingFormulaOnOpen = true;
            loadOptions.ParsingPivotCachedRecords = false;
            loadOptions.LanguageCode = CountryCode.USA;
            loadOptions.Region = CountryCode.USA;
            loadOptions.CultureInfo = new System.Globalization.CultureInfo("en-US");
            loadOptions.StandardFont = "Arial";
            loadOptions.StandardFontSize = 10.5;
            loadOptions.IgnoreNotPrinted = true;
            loadOptions.CheckDataValid = true;
            loadOptions.CheckExcelRestriction = true;
            loadOptions.KeepUnparsedData = true;
            loadOptions.LoadFilter = new LoadFilter(LoadDataFilterOptions.All);
            loadOptions.LightCellsDataHandler = new CustomLightCellsDataHandler();
            loadOptions.MemorySetting = MemorySetting.MemoryPreference;
            loadOptions.WarningCallback = new CustomWarningCallback();
            loadOptions.AutoFitterOptions = new AutoFitterOptions { AutoFitMergedCells = true };
            loadOptions.AutoFilter = true;
            loadOptions.FontConfigs = new IndividualFontConfigs();
            loadOptions.IgnoreUselessShapes = true;
            loadOptions.PreservePaddingSpacesInFormula = false;

            // Carga un archivo ODS con las opciones especificadas
            Workbook workbook = new Workbook("OdsLoadOptionsExample_original.ods", loadOptions);

            // Guardar el libro de trabajo en un archivo nuevo
            workbook.Save("OdsLoadOptionsExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* class [LoadOptions](../loadoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


