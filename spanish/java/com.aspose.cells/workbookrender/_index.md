---
title: "WorkbookRender"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa una representación de libro de trabajo."
type: docs
url: /es/java/com.aspose.cells/workbookrender/
---

**Inheritance:**
java.lang.Object
```
public class WorkbookRender
```

Representa una renderización de Workbook. El constructor de esta clase debe usarse después de la modificación de la configuración de página y el estilo de celda.

**Remarks**
## Constructores

| Constructor | Descripción |
| --- | --- |
| [WorkbookRender(Workbook workbook, ImageOrPrintOptions options)](#WorkbookRender-com.aspose.cells.Workbook-com.aspose.cells.ImageOrPrintOptions-) | El constructor de WorkbookRender |
## Métodos

| Método | Descripción |
| --- | --- |
| [dispose()](#dispose--) | Libera los recursos creados y usados para la renderización. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPageCount()](#getPageCount--) | Obtiene el recuento total de páginas del workbook. |
| [getPageSizeInch(int pageIndex)](#getPageSizeInch-int-) | Obtiene el tamaño de página en pulgadas de la imagen de salida. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toImage(int pageIndex, InputStream stream)](#toImage-int-java.io.InputStream-) | Renderiza una página determinada a un flujo. |
| [toImage(int pageIndex, OutputStream stream)](#toImage-int-java.io.OutputStream-) | Renderiza una página determinada a un flujo. |
| [toImage(int pageIndex, String fileName)](#toImage-int-java.lang.String-) | Renderiza una página determinada a un archivo. |
| [toImage(OutputStream stream)](#toImage-java.io.OutputStream-) | Renderiza todo el workbook como imagen Tiff a un flujo. |
| [toImage(String filename)](#toImage-java.lang.String-) | Renderiza todo el workbook como imagen Tiff a un archivo. |
| [toPrinter(String printerName)](#toPrinter-java.lang.String-) | Renderiza el workbook a la impresora |
| [toPrinter(String printerName, int printPageIndex, int printPageCount)](#toPrinter-java.lang.String-int-int-) | Renderiza el workbook a la impresora |
| [toPrinter(String printerName, String jobName)](#toPrinter-java.lang.String-java.lang.String-) | Renderiza el workbook a la impresora |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### WorkbookRender(Workbook workbook, ImageOrPrintOptions options) {#WorkbookRender-com.aspose.cells.Workbook-com.aspose.cells.ImageOrPrintOptions-}
```
public WorkbookRender(Workbook workbook, ImageOrPrintOptions options)
```


El constructor de WorkbookRender

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| workbook | [Workbook](../../com.aspose.cells/workbook) | Indica qué workbook se debe renderizar. |
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


Obtiene el recuento total de páginas del workbook.

**Returns:**
int
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

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pageIndex | int | indica qué página se debe convertir |
| fileName | java.lang.String | nombre de archivo de la imagen de salida |

### toImage(OutputStream stream) {#toImage-java.io.OutputStream-}
```
public void toImage(OutputStream stream)
```


Renderiza todo el workbook como imagen Tiff a un flujo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.OutputStream | el flujo de la imagen de salida |

### toImage(String filename) {#toImage-java.lang.String-}
```
public void toImage(String filename)
```


Renderiza todo el workbook como imagen Tiff a un archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre de archivo | java.lang.String | el nombre de archivo de la imagen de salida |

### toPrinter(String printerName) {#toPrinter-java.lang.String-}
```
public void toPrinter(String printerName)
```


Renderiza el workbook a la impresora

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| printerName | java.lang.String | el nombre de la impresora, por ejemplo: "Microsoft Office Document Image Writer" |

### toPrinter(String printerName, int printPageIndex, int printPageCount) {#toPrinter-java.lang.String-int-int-}
```
public void toPrinter(String printerName, int printPageIndex, int printPageCount)
```


Renderiza el workbook a la impresora

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, utilice ToPrinter(string PrinterName) y ImageOrPrintOptions.PageIndex, PageCount para establecer la primera página y el número de páginas a imprimir. Esta propiedad será eliminada 12 meses después desde diciembre de 2021. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| printerName | java.lang.String | el nombre de la impresora, por ejemplo: "Microsoft Office Document Image Writer" |
| printPageIndex | int | el índice basado en cero de la primera página a imprimir, debe estar en el rango [0, WorkbookRender.PageCount-1] |
| printPageCount | int | el número de páginas a imprimir, debe ser mayor que cero |

### toPrinter(String printerName, String jobName) {#toPrinter-java.lang.String-java.lang.String-}
```
public void toPrinter(String printerName, String jobName)
```


Renderiza el workbook a la impresora

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

