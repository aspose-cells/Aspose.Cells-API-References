---
title: "SheetPrintingPreview"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Anteprima di stampa del foglio di lavoro."
type: docs
url: /it/java/com.aspose.cells/sheetprintingpreview/
---

**Inheritance:**
java.lang.Object
```
public class SheetPrintingPreview
```

Anteprima di stampa del foglio di lavoro.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [SheetPrintingPreview(Worksheet sheet, ImageOrPrintOptions options)](#SheetPrintingPreview-com.aspose.cells.Worksheet-com.aspose.cells.ImageOrPrintOptions-) | La struttura di SheetPrintingPreview |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getEvaluatedPageCount()](#getEvaluatedPageCount--) | Calcola il numero totale di pagine di questo foglio di lavoro |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SheetPrintingPreview(Worksheet sheet, ImageOrPrintOptions options) {#SheetPrintingPreview-com.aspose.cells.Worksheet-com.aspose.cells.ImageOrPrintOptions-}
```
public SheetPrintingPreview(Worksheet sheet, ImageOrPrintOptions options)
```


La struttura di SheetPrintingPreview

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheet | [Worksheet](../../com.aspose.cells/worksheet) | Indica quale foglio di calcolo deve essere stampato. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | ImageOrPrintOptions contiene alcune proprietà di output |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
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


Calcola il numero totale di pagine di questo foglio di lavoro

**Example**

Il codice seguente mostra il modo più veloce per ottenere il conteggio delle pagine di un foglio di lavoro.

```
         Workbook workbook = new Workbook("Book1.xlsx");
 
         SheetPrintingPreview sheetPrintingPreview = new SheetPrintingPreview(workbook.getWorksheets().get(0), new ImageOrPrintOptions());
 
         //fastest way to get page count especailly when there are massive data in worksheet.
         System.out.println(sheetPrintingPreview.getEvaluatedPageCount());
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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

