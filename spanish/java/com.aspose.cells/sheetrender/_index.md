---
title: "SheetRender"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa una representación de hoja de cálculo que puede renderizar la hoja a varias imágenes como BMP PNG JPEG TIFF.."
type: docs
url: /es/java/com.aspose.cells/sheetrender/
---

**Inheritance:**
java.lang.Object
```
public class SheetRender
```

Representa una representación de hoja de cálculo que puede renderizar la hoja a varias imágenes como (BMP, PNG, JPEG, TIFF..). El constructor de esta clase debe usarse después de modificar la configuración de página, el estilo de celda.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [SheetRender(Worksheet worksheet, ImageOrPrintOptions options)](#SheetRender-com.aspose.cells.Worksheet-com.aspose.cells.ImageOrPrintOptions-) | la construcción de SheetRender, necesita hoja de cálculo y ImageOrPrintOptions como parámetros |
## Métodos

| Método | Descripción |
| --- | --- |
| [dispose()](#dispose--) | Libera los recursos creados y usados para la renderización. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPageCount()](#getPageCount--) | Obtiene el recuento total de páginas de la hoja de cálculo actual. |
| [getPageScale()](#getPageScale--) | Obtiene la escala de página calculada de la hoja. |
| [getPageSizeInch(int pageIndex)](#getPageSizeInch-int-) | Obtiene el tamaño de página en pulgadas de la imagen de salida. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toImage(int pageIndex, InputStream stream)](#toImage-int-java.io.InputStream-) | Renderiza una página determinada a un flujo. |
| [toImage(int pageIndex, OutputStream stream)](#toImage-int-java.io.OutputStream-) | Renderiza una página determinada a un flujo. |
| [toImage(int pageIndex, String fileName)](#toImage-int-java.lang.String-) | Renderiza una página determinada a un archivo. |
| [toPrinter(String printerName)](#toPrinter-java.lang.String-) | Renderiza la hoja de cálculo a la impresora |
| [toPrinter(String printerName, int printPageIndex, int printPageCount)](#toPrinter-java.lang.String-int-int-) | Renderiza la hoja de cálculo a la impresora |
| [toPrinter(String printerName, String jobName)](#toPrinter-java.lang.String-java.lang.String-) | Renderiza la hoja de cálculo a la impresora |
| [toString()](#toString--) |  |
| [toTiff(InputStream stream)](#toTiff-java.io.InputStream-) | Renderiza toda la hoja de cálculo como imagen Tiff al flujo. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SheetRender(Worksheet worksheet, ImageOrPrintOptions options) {#SheetRender-com.aspose.cells.Worksheet-com.aspose.cells.ImageOrPrintOptions-}
```
public SheetRender(Worksheet worksheet, ImageOrPrintOptions options)
```


la construcción de SheetRender, necesita hoja de cálculo y ImageOrPrintOptions como parámetros

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| worksheet | [Worksheet](../../com.aspose.cells/worksheet) | Indica qué hoja de cálculo se debe renderizar. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | ImageOrPrintOptions contiene algunas propiedades de la imagen de salida |

### dispose() {#dispose--}
```
public void dispose()
```


Libera los recursos creados y usados para la renderización.

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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getPageCount() {#getPageCount--}
```
public int getPageCount()
```


Obtiene el recuento total de páginas de la hoja de cálculo actual.

**Returns:**
int
### getPageScale() {#getPageScale--}
```
public double getPageScale()
```


Obtiene la escala de página calculada de la hoja. Devuelve la escala establecida si [PageSetup.getZoom()](../../com.aspose.cells/pagesetup\#getZoom--) está configurada. De lo contrario, devuelve la escala calculada según [PageSetup.getFitToPagesWide()](../../com.aspose.cells/pagesetup\#getFitToPagesWide--) y [PageSetup.getFitToPagesTall()](../../com.aspose.cells/pagesetup\#getFitToPagesTall--).

**Example**

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         SheetRender sheetRender = new SheetRender(wb.getWorksheets().get(0), new ImageOrPrintOptions());
 
         //Gets calculated page scale of the sheet.
         double pageScale = sheetRender.getPageScale();
```

**Returns:**
double
### getPageSizeInch(int pageIndex) {#getPageSizeInch-int-}
```
public float[] getPageSizeInch(int pageIndex)
```


Obtiene el tamaño de página en pulgadas de la imagen de salida.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pageIndex | int | El índice de página se basa en cero. |

**Returns:**
float[] - Tamaño de página de la imagen, [0] para ancho y [1] para alto
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### toImage(int pageIndex, InputStream stream) {#toImage-int-java.io.InputStream-}
```
public void toImage(int pageIndex, InputStream stream)
```


Renderiza una página determinada a un flujo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pageIndex | int | indica qué página se debe convertir |
| stream | java.io.InputStream | el flujo de la imagen de salida |

### toImage(int pageIndex, OutputStream stream) {#toImage-int-java.io.OutputStream-}
```
public void toImage(int pageIndex, OutputStream stream)
```


Renderiza una página determinada a un flujo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pageIndex | int | indica qué página se debe convertir |
| stream | java.io.OutputStream | el flujo de la imagen de salida |

### toImage(int pageIndex, String fileName) {#toImage-int-java.lang.String-}
```
public void toImage(int pageIndex, String fileName)
```


Renderiza una página determinada a un archivo.

**Example**

El siguiente código genera la primera página de la primera hoja en una imagen png.

```
         //load the source file with images.
         Workbook wb = new Workbook("Book1.xlsx");
 
         ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
 
         //set output image type.
         imgOpt.setImageType(ImageType.PNG);
 
         //render the first sheet.
         SheetRender sr = new SheetRender(wb.getWorksheets().get(0), imgOpt);
 
         //output the first page of the sheet to image.
         sr.toImage(0, "output.png");
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pageIndex | int | indica qué página se debe convertir |
| fileName | java.lang.String | nombre de archivo de la imagen de salida |

### toPrinter(String printerName) {#toPrinter-java.lang.String-}
```
public void toPrinter(String printerName)
```


Renderiza la hoja de cálculo a la impresora

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| printerName | java.lang.String | el nombre de la impresora, por ejemplo: "Microsoft Office Document Image Writer" |

### toPrinter(String printerName, int printPageIndex, int printPageCount) {#toPrinter-java.lang.String-int-int-}
```
public void toPrinter(String printerName, int printPageIndex, int printPageCount)
```


Renderiza la hoja de cálculo a la impresora

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice ToPrinter(string PrinterName) y ImageOrPrintOptions.PageIndex, PageCount para establecer la primera página y el número de páginas a imprimir. Esta propiedad será eliminada 12 meses después desde diciembre de 2021. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| printerName | java.lang.String | el nombre de la impresora, por ejemplo: "Microsoft Office Document Image Writer" |
| printPageIndex | int | el índice basado en cero de la primera página a imprimir, debe estar en el rango [0, SheetRender.PageCount-1] |
| printPageCount | int | el número de páginas a imprimir, debe ser mayor que cero |

### toPrinter(String printerName, String jobName) {#toPrinter-java.lang.String-java.lang.String-}
```
public void toPrinter(String printerName, String jobName)
```


Renderiza la hoja de cálculo a la impresora

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| printerName | java.lang.String | el nombre de la impresora, por ejemplo: "Microsoft Office Document Image Writer" |
| jobName | java.lang.String | establecer el nombre del trabajo de impresión |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### toTiff(InputStream stream) {#toTiff-java.io.InputStream-}
```
public void toTiff(InputStream stream)
```


Renderiza toda la hoja de cálculo como imagen Tiff al flujo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.InputStream | el flujo de la imagen de salida |

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

