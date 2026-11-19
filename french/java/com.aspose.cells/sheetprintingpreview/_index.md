---
title: "SheetPrintingPreview"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Aperçu d'impression de la feuille de calcul."
type: docs
url: /fr/java/com.aspose.cells/sheetprintingpreview/
---

**Inheritance:**
java.lang.Object
```
public class SheetPrintingPreview
```

Aperçu d'impression de la feuille de calcul.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [SheetPrintingPreview(Worksheet sheet, ImageOrPrintOptions options)](#SheetPrintingPreview-com.aspose.cells.Worksheet-com.aspose.cells.ImageOrPrintOptions-) | La construction de SheetPrintingPreview |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getEvaluatedPageCount()](#getEvaluatedPageCount--) | Évaluer le nombre total de pages de cette feuille de calcul |
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


La construction de SheetPrintingPreview

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sheet | [Worksheet](../../com.aspose.cells/worksheet) | Indiquer quelle feuille de calcul doit être imprimée. |
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


Évaluer le nombre total de pages de cette feuille de calcul

**Example**

Le code suivant montre la façon la plus rapide d'obtenir le nombre de pages d'une feuille de calcul.

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

