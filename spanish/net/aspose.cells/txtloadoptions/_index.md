---
title: "Clase TxtLoadOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.TxtLoadOptions. Representa las opciones para cargar un archivo de texto"
type: docs
url: /es/net/aspose.cells/txtloadoptions/
---
## TxtLoadOptions class

Representa las opciones para cargar un archivo de texto.

```csharp
public class TxtLoadOptions : AbstractTextLoadOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [TxtLoadOptions](txtloadoptions/#constructor)() | Crea las opciones para cargar un archivo de texto. |
| [TxtLoadOptions](txtloadoptions/#constructor_1)(LoadFormat) | Crea las opciones para cargar un archivo de texto. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Indica si se filtra automáticamente los datos al cargar los archivos.(Hereda de [`LoadOptions`](../loadoptions/).) |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Obtiene y establece las opciones de ajuste automático (Hereda de [`LoadOptions`](../loadoptions/).) |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Comprueba si los datos son válidos en el archivo de plantilla.(Hereda de [`LoadOptions`](../loadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, Excel no permite ingresar un valor de cadena mayor a 32 K. Cuando ingresas un valor mayor a 32 K, por ejemplo mediante Cell.PutValue(string), si esta propiedad es verdadera, obtendrás una excepción. Si es falsa, aceptaremos tu cadena de entrada como el valor de la celda, de modo que luego puedas exportar la cadena completa a otros formatos de archivo como CSV. Sin embargo, si has establecido un valor que es inválido para el formato de archivo Excel, no deberías guardar el libro de trabajo como formato Excel más adelante. De lo contrario, podría haber errores inesperados en el archivo Excel generado.(Hereda de [`LoadOptions`](../loadoptions/).) |
| [ConvertDateTimeData](../../aspose.cells/abstracttextloadoptions/convertdatetimedata/) { get; set; } | Obtiene o establece un valor que indica si la cadena en el archivo de texto se convierte en datos de fecha. El valor predeterminado es true.(Heredado de [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [ConvertNumericData](../../aspose.cells/abstracttextloadoptions/convertnumericdata/) { get; set; } | Obtiene o establece un valor que indica si la cadena en el archivo de texto se convierte en datos numéricos. El valor predeterminado es true.(Heredado de [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Obtiene o establece la configuración regional utilizada para el Workbook que se cargará.(Hereda de [`LoadOptions`](../loadoptions/).) |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | Obtiene la configuración de estilo predeterminada para inicializar los estilos del libro de trabajo (Hereda de [`LoadOptions`](../loadoptions/).) |
| [Encoding](../../aspose.cells/abstracttextloadoptions/encoding/) { get; set; } | Obtiene y establece la codificación predeterminada. Solo se aplica para archivos csv. (Heredado de [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [ExtendToNextSheet](../../aspose.cells/txtloadoptions/extendtonextsheet/) { get; set; } | Indica si extiende los datos a la siguiente hoja cuando las filas o columnas de datos superan el límite. El valor predeterminado es falso. |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Obtiene y establece configuraciones de fuentes individuales. Solo funciona para el [`Workbook`](../workbook/) que usa este [`LoadOptions`](../loadoptions/) para cargar. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [HasFormula](../../aspose.cells/txtloadoptions/hasformula/) { get; set; } | Indica si el texto es una fórmula si comienza con "=". |
| [HasTextQualifier](../../aspose.cells/txtloadoptions/hastextqualifier/) { get; set; } | Indica si hay calificador de texto para el valor de la celda. El valor predeterminado es verdadero. |
| [HeaderColumnsCount](../../aspose.cells/txtloadoptions/headercolumnscount/) { get; set; } | La cantidad de columnas de encabezado que se repetirán en hojas extendidas. |
| [HeaderRowsCount](../../aspose.cells/txtloadoptions/headerrowscount/) { get; set; } | La cantidad de filas de encabezado que se repetirán en hojas extendidas. |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Ignora los datos que no se imprimen al imprimir directamente el archivo (Hereda de [`LoadOptions`](../loadoptions/).) |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Indica si se ignoran formas inútiles. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Obtiene y establece el monitor de interrupción. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [IsMultiEncoded](../../aspose.cells/txtloadoptions/ismultiencoded/) { get; set; } | Verdadero indica que el archivo contiene varias codificaciones. |
| [KeepPrecision](../../aspose.cells/abstracttextloadoptions/keepprecision/) { get; set; } | Indica si no se analiza un valor de cadena cuando la longitud es 15. (Heredado de [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Indica si se mantiene los datos no analizados en memoria para el Workbook cuando se carga desde un archivo de plantilla. El valor predeterminado es true. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Obtiene o establece el idioma de la interfaz de usuario de la versión del Workbook basado en CountryCode que guardó el archivo. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | El manejador de datos para procesar los datos de celdas al leer el archivo de plantilla. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | El filtro que indica cómo cargar los datos. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Obtiene el formato de carga. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [LoadStyleStrategy](../../aspose.cells/abstracttextloadoptions/loadstylestrategy/) { get; set; } | Indica la estrategia para aplicar estilo a los valores analizados al convertir un valor de cadena a número o fecha/hora. (Heredado de [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [MaxColumnCount](../../aspose.cells/txtloadoptions/maxcolumncount/) { get; set; } | La cantidad máxima de columnas que se importarán para una hoja. |
| [MaxRowCount](../../aspose.cells/txtloadoptions/maxrowcount/) { get; set; } | La cantidad máxima de filas que se importarán para una hoja. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Obtiene o establece el modo de memoria para el libro de trabajo cargado. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Indica si se analiza la fórmula al leer el archivo. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Indica si se analizan los registros en caché de pivote al cargar el archivo. El valor predeterminado es false. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Obtiene y establece la contraseña del libro de trabajo. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [PreferredParsers](../../aspose.cells/txtloadoptions/preferredparsers/) { get; set; } | Obtiene y establece los analizadores de valores preferidos para cargar un archivo de texto. |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Indica si se conservan esos espacios y saltos de línea que se rellenan entre los tokens de fórmula al obtener y establecer fórmulas. El valor predeterminado es false.(Heredado de [`LoadOptions`](../loadoptions/).) |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Obtiene o establece la configuración regional utilizada para el Workbook que se cargará.(Hereda de [`LoadOptions`](../loadoptions/).) |
| [Separator](../../aspose.cells/txtloadoptions/separator/) { get; set; } | Obtiene y establece el separador de caracteres del archivo de texto. |
| [SeparatorString](../../aspose.cells/txtloadoptions/separatorstring/) { get; set; } | Obtiene y establece un valor de cadena como separador. |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsoleto.**) Establece el nombre de fuente estándar predeterminado(Heredado de [`LoadOptions`](../loadoptions/).) |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsoleto.**) Establece el tamaño de fuente estándar predeterminado.(Heredado de [`LoadOptions`](../loadoptions/).) |
| [TextQualifier](../../aspose.cells/txtloadoptions/textqualifier/) { get; set; } | Especifica el calificador de texto para los valores de celda. El calificador predeterminado es '\"'. |
| [TreatConsecutiveDelimitersAsOne](../../aspose.cells/txtloadoptions/treatconsecutivedelimitersasone/) { get; set; } | Indica si los delimitadores consecutivos deben tratarse como uno. |
| [TreatQuotePrefixAsValue](../../aspose.cells/txtloadoptions/treatquoteprefixasvalue/) { get; set; } | Indica si el signo de comilla simple inicial debe tomarse como parte del valor de una celda. El valor predeterminado es true. Si es false, la comilla simple inicial se eliminará del valor de la celda correspondiente y [`QuotePrefix`](../style/quoteprefix/) se establecerá como true para la celda. |
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
    using System.Text;

    public class TxtLoadOptionsDemo
    {
        public static void TxtLoadOptionsExample()
        {
            // Crear una instancia de TxtLoadOptions
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
            {
                Separator = ',',
                SeparatorString = ",",
                IsMultiEncoded = false,
                HasFormula = true,
                HasTextQualifier = true,
                TextQualifier = '\"',
                TreatConsecutiveDelimitersAsOne = true,
                TreatQuotePrefixAsValue = true,
                ExtendToNextSheet = false,
                HeaderRowsCount = 1,
                HeaderColumnsCount = 1,
                MaxRowCount = 1000,
                MaxColumnCount = 50,
                Encoding = Encoding.UTF8,
                LoadStyleStrategy = TxtLoadStyleStrategy.BuiltIn,
                ConvertNumericData = true,
                ConvertDateTimeData = true,
                KeepPrecision = true,
                Password = "password",
                ParsingFormulaOnOpen = true,
                ParsingPivotCachedRecords = true,
                LanguageCode = CountryCode.USA,
                Region = CountryCode.USA,
                CultureInfo = new System.Globalization.CultureInfo("en-US"),
                StandardFont = "Arial",
                StandardFontSize = 10.5,
                InterruptMonitor = new InterruptMonitor(),
                IgnoreNotPrinted = true,
                CheckDataValid = true,
                CheckExcelRestriction = true,
                KeepUnparsedData = true,
                LoadFilter = new LoadFilter(LoadDataFilterOptions.All),
                LightCellsDataHandler = new LightCellsDataHandler(),
                MemorySetting = MemorySetting.MemoryPreference,
                WarningCallback = new WarningCallback(),
                AutoFitterOptions = new AutoFitterOptions(),
                AutoFilter = true,
                FontConfigs = new IndividualFontConfigs(),
                IgnoreUselessShapes = true,
                PreservePaddingSpacesInFormula = true
            };

            // Cargar un archivo CSV con las opciones especificadas
            Workbook workbook = new Workbook("TxtLoadOptionsExample_original.csv", loadOptions);

            // Guarda el libro de trabajo en un archivo Excel
            workbook.Save("TxtLoadOptionsExample.xlsx");

            return;
        }
    }

    // Implementaciones ficticias para clases/interfaces referenciadas
    public class InterruptMonitor : AbstractInterruptMonitor
    {
        public override bool IsInterruptionRequested => false;
    }

    public class WarningCallback : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            Console.WriteLine(warningInfo.Description);
        }
    }

    public class LightCellsDataHandler : Aspose.Cells.LightCellsDataHandler
    {
        public bool StartSheet(Worksheet sheet) => true;
        public bool StartRow(int rowIndex) => true;
        public bool ProcessRow(Row row) => true;
        public bool StartCell(int columnIndex) => true;
        public bool ProcessCell(Cell cell) => true;
    }
}
```

### Ver también

* class [AbstractTextLoadOptions](../abstracttextloadoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


