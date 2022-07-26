---
title: AbstractTextLoadOptions
second_title: Referencia de API de Aspose.Cells para .NET
description: Opciones comunes para cargar valores de texto
type: docs
weight: 60
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
| [AutoFilter](../../aspose.cells/loadoptions/autofilter) { get; set; } | Indica si se filtran automáticamente los datos al cargar los archivos. |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions) { get; set; } | Obtiene y establece las opciones de ajuste automático |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid) { get; set; } | Comprobar si los datos son válidos en el archivo de plantilla. |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction) { get; set; } | Si verifica la restricción del archivo de Excel cuando el usuario modifica los objetos relacionados con las celdas. Por ejemplo, Excel no permite ingresar un valor de cadena mayor a 32K. Cuando ingresa un valor mayor a 32K como por Cell.PutValue(cadena), si esto es verdadera, obtendrá una excepción. Si esta propiedad es falsa, aceptaremos su valor de cadena de entrada como el valor de la celda para que luego pueda generar el valor de cadena completo para otros formatos de archivo como CSV. Sin embargo, si ha establecido un tipo de valor que no es válido para el formato de archivo de Excel, , no debe guardar el libro de trabajo como formato de archivo de Excel más adelante. De lo contrario, puede haber un error inesperado para el archivo de Excel generado. |
| [ConvertDateTimeData](../../aspose.cells/abstracttextloadoptions/convertdatetimedata) { get; set; } | Obtiene o establece un valor que indica si la cadena del archivo de texto se convierte en datos de fecha. |
| [ConvertNumericData](../../aspose.cells/abstracttextloadoptions/convertnumericdata) { get; set; } | Obtiene o establece un valor que indica si la cadena del archivo de texto se convierte en datos numéricos. |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo) { get; set; } | Obtiene o establece la información cultural del sistema en el momento en que se cargó el archivo. |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings) { get; } | Obtiene la configuración de estilo predeterminada para inicializar estilos del libro de trabajo |
| [Encoding](../../aspose.cells/abstracttextloadoptions/encoding) { get; set; } | Obtiene y establece la codificación predeterminada. Solo aplica para archivo csv. |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs) { get; set; } | Obtiene y establece configuraciones de fuentes individuales. Solo funciona para el[`Workbook`](../workbook) que usa esto[`LoadOptions`](../loadoptions) para cargar.&gt; |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted) { get; set; } | Ignora los datos que no se imprimen si se imprime directamente el archivo |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor) { get; set; } | Obtiene y establece el monitor de interrupción. |
| [KeepPrecision](../../aspose.cells/abstracttextloadoptions/keepprecision) { get; set; } | Indica si no se analiza un valor de cadena si la longitud es 15. |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata) { get; set; } | Si se mantienen los datos no analizados en la memoria para el libro de trabajo cuando se carga desde un archivo de plantilla. El valor predeterminado es verdadero. |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode) { get; set; } | Obtiene o establece el idioma de la interfaz de usuario de la versión del libro de trabajo según el código de país que guardó el archivo. |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler) { get; set; } | El controlador de datos para procesar datos de celdas al leer el archivo de plantilla. |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter) { get; set; } | El filtro para indicar cómo cargar datos. |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat) { get; } | Obtiene el formato de carga. |
| [LoadStyleStrategy](../../aspose.cells/abstracttextloadoptions/loadstylestrategy) { get; set; } | Indica la estrategia para aplicar estilo a los valores analizados al convertir un valor de cadena en un número o una fecha y hora. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting) { get; set; } | Obtiene o establece las opciones de uso de memoria. |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen) { get; set; } | Indica si analiza la fórmula al leer el archivo. |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords) { get; set; } | Indica si se están analizando los registros almacenados en caché dinámica al cargar el archivo. El valor predeterminado es falso. |
| [Password](../../aspose.cells/loadoptions/password) { get; set; } | Obtiene y establece la contraseña del libro de trabajo. |
| [Region](../../aspose.cells/loadoptions/region) { get; set; } | Obtiene o establece la configuración regional del sistema según el código de país en el momento en que se cargó el archivo. |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback) { get; set; } | Obtiene o establece la devolución de llamada de advertencia. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize)(PaperSizeType) | Establece el tamaño de papel de impresión predeterminado a partir de la configuración predeterminada de la impresora. |

### Ver también

* class [LoadOptions](../loadoptions)
* espacio de nombres [Aspose.Cells](../../aspose.cells)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
