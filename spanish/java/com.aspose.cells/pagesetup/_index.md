---
title: "PageSetup"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Encapsula el objeto que representa la descripción de la configuración de página."
type: docs
url: /es/java/com.aspose.cells/pagesetup/
---

**Inheritance:**
java.lang.Object
```
public class PageSetup
```

Encapsula el objeto que representa la descripción de la configuración de página. El objeto PageSetup contiene todas las opciones de configuración de página.

**Example**

```
         Workbook workbook = new Workbook();
 
         WorksheetCollection sheets = workbook.getWorksheets();
 
         //Add a worksheet
         sheets.add();
         Worksheet sheet = sheets.get(1);
         PageSetup pageSetup = sheet.getPageSetup();
         pageSetup.setPrintArea("D1:K13");
 
         //do your business
```
## Métodos

| Método | Descripción |
| --- | --- |
| [clearHeaderFooter()](#clearHeaderFooter--) | Borra la configuración de encabezado y pie de página. |
| [copy(PageSetup source, CopyOptions copyOptions)](#copy-com.aspose.cells.PageSetup-com.aspose.cells.CopyOptions-) | Copia la configuración de la configuración de página. |
| [customPaperSize(double width, double height)](#customPaperSize-double-double-) | Establece el tamaño de papel personalizado, en unidades de pulgadas. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBlackAndWhite()](#getBlackAndWhite--) | Representa si los elementos del documento se imprimirán en blanco y negro. |
| [getBottomMargin()](#getBottomMargin--) | Representa el tamaño del margen inferior, en unidades de centímetros. |
| [getBottomMarginInch()](#getBottomMarginInch--) | Representa el tamaño del margen inferior, en unidades de pulgadas. |
| [getCenterHorizontally()](#getCenterHorizontally--) | Representa si la hoja se imprime centrada horizontalmente. |
| [getCenterVertically()](#getCenterVertically--) | Representa si la hoja se imprime centrada verticalmente. |
| [getClass()](#getClass--) |  |
| [getCommands(String headerFooterScript)](#getCommands-java.lang.String-) | Obtiene todos los comandos del encabezado o pie de página. |
| [getEvenFooter(int section)](#getEvenFooter-int-) | Obtiene un script que formatea el pie de página par de un archivo Excel. |
| [getEvenHeader(int section)](#getEvenHeader-int-) | Obtiene un script que formatea el encabezado par de un archivo Excel. |
| [getFirstPageFooter(int section)](#getFirstPageFooter-int-) | Obtiene un script que formatea el pie de página de la primera página de un archivo Excel. |
| [getFirstPageHeader(int section)](#getFirstPageHeader-int-) | Obtiene un script que formatea el encabezado de la primera página de un archivo Excel. |
| [getFirstPageNumber()](#getFirstPageNumber--) | Representa el número de la primera página que se usará cuando se imprima esta hoja. |
| [getFitToPagesTall()](#getFitToPagesTall--) | Representa la cantidad de páginas de alto a la que se escalará la hoja de cálculo cuando se imprima. |
| [getFitToPagesWide()](#getFitToPagesWide--) | Representa la cantidad de páginas de ancho a la que se escalará la hoja de cálculo cuando se imprima. |
| [getFooter(int section)](#getFooter-int-) | Obtiene un script que formatea el pie de página de un archivo Excel. |
| [getFooterMargin()](#getFooterMargin--) | Representa la distancia desde la parte inferior de la página hasta el pie de página, en unidades de centímetros. |
| [getFooterMarginInch()](#getFooterMarginInch--) | Representa la distancia desde la parte inferior de la página hasta el pie de página, en unidades de pulgadas. |
| [getHeader(int section)](#getHeader-int-) | Obtiene un script que formatea el encabezado de un archivo Excel. |
| [getHeaderMargin()](#getHeaderMargin--) | Representa la distancia desde la parte superior de la página hasta el encabezado, en unidades de centímetros. |
| [getHeaderMarginInch()](#getHeaderMarginInch--) | Representa la distancia desde la parte superior de la página hasta el encabezado, en unidades de pulgadas. |
| [getLeftMargin()](#getLeftMargin--) | Representa el tamaño del margen izquierdo, en unidades de centímetros. |
| [getLeftMarginInch()](#getLeftMarginInch--) | Representa el tamaño del margen izquierdo, en unidades de pulgadas. |
| [getODSPageBackground()](#getODSPageBackground--) | Obtiene el fondo de ODS. |
| [getOrder()](#getOrder--) | Representa el orden que Microsoft Excel utiliza para numerar las páginas al imprimir una hoja de cálculo grande. |
| [getOrientation()](#getOrientation--) | Representa la orientación de impresión de la página. |
| [getPaperHeight()](#getPaperHeight--) | Obtiene la altura del papel en unidades de pulgadas, considerando la orientación de la página. |
| [getPaperSize()](#getPaperSize--) | Representa el tamaño del papel. |
| [getPaperWidth()](#getPaperWidth--) | Obtiene el ancho del papel en unidades de pulgadas, considerando la orientación de la página. |
| [getPicture(boolean isFirst, boolean isEven, boolean isHeader, int section)](#getPicture-boolean-boolean-boolean-int-) | Obtiene el objeto [Picture](../../com.aspose.cells/picture) del encabezado / pie de página. |
| [getPicture(boolean isHeader, int section)](#getPicture-boolean-int-) | Obtiene el objeto [Picture](../../com.aspose.cells/picture) del encabezado / pie de página. |
| [getPrintArea()](#getPrintArea--) | Representa el rango a imprimir. |
| [getPrintComments()](#getPrintComments--) | Representa la forma en que los comentarios se imprimen con la hoja. |
| [getPrintCopies()](#getPrintCopies--) | Obtiene el número de copias a imprimir. |
| [getPrintDraft()](#getPrintDraft--) | Representa si la hoja se imprimirá sin gráficos. |
| [getPrintErrors()](#getPrintErrors--) | Especifica el tipo de error de impresión mostrado. |
| [getPrintGridlines()](#getPrintGridlines--) | Representa si las líneas de cuadrícula de las celdas se imprimen en la página. |
| [getPrintHeadings()](#getPrintHeadings--) | Representa si los encabezados de filas y columnas se imprimen con esta página. |
| [getPrintQuality()](#getPrintQuality--) | Representa la calidad de impresión. |
| [getPrintTitleColumns()](#getPrintTitleColumns--) | Representa las columnas que contienen las celdas que se repetirán en el lado izquierdo de cada página. |
| [getPrintTitleRows()](#getPrintTitleRows--) | Representa las filas que contienen las celdas que se repetirán en la parte superior de cada página. |
| [getPrinterSettings()](#getPrinterSettings--) | Obtiene la configuración de la impresora predeterminada. |
| [getRightMargin()](#getRightMargin--) | Representa el tamaño del margen derecho, en unidades de centímetros. |
| [getRightMarginInch()](#getRightMarginInch--) | Representa el tamaño del margen derecho, en unidades de pulgadas. |
| [getTopMargin()](#getTopMargin--) | Representa el tamaño del margen superior, en unidades de centímetros. |
| [getTopMarginInch()](#getTopMarginInch--) | Representa el tamaño del margen superior, en unidades de pulgadas. |
| [getZoom()](#getZoom--) | Representa el factor de escala en porcentaje. |
| [hashCode()](#hashCode--) |  |
| [isAutoFirstPageNumber()](#isAutoFirstPageNumber--) | Indica si el número de la primera página se asigna automáticamente. |
| [isAutomaticPaperSize()](#isAutomaticPaperSize--) | Indica si el tamaño del papel es automático. |
| [isHFAlignMargins()](#isHFAlignMargins--) | Indica si los márgenes de encabezado y pie de página están alineados con los márgenes de la página. |
| [isHFDiffFirst()](#isHFDiffFirst--) | True significa que el encabezado/pie de página de la primera página es diferente de las demás páginas. |
| [isHFDiffOddEven()](#isHFDiffOddEven--) | True significa que el encabezado/pie de página de las páginas impares es diferente de las páginas impares. |
| [isHFScaleWithDoc()](#isHFScaleWithDoc--) | Indica si el encabezado y el pie de página se escalan con el escalado del documento. |
| [isPercentScale()](#isPercentScale--) | Si esta propiedad es False, las propiedades FitToPagesWide y FitToPagesTall controlan cómo se escala la hoja de cálculo. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFirstPageNumber(boolean value)](#setAutoFirstPageNumber-boolean-) | Indica si el número de la primera página se asigna automáticamente. |
| [setBlackAndWhite(boolean value)](#setBlackAndWhite-boolean-) | Representa si los elementos del documento se imprimirán en blanco y negro. |
| [setBottomMargin(double value)](#setBottomMargin-double-) | Representa el tamaño del margen inferior, en unidades de centímetros. |
| [setBottomMarginInch(double value)](#setBottomMarginInch-double-) | Representa el tamaño del margen inferior, en unidades de pulgadas. |
| [setCenterHorizontally(boolean value)](#setCenterHorizontally-boolean-) | Representa si la hoja se imprime centrada horizontalmente. |
| [setCenterVertically(boolean value)](#setCenterVertically-boolean-) | Representa si la hoja se imprime centrada verticalmente. |
| [setEvenFooter(int section, String footerScript)](#setEvenFooter-int-java.lang.String-) | Establece un script que formatea el pie de página de las páginas pares de un archivo Excel. |
| [setEvenHeader(int section, String headerScript)](#setEvenHeader-int-java.lang.String-) | Establece un script que formatea el encabezado de las páginas pares de un archivo Excel. |
| [setFirstPageFooter(int section, String footerScript)](#setFirstPageFooter-int-java.lang.String-) | Establece un script que formatea el pie de página de la primera página de un archivo Excel. |
| [setFirstPageHeader(int section, String headerScript)](#setFirstPageHeader-int-java.lang.String-) | Establece un script que formatea el encabezado de la primera página de un archivo Excel. |
| [setFirstPageNumber(int value)](#setFirstPageNumber-int-) | Representa el número de la primera página que se usará cuando se imprima esta hoja. |
| [setFitToPages(int wide, int tall)](#setFitToPages-int-int-) | Establece el número de páginas a las que se escalará la hoja de cálculo cuando se imprima. |
| [setFitToPagesTall(int value)](#setFitToPagesTall-int-) | Representa la cantidad de páginas de alto a la que se escalará la hoja de cálculo cuando se imprima. |
| [setFitToPagesWide(int value)](#setFitToPagesWide-int-) | Representa la cantidad de páginas de ancho a la que se escalará la hoja de cálculo cuando se imprima. |
| [setFooter(int section, String footerScript)](#setFooter-int-java.lang.String-) | Establece un script que da formato al pie de página de un archivo Excel. |
| [setFooterMargin(double value)](#setFooterMargin-double-) | Representa la distancia desde la parte inferior de la página hasta el pie de página, en unidades de centímetros. |
| [setFooterMarginInch(double value)](#setFooterMarginInch-double-) | Representa la distancia desde la parte inferior de la página hasta el pie de página, en unidades de pulgadas. |
| [setFooterPicture(int section, byte[] footerPicture)](#setFooterPicture-int-byte---) | Establece una imagen en el pie de página de una hoja de cálculo. |
| [setHFAlignMargins(boolean value)](#setHFAlignMargins-boolean-) | Indica si los márgenes de encabezado y pie de página están alineados con los márgenes de la página. |
| [setHFDiffFirst(boolean value)](#setHFDiffFirst-boolean-) | True significa que el encabezado/pie de página de la primera página es diferente de las demás páginas. |
| [setHFDiffOddEven(boolean value)](#setHFDiffOddEven-boolean-) | True significa que el encabezado/pie de página de las páginas impares es diferente de las páginas impares. |
| [setHFScaleWithDoc(boolean value)](#setHFScaleWithDoc-boolean-) | Indica si el encabezado y el pie de página se escalan con el escalado del documento. |
| [setHeader(int section, String headerScript)](#setHeader-int-java.lang.String-) | Establece un script que da formato al encabezado de un archivo Excel. |
| [setHeaderMargin(double value)](#setHeaderMargin-double-) | Representa la distancia desde la parte superior de la página hasta el encabezado, en unidades de centímetros. |
| [setHeaderMarginInch(double value)](#setHeaderMarginInch-double-) | Representa la distancia desde la parte superior de la página hasta el encabezado, en unidades de pulgadas. |
| [setHeaderPicture(int section, byte[] headerPicture)](#setHeaderPicture-int-byte---) | Establece una imagen en el encabezado de una hoja de cálculo. |
| [setLeftMargin(double value)](#setLeftMargin-double-) | Representa el tamaño del margen izquierdo, en unidades de centímetros. |
| [setLeftMarginInch(double value)](#setLeftMarginInch-double-) | Representa el tamaño del margen izquierdo, en unidades de pulgadas. |
| [setOrder(int value)](#setOrder-int-) | Representa el orden que Microsoft Excel utiliza para numerar las páginas al imprimir una hoja de cálculo grande. |
| [setOrientation(int value)](#setOrientation-int-) | Representa la orientación de impresión de la página. |
| [setPaperSize(int value)](#setPaperSize-int-) | Representa el tamaño del papel. |
| [setPercentScale(boolean value)](#setPercentScale-boolean-) | Si esta propiedad es False, las propiedades FitToPagesWide y FitToPagesTall controlan cómo se escala la hoja de cálculo. |
| [setPicture(boolean isFirst, boolean isEven, boolean isHeader, int section, byte[] imageData)](#setPicture-boolean-boolean-boolean-int-byte---) | Establece una imagen en el encabezado/pie de página de una hoja de cálculo. |
| [setPrintArea(String value)](#setPrintArea-java.lang.String-) | Representa el rango a imprimir. |
| [setPrintComments(int value)](#setPrintComments-int-) | Representa la forma en que los comentarios se imprimen con la hoja. |
| [setPrintCopies(int value)](#setPrintCopies-int-) | Establece el número de copias a imprimir. |
| [setPrintDraft(boolean value)](#setPrintDraft-boolean-) | Representa si la hoja se imprimirá sin gráficos. |
| [setPrintErrors(int value)](#setPrintErrors-int-) | Especifica el tipo de error de impresión mostrado. |
| [setPrintGridlines(boolean value)](#setPrintGridlines-boolean-) | Representa si las líneas de cuadrícula de las celdas se imprimen en la página. |
| [setPrintHeadings(boolean value)](#setPrintHeadings-boolean-) | Representa si los encabezados de filas y columnas se imprimen con esta página. |
| [setPrintQuality(int value)](#setPrintQuality-int-) | Representa la calidad de impresión. |
| [setPrintTitleColumns(String value)](#setPrintTitleColumns-java.lang.String-) | Representa las columnas que contienen las celdas que se repetirán en el lado izquierdo de cada página. |
| [setPrintTitleRows(String value)](#setPrintTitleRows-java.lang.String-) | Representa las filas que contienen las celdas que se repetirán en la parte superior de cada página. |
| [setPrinterSettings(byte[] value)](#setPrinterSettings-byte---) | Establece la configuración de la impresora predeterminada. |
| [setRightMargin(double value)](#setRightMargin-double-) | Representa el tamaño del margen derecho, en unidades de centímetros. |
| [setRightMarginInch(double value)](#setRightMarginInch-double-) | Representa el tamaño del margen derecho, en unidades de pulgadas. |
| [setTopMargin(double value)](#setTopMargin-double-) | Representa el tamaño del margen superior, en unidades de centímetros. |
| [setTopMarginInch(double value)](#setTopMarginInch-double-) | Representa el tamaño del margen superior, en unidades de pulgadas. |
| [setZoom(int value)](#setZoom-int-) | Representa el factor de escala en porcentaje. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### clearHeaderFooter() {#clearHeaderFooter--}
```
public void clearHeaderFooter()
```


Borra la configuración de encabezado y pie de página.

### copy(PageSetup source, CopyOptions copyOptions) {#copy-com.aspose.cells.PageSetup-com.aspose.cells.CopyOptions-}
```
public void copy(PageSetup source, CopyOptions copyOptions)
```


Copia la configuración de la configuración de página.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| source | [PageSetup](../../com.aspose.cells/pagesetup) | La fuente. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | Las opciones de copia. |

### customPaperSize(double width, double height) {#customPaperSize-double-double-}
```
public void customPaperSize(double width, double height)
```


Establece el tamaño de papel personalizado, en unidades de pulgadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ancho | double | El ancho del papel. |
| altura | double | La altura del papel. |

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
### getBlackAndWhite() {#getBlackAndWhite--}
```
public boolean getBlackAndWhite()
```


Representa si los elementos del documento se imprimirán en blanco y negro.

**Returns:**
boolean
### getBottomMargin() {#getBottomMargin--}
```
public double getBottomMargin()
```


Representa el tamaño del margen inferior, en unidades de centímetros.

**Returns:**
double
### getBottomMarginInch() {#getBottomMarginInch--}
```
public double getBottomMarginInch()
```


Representa el tamaño del margen inferior, en unidades de pulgadas.

**Returns:**
double
### getCenterHorizontally() {#getCenterHorizontally--}
```
public boolean getCenterHorizontally()
```


Representa si la hoja se imprime centrada horizontalmente.

**Returns:**
boolean
### getCenterVertically() {#getCenterVertically--}
```
public boolean getCenterVertically()
```


Representa si la hoja se imprime centrada verticalmente.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCommands(String headerFooterScript) {#getCommands-java.lang.String-}
```
public HeaderFooterCommand[] getCommands(String headerFooterScript)
```


Obtiene todos los comandos del encabezado o pie de página.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| headerFooterScript | java.lang.String | El script de encabezado/pie de página |

**Returns:**
com.aspose.cells.HeaderFooterCommand[] - Devuelve todos los comandos del encabezado o pie de página.
### getEvenFooter(int section) {#getEvenFooter-int-}
```
public String getEvenFooter(int section)
```


Obtiene un script que formatea el pie de página par de un archivo Excel.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| section | int | 0: Sección izquierda, 1: Sección central, 2: Sección derecha. |

**Returns:**
java.lang.String
### getEvenHeader(int section) {#getEvenHeader-int-}
```
public String getEvenHeader(int section)
```


Obtiene un script que formatea el encabezado par de un archivo Excel.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| section | int | 0: Sección izquierda, 1: Sección central, 2: Sección derecha. |

**Returns:**
java.lang.String
### getFirstPageFooter(int section) {#getFirstPageFooter-int-}
```
public String getFirstPageFooter(int section)
```


Obtiene un script que formatea el pie de página de la primera página de un archivo Excel.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| section | int | 0: Sección izquierda, 1: Sección central, 2: Sección derecha. |

**Returns:**
java.lang.String
### getFirstPageHeader(int section) {#getFirstPageHeader-int-}
```
public String getFirstPageHeader(int section)
```


Obtiene un script que formatea el encabezado de la primera página de un archivo Excel.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| section | int | 0: Sección izquierda, 1: Sección central, 2: Sección derecha. |

**Returns:**
java.lang.String
### getFirstPageNumber() {#getFirstPageNumber--}
```
public int getFirstPageNumber()
```


Representa el número de la primera página que se usará cuando se imprima esta hoja.

**Returns:**
int
### getFitToPagesTall() {#getFitToPagesTall--}
```
public int getFitToPagesTall()
```


Representa la cantidad de páginas de alto a la que se escalará la hoja de cálculo al imprimirse. El valor predeterminado es 1.

**Remarks**

Debe establecer FitToPagesWide en cero si desea ajustar todas las filas en una sola página.

**Returns:**
int
### getFitToPagesWide() {#getFitToPagesWide--}
```
public int getFitToPagesWide()
```


Representa la cantidad de páginas de ancho a la que se escalará la hoja de cálculo al imprimirse. El valor predeterminado es 1.

**Remarks**

Debe establecer FitToPagesTall en cero si desea ajustar todas las columnas en una sola página.

**Returns:**
int
### getFooter(int section) {#getFooter-int-}
```
public String getFooter(int section)
```


Obtiene un script que formatea el pie de página de un archivo Excel.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| section | int | 0: Sección izquierda, 1: Sección central, 2: Sección derecha. |

**Returns:**
java.lang.String
### getFooterMargin() {#getFooterMargin--}
```
public double getFooterMargin()
```


Representa la distancia desde la parte inferior de la página hasta el pie de página, en unidades de centímetros.

**Returns:**
double
### getFooterMarginInch() {#getFooterMarginInch--}
```
public double getFooterMarginInch()
```


Representa la distancia desde la parte inferior de la página hasta el pie de página, en unidades de pulgadas.

**Returns:**
double
### getHeader(int section) {#getHeader-int-}
```
public String getHeader(int section)
```


Obtiene un script que formatea el encabezado de un archivo Excel.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| section | int | 0: Sección izquierda, 1: Sección central, 2: Sección derecha. |

**Returns:**
java.lang.String
### getHeaderMargin() {#getHeaderMargin--}
```
public double getHeaderMargin()
```


Representa la distancia desde la parte superior de la página hasta el encabezado, en unidades de centímetros.

**Returns:**
double
### getHeaderMarginInch() {#getHeaderMarginInch--}
```
public double getHeaderMarginInch()
```


Representa la distancia desde la parte superior de la página hasta el encabezado, en unidades de pulgadas.

**Returns:**
double
### getLeftMargin() {#getLeftMargin--}
```
public double getLeftMargin()
```


Representa el tamaño del margen izquierdo, en unidades de centímetros.

**Returns:**
double
### getLeftMarginInch() {#getLeftMarginInch--}
```
public double getLeftMarginInch()
```


Representa el tamaño del margen izquierdo, en unidades de pulgadas.

**Returns:**
double
### getODSPageBackground() {#getODSPageBackground--}
```
public OdsPageBackground getODSPageBackground()
```


Obtiene el fondo de ODS.

**Returns:**
[OdsPageBackground](../../com.aspose.cells/odspagebackground)
### getOrder() {#getOrder--}
```
public int getOrder()
```


Representa el orden que Microsoft Excel utiliza para numerar las páginas al imprimir una hoja de cálculo grande.

Ver [PrintOrderType](../../com.aspose.cells/printordertype).

**Returns:**
int
### getOrientation() {#getOrientation--}
```
public int getOrientation()
```


Representa la orientación de impresión de la página.

Ver [PageOrientationType](../../com.aspose.cells/pageorientationtype).

**Returns:**
int
### getPaperHeight() {#getPaperHeight--}
```
public double getPaperHeight()
```


Obtiene la altura del papel en unidades de pulgadas, considerando la orientación de la página.

**Returns:**
double
### getPaperSize() {#getPaperSize--}
```
public int getPaperSize()
```


Representa el tamaño del papel.

Ver [PaperSizeType](../../com.aspose.cells/papersizetype).

**Returns:**
int
### getPaperWidth() {#getPaperWidth--}
```
public double getPaperWidth()
```


Obtiene el ancho del papel en unidades de pulgadas, considerando la orientación de la página.

**Returns:**
double
### getPicture(boolean isFirst, boolean isEven, boolean isHeader, int section) {#getPicture-boolean-boolean-boolean-int-}
```
public Picture getPicture(boolean isFirst, boolean isEven, boolean isHeader, int section)
```


Obtiene el objeto [Picture](../../com.aspose.cells/picture) del encabezado / pie de página.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isFirst | boolean | Indica si se está obteniendo la imagen del encabezado/pie de página de la primera página. |
| isEven | boolean | Indica si se está obteniendo la imagen del encabezado/pie de página de una página par. |
| isHeader | boolean | Indica si se obtiene la imagen del encabezado/pie de página. |
| section | int | 0: Sección izquierda, 1: Sección central, 2: Sección derecha. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### getPicture(boolean isHeader, int section) {#getPicture-boolean-int-}
```
public Picture getPicture(boolean isHeader, int section)
```


Obtiene el objeto [Picture](../../com.aspose.cells/picture) del encabezado / pie de página.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isHeader | boolean | Indica si está en el encabezado o en el pie de página. |
| section | int | 0: Sección izquierda, 1: Sección central, 2: Sección derecha. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object. Returns null if there is no picture.
### getPrintArea() {#getPrintArea--}
```
public String getPrintArea()
```


Representa el rango a imprimir.

**Returns:**
java.lang.String
### getPrintComments() {#getPrintComments--}
```
public int getPrintComments()
```


Representa la forma en que los comentarios se imprimen con la hoja.

Ver [PrintCommentsType](../../com.aspose.cells/printcommentstype).

**Returns:**
int
### getPrintCopies() {#getPrintCopies--}
```
public int getPrintCopies()
```


Obtiene el número de copias a imprimir.

**Returns:**
int
### getPrintDraft() {#getPrintDraft--}
```
public boolean getPrintDraft()
```


Representa si la hoja se imprimirá sin gráficos.

**Returns:**
boolean
### getPrintErrors() {#getPrintErrors--}
```
public int getPrintErrors()
```


Especifica el tipo de error de impresión mostrado.

Ver [PrintErrorsType](../../com.aspose.cells/printerrorstype).

**Returns:**
int
### getPrintGridlines() {#getPrintGridlines--}
```
public boolean getPrintGridlines()
```


Representa si las líneas de cuadrícula de las celdas se imprimen en la página.

**Returns:**
boolean
### getPrintHeadings() {#getPrintHeadings--}
```
public boolean getPrintHeadings()
```


Representa si los encabezados de filas y columnas se imprimen con esta página.

**Returns:**
boolean
### getPrintQuality() {#getPrintQuality--}
```
public int getPrintQuality()
```


Representa la calidad de impresión.

**Returns:**
int
### getPrintTitleColumns() {#getPrintTitleColumns--}
```
public String getPrintTitleColumns()
```


Representa las columnas que contienen las celdas que se repetirán en el lado izquierdo de cada página.

**Example**

```
         pageSetup.setPrintTitleColumns("$A:$A");
```

**Returns:**
java.lang.String
### getPrintTitleRows() {#getPrintTitleRows--}
```
public String getPrintTitleRows()
```


Representa las filas que contienen las celdas que se repetirán en la parte superior de cada página.

**Example**

```
         pageSetup.setPrintTitleRows("$1:$1");
```

**Returns:**
java.lang.String
### getPrinterSettings() {#getPrinterSettings--}
```
public byte[] getPrinterSettings()
```


Obtiene la configuración de la impresora predeterminada.

**Returns:**
byte[]
### getRightMargin() {#getRightMargin--}
```
public double getRightMargin()
```


Representa el tamaño del margen derecho, en unidades de centímetros.

**Returns:**
double
### getRightMarginInch() {#getRightMarginInch--}
```
public double getRightMarginInch()
```


Representa el tamaño del margen derecho, en unidades de pulgadas.

**Returns:**
double
### getTopMargin() {#getTopMargin--}
```
public double getTopMargin()
```


Representa el tamaño del margen superior, en unidades de centímetros.

**Returns:**
double
### getTopMarginInch() {#getTopMarginInch--}
```
public double getTopMarginInch()
```


Representa el tamaño del margen superior, en unidades de pulgadas.

**Returns:**
double
### getZoom() {#getZoom--}
```
public int getZoom()
```


Representa el factor de escala en porcentaje. Debe estar entre 10 y 400.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoFirstPageNumber() {#isAutoFirstPageNumber--}
```
public boolean isAutoFirstPageNumber()
```


Indica si el número de la primera página se asigna automáticamente.

**Returns:**
boolean
### isAutomaticPaperSize() {#isAutomaticPaperSize--}
```
public boolean isAutomaticPaperSize()
```


Indica si el tamaño del papel es automático.

**Returns:**
boolean
### isHFAlignMargins() {#isHFAlignMargins--}
```
public boolean isHFAlignMargins()
```


Indica si los márgenes del encabezado y pie de página están alineados con los márgenes de la página. Si esta propiedad es verdadera, el encabezado y pie de página izquierdo se alinearán con el margen izquierdo, y el encabezado y pie de página derecho se alinearán con el margen derecho. Esta opción está habilitada por defecto.

**Returns:**
boolean
### isHFDiffFirst() {#isHFDiffFirst--}
```
public boolean isHFDiffFirst()
```


True significa que el encabezado/pie de página de la primera página es diferente de las demás páginas.

**Returns:**
boolean
### isHFDiffOddEven() {#isHFDiffOddEven--}
```
public boolean isHFDiffOddEven()
```


True significa que el encabezado/pie de página de las páginas impares es diferente de las páginas impares.

**Returns:**
boolean
### isHFScaleWithDoc() {#isHFScaleWithDoc--}
```
public boolean isHFScaleWithDoc()
```


Indica si el encabezado y pie de página se escalan con el escalado del documento. Solo se aplica a Excel 2007.

**Returns:**
boolean
### isPercentScale() {#isPercentScale--}
```
public boolean isPercentScale()
```


Si esta propiedad es False, las propiedades FitToPagesWide y FitToPagesTall controlan cómo se escala la hoja de cálculo.

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




### setAutoFirstPageNumber(boolean value) {#setAutoFirstPageNumber-boolean-}
```
public void setAutoFirstPageNumber(boolean value)
```


Indica si el número de la primera página se asigna automáticamente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setBlackAndWhite(boolean value) {#setBlackAndWhite-boolean-}
```
public void setBlackAndWhite(boolean value)
```


Representa si los elementos del documento se imprimirán en blanco y negro.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setBottomMargin(double value) {#setBottomMargin-double-}
```
public void setBottomMargin(double value)
```


Representa el tamaño del margen inferior, en unidades de centímetros.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setBottomMarginInch(double value) {#setBottomMarginInch-double-}
```
public void setBottomMarginInch(double value)
```


Representa el tamaño del margen inferior, en unidades de pulgadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setCenterHorizontally(boolean value) {#setCenterHorizontally-boolean-}
```
public void setCenterHorizontally(boolean value)
```


Representa si la hoja se imprime centrada horizontalmente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setCenterVertically(boolean value) {#setCenterVertically-boolean-}
```
public void setCenterVertically(boolean value)
```


Representa si la hoja se imprime centrada verticalmente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setEvenFooter(int section, String footerScript) {#setEvenFooter-int-java.lang.String-}
```
public void setEvenFooter(int section, String footerScript)
```


Establece un script que formatea el pie de página de las páginas pares de un archivo Excel. Solo tiene efecto en Excel 2007 cuando IsHFDiffOddEven es verdadero.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| section | int | 0: Sección izquierda, 1: Sección central, 2: Sección derecha. |
| footerScript | java.lang.String | Script de formato de pie de página. |

### setEvenHeader(int section, String headerScript) {#setEvenHeader-int-java.lang.String-}
```
public void setEvenHeader(int section, String headerScript)
```


Establece un script que formatea el encabezado de las páginas pares de un archivo Excel. Solo tiene efecto en Excel 2007 cuando IsHFDiffOddEven es verdadero.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| section | int | 0: Sección izquierda, 1: Sección central, 2: Sección derecha. |
| headerScript | java.lang.String | Script de formato de encabezado. |

### setFirstPageFooter(int section, String footerScript) {#setFirstPageFooter-int-java.lang.String-}
```
public void setFirstPageFooter(int section, String footerScript)
```


Establece un script que formatea el pie de página de la primera página de un archivo Excel.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| section | int | 0: Sección izquierda, 1: Sección central, 2: Sección derecha. |
| footerScript | java.lang.String | Script de formato de pie de página. |

### setFirstPageHeader(int section, String headerScript) {#setFirstPageHeader-int-java.lang.String-}
```
public void setFirstPageHeader(int section, String headerScript)
```


Establece un script que formatea el encabezado de la primera página de un archivo Excel. Solo tiene efecto en Excel 2007 cuando IsHFDiffFirst es verdadero.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| section | int | 0: Sección izquierda, 1: Sección central, 2: Sección derecha. |
| headerScript | java.lang.String | Script de formato de encabezado. |

### setFirstPageNumber(int value) {#setFirstPageNumber-int-}
```
public void setFirstPageNumber(int value)
```


Representa el número de la primera página que se usará cuando se imprima esta hoja.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setFitToPages(int wide, int tall) {#setFitToPages-int-int-}
```
public void setFitToPages(int wide, int tall)
```


Establece el número de páginas a las que se escalará la hoja de cálculo cuando se imprima.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ancho | int | Páginas anchas. |
| alto | int | Páginas altas. |

### setFitToPagesTall(int value) {#setFitToPagesTall-int-}
```
public void setFitToPagesTall(int value)
```


Representa la cantidad de páginas de alto a la que se escalará la hoja de cálculo al imprimirse. El valor predeterminado es 1.

**Remarks**

Debe establecer FitToPagesWide en cero si desea ajustar todas las filas en una sola página.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setFitToPagesWide(int value) {#setFitToPagesWide-int-}
```
public void setFitToPagesWide(int value)
```


Representa la cantidad de páginas de ancho a la que se escalará la hoja de cálculo al imprimirse. El valor predeterminado es 1.

**Remarks**

Debe establecer FitToPagesTall en cero si desea ajustar todas las columnas en una sola página.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setFooter(int section, String footerScript) {#setFooter-int-java.lang.String-}
```
public void setFooter(int section, String footerScript)
```


Establece un script que da formato al pie de página de un archivo Excel.

**Remarks**

Comandos de script:

| Comando | Descripción |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &P | Número de página actual\u9286\u20ac |
| &N | Recuento de páginas\u9286\u20ac |
| &D | Fecha actual\u9286\u20ac |
| &T | Hora actual |
| &A | Nombre de hoja |
| &F | Nombre de archivo sin ruta |
| &"<FontName>" | Nombre de fuente, por ejemplo: &"Arial" |
| &"<FontName>, <FontStyle>" | Nombre de fuente y estilo de fuente, por ejemplo: &"Arial,Bold" |
| &<FontSize> | Tamaño de fuente. Si este comando es seguido por un número simple que se imprimirá en el encabezado, se separará de la altura de la fuente con un carácter de espacio. |
| &K<RRGGBB> | Color de fuente, por ejemplo(ROJO): &KFF0000 |
| &G | Script de imagen |

Por ejemplo: "&Arial,Bold&8Footer Note"

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| section | int | 0: Sección izquierda, 1: Sección central, 2: Sección derecha. |
| footerScript | java.lang.String | Script de formato de pie de página. |

### setFooterMargin(double value) {#setFooterMargin-double-}
```
public void setFooterMargin(double value)
```


Representa la distancia desde la parte inferior de la página hasta el pie de página, en unidades de centímetros.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setFooterMarginInch(double value) {#setFooterMarginInch-double-}
```
public void setFooterMarginInch(double value)
```


Representa la distancia desde la parte inferior de la página hasta el pie de página, en unidades de pulgadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setFooterPicture(int section, byte[] footerPicture) {#setFooterPicture-int-byte---}
```
public Picture setFooterPicture(int section, byte[] footerPicture)
```


Establece una imagen en el pie de página de una hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| section | int | 0: Sección izquierda, 1: Sección central, 2: Sección derecha. |
| footerPicture | byte[] | Datos de imagen. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### setHFAlignMargins(boolean value) {#setHFAlignMargins-boolean-}
```
public void setHFAlignMargins(boolean value)
```


Indica si los márgenes del encabezado y pie de página están alineados con los márgenes de la página. Si esta propiedad es verdadera, el encabezado y pie de página izquierdo se alinearán con el margen izquierdo, y el encabezado y pie de página derecho se alinearán con el margen derecho. Esta opción está habilitada por defecto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setHFDiffFirst(boolean value) {#setHFDiffFirst-boolean-}
```
public void setHFDiffFirst(boolean value)
```


True significa que el encabezado/pie de página de la primera página es diferente de las demás páginas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setHFDiffOddEven(boolean value) {#setHFDiffOddEven-boolean-}
```
public void setHFDiffOddEven(boolean value)
```


True significa que el encabezado/pie de página de las páginas impares es diferente de las páginas impares.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setHFScaleWithDoc(boolean value) {#setHFScaleWithDoc-boolean-}
```
public void setHFScaleWithDoc(boolean value)
```


Indica si el encabezado y pie de página se escalan con el escalado del documento. Solo se aplica a Excel 2007.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setHeader(int section, String headerScript) {#setHeader-int-java.lang.String-}
```
public void setHeader(int section, String headerScript)
```


Establece un script que da formato al encabezado de un archivo Excel.

**Remarks**

Comandos de script:

| Comando | Descripción |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| &P | Número de página actual\u9286\u20ac |
| &N | Recuento de páginas\u9286\u20ac |
| &D | Fecha actual\u9286\u20ac |
| &T | Hora actual |
| &A | Nombre de hoja |
| &F | Nombre de archivo sin ruta |
| &"<FontName>" | Nombre de fuente, por ejemplo: &"Arial" |
| &"<FontName>, <FontStyle>" | Nombre de fuente y estilo de fuente, por ejemplo: &"Arial,Bold" |
| &<FontSize> | Tamaño de fuente. Si este comando es seguido por un número simple que se imprimirá en el encabezado, se separará de la altura de la fuente con un carácter de espacio. |
| &K<RRGGBB> | Color de fuente, por ejemplo(ROJO): &KFF0000 |
| &G | Script de imagen |

Por ejemplo: "&Arial,Bold&8Header Note"

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| section | int | 0: Sección izquierda, 1: Sección central, 2: Sección derecha. |
| headerScript | java.lang.String | Script de formato de encabezado. |

### setHeaderMargin(double value) {#setHeaderMargin-double-}
```
public void setHeaderMargin(double value)
```


Representa la distancia desde la parte superior de la página hasta el encabezado, en unidades de centímetros.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setHeaderMarginInch(double value) {#setHeaderMarginInch-double-}
```
public void setHeaderMarginInch(double value)
```


Representa la distancia desde la parte superior de la página hasta el encabezado, en unidades de pulgadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setHeaderPicture(int section, byte[] headerPicture) {#setHeaderPicture-int-byte---}
```
public Picture setHeaderPicture(int section, byte[] headerPicture)
```


Establece una imagen en el encabezado de una hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| section | int | 0: Sección izquierda, 1: Sección central, 2: Sección derecha. |
| headerPicture | byte[] | Datos de imagen. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### setLeftMargin(double value) {#setLeftMargin-double-}
```
public void setLeftMargin(double value)
```


Representa el tamaño del margen izquierdo, en unidades de centímetros.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setLeftMarginInch(double value) {#setLeftMarginInch-double-}
```
public void setLeftMarginInch(double value)
```


Representa el tamaño del margen izquierdo, en unidades de pulgadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setOrder(int value) {#setOrder-int-}
```
public void setOrder(int value)
```


Representa el orden que Microsoft Excel utiliza para numerar las páginas al imprimir una hoja de cálculo grande.

Ver [PrintOrderType](../../com.aspose.cells/printordertype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setOrientation(int value) {#setOrientation-int-}
```
public void setOrientation(int value)
```


Representa la orientación de impresión de la página.

Ver [PageOrientationType](../../com.aspose.cells/pageorientationtype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setPaperSize(int value) {#setPaperSize-int-}
```
public void setPaperSize(int value)
```


Representa el tamaño del papel.

Ver [PaperSizeType](../../com.aspose.cells/papersizetype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setPercentScale(boolean value) {#setPercentScale-boolean-}
```
public void setPercentScale(boolean value)
```


Si esta propiedad es False, las propiedades FitToPagesWide y FitToPagesTall controlan cómo se escala la hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setPicture(boolean isFirst, boolean isEven, boolean isHeader, int section, byte[] imageData) {#setPicture-boolean-boolean-boolean-int-byte---}
```
public Picture setPicture(boolean isFirst, boolean isEven, boolean isHeader, int section, byte[] imageData)
```


Establece una imagen en el encabezado/pie de página de una hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isFirst | boolean | Indica si se establece la imagen del encabezado/pie de página de la primera página. |
| isEven | boolean | Indica si se establece la imagen del encabezado/pie de página de las páginas pares. |
| isHeader | boolean | Indica si se establece la imagen del encabezado/pie de página. |
| section | int | 0: Sección izquierda, 1: Sección central, 2: Sección derecha. |
| imageData | byte[] | Datos de imagen. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns [Picture](../../com.aspose.cells/picture) object.
### setPrintArea(String value) {#setPrintArea-java.lang.String-}
```
public void setPrintArea(String value)
```


Representa el rango a imprimir.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setPrintComments(int value) {#setPrintComments-int-}
```
public void setPrintComments(int value)
```


Representa la forma en que los comentarios se imprimen con la hoja.

Ver [PrintCommentsType](../../com.aspose.cells/printcommentstype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setPrintCopies(int value) {#setPrintCopies-int-}
```
public void setPrintCopies(int value)
```


Establece el número de copias a imprimir.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setPrintDraft(boolean value) {#setPrintDraft-boolean-}
```
public void setPrintDraft(boolean value)
```


Representa si la hoja se imprimirá sin gráficos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setPrintErrors(int value) {#setPrintErrors-int-}
```
public void setPrintErrors(int value)
```


Especifica el tipo de error de impresión mostrado.

Ver [PrintErrorsType](../../com.aspose.cells/printerrorstype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setPrintGridlines(boolean value) {#setPrintGridlines-boolean-}
```
public void setPrintGridlines(boolean value)
```


Representa si las líneas de cuadrícula de las celdas se imprimen en la página.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setPrintHeadings(boolean value) {#setPrintHeadings-boolean-}
```
public void setPrintHeadings(boolean value)
```


Representa si los encabezados de filas y columnas se imprimen con esta página.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setPrintQuality(int value) {#setPrintQuality-int-}
```
public void setPrintQuality(int value)
```


Representa la calidad de impresión.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setPrintTitleColumns(String value) {#setPrintTitleColumns-java.lang.String-}
```
public void setPrintTitleColumns(String value)
```


Representa las columnas que contienen las celdas que se repetirán en el lado izquierdo de cada página.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setPrintTitleRows(String value) {#setPrintTitleRows-java.lang.String-}
```
public void setPrintTitleRows(String value)
```


Representa las filas que contienen las celdas que se repetirán en la parte superior de cada página.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setPrinterSettings(byte[] value) {#setPrinterSettings-byte---}
```
public void setPrinterSettings(byte[] value)
```


Establece la configuración de la impresora predeterminada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | byte[] |  |

### setRightMargin(double value) {#setRightMargin-double-}
```
public void setRightMargin(double value)
```


Representa el tamaño del margen derecho, en unidades de centímetros.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setRightMarginInch(double value) {#setRightMarginInch-double-}
```
public void setRightMarginInch(double value)
```


Representa el tamaño del margen derecho, en unidades de pulgadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setTopMargin(double value) {#setTopMargin-double-}
```
public void setTopMargin(double value)
```


Representa el tamaño del margen superior, en unidades de centímetros.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setTopMarginInch(double value) {#setTopMarginInch-double-}
```
public void setTopMarginInch(double value)
```


Representa el tamaño del margen superior, en unidades de pulgadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setZoom(int value) {#setZoom-int-}
```
public void setZoom(int value)
```


Representa el factor de escala en porcentaje. Debe estar entre 10 y 400.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

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

