---
title: "Clase WorkbookSettings"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.WorkbookSettings. Representa todas las configuraciones del libro de trabajo"
type: docs
url: /es/net/aspose.cells/workbooksettings/
---
## WorkbookSettings class

Representa todas las configuraciones del libro de trabajo.

```csharp
public class WorkbookSettings : IDisposable
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Author](../../aspose.cells/workbooksettings/author/) { get; set; } | Obtiene y establece el autor del archivo. |
| [AutoCompressPictures](../../aspose.cells/workbooksettings/autocompresspictures/) { get; set; } | Especifica un valor booleano que indica que la aplicación comprime automáticamente las imágenes en el libro de trabajo. |
| [AutoRecover](../../aspose.cells/workbooksettings/autorecover/) { get; set; } | Indica si el archivo está marcado para recuperación automática. |
| [BuildVersion](../../aspose.cells/workbooksettings/buildversion/) { get; set; } | Especifica la versión incremental pública de la aplicación. |
| [CheckCompatibility](../../aspose.cells/workbooksettings/checkcompatibility/) { get; set; } | Indica si se verifica la compatibilidad con versiones anteriores al guardar el libro. |
| [CheckCustomNumberFormat](../../aspose.cells/workbooksettings/checkcustomnumberformat/) { get; set; } | Indica si se verifica el formato numérico personalizado al establecer Style.Custom. |
| [CheckExcelRestriction](../../aspose.cells/workbooksettings/checkexcelrestriction/) { get; set; } | Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, Excel no permite introducir un valor de cadena superior a 32 K. Cuando introduces un valor superior a 32 K, como mediante Cell.PutValue(string), si esta propiedad es verdadera, obtendrás una excepción. Si esta propiedad es falsa, aceptaremos la cadena introducida como el valor de la celda, de modo que posteriormente puedas exportar la cadena completa a otros formatos de archivo como CSV. Sin embargo, si has establecido un valor que no es válido para el formato de archivo Excel, no deberías guardar el libro posteriormente en formato Excel. De lo contrario, podría producirse un error inesperado en el archivo Excel generado. |
| [Compliance](../../aspose.cells/workbooksettings/compliance/) { get; set; } | Especifica la versión OOXML para el documento de salida. El valor predeterminado es Ecma376_2006. |
| [CrashSave](../../aspose.cells/workbooksettings/crashsave/) { get; set; } | Indica si la aplicación guardó por última vez el archivo del libro después de un bloqueo. |
| [CultureInfo](../../aspose.cells/workbooksettings/cultureinfo/) { get; set; } | Obtiene o establece la información de cultura del sistema. |
| [DataExtractLoad](../../aspose.cells/workbooksettings/dataextractload/) { get; set; } | Indica si la aplicación abrió por última vez el libro para recuperación de datos. |
| [Date1904](../../aspose.cells/workbooksettings/date1904/) { get; set; } | Obtiene o establece un valor que indica si el libro usa el sistema de fechas 1904. |
| [DefaultImageResolution](../../aspose.cells/workbooksettings/defaultimageresolution/) { get; set; } | Obtiene y establece la resolución predeterminada de la imagen. |
| [DefaultStyleSettings](../../aspose.cells/workbooksettings/defaultstylesettings/) { get; } | Obtiene la configuración de los valores predeterminados de las propiedades relacionadas con estilos para este libro. |
| [DiscardImageEditData](../../aspose.cells/workbooksettings/discardimageeditdata/) { get; set; } | Indica si se descarta la edición de datos de imagen. |
| [DisplayDrawingObjects](../../aspose.cells/workbooksettings/displaydrawingobjects/) { get; set; } | Indica si y cómo mostrar objetos en el libro. |
| [EnableMacros](../../aspose.cells/workbooksettings/enablemacros/) { get; set; } | Habilitar macros; |
| [FirstVisibleTab](../../aspose.cells/workbooksettings/firstvisibletab/) { get; set; } | Obtiene o establece la primera pestaña de hoja visible. |
| [FormulaSettings](../../aspose.cells/workbooksettings/formulasettings/) { get; } | Obtiene la configuración de las funciones relacionadas con fórmulas. |
| [GlobalizationSettings](../../aspose.cells/workbooksettings/globalizationsettings/) { get; set; } | Obtiene y establece la configuración de globalización. |
| [HidePivotFieldList](../../aspose.cells/workbooksettings/hidepivotfieldlist/) { get; set; } | Obtiene y establece si se oculta la lista de campos para la tabla dinámica. |
| [IsDefaultEncrypted](../../aspose.cells/workbooksettings/isdefaultencrypted/) { get; set; } | Indica si se cifra el libro con la contraseña predeterminada cuando la estructura y las ventanas del libro están bloqueadas. |
| [IsEncrypted](../../aspose.cells/workbooksettings/isencrypted/) { get; } | Obtiene un valor que indica si se requiere una contraseña para abrir este libro. |
| [IsHidden](../../aspose.cells/workbooksettings/ishidden/) { get; set; } | Indica si este libro está oculto. |
| [IsHScrollBarVisible](../../aspose.cells/workbooksettings/ishscrollbarvisible/) { get; set; } | Obtiene o establece un valor que indica si la hoja de cálculo generada contendrá una barra de desplazamiento horizontal. |
| [IsMinimized](../../aspose.cells/workbooksettings/isminimized/) { get; set; } | Representa si la hoja de cálculo generada se abrirá minimizada. |
| [IsProtected](../../aspose.cells/workbooksettings/isprotected/) { get; } | Obtiene un valor que indica si la estructura o la ventana del libro están protegidas. |
| [IsVScrollBarVisible](../../aspose.cells/workbooksettings/isvscrollbarvisible/) { get; set; } | Obtiene o establece un valor que indica si la hoja de cálculo generada contendrá una barra de desplazamiento vertical. |
| [LanguageCode](../../aspose.cells/workbooksettings/languagecode/) { get; set; } | Obtiene o establece el idioma de la interfaz de usuario de la versión del Workbook basado en CountryCode que ha guardado el archivo. |
| [MaxColumn](../../aspose.cells/workbooksettings/maxcolumn/) { get; } | Obtiene el índice máximo de columna, basado en cero. |
| [MaxRow](../../aspose.cells/workbooksettings/maxrow/) { get; } | Obtiene el índice máximo de fila, basado en cero. |
| [MaxRowsOfSharedFormula](../../aspose.cells/workbooksettings/maxrowsofsharedformula/) { get; set; } | Obtiene y establece el número máximo de fila de la fórmula compartida. |
| [MaxUniqueItemsPerField](../../aspose.cells/workbooksettings/maxuniqueitemsperfield/) { get; set; } | Obtiene y establece la limitación de elementos únicos por campo |
| [MemorySetting](../../aspose.cells/workbooksettings/memorysetting/) { get; set; } | Obtiene o establece las opciones de uso de memoria. La nueva opción se tomará como la opción predeterminada para las hojas de cálculo recién creadas, pero no tendrá efecto en las hojas de cálculo existentes. |
| [NumberDecimalSeparator](../../aspose.cells/workbooksettings/numberdecimalseparator/) { get; set; } | Obtiene o establece el separador decimal para formatear/analizar valores numéricos. El predeterminado es el separador decimal de la región actual. |
| [NumberGroupSeparator](../../aspose.cells/workbooksettings/numbergroupseparator/) { get; set; } | Obtiene o establece el carácter que separa grupos de dígitos a la izquierda del decimal en valores numéricos. El predeterminado es el separador de grupos de la región actual. |
| [PaperSize](../../aspose.cells/workbooksettings/papersize/) { get; set; } | Obtiene y establece el tamaño de papel de impresión predeterminado. |
| [Password](../../aspose.cells/workbooksettings/password/) { get; set; } | Representa la contraseña de cifrado del archivo Workbook. |
| [PropertiesFollowChartPoint](../../aspose.cells/workbooksettings/propertiesfollowchartpoint/) { get; set; } | Indica si las propiedades de los puntos de datos y las etiquetas de datos en todos los gráficos de este workbook siguen su referencia. |
| [ProtectionType](../../aspose.cells/workbooksettings/protectiontype/) { get; } | Obtiene el tipo de protección del workbook. |
| [QuotePrefixToStyle](../../aspose.cells/workbooksettings/quoteprefixtostyle/) { get; set; } | Indica si al establecer la propiedad [`QuotePrefix`](../style/quoteprefix/) al ingresar el valor de cadena (que comienza con una comilla simple) en la celda |
| [Region](../../aspose.cells/workbooksettings/region/) { get; set; } | Obtiene o establece la configuración regional para el workbook. |
| [RemovePersonalInformation](../../aspose.cells/workbooksettings/removepersonalinformation/) { get; set; } | Verdadero si la información personal puede eliminarse del workbook especificado. |
| [RepairLoad](../../aspose.cells/workbooksettings/repairload/) { get; set; } | Indica si la aplicación abrió por última vez el workbook en modo seguro o de reparación. |
| [ResourceProvider](../../aspose.cells/workbooksettings/resourceprovider/) { get; set; } | Obtiene y establece el proveedor de flujo para recursos externos, como cargar datos de imagen para una imagen de tipo "LinkToFile". |
| [ShapeDisplayType](../../aspose.cells/workbooksettings/shapedisplaytype/) { get; set; } | Obtiene y establece cómo la aplicación muestra las formas en este workbook |
| [Shared](../../aspose.cells/workbooksettings/shared/) { get; set; } | Obtiene o establece un valor que indica si el Workbook está compartido. |
| [SheetTabBarWidth](../../aspose.cells/workbooksettings/sheettabbarwidth/) { get; set; } | Ancho de la barra de pestañas de la hoja de cálculo (en 1/1000 del ancho de la ventana). |
| [ShowTabs](../../aspose.cells/workbooksettings/showtabs/) { get; set; } | Obtiene o establece un valor que indica si se muestran las pestañas del Workbook. |
| [SignificantDigits](../../aspose.cells/workbooksettings/significantdigits/) { get; set; } | (**Obsolete.**) Obtiene y establece el número de dígitos significativos. El valor predeterminado es [`SignificantDigits`](../cellshelper/significantdigits/). |
| [SignificantDigitsType](../../aspose.cells/workbooksettings/significantdigitstype/) { get; set; } | Obtiene y establece el tipo de dígitos significativos para la salida de valores numéricos en este workbook. El valor predeterminado es [`SignificantDigitsType`](../cellshelper/significantdigitstype/). |
| [SmartTagOptions](../../aspose.cells/workbooksettings/smarttagoptions/) { get; } | Obtiene las opciones de la etiqueta inteligente. |
| [StreamProvider](../../aspose.cells/workbooksettings/streamprovider/) { get; set; } | (**Obsolete.**) Obtiene y establece el proveedor de flujo para recursos externos. |
| [UpdateAdjacentCellsBorder](../../aspose.cells/workbooksettings/updateadjacentcellsborder/) { get; set; } | Indica si se actualiza el borde de las celdas adyacentes. |
| [UpdateLinksType](../../aspose.cells/workbooksettings/updatelinkstype/) { get; set; } | Obtiene y establece cómo se actualizan los enlaces externos cuando se abre el libro de trabajo. |
| [WarningCallback](../../aspose.cells/workbooksettings/warningcallback/) { get; set; } | Obtiene o establece la devolución de llamada de advertencia. |
| [WindowHeight](../../aspose.cells/workbooksettings/windowheight/) { get; set; } | La altura de la ventana, en unidades de punto. |
| [WindowHeightCM](../../aspose.cells/workbooksettings/windowheightcm/) { get; set; } | La altura de la ventana, en unidades de centímetro. |
| [WindowHeightInch](../../aspose.cells/workbooksettings/windowheightinch/) { get; set; } | La altura de la ventana, en unidades de pulgada. |
| [WindowLeft](../../aspose.cells/workbooksettings/windowleft/) { get; set; } | La distancia desde el borde izquierdo del área cliente hasta el borde izquierdo de la ventana, en unidades de punto. |
| [WindowLeftCM](../../aspose.cells/workbooksettings/windowleftcm/) { get; set; } | La distancia desde el borde izquierdo del área cliente hasta el borde izquierdo de la ventana. En unidades de centímetro. |
| [WindowLeftInch](../../aspose.cells/workbooksettings/windowleftinch/) { get; set; } | La distancia desde el borde izquierdo del área cliente hasta el borde izquierdo de la ventana. En unidades de pulgada. |
| [WindowTop](../../aspose.cells/workbooksettings/windowtop/) { get; set; } | La distancia desde el borde superior del área cliente hasta el borde superior de la ventana, en unidades de punto. |
| [WindowTopCM](../../aspose.cells/workbooksettings/windowtopcm/) { get; set; } | La distancia desde el borde superior del área cliente hasta el borde superior de la ventana, en unidades de centímetro. |
| [WindowTopInch](../../aspose.cells/workbooksettings/windowtopinch/) { get; set; } | La distancia desde el borde superior del área cliente hasta el borde superior de la ventana, en unidades de pulgada. |
| [WindowWidth](../../aspose.cells/workbooksettings/windowwidth/) { get; set; } | El ancho de la ventana, en unidades de punto. |
| [WindowWidthCM](../../aspose.cells/workbooksettings/windowwidthcm/) { get; set; } | El ancho de la ventana, en unidades de centímetro. |
| [WindowWidthInch](../../aspose.cells/workbooksettings/windowwidthinch/) { get; set; } | El ancho de la ventana, en unidades de pulgada. |
| [WpsCompatibility](../../aspose.cells/workbooksettings/wpscompatibility/) { get; set; } | Indica si es compatible con WPS. |
| [WriteProtection](../../aspose.cells/workbooksettings/writeprotection/) { get; } | Proporciona acceso a las opciones de protección contra escritura del libro de trabajo. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Dispose](../../aspose.cells/workbooksettings/dispose/)() | Libera recursos. |
| [GetThemeFont](../../aspose.cells/workbooksettings/getthemefont/)(FontSchemeType) | Obtiene el nombre de fuente predeterminado del tema. |
| [SetPageOrientationType](../../aspose.cells/workbooksettings/setpageorientationtype/)(PageOrientationType) | Establece el tipo de orientación de impresión para todo el libro de trabajo. |

### Ejemplos

```csharp
using Aspose.Cells;
using System;
using System.Globalization;

