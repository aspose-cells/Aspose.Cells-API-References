---
title: "PdfBookmarkEntry"
second_title: "Aspose.Cells för Java API-referens"
description: "PdfBookmarkEntry är ett objekt i PDF-bokmärket."
type: docs
url: /sv/java/com.aspose.cells/pdfbookmarkentry/
---

**Inheritance:**
java.lang.Object
```
public class PdfBookmarkEntry
```

PdfBookmarkEntry är ett objekt i pdf-bokmärket. Om Text‑egenskapen för den aktuella instansen är null eller "", kommer den aktuella instansen att döljas och barnobjekt kommer att infogas på samma nivå.

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
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [PdfBookmarkEntry()](#PdfBookmarkEntry--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDestination()](#getDestination--) | Den cell som bokmärkeslänken pekar på. |
| [getDestinationName()](#getDestinationName--) | Hämtar namn på destinationen. |
| [getSubEntry()](#getSubEntry--) | Underpost för ett bokmärke. |
| [getText()](#getText--) | Titel för ett bokmärke. |
| [hashCode()](#hashCode--) |  |
| [isCollapse()](#isCollapse--) | När denna egenskap är true kommer bookmarkentry att kollapsa, annars kommer den att expandera. |
| [isOpen()](#isOpen--) | När denna egenskap är true kommer bookmarkentry att expandera, annars kommer den att kollapsa. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCollapse(boolean value)](#setCollapse-boolean-) | När denna egenskap är true kommer bookmarkentry att kollapsa, annars kommer den att expandera. |
| [setDestination(Cell value)](#setDestination-com.aspose.cells.Cell-) | Den cell som bokmärkeslänken pekar på. |
| [setDestinationName(String value)](#setDestinationName-java.lang.String-) | Sätter namn på destinationen. |
| [setOpen(boolean value)](#setOpen-boolean-) | När denna egenskap är true kommer bookmarkentry att expandera, annars kommer den att kollapsa. |
| [setSubEntry(ArrayList value)](#setSubEntry-java.util.ArrayList-) | Underpost för ett bokmärke. |
| [setText(String value)](#setText-java.lang.String-) | Titel för ett bokmärke. |
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
| Parameter | Typ | Beskrivning |
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


Den cell som bokmärkeslänken pekar på.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getDestinationName() {#getDestinationName--}
```
public String getDestinationName()
```


Hämtar namn på destinationen.

**Remarks**

Om destinationsnamnet är satt kommer destinationen att definieras som en namngiven destination med detta namn.

**Returns:**
java.lang.String
### getSubEntry() {#getSubEntry--}
```
public ArrayList getSubEntry()
```


Underpost för ett bokmärke.

**Returns:**
java.util.ArrayList
### getText() {#getText--}
```
public String getText()
```


Titel för ett bokmärke.

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


När denna egenskap är true kommer bookmarkentry att kollapsa, annars kommer den att expandera.

**Returns:**
boolean
### isOpen() {#isOpen--}
```
public boolean isOpen()
```


När denna egenskap är true kommer bookmarkentry att expandera, annars kommer den att kollapsa.

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


När denna egenskap är true kommer bookmarkentry att kollapsa, annars kommer den att expandera.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setDestination(Cell value) {#setDestination-com.aspose.cells.Cell-}
```
public void setDestination(Cell value)
```


Den cell som bokmärkeslänken pekar på.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Cell](../../com.aspose.cells/cell) |  |

### setDestinationName(String value) {#setDestinationName-java.lang.String-}
```
public void setDestinationName(String value)
```


Sätter namn på destinationen.

**Remarks**

Om destinationsnamnet är satt kommer destinationen att definieras som en namngiven destination med detta namn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setOpen(boolean value) {#setOpen-boolean-}
```
public void setOpen(boolean value)
```


När denna egenskap är true kommer bookmarkentry att expandera, annars kommer den att kollapsa.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSubEntry(ArrayList value) {#setSubEntry-java.util.ArrayList-}
```
public void setSubEntry(ArrayList value)
```


Underpost för ett bokmärke.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.ArrayList |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Titel för ett bokmärke.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

