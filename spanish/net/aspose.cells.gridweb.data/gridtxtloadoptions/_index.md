---
title: "Clase GridTxtLoadOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.GridWeb.Data.GridTxtLoadOptions. Representa las opciones para cargar un archivo de texto."
type: docs
url: /es/net/aspose.cells.gridweb.data/gridtxtloadoptions/
---
## GridTxtLoadOptions class

Representa las opciones para cargar un archivo de texto.

```csharp
[Obsolete("This class will be obsoleted after stand alone dll usage of cells public api,instead you can use Aspose.Cells.TxtLoadOptions ")]
public class GridTxtLoadOptions : GridLoadOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [GridTxtLoadOptions](gridtxtloadoptions/)() | Crea las opciones para cargar un archivo de texto. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AutoFilter](../../aspose.cells.gridweb.data/gridloadoptions/autofilter/) { get; set; } | Indica si se filtra automáticamente los datos al cargar los archivos. (Hereda de [`GridLoadOptions`](../gridloadoptions/).) |
| [CheckDataValid](../../aspose.cells.gridweb.data/gridloadoptions/checkdatavalid/) { get; set; } | Comprueba si los datos son válidos en el archivo de plantilla. (Hereda de [`GridLoadOptions`](../gridloadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells.gridweb.data/gridloadoptions/checkexcelrestriction/) { get; set; } | Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, Excel no permite introducir un valor de cadena mayor a 32 K. Cuando introduce un valor mayor a 32 K, como mediante Cell.PutValue(string), si esta propiedad es verdadera, obtendrá una Exception. Si la propiedad es falsa, aceptaremos su cadena de entrada como el valor de la celda, de modo que luego pueda exportar la cadena completa a otros formatos de archivo como CSV. Sin embargo, si ha establecido un valor que no es válido para el formato de archivo Excel, no debe guardar el libro de trabajo como formato Excel posteriormente. De lo contrario, podrían producirse errores inesperados en el archivo Excel generado. (Hereda de [`GridLoadOptions`](../gridloadoptions/).) |
| [ConvertDateTimeData](../../aspose.cells.gridweb.data/gridtxtloadoptions/convertdatetimedata/) { get; set; } | Obtiene o establece un valor que indica si la cadena en el archivo de texto se convierte a datos de fecha. |
| [ConvertNumericData](../../aspose.cells.gridweb.data/gridtxtloadoptions/convertnumericdata/) { get; set; } | Obtiene o establece un valor que indica si la cadena en el archivo de texto se convierte a datos numéricos. |
| [Encoding](../../aspose.cells.gridweb.data/gridtxtloadoptions/encoding/) { get; set; } | Obtiene y establece la codificación predeterminada. Solo se aplica a archivos csv. |
| [ExtendToNextSheet](../../aspose.cells.gridweb.data/gridtxtloadoptions/extendtonextsheet/) { get; set; } | Indica si se extienden los datos a la hoja siguiente cuando las filas o columnas de datos superan el límite. Si esta propiedad es verdadera, los datos adicionales se extenderán a la hoja siguiente detrás de la actual (si la hoja actual es la última, se añadirá una nueva hoja al libro de trabajo). Si la propiedad es falsa, los datos que superen el límite se ignorarán. El valor predeterminado es false; |
| [HasFormula](../../aspose.cells.gridweb.data/gridtxtloadoptions/hasformula/) { get; set; } | Indica si el texto es una fórmula si comienza con "=". |
| [HasTextQualifier](../../aspose.cells.gridweb.data/gridtxtloadoptions/hastextqualifier/) { get; set; } | Indica si hay calificador de texto para el valor de la celda. El valor predeterminado es verdadero. |
| [IgnoreNotPrinted](../../aspose.cells.gridweb.data/gridloadoptions/ignorenotprinted/) { get; set; } | Ignora los datos que no se imprimen si se imprime directamente el archivo (Hereda de [`GridLoadOptions`](../gridloadoptions/).) |
| [IsMultiEncoded](../../aspose.cells.gridweb.data/gridtxtloadoptions/ismultiencoded/) { get; set; } | Verdadero indica que el archivo contiene varias codificaciones. |
| [KeepPrecision](../../aspose.cells.gridweb.data/gridtxtloadoptions/keepprecision/) { get; set; } | Indica si no se analiza un valor de cadena cuando la longitud es 15. |
| [KeepUnparsedData](../../aspose.cells.gridweb.data/gridloadoptions/keepunparseddata/) { get; set; } | Indica si se mantiene los datos no analizados en memoria para el Workbook cuando se carga desde un archivo de plantilla. El valor predeterminado es true. (Hereda de [`GridLoadOptions`](../gridloadoptions/).) |
| [OnlyAuto](../../aspose.cells.gridweb.data/gridloadoptions/onlyauto/) { get; set; } | Indica si solo se ajustan las filas cuya altura no está personalizada. (Hereda de [`GridLoadOptions`](../gridloadoptions/).) |
| [ParsingFormulaOnOpen](../../aspose.cells.gridweb.data/gridloadoptions/parsingformulaonopen/) { get; set; } | Indica si se analiza la fórmula al leer el archivo. (Hereda de [`GridLoadOptions`](../gridloadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells.gridweb.data/gridloadoptions/parsingpivotcachedrecords/) { get; set; } | Indica si se analizan los registros en caché de la tabla dinámica al cargar el archivo. El valor predeterminado es false. (Hereda de [`GridLoadOptions`](../gridloadoptions/).) |
| [Password](../../aspose.cells.gridweb.data/gridloadoptions/password/) { get; set; } | Obtiene y establece la contraseña del libro de trabajo. (Hereda de [`GridLoadOptions`](../gridloadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells.gridweb.data/gridloadoptions/preservepaddingspacesinformula/) { get; set; } | Indica si se conservan los espacios y saltos de línea que se insertan entre los tokens de la fórmula al obtener y establecer fórmulas. El valor predeterminado es false. (Hereda de [`GridLoadOptions`](../gridloadoptions/).) |
| [Separator](../../aspose.cells.gridweb.data/gridtxtloadoptions/separator/) { get; set; } | Obtiene y establece el separador de caracteres del archivo de texto. |
| [SeparatorString](../../aspose.cells.gridweb.data/gridtxtloadoptions/separatorstring/) { get; set; } | Obtiene y establece un valor de cadena como separador. |
| [TextQualifier](../../aspose.cells.gridweb.data/gridtxtloadoptions/textqualifier/) { get; set; } | Especifica el calificador de texto para los valores de celda. El calificador predeterminado es '\"'. |
| [TreatConsecutiveDelimitersAsOne](../../aspose.cells.gridweb.data/gridtxtloadoptions/treatconsecutivedelimitersasone/) { get; set; } | Indica si los delimitadores consecutivos deben tratarse como uno. |
| [TreatQuotePrefixAsValue](../../aspose.cells.gridweb.data/gridtxtloadoptions/treatquoteprefixasvalue/) { get; set; } | Indica si el signo de comilla simple inicial debe tomarse como parte del valor de una celda. El valor predeterminado es true. Si es false, la comilla simple inicial se eliminará del valor de la celda correspondiente y [`QuotePrefix`](../../aspose.cells.gridweb/gridtableitemstyle/quoteprefix/) se establecerá como true para la celda. |

### Ver también

* class [GridLoadOptions](../gridloadoptions/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