public class WorkbookSettingsDemo
{
    public static void RunDemo()
    {
        // Crear un nuevo libro de trabajo
        Workbook workbook = new Workbook();
        Worksheet sheet = workbook.Worksheets[0];

        // Agregar algunos datos de ejemplo
        sheet.Cells["A1"].PutValue("Sample Data");
        sheet.Cells["A2"].PutValue(123);
        sheet.Cells["A3"].PutValue(DateTime.Now);

        // Acceder a WorkbookSettings
        WorkbookSettings settings = workbook.Settings;

        // Establecer varias configuraciones
        settings.Author = "John Doe";
        settings.CheckCustomNumberFormat = true;
        settings.EnableMacros = false;
        settings.Date1904 = false;
        settings.DisplayDrawingObjects = DisplayDrawingObjects.DisplayShapes;
        settings.SheetTabBarWidth = 1000;
        settings.ShowTabs = true;
        settings.FirstVisibleTab = 0;
        settings.IsHScrollBarVisible = true;
        settings.IsVScrollBarVisible = true;
        settings.Shared = false;
        settings.LanguageCode = CountryCode.USA;
        settings.Region = CountryCode.USA;
        settings.CultureInfo = new CultureInfo("en-US");
        settings.GlobalizationSettings = new GlobalizationSettings();
        settings.NumberDecimalSeparator = '.';
        settings.NumberGroupSeparator = ',';
        settings.Password = "password123";
        settings.IsDefaultEncrypted = false;
        settings.IsMinimized = false;
        settings.IsHidden = false;
        settings.AutoCompressPictures = true;
        settings.RemovePersonalInformation = false;
        settings.HidePivotFieldList = false;
        settings.UpdateLinksType = UpdateLinksType.UserSet;
        settings.WindowLeft = 0;
        settings.WindowLeftInch = 0;
        settings.WindowLeftCM = 0;
        settings.WindowTop = 0;
        settings.WindowTopInch = 0;
        settings.WindowTopCM = 0;
        settings.WindowWidth = 800;
        settings.WindowWidthInch = 8;
        settings.WindowWidthCM = 20.32;
        settings.WindowHeight = 600;
        settings.WindowHeightInch = 6;
        settings.WindowHeightCM = 15.24;
        settings.UpdateAdjacentCellsBorder = true;
        settings.SignificantDigits = 15;
        settings.CheckCompatibility = true;
        settings.CheckExcelRestriction = true;
        settings.AutoRecover = true;
        settings.CrashSave = false;
        settings.DataExtractLoad = false;
        settings.RepairLoad = false;
        settings.BuildVersion = "1.0.0";
        settings.MemorySetting = MemorySetting.Normal;
        settings.PaperSize = PaperSizeType.PaperA4;
        settings.WarningCallback = null;
        settings.MaxRowsOfSharedFormula = 1048576;
        settings.Compliance = OoxmlCompliance.Ecma376_2006;
        settings.QuotePrefixToStyle = false;

        // Guarda el libro de trabajo
        workbook.Save("WorkbookSettingsDemo.xlsx");
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


