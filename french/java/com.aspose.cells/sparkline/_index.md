---
title: "Sparkline"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Un sparkline représente un petit graphique ou une petite illustration dans une cellule de feuille de calcul qui fournit une représentation visuelle des données."
type: docs
url: /fr/java/com.aspose.cells/sparkline/
---

**Inheritance:**
java.lang.Object
```
public class Sparkline
```

Un sparkline représente un petit graphique ou une petite illustration dans une cellule de feuille de calcul qui fournit une représentation visuelle des données.

**Example**

```
         Workbook book = new Workbook(); 
         Worksheet sheet = book.getWorksheets().get(0);
 
         sheet.getCells().get("A1").putValue(5);
         sheet.getCells().get("B1").putValue(2);
         sheet.getCells().get("C1").putValue(1);
         sheet.getCells().get("D1").putValue(3);
 
         // Define the CellArea
         CellArea ca = new CellArea();
         ca.StartColumn = 4;
         ca.EndColumn = 4;
         ca.StartRow = 0;
         ca.EndRow = 0;
 
         int idx = sheet.getSparklineGroups().add(com.aspose.cells.SparklineType.LINE, sheet.getName() + "!A1:D1", false, ca);
 
         SparklineGroup group = sheet.getSparklineGroups().get(idx);
         idx = group.getSparklines().add(sheet.getName() + "!A1:D1", 0, 4);
         Sparkline line = group.getSparklines().get(idx);
         System.out.println("Saprkline data range: " + line.getDataRange() + ", row: " + line.getRow() + ", column: " + line.getColumn());
         line.toImage("output.png", new ImageOrPrintOptions());
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Obtient l'index de colonne du sparkline. |
| [getDataRange()](#getDataRange--) | Représente la plage de données du sparkline. |
| [getRow()](#getRow--) | Obtient l'index de ligne du sparkline. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDataRange(String value)](#setDataRange-java.lang.String-) | Représente la plage de données du sparkline. |
| [toImage(OutputStream stream, ImageOrPrintOptions options)](#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-) | Convertit un sparkline en image. |
| [toImage(String fileName, ImageOrPrintOptions options)](#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-) | Convertit un sparkline en image. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getColumn() {#getColumn--}
```
public int getColumn()
```


Obtient l'index de colonne du sparkline.

**Returns:**
int
### getDataRange() {#getDataRange--}
```
public String getDataRange()
```


Représente la plage de données du sparkline.

**Returns:**
java.lang.String
### getRow() {#getRow--}
```
public int getRow()
```


Obtient l'index de ligne du sparkline.

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




### setDataRange(String value) {#setDataRange-java.lang.String-}
```
public void setDataRange(String value)
```


Représente la plage de données du sparkline.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### toImage(OutputStream stream, ImageOrPrintOptions options) {#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(OutputStream stream, ImageOrPrintOptions options)
```


Convertit un sparkline en image.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | Le flux d'image. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | Les options d'image. |

### toImage(String fileName, ImageOrPrintOptions options) {#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(String fileName, ImageOrPrintOptions options)
```


Convertit un sparkline en image.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | Le nom de fichier d'image. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | Les options d'image |

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

