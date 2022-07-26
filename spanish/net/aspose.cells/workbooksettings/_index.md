---
title: WorkbookSettings
second_title: Referencia de API de Aspose.Cells para .NET
description: Representa todas las configuraciones del libro.
type: docs
weight: 6500
url: /es/net/aspose.cells/workbooksettings/
---
## WorkbookSettings class

Representa todas las configuraciones del libro.

```csharp
public class WorkbookSettings : IDisposable
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Author](../../aspose.cells/workbooksettings/author) { get; set; } | Obtiene y establece el autor del archivo. |
| [AutoCompressPictures](../../aspose.cells/workbooksettings/autocompresspictures) { get; set; } | Especifica un valor booleano que indica que la aplicación comprimió automáticamente las imágenes del libro. |
| [AutoRecover](../../aspose.cells/workbooksettings/autorecover) { get; set; } | Indica si el archivo está marcado para recuperación automática. |
| [BuildVersion](../../aspose.cells/workbooksettings/buildversion) { get; set; } | Especifica la versión pública incremental de la aplicación. |
| [CheckCompatibility](../../aspose.cells/workbooksettings/checkcompatibility) { get; set; } | Indica si se comprueba la compatibilidad con versiones anteriores al guardar el libro de trabajo. |
| [CheckCustomNumberFormat](../../aspose.cells/workbooksettings/checkcustomnumberformat) { get; set; } | Indica si se verifica el formato de número personalizado al configurar Style.Custom. |
| [CheckExcelRestriction](../../aspose.cells/workbooksettings/checkexcelrestriction) { get; set; } | Si verifica la restricción del archivo de Excel cuando el usuario modifica los objetos relacionados con las celdas. Por ejemplo, Excel no permite ingresar un valor de cadena mayor a 32K. Cuando ingresa un valor mayor a 32K como por Cell.PutValue(cadena), si esto es verdadera, obtendrá una excepción. Si esta propiedad es falsa, aceptaremos su valor de cadena de entrada como el valor de la celda para que luego pueda generar el valor de cadena completo para otros formatos de archivo como CSV. Sin embargo, si ha establecido un tipo de valor que no es válido para el formato de archivo de Excel, , no debe guardar el libro de trabajo como formato de archivo de Excel más adelante. De lo contrario, puede haber un error inesperado para el archivo de Excel generado. |
| [Compliance](../../aspose.cells/workbooksettings/compliance) { get; set; } | Especifica la versión OOXML del documento de salida. El valor predeterminado es Ecma376_2006. |
| [CrashSave](../../aspose.cells/workbooksettings/crashsave) { get; set; } | indica si la aplicación guardó por última vez el archivo del libro de trabajo después de un bloqueo. |
| [CultureInfo](../../aspose.cells/workbooksettings/cultureinfo) { get; set; } | Obtiene o establece la cultura del sistema info. |
| [DataExtractLoad](../../aspose.cells/workbooksettings/dataextractload) { get; set; } | indica si la aplicación abrió por última vez el libro de trabajo para la recuperación de datos. |
| [Date1904](../../aspose.cells/workbooksettings/date1904) { get; set; } | Obtiene o establece un valor que representa si el libro de trabajo usa el sistema de fechas de 1904. |
| [DisplayDrawingObjects](../../aspose.cells/workbooksettings/displaydrawingobjects) { get; set; } | Indica si y cómo mostrar objetos en el libro de trabajo. |
| [EnableMacros](../../aspose.cells/workbooksettings/enablemacros) { get; set; } | Habilitar macros; |
| [FirstVisibleTab](../../aspose.cells/workbooksettings/firstvisibletab) { get; set; } | Obtiene o establece la primera pestaña visible de la hoja de cálculo. |
| [FormulaSettings](../../aspose.cells/workbooksettings/formulasettings) { get; } | Obtiene la configuración de las funciones relacionadas con fórmulas. |
| [GlobalizationSettings](../../aspose.cells/workbooksettings/globalizationsettings) { get; set; } | Obtiene y establece la configuración de globalización. |
| [HidePivotFieldList](../../aspose.cells/workbooksettings/hidepivotfieldlist) { get; set; } | Obtiene y establece si ocultar la lista de campos para la tabla dinámica. |
| [IsDefaultEncrypted](../../aspose.cells/workbooksettings/isdefaultencrypted) { get; set; } | Indica si cifrar el libro de trabajo con la contraseña predeterminada si la estructura y las ventanas del libro de trabajo están bloqueadas. |
| [IsEncrypted](../../aspose.cells/workbooksettings/isencrypted) { get; } | Obtiene un valor que indica si se requiere una contraseña para abrir este libro. |
| [IsHidden](../../aspose.cells/workbooksettings/ishidden) { get; set; } | Indica si este libro está oculto. |
| [IsHScrollBarVisible](../../aspose.cells/workbooksettings/ishscrollbarvisible) { get; set; } | Obtiene o establece un valor que indica si la hoja de cálculo generada contendrá una barra de desplazamiento horizontal. |
| [IsMinimized](../../aspose.cells/workbooksettings/isminimized) { get; set; } | Representa si la hoja de cálculo generada se abrirá Minimizada. |
| [IsProtected](../../aspose.cells/workbooksettings/isprotected) { get; } | Obtiene un valor que indica si la estructura o ventana del Workbook está protegida. |
| [IsVScrollBarVisible](../../aspose.cells/workbooksettings/isvscrollbarvisible) { get; set; } | Obtiene o establece un valor que indica si la hoja de cálculo generada contendrá una barra de desplazamiento vertical. |
| [LanguageCode](../../aspose.cells/workbooksettings/languagecode) { get; set; } | Obtiene o establece el idioma de la interfaz de usuario de la versión del libro de trabajo según el código de país que guardó el archivo. |
| [MaxColumn](../../aspose.cells/workbooksettings/maxcolumn) { get; } | Obtiene el índice de columna máximo, basado en cero. |
| [MaxRow](../../aspose.cells/workbooksettings/maxrow) { get; } | Obtiene el índice de fila máximo, basado en cero. |
| [MaxRowsOfSharedFormula](../../aspose.cells/workbooksettings/maxrowsofsharedformula) { get; set; } | Obtiene y establece el número máximo de filas de la fórmula compartida. |
| [MemorySetting](../../aspose.cells/workbooksettings/memorysetting) { get; set; } | Obtiene o establece las opciones de uso de memoria. La nueva opción se tomará como la opción predeterminada para las hojas de trabajo recién creadas, pero no tendrá efecto para las hojas de trabajo existentes. |
| [NumberDecimalSeparator](../../aspose.cells/workbooksettings/numberdecimalseparator) { get; set; } | Obtiene o establece el separador decimal para formatear/analizar valores numéricos. El valor predeterminado es el separador decimal de la Región actual. |
| [NumberGroupSeparator](../../aspose.cells/workbooksettings/numbergroupseparator) { get; set; } | Obtiene o establece el carácter que separa grupos de dígitos a la izquierda del decimal en valores numéricos. El valor predeterminado es el separador de grupo de la Región actual. |
| [PaperSize](../../aspose.cells/workbooksettings/papersize) { get; set; } | Obtiene y establece el tamaño de papel de impresión predeterminado. |
| [Password](../../aspose.cells/workbooksettings/password) { get; set; } | Representa la contraseña de cifrado del archivo del libro de trabajo. |
| [ProtectionType](../../aspose.cells/workbooksettings/protectiontype) { get; } | Obtiene el tipo de protección del libro. |
| [QuotePrefixToStyle](../../aspose.cells/workbooksettings/quoteprefixtostyle) { get; set; } | Indica si el ajuste[`QuotePrefix`](../style/quoteprefix) propiedad al ingresar el valor de la cadena (que comienza con una comilla simple) en la celda |
| [Region](../../aspose.cells/workbooksettings/region) { get; set; } | Obtiene o establece la configuración regional para el libro de trabajo. |
| [RemovePersonalInformation](../../aspose.cells/workbooksettings/removepersonalinformation) { get; set; } | Verdadero si la información personal se puede eliminar del libro de trabajo especificado. |
| [RepairLoad](../../aspose.cells/workbooksettings/repairload) { get; set; } | Indica si la aplicación abrió por última vez el libro en modo seguro o de reparación. |
| [ResourceProvider](../../aspose.cells/workbooksettings/resourceprovider) { get; set; } | Obtiene y establece el proveedor de flujo para un recurso externo, como cargar datos de imagen para una imagen de tipo "LinkToFile". |
| [Shared](../../aspose.cells/workbooksettings/shared) { get; set; } | Obtiene o establece un valor que indica si el libro de trabajo está compartido. |
| [SheetTabBarWidth](../../aspose.cells/workbooksettings/sheettabbarwidth) { get; set; } | Ancho de la barra de pestañas de la hoja de trabajo (en 1/1000 del ancho de la ventana). |
| [ShowTabs](../../aspose.cells/workbooksettings/showtabs) { get; set; } | Obtener o establecer un valor si se muestran las pestañas del Libro de trabajo. |
| [SignificantDigits](../../aspose.cells/workbooksettings/significantdigits) { get; set; } | Obtiene y establece el número de dígitos significativos. El valor predeterminado es[`SignificantDigits`](../cellshelper/significantdigits) . |
| [UpdateAdjacentCellsBorder](../../aspose.cells/workbooksettings/updateadjacentcellsborder) { get; set; } | Indica si actualizar el borde de las celdas adyacentes. |
| [UpdateLinksType](../../aspose.cells/workbooksettings/updatelinkstype) { get; set; } | Obtiene y establece cómo se actualizan los enlaces externos cuando se abre el libro. |
| [WarningCallback](../../aspose.cells/workbooksettings/warningcallback) { get; set; } | Obtiene o establece la devolución de llamada de advertencia. |
| [WindowHeight](../../aspose.cells/workbooksettings/windowheight) { get; set; } | La altura de la ventana, en unidad de punto. |
| [WindowHeightCM](../../aspose.cells/workbooksettings/windowheightcm) { get; set; } | La altura de la ventana, en unidades de centímetro. |
| [WindowHeightInch](../../aspose.cells/workbooksettings/windowheightinch) { get; set; } | La altura de la ventana, en unidades de pulgada. |
| [WindowLeft](../../aspose.cells/workbooksettings/windowleft) { get; set; } | La distancia desde el borde izquierdo del área del cliente hasta el borde izquierdo de la ventana, en unidades de punto. |
| [WindowLeftCM](../../aspose.cells/workbooksettings/windowleftcm) { get; set; } | La distancia desde el borde izquierdo del área del cliente hasta el borde izquierdo de la ventana. En unidades de centímetro. |
| [WindowLeftInch](../../aspose.cells/workbooksettings/windowleftinch) { get; set; } | La distancia desde el borde izquierdo del área del cliente hasta el borde izquierdo de la ventana. En unidades de pulgada. |
| [WindowTop](../../aspose.cells/workbooksettings/windowtop) { get; set; } | La distancia desde el borde superior del área del cliente hasta el borde superior de la ventana, en unidades de punto. |
| [WindowTopCM](../../aspose.cells/workbooksettings/windowtopcm) { get; set; } | La distancia desde el borde superior del área del cliente hasta el borde superior de la ventana, en unidades de centímetro. |
| [WindowTopInch](../../aspose.cells/workbooksettings/windowtopinch) { get; set; } | La distancia desde el borde superior del área del cliente hasta el borde superior de la ventana, en unidades de pulgada. |
| [WindowWidth](../../aspose.cells/workbooksettings/windowwidth) { get; set; } | El ancho de la ventana, en unidades de punto. |
| [WindowWidthCM](../../aspose.cells/workbooksettings/windowwidthcm) { get; set; } | El ancho de la ventana, en unidades de centímetro. |
| [WindowWidthInch](../../aspose.cells/workbooksettings/windowwidthinch) { get; set; } | El ancho de la ventana, en unidades de pulgada. |
| [WriteProtection](../../aspose.cells/workbooksettings/writeprotection) { get; } | Proporciona acceso a las opciones de protección contra escritura del libro. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Dispose](../../aspose.cells/workbooksettings/dispose)() | Libera recursos. |
| [GetThemeFont](../../aspose.cells/workbooksettings/getthemefont)(FontSchemeType) | Obtiene el nombre de fuente del tema predeterminado. |
| [SetPageOrientationType](../../aspose.cells/workbooksettings/setpageorientationtype)(PageOrientationType) | Establecer el tipo de orientación de impresión para todo el libro. |

### Ejemplos

```csharp
[C#]

Workbook workbook = new Workbook();

WorkbookSettings settings = workbook.Settings;

//haz tu negocio

[Visual Basic]
Dim workbook as Workbook = new Workbook()

Dim settings as WorkbookSettings = workbook.Settings

'haz tu negocio
```

### Ver también

* espacio de nombres [Aspose.Cells](../../aspose.cells)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
