---
title: "WorkbookPrintingPreview"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Aperçu d'impression du classeur."
type: docs
url: /fr/java/com.aspose.cells/workbookprintingpreview/
---

**Inheritance:**
java.lang.Object
```
public class WorkbookPrintingPreview
```

Aperçu d'impression du classeur.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [WorkbookPrintingPreview(Workbook workbook, ImageOrPrintOptions options)](#WorkbookPrintingPreview-com.aspose.cells.Workbook-com.aspose.cells.ImageOrPrintOptions-) | La construction de WorkbookPrintingPreview |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getEvaluatedPageCount()](#getEvaluatedPageCount--) | Évaluer le nombre total de pages de ce classeur |
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


La construction de WorkbookPrintingPreview

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| workbook | [Workbook](../../com.aspose.cells/workbook) | Indiquer quel classeur doit être imprimé. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | ImageOrPrintOptions contient certaines propriétés de sortie |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Paramètre | Type | Description |
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


Évaluer le nombre total de pages de ce classeur

**Example**

Le code suivant montre la façon la plus rapide d'obtenir le nombre de pages d'un classeur.

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
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

