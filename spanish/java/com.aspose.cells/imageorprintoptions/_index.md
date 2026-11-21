---
title: "ImageOrPrintOptions"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Permite especificar opciones al renderizar la hoja de cálculo a imágenes, imprimir la hoja de cálculo o renderizar el gráfico a una imagen."
type: docs
url: /es/java/com.aspose.cells/imageorprintoptions/
---

**Inheritance:**
java.lang.Object
```
public class ImageOrPrintOptions
```

Permite especificar opciones al renderizar una hoja de cálculo a imágenes, imprimir la hoja de cálculo o renderizar un gráfico a imagen.

**Example**

```
         //Set Image Or Print Options
         ImageOrPrintOptions options = new ImageOrPrintOptions();
 
         //Set output image format
         options.setImageType(ImageType.PNG);
 
         //Set Horizontal resolution
         options.setHorizontalResolution(300);
 
         //Set Vertical Resolution
         options.setVerticalResolution(300);
 
         //Instantiate Workbook
         Workbook book = new Workbook("test.xls");
 
         //Save chart as Image using ImageOrPrint Options
         book.getWorksheets().get(0).getCharts().get(0).toImage("chart.png", options);
```
## Constructores

| Constructor | Descripción |
| --- | --- |
| [ImageOrPrintOptions()](#ImageOrPrintOptions--) | Ctor. |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllColumnsInOnePagePerSheet()](#getAllColumnsInOnePagePerSheet--) | Si AllColumnsInOnePagePerSheet es true, todo el contenido de columnas de una hoja se exportará a una sola página en el resultado. |
| [getChartImageType()](#getChartImageType--) | Indique el tipo de imagen del gráfico al convertir. |
| [getCheckWorkbookDefaultFont()](#getCheckWorkbookDefaultFont--) | Cuando los caracteres en Excel son Unicode y no se establece la fuente correcta en el estilo de celda, pueden aparecer como bloques en pdf, imagen. |
| [getClass()](#getClass--) |  |
| [getCustomRenderSettings()](#getCustomRenderSettings--) | Obtiene configuraciones personalizadas durante el renderizado. |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | Obtiene el idioma de edición predeterminado. |
| [getDefaultFont()](#getDefaultFont--) | Cuando los caracteres en Excel son Unicode y no se establece la fuente correcta en el estilo de celda, pueden aparecer como bloques en pdf, imagen. |
| [getDrawObjectEventHandler()](#getDrawObjectEventHandler--) | Implemente esta interfaz para obtener DrawObject y Bound durante la renderización. |
| [getEmbededImageNameInSvg()](#getEmbededImageNameInSvg--) | Indique el nombre de archivo de la imagen incrustada en svg. |
| [getEmfRenderSetting()](#getEmfRenderSetting--) | Configuración para renderizar metarchivos Emf en el archivo fuente. |
| [getGridlineColor()](#getGridlineColor--) | Obtiene el color de la línea de cuadrícula. |
| [getGridlineType()](#getGridlineType--) | Obtiene el tipo de línea de cuadrícula. |
| [getHorizontalResolution()](#getHorizontalResolution--) | Obtiene la resolución horizontal para las imágenes generadas, en puntos por pulgada. |
| [getImageType()](#getImageType--) | Obtiene el formato de las imágenes generadas. |
| [getOnePagePerSheet()](#getOnePagePerSheet--) | Si OnePagePerSheet es true, todo el contenido de una hoja se exportará a una sola página en el resultado. |
| [getOnlyArea()](#getOnlyArea--) | Si esta propiedad es verdadera, se generará una Área, y no se aplicará escala. |
| [getOutputBlankPageWhenNothingToPrint()](#getOutputBlankPageWhenNothingToPrint--) | Indica si se debe generar una página en blanco cuando no hay nada que imprimir. |
| [getPageCount()](#getPageCount--) | Obtiene el número de páginas a guardar. |
| [getPageIndex()](#getPageIndex--) | Obtiene el índice basado en cero de la primera página a guardar. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Controla/Indica el progreso del proceso de guardado de página. |
| [getPrintWithStatusDialog()](#getPrintWithStatusDialog--) | Si PrintWithStatusDialog = true, aparecerá un diálogo que muestra el estado actual de la impresión. |
| [getPrintingPage()](#getPrintingPage--) | Indica qué páginas no se imprimirán. |
| [getQuality()](#getQuality--) | Obtiene un valor que determina la calidad de las imágenes generadas, aplicable solo al guardar páginas en formato `Jpeg`. |
| [getSVGFitToViewPort()](#getSVGFitToViewPort--) | si esta propiedad es verdadera, el svg generado se ajustará al viewport. |
| [getSaveFormat()](#getSaveFormat--) | Obtiene el tipo de formato de archivo de salida. Soporta Tiff/XPS |
| [getSheetSet()](#getSheetSet--) | Obtiene las hojas a renderizar. |
| [getSvgCssPrefix()](#getSvgCssPrefix--) | Obtiene el prefijo del nombre css en svg, el valor predeterminado es una cadena vacía. |
| [getTextCrossType()](#getTextCrossType--) | Obtiene el tipo de texto de visualización cuando el ancho del texto es mayor que el ancho de la celda. |
| [getTiffColorDepth()](#getTiffColorDepth--) | Obtiene la profundidad de bits, aplicable solo al guardar páginas en formato `Tiff`. |
| [getTiffCompression()](#getTiffCompression--) | Obtiene el tipo de compresión, aplicable solo al guardar páginas en formato `Tiff`. |
| [getTiffPhotometricInterpretation()](#getTiffPhotometricInterpretation--) | Obtiene el tipo de PhotometricInterpretation, aplicable solo al guardar páginas en formato `Tiff`. |
| [getTransparent()](#getTransparent--) | Indica si el fondo de la imagen generada debe ser transparente. |
| [getVerticalResolution()](#getVerticalResolution--) | Obtiene la resolución vertical para las imágenes generadas, en puntos por pulgada. |
| [getWarningCallback()](#getWarningCallback--) | Obtiene la devolución de llamada de advertencia. |
| [hashCode()](#hashCode--) |  |
| [isCellAutoFit()](#isCellAutoFit--) | Indica si el ancho y alto de las celdas se ajustan automáticamente al valor de la celda. |
| [isFontSubstitutionCharGranularity()](#isFontSubstitutionCharGranularity--) | Indica si solo se debe sustituir la fuente del carácter cuando la fuente de la celda no es compatible con ella. |
| [isOptimized()](#isOptimized--) | Indica si se deben optimizar los elementos de salida. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllColumnsInOnePagePerSheet(boolean value)](#setAllColumnsInOnePagePerSheet-boolean-) | Si AllColumnsInOnePagePerSheet es true, todo el contenido de columnas de una hoja se exportará a una sola página en el resultado. |
| [setCellAutoFit(boolean value)](#setCellAutoFit-boolean-) | Indica si el ancho y alto de las celdas se ajustan automáticamente al valor de la celda. |
| [setChartImageType(ImageFormat value)](#setChartImageType-com.aspose.cells.ImageFormat-) | Indique el tipo de imagen del gráfico al convertir. |
| [setCheckWorkbookDefaultFont(boolean value)](#setCheckWorkbookDefaultFont-boolean-) | Cuando los caracteres en Excel son Unicode y no se establece la fuente correcta en el estilo de celda, pueden aparecer como bloques en pdf, imagen. |
| [setCustomRenderSettings(CustomRenderSettings value)](#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-) | Establece configuraciones personalizadas durante la renderización. |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) | Establece el idioma de edición predeterminado. |
| [setDefaultFont(String value)](#setDefaultFont-java.lang.String-) | Cuando los caracteres en Excel son Unicode y no se establece la fuente correcta en el estilo de celda, pueden aparecer como bloques en pdf, imagen. |
| [setDesiredSize(int desiredWidth, int desiredHeight)](#setDesiredSize-int-int-) | Establece el ancho y alto deseados de la imagen. |
| [setDesiredSize(int desiredWidth, int desiredHeight, boolean keepAspectRatio)](#setDesiredSize-int-int-boolean-) | Establece el ancho y alto deseados de la imagen. |
| [setDrawObjectEventHandler(DrawObjectEventHandler value)](#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-) | Implemente esta interfaz para obtener DrawObject y Bound durante la renderización. |
| [setEmbededImageNameInSvg(String value)](#setEmbededImageNameInSvg-java.lang.String-) | Indique el nombre de archivo de la imagen incrustada en svg. |
| [setEmfRenderSetting(int value)](#setEmfRenderSetting-int-) | Configuración para renderizar metarchivos Emf en el archivo fuente. |
| [setFontSubstitutionCharGranularity(boolean value)](#setFontSubstitutionCharGranularity-boolean-) | Indica si solo se debe sustituir la fuente del carácter cuando la fuente de la celda no es compatible con ella. |
| [setGridlineColor(Color value)](#setGridlineColor-com.aspose.cells.Color-) | Establece el color de la línea de la cuadrícula. |
| [setGridlineType(int value)](#setGridlineType-int-) | Establece el tipo de línea de cuadrícula. |
| [setHorizontalResolution(int value)](#setHorizontalResolution-int-) | Establece la resolución horizontal para las imágenes generadas, en puntos por pulgada. |
| [setImageType(int value)](#setImageType-int-) | Establece el formato de las imágenes generadas. |
| [setOnePagePerSheet(boolean value)](#setOnePagePerSheet-boolean-) | Si OnePagePerSheet es true, todo el contenido de una hoja se exportará a una sola página en el resultado. |
| [setOnlyArea(boolean value)](#setOnlyArea-boolean-) | Si esta propiedad es verdadera, se generará una Área, y no se aplicará escala. |
| [setOptimized(boolean value)](#setOptimized-boolean-) | Indica si se deben optimizar los elementos de salida. |
| [setOutputBlankPageWhenNothingToPrint(boolean value)](#setOutputBlankPageWhenNothingToPrint-boolean-) | Indica si se debe generar una página en blanco cuando no hay nada que imprimir. |
| [setPageCount(int value)](#setPageCount-int-) | Establece el número de páginas a guardar. |
| [setPageIndex(int value)](#setPageIndex-int-) | Establece el índice basado en cero de la primera página a guardar. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-) | Controla/Indica el progreso del proceso de guardado de página. |
| [setPrintWithStatusDialog(boolean value)](#setPrintWithStatusDialog-boolean-) | Si PrintWithStatusDialog = true, aparecerá un diálogo que muestra el estado actual de la impresión. |
| [setPrintingPage(int value)](#setPrintingPage-int-) | Indica qué páginas no se imprimirán. |
| [setQuality(int value)](#setQuality-int-) | Establece un valor que determina la calidad de las imágenes generadas y que se aplica solo al guardar páginas en el formato `Jpeg`. |
| [setRenderingHint(RenderingHints.Key key, Object value)](#setRenderingHint-java.awt.RenderingHints.Key-java.lang.Object-) | Establece el valor de una única preferencia para los algoritmos de renderizado. |
| [setSVGFitToViewPort(boolean value)](#setSVGFitToViewPort-boolean-) | si esta propiedad es verdadera, el svg generado se ajustará al viewport. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | Establece el tipo de formato de archivo de salida. Soporta Tiff/XPS. |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | Establece las hojas a renderizar. |
| [setSvgCssPrefix(String value)](#setSvgCssPrefix-java.lang.String-) | Establece el prefijo del nombre css en svg, el valor predeterminado es una cadena vacía. |
| [setTextCrossType(int value)](#setTextCrossType-int-) | Establece el tipo de texto de visualización cuando el ancho del texto es mayor que el ancho de la celda. |
| [setTiffColorDepth(int value)](#setTiffColorDepth-int-) | Establece la profundidad de bits que se aplica solo al guardar páginas en el formato `Tiff`. |
| [setTiffCompression(int value)](#setTiffCompression-int-) | Establece el tipo de compresión que se aplica solo al guardar páginas en el formato `Tiff`. |
| [setTiffPhotometricInterpretation(int value)](#setTiffPhotometricInterpretation-int-) | Establece el tipo de PhotometricInterpretation que se aplica solo al guardar páginas en el formato `Tiff`. |
| [setTransparent(boolean value)](#setTransparent-boolean-) | Indica si el fondo de la imagen generada debe ser transparente. |
| [setVerticalResolution(int value)](#setVerticalResolution-int-) | Establece la resolución vertical para las imágenes generadas, en puntos por pulgada. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Establece la devolución de llamada de advertencia. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ImageOrPrintOptions() {#ImageOrPrintOptions--}
```
public ImageOrPrintOptions()
```


Ctor.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAllColumnsInOnePagePerSheet() {#getAllColumnsInOnePagePerSheet--}
```
public boolean getAllColumnsInOnePagePerSheet()
```


Si AllColumnsInOnePagePerSheet es true, todo el contenido de columnas de una hoja se exportará a una sola página en el resultado. El ancho del tamaño de papel de pagesetup será inválido, y los demás ajustes de pagesetup seguirán teniendo efecto.

**Returns:**
boolean
### getChartImageType() {#getChartImageType--}
```
public ImageFormat getChartImageType()
```


Indica el tipo de imagen del gráfico al convertir. Valor predeterminado: PNG.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, Chart y Shape siempre se renderizan como elementos vectoriales (p. ej., punto, línea) para mejorar la calidad del renderizado. Esta propiedad será eliminada 12 meses después, a partir de junio de 2022. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
[ImageFormat](../../com.aspose.cells/imageformat)
### getCheckWorkbookDefaultFont() {#getCheckWorkbookDefaultFont--}
```
public boolean getCheckWorkbookDefaultFont()
```


Cuando los caracteres en Excel son Unicode y no se establece la fuente correcta en el estilo de celda, pueden aparecer como bloques en PDF, imagen. Establezca esto en verdadero para intentar usar la fuente predeterminada del libro de trabajo para mostrar primero estos caracteres.

**Remarks**

El valor predeterminado es verdadero.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCustomRenderSettings() {#getCustomRenderSettings--}
```
public CustomRenderSettings getCustomRenderSettings()
```


Obtiene configuraciones personalizadas durante el renderizado.

**Returns:**
[CustomRenderSettings](../../com.aspose.cells/customrendersettings)
### getDefaultEditLanguage() {#getDefaultEditLanguage--}
```
public int getDefaultEditLanguage()
```


Obtiene el idioma de edición predeterminado.

Ver [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

Puede mostrar/renderizar diferentes diseños para el párrafo de texto cuando se establece un idioma de edición diferente. El valor predeterminado es [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO).

**Returns:**
int
### getDefaultFont() {#getDefaultFont--}
```
public String getDefaultFont()
```


Cuando los caracteres en Excel son Unicode y no se establece la fuente correcta en el estilo de celda, establezca la DefaultFont como MingLiu o MS Gothic para mostrar estos caracteres. Si esta propiedad no se establece, Aspose.Cells usará la fuente predeterminada del sistema para mostrar estos caracteres Unicode.

**Returns:**
java.lang.String
### getDrawObjectEventHandler() {#getDrawObjectEventHandler--}
```
public DrawObjectEventHandler getDrawObjectEventHandler()
```


Implemente esta interfaz para obtener DrawObject y Bound durante la renderización.

**Returns:**
[DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler)
### getEmbededImageNameInSvg() {#getEmbededImageNameInSvg--}
```
public String getEmbededImageNameInSvg()
```


Indica el nombre de archivo de la imagen incrustada en svg. Esto debe ser una ruta completa con directorio, como "c:\\\\xpsEmbedded"

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, elimine esta propiedad porque las imágenes ahora siempre se incrustan en Svg con formato base64. Esta propiedad será eliminada 12 meses después, a partir de abril de 2025. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Returns:**
java.lang.String
### getEmfRenderSetting() {#getEmfRenderSetting--}
```
public int getEmfRenderSetting()
```


Configuración para renderizar metarchivos Emf en el archivo fuente.

Ver [EmfRenderSetting](../../com.aspose.cells/emfrendersetting).

**Remarks**

Los metarchivos EMF identificados como "EMF+ Dual" pueden contener tanto registros EMF+ como registros EMF. Cualquiera de los tipos de registro puede usarse para renderizar la imagen, solo registros EMF+, o solo registros EMF. Cuando se establece [EmfRenderSetting.EMF\_PLUS\_PREFER](../../com.aspose.cells/emfrendersetting\#EMF-PLUS-PREFER), los registros EMF+ se analizarán al renderizar la imagen; de lo contrario, solo se analizarán los registros EMF. El valor predeterminado es [EmfRenderSetting.EMF\_ONLY](../../com.aspose.cells/emfrendersetting\#EMF-ONLY). Para los frameworks que dependen de .NET System.Drawing.Common, esta configuración se ignora.

**Returns:**
int
### getGridlineColor() {#getGridlineColor--}
```
public Color getGridlineColor()
```


Obtiene el color de la línea de cuadrícula.

**Remarks**

Ignorará la configuración del color de la línea de cuadrícula en el archivo fuente.

**Returns:**
[Color](../../com.aspose.cells/color)
### getGridlineType() {#getGridlineType--}
```
public int getGridlineType()
```


Obtiene el tipo de línea de cuadrícula.

Ver [GridlineType](../../com.aspose.cells/gridlinetype).

**Remarks**

El valor predeterminado es tipo punteado.

**Returns:**
int
### getHorizontalResolution() {#getHorizontalResolution--}
```
public int getHorizontalResolution()
```


Obtiene la resolución horizontal para las imágenes generadas, en puntos por pulgada.

**Remarks**

El valor predeterminado es 96. Configurar  y  afecta el ancho y alto de la imagen de salida en píxeles.

**Example**

El siguiente código establece la resolución a 192; el ancho y alto de la imagen generada son el doble que cuando la resolución se deja en el valor predeterminado 96.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         ImageOrPrintOptions opts = new ImageOrPrintOptions();
 
         //Set output image type: png.
         opts.setImageType(ImageType.PNG);
 
         //Set resolution to 192.
         opts.setHorizontalResolution(192);
         opts.setVerticalResolution(192);
 
         //Render worksheet page to image.
         SheetRender sr = new SheetRender(wb.getWorksheets().get(0), opts);
         sr.toImage(0, "Sheet_Page1.png");
```

**Returns:**
int
### getImageType() {#getImageType--}
```
public int getImageType()
```


Obtiene el formato de las imágenes generadas. Valor predeterminado: PNG.

Ver [ImageType](../../com.aspose.cells/imagetype).

**Returns:**
int
### getOnePagePerSheet() {#getOnePagePerSheet--}
```
public boolean getOnePagePerSheet()
```


Si OnePagePerSheet es verdadero, todo el contenido de una hoja se exportará a una sola página en el resultado. El tamaño de papel de pagesetup será inválido, y los demás ajustes de pagesetup seguirán aplicándose.

**Returns:**
boolean
### getOnlyArea() {#getOnlyArea--}
```
public boolean getOnlyArea()
```


Si esta propiedad es verdadera, se generará una Área, y no se aplicará escala.

**Returns:**
boolean
### getOutputBlankPageWhenNothingToPrint() {#getOutputBlankPageWhenNothingToPrint--}
```
public boolean getOutputBlankPageWhenNothingToPrint()
```


Indica si se debe generar una página en blanco cuando no hay nada que imprimir.

**Remarks**

El valor predeterminado es false.

**Returns:**
boolean
### getPageCount() {#getPageCount--}
```
public int getPageCount()
```


Obtiene el número de páginas a guardar.

**Remarks**

El valor predeterminado es System.Int32.MaxValue, lo que significa que se renderizarán todas las páginas.

**Returns:**
int
### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


Obtiene el índice basado en cero de la primera página a guardar.

**Remarks**

El valor predeterminado es 0.

**Returns:**
int
### getPageSavingCallback() {#getPageSavingCallback--}
```
public IPageSavingCallback getPageSavingCallback()
```


Controla/Indica el progreso del proceso de guardado de página.

**Returns:**
[IPageSavingCallback](../../com.aspose.cells/ipagesavingcallback)
### getPrintWithStatusDialog() {#getPrintWithStatusDialog--}
```
public boolean getPrintWithStatusDialog()
```


Si PrintWithStatusDialog = true, se mostrará un diálogo que indica el estado actual de la impresión. De lo contrario, no se mostrará ningún diálogo.

**Returns:**
boolean
### getPrintingPage() {#getPrintingPage--}
```
public int getPrintingPage()
```


Indica qué páginas no se imprimirán.

Ver [PrintingPageType](../../com.aspose.cells/printingpagetype).

**Returns:**
int
### getQuality() {#getQuality--}
```
public int getQuality()
```


Obtiene un valor que determina la calidad de las imágenes generadas para aplicar solo al guardar páginas en el formato `Jpeg`. El valor predeterminado es 100.

**Remarks**

Tiene efecto solo al guardar en JPEG. El valor debe estar entre 0 y 100. El valor predeterminado es 100.

**Returns:**
int
### getSVGFitToViewPort() {#getSVGFitToViewPort--}
```
public boolean getSVGFitToViewPort()
```


si esta propiedad es verdadera, el svg generado se ajustará al viewport.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice [SvgImageOptions.getFitToViewPort()](../../com.aspose.cells/svgimageoptions\#getFitToViewPort--). Esta propiedad será eliminada 12 meses después, a partir de abril de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Obtiene el tipo de formato de archivo de salida. Soporta Tiff/XPS

Ver [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, para Tiff/Svg, use [getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--); para Xps, use [Workbook.save(String,SaveOptions)](../../com.aspose.cells/workbook\#save-String-SaveOptions-) con [XpsSaveOptions](../../com.aspose.cells/xpssaveoptions). Esta propiedad será eliminada 12 meses después, a partir de agosto de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
int
### getSheetSet() {#getSheetSet--}
```
public SheetSet getSheetSet()
```


Obtiene las hojas a renderizar. El valor predeterminado son todas las hojas visibles en el libro: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Remarks**

El conjunto se ignora cuando se usa en [SheetRender](../../com.aspose.cells/sheetrender).

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getSvgCssPrefix() {#getSvgCssPrefix--}
```
public String getSvgCssPrefix()
```


Obtiene el prefijo del nombre css en svg, el valor predeterminado es una cadena vacía.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice [SvgImageOptions.getCssPrefix()](../../com.aspose.cells/svgimageoptions\#getCssPrefix--). Esta propiedad será eliminada 12 meses después, a partir de abril de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
java.lang.String
### getTextCrossType() {#getTextCrossType--}
```
public int getTextCrossType()
```


Obtiene el tipo de texto de visualización cuando el ancho del texto es mayor que el ancho de la celda.

Ver [TextCrossType](../../com.aspose.cells/textcrosstype).

**Returns:**
int
### getTiffColorDepth() {#getTiffColorDepth--}
```
public int getTiffColorDepth()
```


Obtiene la profundidad de bits, aplicable solo al guardar páginas en formato `Tiff`.

Vea [ColorDepth](../../com.aspose.cells/colordepth).

**Remarks**

Tiene efecto solo al guardar en TIFF. Si TiffCompression está configurado a CCITT3 o CCITT4, esto no tendrá efecto; la profundidad de bits de la imagen TIFF generada será siempre 1.

**Returns:**
int
### getTiffCompression() {#getTiffCompression--}
```
public int getTiffCompression()
```


Obtiene el tipo de compresión, aplicable solo al guardar páginas en formato `Tiff`.

Vea [TiffCompression](../../com.aspose.cells/tiffcompression).

**Remarks**

Tiene efecto solo al guardar en TIFF. El valor predeterminado es Lzw.

**Returns:**
int
### getTiffPhotometricInterpretation() {#getTiffPhotometricInterpretation--}
```
public int getTiffPhotometricInterpretation()
```


Obtiene el tipo de PhotometricInterpretation, aplicable solo al guardar páginas en formato `Tiff`.

**Remarks**

Tiene efecto solo al guardar en TIFF. El valor predeterminado es -1, lo que indica que no se aplica PhotometricInterpretation.

**Returns:**
int
### getTransparent() {#getTransparent--}
```
public boolean getTransparent()
```


Indica si el fondo de la imagen generada debe ser transparente.

**Remarks**

El valor predeterminado es false. Eso significa que el fondo de las imágenes generadas es blanco.

**Returns:**
boolean
### getVerticalResolution() {#getVerticalResolution--}
```
public int getVerticalResolution()
```


Obtiene la resolución vertical para las imágenes generadas, en puntos por pulgada.

**Remarks**

El valor predeterminado es 96. Configurar  y  afecta el ancho y alto de la imagen de salida en píxeles.

**Example**

El siguiente código establece la resolución a 192; el ancho y alto de la imagen generada son el doble que cuando la resolución se deja en el valor predeterminado 96.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         ImageOrPrintOptions opts = new ImageOrPrintOptions();
 
         //Set output image type: png.
         opts.setImageType(ImageType.PNG);
 
         //Set resolution to 192.
         opts.setHorizontalResolution(192);
         opts.setVerticalResolution(192);
 
         //Render Chart to image.
         wb.getWorksheets().get(0).getCharts().get(0).toImage("Chart.png", opts);
```

**Returns:**
int
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Obtiene la devolución de llamada de advertencia.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCellAutoFit() {#isCellAutoFit--}
```
public boolean isCellAutoFit()
```


Indica si el ancho y alto de las celdas se ajustan automáticamente al valor de la celda. El valor predeterminado es false.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, esta propiedad no se usa, por favor elimine esta propiedad. Esta propiedad será eliminada 12 meses después, a partir de agosto de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
boolean
### isFontSubstitutionCharGranularity() {#isFontSubstitutionCharGranularity--}
```
public boolean isFontSubstitutionCharGranularity()
```


Indica si solo se debe sustituir la fuente del carácter cuando la fuente de la celda no es compatible con ella.

**Remarks**

El valor predeterminado es false. Primero intentaremos la fuente predeterminada del Workbook y PdfSaveOption/system para la fuente de la celda.

**Returns:**
boolean
### isOptimized() {#isOptimized--}
```
public boolean isOptimized()
```


Indica si se deben optimizar los elementos de salida.

**Remarks**

El valor predeterminado es false. Actualmente, cuando esta propiedad se establece en true, se realizarán las siguientes optimizaciones: 1. optimizar las líneas de borde. 2. optimizar el tamaño del archivo al renderizar a imagen Svg.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAllColumnsInOnePagePerSheet(boolean value) {#setAllColumnsInOnePagePerSheet-boolean-}
```
public void setAllColumnsInOnePagePerSheet(boolean value)
```


Si AllColumnsInOnePagePerSheet es true, todo el contenido de columnas de una hoja se exportará a una sola página en el resultado. El ancho del tamaño de papel de pagesetup será inválido, y los demás ajustes de pagesetup seguirán teniendo efecto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setCellAutoFit(boolean value) {#setCellAutoFit-boolean-}
```
public void setCellAutoFit(boolean value)
```


Indica si el ancho y alto de las celdas se ajustan automáticamente al valor de la celda. El valor predeterminado es false.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, esta propiedad no se usa, por favor elimine esta propiedad. Esta propiedad será eliminada 12 meses después, a partir de agosto de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setChartImageType(ImageFormat value) {#setChartImageType-com.aspose.cells.ImageFormat-}
```
public void setChartImageType(ImageFormat value)
```


Indica el tipo de imagen del gráfico al convertir. Valor predeterminado: PNG.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, Chart y Shape siempre se renderizan como elementos vectoriales (p. ej., punto, línea) para mejorar la calidad del renderizado. Esta propiedad será eliminada 12 meses después, a partir de junio de 2022. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [ImageFormat](../../com.aspose.cells/imageformat) |  |

### setCheckWorkbookDefaultFont(boolean value) {#setCheckWorkbookDefaultFont-boolean-}
```
public void setCheckWorkbookDefaultFont(boolean value)
```


Cuando los caracteres en Excel son Unicode y no se establece la fuente correcta en el estilo de celda, pueden aparecer como bloques en PDF, imagen. Establezca esto en verdadero para intentar usar la fuente predeterminada del libro de trabajo para mostrar primero estos caracteres.

**Remarks**

El valor predeterminado es verdadero.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setCustomRenderSettings(CustomRenderSettings value) {#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-}
```
public void setCustomRenderSettings(CustomRenderSettings value)
```


Establece configuraciones personalizadas durante la renderización.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [CustomRenderSettings](../../com.aspose.cells/customrendersettings) |  |

### setDefaultEditLanguage(int value) {#setDefaultEditLanguage-int-}
```
public void setDefaultEditLanguage(int value)
```


Establece el idioma de edición predeterminado.

Ver [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

Puede mostrar/renderizar diferentes diseños para el párrafo de texto cuando se establece un idioma de edición diferente. El valor predeterminado es [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setDefaultFont(String value) {#setDefaultFont-java.lang.String-}
```
public void setDefaultFont(String value)
```


Cuando los caracteres en Excel son Unicode y no se establece la fuente correcta en el estilo de celda, establezca la DefaultFont como MingLiu o MS Gothic para mostrar estos caracteres. Si esta propiedad no se establece, Aspose.Cells usará la fuente predeterminada del sistema para mostrar estos caracteres Unicode.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setDesiredSize(int desiredWidth, int desiredHeight) {#setDesiredSize-int-int-}
```
public void setDesiredSize(int desiredWidth, int desiredHeight)
```


Establece el ancho y alto deseados de la imagen.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice [setDesiredSize(int,int,boolean)](../../com.aspose.cells/imageorprintoptions\#setDesiredSize-int-int-boolean-) estableciendo el parámetro keepAspectRatio a false. Esta propiedad será eliminada 12 meses después, a partir de mayo de 2023. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| desiredWidth | int | ancho deseado en píxeles |
| desiredHeight | int | alto deseado en píxeles |

### setDesiredSize(int desiredWidth, int desiredHeight, boolean keepAspectRatio) {#setDesiredSize-int-int-boolean-}
```
public void setDesiredSize(int desiredWidth, int desiredHeight, boolean keepAspectRatio)
```


Establece el ancho y alto deseados de la imagen.

**Remarks**

El ancho y alto de la imagen de salida en píxeles se basarán únicamente en el ancho y alto deseados establecidos. Los  y  no afectarán el ancho y alto de la imagen de salida en este caso.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| desiredWidth | int | ancho deseado en píxeles |
| desiredHeight | int | alto deseado en píxeles |
| keepAspectRatio | boolean | si se debe mantener la relación de aspecto de la imagen original |

### setDrawObjectEventHandler(DrawObjectEventHandler value) {#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-}
```
public void setDrawObjectEventHandler(DrawObjectEventHandler value)
```


Implemente esta interfaz para obtener DrawObject y Bound durante la renderización.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler) |  |

### setEmbededImageNameInSvg(String value) {#setEmbededImageNameInSvg-java.lang.String-}
```
public void setEmbededImageNameInSvg(String value)
```


Indica el nombre de archivo de la imagen incrustada en svg. Esto debe ser una ruta completa con directorio, como "c:\\\\xpsEmbedded"

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, elimine esta propiedad porque las imágenes ahora siempre se incrustan en Svg con formato base64. Esta propiedad será eliminada 12 meses después, a partir de abril de 2025. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setEmfRenderSetting(int value) {#setEmfRenderSetting-int-}
```
public void setEmfRenderSetting(int value)
```


Configuración para renderizar metarchivos Emf en el archivo fuente.

Ver [EmfRenderSetting](../../com.aspose.cells/emfrendersetting).

**Remarks**

Los metarchivos EMF identificados como "EMF+ Dual" pueden contener tanto registros EMF+ como registros EMF. Cualquiera de los tipos de registro puede usarse para renderizar la imagen, solo registros EMF+, o solo registros EMF. Cuando se establece [EmfRenderSetting.EMF\_PLUS\_PREFER](../../com.aspose.cells/emfrendersetting\#EMF-PLUS-PREFER), los registros EMF+ se analizarán al renderizar la imagen; de lo contrario, solo se analizarán los registros EMF. El valor predeterminado es [EmfRenderSetting.EMF\_ONLY](../../com.aspose.cells/emfrendersetting\#EMF-ONLY). Para los frameworks que dependen de .NET System.Drawing.Common, esta configuración se ignora.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setFontSubstitutionCharGranularity(boolean value) {#setFontSubstitutionCharGranularity-boolean-}
```
public void setFontSubstitutionCharGranularity(boolean value)
```


Indica si solo se debe sustituir la fuente del carácter cuando la fuente de la celda no es compatible con ella.

**Remarks**

El valor predeterminado es false. Primero intentaremos la fuente predeterminada del Workbook y PdfSaveOption/system para la fuente de la celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setGridlineColor(Color value) {#setGridlineColor-com.aspose.cells.Color-}
```
public void setGridlineColor(Color value)
```


Establece el color de la línea de la cuadrícula.

**Remarks**

Ignorará la configuración del color de la línea de cuadrícula en el archivo fuente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setGridlineType(int value) {#setGridlineType-int-}
```
public void setGridlineType(int value)
```


Establece el tipo de línea de cuadrícula.

Ver [GridlineType](../../com.aspose.cells/gridlinetype).

**Remarks**

El valor predeterminado es tipo punteado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setHorizontalResolution(int value) {#setHorizontalResolution-int-}
```
public void setHorizontalResolution(int value)
```


Establece la resolución horizontal para las imágenes generadas, en puntos por pulgada.

**Remarks**

El valor predeterminado es 96. Configurar  y  afecta el ancho y alto de la imagen de salida en píxeles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setImageType(int value) {#setImageType-int-}
```
public void setImageType(int value)
```


Establece el formato de las imágenes generadas. valor predeterminado: PNG.

Ver [ImageType](../../com.aspose.cells/imagetype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setOnePagePerSheet(boolean value) {#setOnePagePerSheet-boolean-}
```
public void setOnePagePerSheet(boolean value)
```


Si OnePagePerSheet es verdadero, todo el contenido de una hoja se exportará a una sola página en el resultado. El tamaño de papel de pagesetup será inválido, y los demás ajustes de pagesetup seguirán aplicándose.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setOnlyArea(boolean value) {#setOnlyArea-boolean-}
```
public void setOnlyArea(boolean value)
```


Si esta propiedad es verdadera, se generará una Área, y no se aplicará escala.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setOptimized(boolean value) {#setOptimized-boolean-}
```
public void setOptimized(boolean value)
```


Indica si se deben optimizar los elementos de salida.

**Remarks**

El valor predeterminado es false. Actualmente, cuando esta propiedad se establece en true, se realizarán las siguientes optimizaciones: 1. optimizar las líneas de borde. 2. optimizar el tamaño del archivo al renderizar a imagen Svg.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setOutputBlankPageWhenNothingToPrint(boolean value) {#setOutputBlankPageWhenNothingToPrint-boolean-}
```
public void setOutputBlankPageWhenNothingToPrint(boolean value)
```


Indica si se debe generar una página en blanco cuando no hay nada que imprimir.

**Remarks**

El valor predeterminado es false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setPageCount(int value) {#setPageCount-int-}
```
public void setPageCount(int value)
```


Establece el número de páginas a guardar.

**Remarks**

El valor predeterminado es System.Int32.MaxValue, lo que significa que se renderizarán todas las páginas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setPageIndex(int value) {#setPageIndex-int-}
```
public void setPageIndex(int value)
```


Establece el índice basado en cero de la primera página a guardar.

**Remarks**

El valor predeterminado es 0.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-}
```
public void setPageSavingCallback(IPageSavingCallback value)
```


Controla/Indica el progreso del proceso de guardado de página.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.cells/ipagesavingcallback) |  |

### setPrintWithStatusDialog(boolean value) {#setPrintWithStatusDialog-boolean-}
```
public void setPrintWithStatusDialog(boolean value)
```


Si PrintWithStatusDialog = true, se mostrará un diálogo que indica el estado actual de la impresión. De lo contrario, no se mostrará ningún diálogo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setPrintingPage(int value) {#setPrintingPage-int-}
```
public void setPrintingPage(int value)
```


Indica qué páginas no se imprimirán.

Ver [PrintingPageType](../../com.aspose.cells/printingpagetype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setQuality(int value) {#setQuality-int-}
```
public void setQuality(int value)
```


Establece un valor que determina la calidad de las imágenes generadas para aplicar solo al guardar páginas en el formato `Jpeg`. El valor predeterminado es 100.

**Remarks**

Tiene efecto solo al guardar en JPEG. El valor debe estar entre 0 y 100. El valor predeterminado es 100.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setRenderingHint(RenderingHints.Key key, Object value) {#setRenderingHint-java.awt.RenderingHints.Key-java.lang.Object-}
```
public void setRenderingHint(RenderingHints.Key key, Object value)
```


Establece el valor de una única preferencia para los algoritmos de renderizado. Las categorías de sugerencias incluyen controles para la calidad de renderizado y el equilibrio general entre tiempo/calidad en el proceso de renderizado. Consulte la clase RenderingHints para obtener definiciones de algunas claves y valores comunes.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| clave | java.awt.RenderingHints.Key | la clave de la sugerencia a establecer. |
| valor | java.lang.Object | el valor que indica las preferencias para la categoría de sugerencia especificada. |

### setSVGFitToViewPort(boolean value) {#setSVGFitToViewPort-boolean-}
```
public void setSVGFitToViewPort(boolean value)
```


si esta propiedad es verdadera, el svg generado se ajustará al viewport.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice [SvgImageOptions.getFitToViewPort()](../../com.aspose.cells/svgimageoptions\#getFitToViewPort--). Esta propiedad será eliminada 12 meses después, a partir de abril de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSaveFormat(int value) {#setSaveFormat-int-}
```
public void setSaveFormat(int value)
```


Establece el tipo de formato de archivo de salida. Soporta Tiff/XPS.

Ver [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, para Tiff/Svg, use [getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--); para Xps, use [Workbook.save(String,SaveOptions)](../../com.aspose.cells/workbook\#save-String-SaveOptions-) con [XpsSaveOptions](../../com.aspose.cells/xpssaveoptions). Esta propiedad será eliminada 12 meses después, a partir de agosto de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setSheetSet(SheetSet value) {#setSheetSet-com.aspose.cells.SheetSet-}
```
public void setSheetSet(SheetSet value)
```


Establece las hojas a renderizar. El predeterminado son todas las hojas visibles en el libro: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Remarks**

El conjunto se ignora cuando se usa en [SheetRender](../../com.aspose.cells/sheetrender).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [SheetSet](../../com.aspose.cells/sheetset) |  |

### setSvgCssPrefix(String value) {#setSvgCssPrefix-java.lang.String-}
```
public void setSvgCssPrefix(String value)
```


Establece el prefijo del nombre css en svg, el valor predeterminado es una cadena vacía.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice [SvgImageOptions.getCssPrefix()](../../com.aspose.cells/svgimageoptions\#getCssPrefix--). Esta propiedad será eliminada 12 meses después, a partir de abril de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setTextCrossType(int value) {#setTextCrossType-int-}
```
public void setTextCrossType(int value)
```


Establece el tipo de texto de visualización cuando el ancho del texto es mayor que el ancho de la celda.

Ver [TextCrossType](../../com.aspose.cells/textcrosstype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setTiffColorDepth(int value) {#setTiffColorDepth-int-}
```
public void setTiffColorDepth(int value)
```


Establece la profundidad de bits que se aplica solo al guardar páginas en el formato `Tiff`.

Vea [ColorDepth](../../com.aspose.cells/colordepth).

**Remarks**

Tiene efecto solo al guardar en TIFF. Si TiffCompression está configurado a CCITT3 o CCITT4, esto no tendrá efecto; la profundidad de bits de la imagen TIFF generada será siempre 1.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public void setTiffCompression(int value)
```


Establece el tipo de compresión que se aplica solo al guardar páginas en el formato `Tiff`.

Vea [TiffCompression](../../com.aspose.cells/tiffcompression).

**Remarks**

Tiene efecto solo al guardar en TIFF. El valor predeterminado es Lzw.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setTiffPhotometricInterpretation(int value) {#setTiffPhotometricInterpretation-int-}
```
public void setTiffPhotometricInterpretation(int value)
```


Establece el tipo de PhotometricInterpretation que se aplica solo al guardar páginas en el formato `Tiff`.

**Remarks**

Tiene efecto solo al guardar en TIFF. El valor predeterminado es -1, lo que indica que no se aplica PhotometricInterpretation.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setTransparent(boolean value) {#setTransparent-boolean-}
```
public void setTransparent(boolean value)
```


Indica si el fondo de la imagen generada debe ser transparente.

**Remarks**

El valor predeterminado es false. Eso significa que el fondo de las imágenes generadas es blanco.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setVerticalResolution(int value) {#setVerticalResolution-int-}
```
public void setVerticalResolution(int value)
```


Establece la resolución vertical para las imágenes generadas, en puntos por pulgada.

**Remarks**

El valor predeterminado es 96. Configurar  y  afecta el ancho y alto de la imagen de salida en píxeles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```


Establece la devolución de llamada de advertencia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

