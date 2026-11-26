---
title: "Clase EbookLoadOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.EbookLoadOptions. Representa opciones al importar un archivo ebook"
type: docs
url: /es/net/aspose.cells/ebookloadoptions/
---
## EbookLoadOptions class

Representa las opciones al importar un archivo ebook.

```csharp
public class EbookLoadOptions : HtmlLoadOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [EbookLoadOptions](ebookloadoptions/#constructor)() | Crea una opción para cargar el archivo ebook. |
| [EbookLoadOptions](ebookloadoptions/#constructor_1)(LoadFormat) | Crea una opción de carga del archivo ebook. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AttachedFilesDirectory](../../aspose.cells/htmlloadoptions/attachedfilesdirectory/) { get; set; } | (**Obsolete.**) El directorio donde se guardarán los archivos adjuntos.(Hereda de [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Indica si se filtra automáticamente los datos al cargar los archivos.(Hereda de [`LoadOptions`](../loadoptions/).) |
| [AutoFitColsAndRows](../../aspose.cells/htmlloadoptions/autofitcolsandrows/) { get; set; } | Indica si se ajustan automáticamente columnas y filas. El valor predeterminado es false.(Hereda de [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Obtiene y establece las opciones de ajuste automático (Hereda de [`LoadOptions`](../loadoptions/).) |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Comprueba si los datos son válidos en el archivo de plantilla.(Hereda de [`LoadOptions`](../loadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, Excel no permite ingresar un valor de cadena mayor a 32 K. Cuando ingresas un valor mayor a 32 K, por ejemplo mediante Cell.PutValue(string), si esta propiedad es verdadera, obtendrás una excepción. Si es falsa, aceptaremos tu cadena de entrada como el valor de la celda, de modo que luego puedas exportar la cadena completa a otros formatos de archivo como CSV. Sin embargo, si has establecido un valor que es inválido para el formato de archivo Excel, no deberías guardar el libro de trabajo como formato Excel más adelante. De lo contrario, podría haber errores inesperados en el archivo Excel generado.(Hereda de [`LoadOptions`](../loadoptions/).) |
| [ConvertDateTimeData](../../aspose.cells/abstracttextloadoptions/convertdatetimedata/) { get; set; } | Obtiene o establece un valor que indica si la cadena en el archivo de texto se convierte en datos de fecha. El valor predeterminado es true.(Heredado de [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [ConvertFormulasData](../../aspose.cells/htmlloadoptions/convertformulasdata/) { get; set; } | (**Obsolete.**) si es true, convierte la cadena a fórmula cuando el valor de cadena comienza con el carácter '=', el valor predeterminado es false.(Hereda de [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [ConvertNumericData](../../aspose.cells/abstracttextloadoptions/convertnumericdata/) { get; set; } | Obtiene o establece un valor que indica si la cadena en el archivo de texto se convierte en datos numéricos. El valor predeterminado es true.(Heredado de [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Obtiene o establece la configuración regional utilizada para el Workbook que se cargará.(Hereda de [`LoadOptions`](../loadoptions/).) |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | Obtiene la configuración de estilo predeterminada para inicializar los estilos del libro de trabajo (Hereda de [`LoadOptions`](../loadoptions/).) |
| [DeleteRedundantSpaces](../../aspose.cells/htmlloadoptions/deleteredundantspaces/) { get; set; } | Indica si se eliminan los espacios redundantes cuando el texto envuelve líneas usando la etiqueta `<br>`. El valor predeterminado es false.(Hereda de [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [DetectLaTeX](../../aspose.cells/htmlloadoptions/detectlatex/) { get; set; } | Indica si se detecta la fórmula LaTeX en el archivo HTML. El valor predeterminado es false.(Hereda de [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [Encoding](../../aspose.cells/abstracttextloadoptions/encoding/) { get; set; } | Obtiene y establece la codificación predeterminada. Solo se aplica para archivos csv. (Heredado de [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Obtiene y establece configuraciones de fuentes individuales. Solo funciona para el [`Workbook`](../workbook/) que usa este [`LoadOptions`](../loadoptions/) para cargar. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [HasFormula](../../aspose.cells/htmlloadoptions/hasformula/) { get; set; } | Indica si el texto es una fórmula si comienza con "=".(Hereda de [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [HyperlinkLoadMode](../../aspose.cells/htmlloadoptions/hyperlinkloadmode/) { get; set; } | Especifica cómo se cargan los hipervínculos al cargar HTML.(Hereda de [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Ignora los datos que no se imprimen al imprimir directamente el archivo (Hereda de [`LoadOptions`](../loadoptions/).) |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Indica si se ignoran formas inútiles. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Obtiene y establece el monitor de interrupción. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [KeepPrecision](../../aspose.cells/abstracttextloadoptions/keepprecision/) { get; set; } | Indica si no se analiza un valor de cadena cuando la longitud es 15. (Heredado de [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Indica si se mantiene los datos no analizados en memoria para el Workbook cuando se carga desde un archivo de plantilla. El valor predeterminado es true. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Obtiene o establece el idioma de la interfaz de usuario de la versión del Workbook basado en CountryCode que guardó el archivo. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | El manejador de datos para procesar los datos de celdas al leer el archivo de plantilla. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | El filtro que indica cómo cargar los datos. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Obtiene el formato de carga. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [LoadFormulas](../../aspose.cells/htmlloadoptions/loadformulas/) { get; set; } | Indica si se importan fórmulas cuando el archivo html original contiene fórmulas(Hereda de [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [LoadStyleStrategy](../../aspose.cells/abstracttextloadoptions/loadstylestrategy/) { get; set; } | Indica la estrategia para aplicar estilo a los valores analizados al convertir un valor de cadena a número o fecha/hora. (Heredado de [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Obtiene o establece el modo de memoria para el libro de trabajo cargado. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [ParagrahLayoutMode](../../aspose.cells/htmlloadoptions/paragrahlayoutmode/) { get; set; } | (**Obsolete.**) Especifica cómo se renderizan los elementos HTML &lt;p&gt; al cargar HTML. El valor predeterminado es Normal.(Hereda de [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [ParagraphLayoutMode](../../aspose.cells/htmlloadoptions/paragraphlayoutmode/) { get; set; } | Especifica cómo se renderizan los elementos HTML &lt;p&gt; al cargar HTML. El valor predeterminado es Normal.(Hereda de [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Indica si se analiza la fórmula al leer el archivo. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Indica si se analizan los registros en caché de pivote al cargar el archivo. El valor predeterminado es false. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Obtiene y establece la contraseña del libro de trabajo. (Hereda de [`LoadOptions`](../loadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Indica si se conservan esos espacios y saltos de línea que se rellenan entre los tokens de fórmula al obtener y establecer fórmulas. El valor predeterminado es false.(Heredado de [`LoadOptions`](../loadoptions/).) |
| [ProgId](../../aspose.cells/htmlloadoptions/progid/) { get; } | Obtiene el id del programa al crear el archivo. Solo para archivos MHT.(Hereda de [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Obtiene o establece la configuración regional utilizada para el Workbook que se cargará.(Hereda de [`LoadOptions`](../loadoptions/).) |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsoleto.**) Establece el nombre de fuente estándar predeterminado(Heredado de [`LoadOptions`](../loadoptions/).) |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsoleto.**) Establece el tamaño de fuente estándar predeterminado.(Heredado de [`LoadOptions`](../loadoptions/).) |
| [StreamProvider](../../aspose.cells/htmlloadoptions/streamprovider/) { get; set; } | Obtiene o establece el StreamProviderImportHtmlFile para importar objetos.(Hereda de [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [SupportDivTag](../../aspose.cells/htmlloadoptions/supportdivtag/) { get; set; } | Indica si se admite el diseño de la etiqueta `<div>` cuando el archivo html la contiene. El valor predeterminado es false.(Hereda de [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [TableLoadOptions](../../aspose.cells/htmlloadoptions/tableloadoptions/) { get; } | Obtenga la instancia de HtmlTableLoadOptionCollection (Hereda de [`HtmlLoadOptions`](../htmlloadoptions/).) |
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
    using System.IO;
    using System.Text;

    public class EbookLoadOptionsDemo
    {
        public static void EbookLoadOptionsExample()
        {
            // Cree una instancia de EbookLoadOptions
            EbookLoadOptions options = new EbookLoadOptions();

            // Estableciendo propiedades
            options.AttachedFilesDirectory = "C:\\AttachedFiles";
            options.LoadFormulas = true;
            options.SupportDivTag = true;
            options.DeleteRedundantSpaces = true;
            options.AutoFitColsAndRows = true;
            options.ConvertFormulasData = true;
            options.HasFormula = true;
            options.Encoding = Encoding.UTF8;
            options.LoadStyleStrategy = TxtLoadStyleStrategy.None;
            options.ConvertNumericData = true;
            options.ConvertDateTimeData = true;
            options.KeepPrecision = true;
            options.Password = "password";
            options.ParsingFormulaOnOpen = true;
            options.ParsingPivotCachedRecords = true;
            options.LanguageCode = CountryCode.USA;
            options.Region = CountryCode.USA;
            options.CultureInfo = new System.Globalization.CultureInfo("en-US");
            options.StandardFont = "Arial";
            options.StandardFontSize = 12.0;
            options.InterruptMonitor = null; // Assuming no interrupt monitor is set
            options.IgnoreNotPrinted = true;
            options.CheckDataValid = true;
            options.CheckExcelRestriction = true;
            options.KeepUnparsedData = true;
            options.LoadFilter = new LoadFilter();
            options.LightCellsDataHandler = null; // Assuming no light cells data handler is set
            options.MemorySetting = MemorySetting.Normal;
            options.WarningCallback = null; // Assuming no warning callback is set
            options.AutoFitterOptions = new AutoFitterOptions();
            options.AutoFilter = true;
            options.FontConfigs = new IndividualFontConfigs();
            options.IgnoreUselessShapes = true;
            options.PreservePaddingSpacesInFormula = true;

            // Cargue un archivo ebook en un Workbook usando las opciones especificadas
            Workbook workbook = new Workbook("EbookLoadOptionsExample_original.ebook", options);

            // Guarda el libro de trabajo en un archivo Excel
            workbook.Save("EbookLoadOptionsExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* class [HtmlLoadOptions](../htmlloadoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


