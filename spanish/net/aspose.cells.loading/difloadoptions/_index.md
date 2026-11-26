---
title: "Clase DifLoadOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Loading.DifLoadOptions. Representa las opciones de carga del archivo .dif"
type: docs
url: /es/net/aspose.cells.loading/difloadoptions/
---
## DifLoadOptions class

Representa las opciones de carga del archivo .dif.

```csharp
public class DifLoadOptions : LoadOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [DifLoadOptions](difloadoptions/)() | Las opciones. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Indica si se filtran automáticamente los datos al cargar los archivos. (Heredado de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Obtiene y establece las opciones del ajuste automático (Heredado de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Comprueba si los datos son válidos en el archivo de plantilla. (Heredado de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, Excel no permite introducir un valor de cadena superior a 32 K. Cuando ingresas un valor mayor a 32 K, por ejemplo mediante Cell.PutValue(string), si esta propiedad es verdadera, obtendrás una excepción. Si la propiedad es falsa, aceptaremos la cadena ingresada como valor de la celda, de modo que luego puedas exportar la cadena completa a otros formatos de archivo como CSV. Sin embargo, si estableces un valor que no es válido para el formato de archivo Excel, no deberías guardar el libro de trabajo como formato Excel más adelante. De lo contrario, podría producirse un error inesperado en el archivo Excel generado. (Heredado de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Obtiene o establece la configuración regional utilizada para el libro de trabajo que se cargará.(Heredado de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | Obtiene la configuración de estilo predeterminada para inicializar los estilos del libro de trabajo(Heredado de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Obtiene y establece configuraciones individuales de fuentes. Solo funciona para el [`Workbook`](../../aspose.cells/workbook/) que utiliza este [`LoadOptions`](../../aspose.cells/loadoptions/) para cargar.(Heredado de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Ignora los datos que no se imprimen si se imprime el archivo directamente(Heredado de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Indica si se ignoran formas inútiles(Heredado de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Obtiene y establece el monitor de interrupción(Heredado de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Indica si se mantiene los datos no analizados en memoria para el libro de trabajo cuando se carga desde un archivo de plantilla. El valor predeterminado es verdadero.(Heredado de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Obtiene o establece el idioma de la interfaz de usuario de la versión del libro de trabajo basado en CountryCode con el que se guardó el archivo.(Heredado de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | El controlador de datos para procesar los datos de celdas al leer el archivo de plantilla.(Heredado de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | El filtro para indicar cómo cargar los datos.(Heredado de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Obtiene el formato de carga.(Heredado de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Obtiene o establece el modo de memoria para el libro de trabajo cargado.(Heredado de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Indica si se analiza la fórmula al leer el archivo.(Heredado de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Indica si se analizan los registros en caché de la tabla dinámica al cargar el archivo. El valor predeterminado es falso.(Heredado de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Obtiene y establece la contraseña del libro de trabajo.(Heredado de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Indica si se conservan los espacios y saltos de línea que se insertan entre los tokens de la fórmula al obtener y establecer fórmulas. El valor predeterminado es falso.(Heredado de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Obtiene o establece la configuración regional utilizada para el libro de trabajo que se cargará.(Heredado de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsoleto.**) Establece el nombre de fuente estándar predeterminado(Heredado de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsoleto.**) Establece el tamaño de fuente estándar predeterminado.(Heredado de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback/) { get; set; } | Obtiene o establece la devolución de llamada de advertencia.(Heredado de [`LoadOptions`](../../aspose.cells/loadoptions/).) |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize/)(PaperSizeType) | Establece el tamaño de papel de impresión predeterminado a partir de la configuración de la impresora predeterminada.(Heredado de [`LoadOptions`](../../aspose.cells/loadoptions/).) |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Loading;

    public class LoadingClassDifLoadOptionsDemo
    {
        public static void Run()
        {
            // Crear instancia de DifLoadOptions
            DifLoadOptions loadOptions = new DifLoadOptions();

            // Crear un libro de trabajo (usando el constructor sin parámetros)
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer algunos datos de muestra
            worksheet.Cells["A1"].PutValue("Sample DIF Data");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(200);
            worksheet.Cells["A4"].PutValue(300);

            // Calcular fórmulas si las hay
            workbook.CalculateFormula();

            // Guardar el libro de trabajo en formato DIF
            workbook.Save("DifLoadOptionsOutput.dif", SaveFormat.Dif);

            // Ahora demostrar la carga del archivo DIF con DifLoadOptions
            DifLoadOptions difOptions = new DifLoadOptions();
            
            // Cargar el archivo DIF guardado con las opciones
            Workbook loadedWorkbook = new Workbook("DifLoadOptionsOutput.dif", difOptions);

            // Acceder a los datos del libro de trabajo cargado
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            string loadedValue = loadedWorksheet.Cells["A1"].StringValue;

            // Guardar los datos cargados en XLSX para verificación
            loadedWorkbook.Save("DifLoadOptionsVerification.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [LoadOptions](../../aspose.cells/loadoptions/)
* namespace [Aspose.Cells.Loading](../../aspose.cells.loading/)
* assembly [Aspose.Cells](../../)


