---
title: "Clase AbstractTextLoadOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.AbstractTextLoadOptions. Opciones comunes para cargar valores de texto"
type: docs
url: /es/net/aspose.cells/abstracttextloadoptions/
---
## AbstractTextLoadOptions class

Opciones comunes para cargar valores de texto

```csharp
public class AbstractTextLoadOptions : LoadOptions
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Indica si se filtra automáticamente los datos al cargar los archivos.(Hereda de [`LoadOptions`](../loadoptions/).) |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Obtiene y establece las opciones de ajuste automático (Hereda de [`LoadOptions`](../loadoptions/).) |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Comprueba si los datos son válidos en el archivo de plantilla.(Hereda de [`LoadOptions`](../loadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, Excel no permite ingresar un valor de cadena mayor a 32 K. Cuando ingresas un valor mayor a 32 K, por ejemplo mediante Cell.PutValue(string), si esta propiedad es verdadera, obtendrás una excepción. Si es falsa, aceptaremos tu cadena de entrada como el valor de la celda, de modo que luego puedas exportar la cadena completa a otros formatos de archivo como CSV. Sin embargo, si has establecido un valor que es inválido para el formato de archivo Excel, no deberías guardar el libro de trabajo como formato Excel más adelante. De lo contrario, podría haber errores inesperados en el archivo Excel generado.(Hereda de [`LoadOptions`](../loadoptions/).) |
| [ConvertDateTimeData](../../aspose.cells/abstracttextloadoptions/convertdatetimedata/) { get; set; } | Obtiene o establece un valor que indica si la cadena en el archivo de texto se convierte en datos de fecha. El valor predeterminado es true. |
| [ConvertNumericData](../../aspose.cells/abstracttextloadoptions/convertnumericdata/) { get; set; } | Obtiene o establece un valor que indica si la cadena en el archivo de texto se convierte en datos numéricos. El valor predeterminado es true. |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Obtiene o establece la configuración regional utilizada para el Workbook que se cargará.(Hereda de [`LoadOptions`](../loadoptions/).) |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | Obtiene la configuración de estilo predeterminada para inicializar los estilos del libro de trabajo (Hereda de [`LoadOptions`](../loadoptions/).) |
| [Encoding](../../aspose.cells/abstracttextloadoptions/encoding/) { get; set; } | Obtiene y establece la codificación predeterminada. Solo se aplica a archivos csv. |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Obtiene y establece configuraciones de fuentes individuales. Solo funciona para el [`Workbook`](../workbook/) que usa este [`LoadOptions`](../loadoptions/) para cargar. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Ignora los datos que no se imprimen al imprimir directamente el archivo (Hereda de [`LoadOptions`](../loadoptions/).) |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Indica si se ignoran formas inútiles. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Obtiene y establece el monitor de interrupción. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [KeepPrecision](../../aspose.cells/abstracttextloadoptions/keepprecision/) { get; set; } | Indica si no se analiza un valor de cadena cuando la longitud es 15. |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Indica si se mantiene los datos no analizados en memoria para el Workbook cuando se carga desde un archivo de plantilla. El valor predeterminado es true. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Obtiene o establece el idioma de la interfaz de usuario de la versión del Workbook basado en CountryCode que guardó el archivo. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | El manejador de datos para procesar los datos de celdas al leer el archivo de plantilla. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | El filtro que indica cómo cargar los datos. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Obtiene el formato de carga. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [LoadStyleStrategy](../../aspose.cells/abstracttextloadoptions/loadstylestrategy/) { get; set; } | Indica la estrategia para aplicar estilo a los valores analizados al convertir una cadena a número o fecha y hora. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Obtiene o establece el modo de memoria para el libro de trabajo cargado. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Indica si se analiza la fórmula al leer el archivo. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Indica si se analizan los registros en caché de pivote al cargar el archivo. El valor predeterminado es false. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Obtiene y establece la contraseña del libro de trabajo. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Indica si se conservan esos espacios y saltos de línea que se rellenan entre los tokens de fórmula al obtener y establecer fórmulas. El valor predeterminado es false.(Heredado de [`LoadOptions`](../loadoptions/).) |
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
using Aspose.Cells;
using System;
using System.Text;

namespace AsposeCellsExamples
{
    // Implementación personalizada de AbstractTextLoadOptions
    public class CustomTextLoadOptions : AbstractTextLoadOptions
    {
        public CustomTextLoadOptions()
        {
            // Establezca la codificación predeterminada a UTF8
            this.Encoding = Encoding.UTF8;

            // Establezca LoadStyleStrategy a None
            this.LoadStyleStrategy = TxtLoadStyleStrategy.None;

            // Habilitar la conversión de datos numéricos
            this.ConvertNumericData = true;

            // Habilitar la conversión de datos de fecha
            this.ConvertDateTimeData = true;

            // Mantener la precisión para cadenas con longitud 15
            this.KeepPrecision = true;
        }
    }

    public class TextLoadOptionsDemo
    {
        public static void RunDemo()
        {
            // Cree una instancia de CustomTextLoadOptions
            CustomTextLoadOptions loadOptions = new CustomTextLoadOptions();

            // Cargue un archivo CSV con las opciones de carga personalizadas
            Workbook workbook = new Workbook("TextLoadOptionsDemo_original.csv", loadOptions);

            // Acceder a la primera hoja de cálculo
            Worksheet sheet = workbook.Worksheets[0];

            // Imprima el valor de la primera celda
            Console.WriteLine(sheet.Cells["A1"].StringValue);

            // Guardar el libro de trabajo en un archivo nuevo
            workbook.Save("TextLoadOptionsDemo.xlsx");
            workbook.Save("TextLoadOptionsDemo.pdf");
        }
    }
}
```

### Ver también

* class [LoadOptions](../loadoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


