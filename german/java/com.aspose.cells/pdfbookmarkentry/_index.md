---
title: "PdfBookmarkEntry"
second_title: "Aspose.Cells for Java API-Referenz"
description: "PdfBookmarkEntry ist ein Eintrag im PDF‑Lesezeichen."
type: docs
url: /de/java/com.aspose.cells/pdfbookmarkentry/
---

**Inheritance:**
java.lang.Object
```
public class PdfBookmarkEntry
```

PdfBookmarkEntry ist ein Eintrag im PDF-Lesezeichen. Wenn die Text‑Eigenschaft der aktuellen Instanz null oder "" ist, wird die aktuelle Instanz ausgeblendet und die Kind‑Einträge werden auf derselben Ebene eingefügt.

**Example**

```
         Workbook workbook = new Workbook();
         workbook.getWorksheets().add();
         workbook.getWorksheets().add();
         Cell cellInPage1 = workbook.getWorksheets().get(0).getCells().get("A1");
         Cell cellInPage2 = workbook.getWorksheets().get(1).getCells().get("A1");
         Cell cellInPage3 = workbook.getWorksheets().get(2).getCells().get("A1");
         cellInPage1.putValue("page1");
         cellInPage2.putValue("page2");
         cellInPage3.putValue("page3");
 
         PdfBookmarkEntry pbeRoot = new PdfBookmarkEntry();
         pbeRoot.setText("root");  // if pbeRoot.Text = null, all children of pbeRoot will be inserted on the top level in the bookmark.
         pbeRoot.setDestination(cellInPage1);
         pbeRoot.setSubEntry(new ArrayList());
         pbeRoot.setOpen(false);
 
         PdfBookmarkEntry subPbe1 = new PdfBookmarkEntry();
         subPbe1.setText("section1");
         subPbe1.setDestination(cellInPage2);
 
         PdfBookmarkEntry subPbe2 = new PdfBookmarkEntry();
         subPbe2.setText("section2");
         subPbe2.setDestination(cellInPage3);
 
         pbeRoot.getSubEntry().add(subPbe1);
         pbeRoot.getSubEntry().add(subPbe2);
 
         PdfSaveOptions saveOptions = new PdfSaveOptions();
         saveOptions.setBookmark(pbeRoot);
         workbook.save("output_bookmark.pdf", saveOptions);
```
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [PdfBookmarkEntry()](#PdfBookmarkEntry--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDestination()](#getDestination--) | Die Zelle, zu der der Lesezeichen‑Link führt. |
| [getDestinationName()](#getDestinationName--) | Liefert den Namen des Ziels. |
| [getSubEntry()](#getSubEntry--) | UnterEintrag eines Lesezeichens. |
| [getText()](#getText--) | Titel eines Lesezeichens. |
| [hashCode()](#hashCode--) |  |
| [isCollapse()](#isCollapse--) | Wenn diese Eigenschaft true ist, wird der Lesezeicheneintrag zusammengeklappt, andernfalls wird er erweitert. |
| [isOpen()](#isOpen--) | Wenn diese Eigenschaft true ist, wird der Lesezeicheneintrag erweitert, andernfalls wird er zusammengeklappt. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCollapse(boolean value)](#setCollapse-boolean-) | Wenn diese Eigenschaft true ist, wird der Lesezeicheneintrag zusammengeklappt, andernfalls wird er erweitert. |
| [setDestination(Cell value)](#setDestination-com.aspose.cells.Cell-) | Die Zelle, zu der der Lesezeichen‑Link führt. |
| [setDestinationName(String value)](#setDestinationName-java.lang.String-) | Setzt den Namen des Ziels. |
| [setOpen(boolean value)](#setOpen-boolean-) | Wenn diese Eigenschaft true ist, wird der Lesezeicheneintrag erweitert, andernfalls wird er zusammengeklappt. |
| [setSubEntry(ArrayList value)](#setSubEntry-java.util.ArrayList-) | UnterEintrag eines Lesezeichens. |
| [setText(String value)](#setText-java.lang.String-) | Titel eines Lesezeichens. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PdfBookmarkEntry() {#PdfBookmarkEntry--}
```
public PdfBookmarkEntry()
```


### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
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
### getDestination() {#getDestination--}
```
public Cell getDestination()
```


Die Zelle, zu der der Lesezeichen‑Link führt.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getDestinationName() {#getDestinationName--}
```
public String getDestinationName()
```


Liefert den Namen des Ziels.

**Remarks**

Wenn der Zielname festgelegt ist, wird das Ziel als benanntes Ziel mit diesem Namen definiert.

**Returns:**
java.lang.String
### getSubEntry() {#getSubEntry--}
```
public ArrayList getSubEntry()
```


UnterEintrag eines Lesezeichens.

**Returns:**
java.util.ArrayList
### getText() {#getText--}
```
public String getText()
```


Titel eines Lesezeichens.

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCollapse() {#isCollapse--}
```
public boolean isCollapse()
```


Wenn diese Eigenschaft true ist, wird der Lesezeicheneintrag zusammengeklappt, andernfalls wird er erweitert.

**Returns:**
boolean
### isOpen() {#isOpen--}
```
public boolean isOpen()
```


Wenn diese Eigenschaft true ist, wird der Lesezeicheneintrag erweitert, andernfalls wird er zusammengeklappt.

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




### setCollapse(boolean value) {#setCollapse-boolean-}
```
public void setCollapse(boolean value)
```


Wenn diese Eigenschaft true ist, wird der Lesezeicheneintrag zusammengeklappt, andernfalls wird er erweitert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setDestination(Cell value) {#setDestination-com.aspose.cells.Cell-}
```
public void setDestination(Cell value)
```


Die Zelle, zu der der Lesezeichen‑Link führt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Cell](../../com.aspose.cells/cell) |  |

### setDestinationName(String value) {#setDestinationName-java.lang.String-}
```
public void setDestinationName(String value)
```


Setzt den Namen des Ziels.

**Remarks**

Wenn der Zielname festgelegt ist, wird das Ziel als benanntes Ziel mit diesem Namen definiert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setOpen(boolean value) {#setOpen-boolean-}
```
public void setOpen(boolean value)
```


Wenn diese Eigenschaft true ist, wird der Lesezeicheneintrag erweitert, andernfalls wird er zusammengeklappt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSubEntry(ArrayList value) {#setSubEntry-java.util.ArrayList-}
```
public void setSubEntry(ArrayList value)
```


UnterEintrag eines Lesezeichens.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.ArrayList |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Titel eines Lesezeichens.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

