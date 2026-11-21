---
title: "WorkbookPrintingPreview"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Vista previa de impresión del libro de trabajo."
type: docs
url: /es/java/com.aspose.cells/workbookprintingpreview/
---

**Inheritance:**
java.lang.Object
```
public class WorkbookPrintingPreview
```

Vista previa de impresión del libro de trabajo.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [WorkbookPrintingPreview(Workbook workbook, ImageOrPrintOptions options)](#WorkbookPrintingPreview-com.aspose.cells.Workbook-com.aspose.cells.ImageOrPrintOptions-) | La construcción de WorkbookPrintingPreview |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getEvaluatedPageCount()](#getEvaluatedPageCount--) | Evaluar el recuento total de páginas de este libro de trabajo |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### WorkbookPrintingPreview(Workbook workbook, ImageOrPrintOptions options) {#WorkbookPrintingPreview-com.aspose.cells.Workbook-com.aspose.cells.ImageOrPrintOptions-}
```
public WorkbookPrintingPreview(Workbook workbook, ImageOrPrintOptions options)
```


La construcción de WorkbookPrintingPreview

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| workbook | [Workbook](../../com.aspose.cells/workbook) | Indicar qué libro de trabajo se imprimirá. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | ImageOrPrintOptions contiene algunas propiedades de salida |

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
### getEvaluatedPageCount() {#getEvaluatedPageCount--}
```
public int getEvaluatedPageCount()
```


Evaluar el recuento total de páginas de este libro de trabajo

**Example**

El siguiente código muestra la forma más rápida de obtener el recuento de páginas de un libro de trabajo.

```
         Workbook workbook = new Workbook("Book1.xlsx");
 
         WorkbookPrintingPreview workbookPrintingPreview = new WorkbookPrintingPreview(workbook, new ImageOrPrintOptions());
 
         //fastest way to get page count especailly when there are massive data in workbook.
         System.out.println(workbookPrintingPreview.getEvaluatedPageCount());
```

**Returns:**
int
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

