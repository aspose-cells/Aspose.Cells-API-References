---
title: "PdfBookmarkEntry"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "PdfBookmarkEntry è una voce nel segnalibro pdf."
type: docs
url: /it/java/com.aspose.cells/pdfbookmarkentry/
---

**Inheritance:**
java.lang.Object
```
public class PdfBookmarkEntry
```

PdfBookmarkEntry è una voce nei segnalibri PDF. Se la proprietà Text dell'istanza corrente è null o "", l'istanza corrente verrà nascosta e i figli saranno inseriti al livello corrente.

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
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [PdfBookmarkEntry()](#PdfBookmarkEntry--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDestination()](#getDestination--) | La cella a cui è collegato il segnalibro. |
| [getDestinationName()](#getDestinationName--) | Ottiene il nome della destinazione. |
| [getSubEntry()](#getSubEntry--) | Sotto voce di un segnalibro. |
| [getText()](#getText--) | Titolo di un segnalibro. |
| [hashCode()](#hashCode--) |  |
| [isCollapse()](#isCollapse--) | Quando questa proprietà è true, la voce del segnalibro si chiuderà, altrimenti si espanderà. |
| [isOpen()](#isOpen--) | Quando questa proprietà è true, la voce del segnalibro si espanderà, altrimenti si chiuderà. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCollapse(boolean value)](#setCollapse-boolean-) | Quando questa proprietà è true, la voce del segnalibro si chiuderà, altrimenti si espanderà. |
| [setDestination(Cell value)](#setDestination-com.aspose.cells.Cell-) | La cella a cui è collegato il segnalibro. |
| [setDestinationName(String value)](#setDestinationName-java.lang.String-) | Imposta il nome della destinazione. |
| [setOpen(boolean value)](#setOpen-boolean-) | Quando questa proprietà è true, la voce del segnalibro si espanderà, altrimenti si chiuderà. |
| [setSubEntry(ArrayList value)](#setSubEntry-java.util.ArrayList-) | Sotto voce di un segnalibro. |
| [setText(String value)](#setText-java.lang.String-) | Titolo di un segnalibro. |
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
### getDestination() {#getDestination--}
```
public Cell getDestination()
```


La cella a cui è collegato il segnalibro.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getDestinationName() {#getDestinationName--}
```
public String getDestinationName()
```


Ottiene il nome della destinazione.

**Remarks**

Se il nome della destinazione è impostato, la destinazione verrà definita come destinazione nominata con questo nome.

**Returns:**
java.lang.String
### getSubEntry() {#getSubEntry--}
```
public ArrayList getSubEntry()
```


Sotto voce di un segnalibro.

**Returns:**
java.util.ArrayList
### getText() {#getText--}
```
public String getText()
```


Titolo di un segnalibro.

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


Quando questa proprietà è true, la voce del segnalibro si chiuderà, altrimenti si espanderà.

**Returns:**
boolean
### isOpen() {#isOpen--}
```
public boolean isOpen()
```


Quando questa proprietà è true, la voce del segnalibro si espanderà, altrimenti si chiuderà.

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


Quando questa proprietà è true, la voce del segnalibro si chiuderà, altrimenti si espanderà.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setDestination(Cell value) {#setDestination-com.aspose.cells.Cell-}
```
public void setDestination(Cell value)
```


La cella a cui è collegato il segnalibro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Cell](../../com.aspose.cells/cell) |  |

### setDestinationName(String value) {#setDestinationName-java.lang.String-}
```
public void setDestinationName(String value)
```


Imposta il nome della destinazione.

**Remarks**

Se il nome della destinazione è impostato, la destinazione verrà definita come destinazione nominata con questo nome.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setOpen(boolean value) {#setOpen-boolean-}
```
public void setOpen(boolean value)
```


Quando questa proprietà è true, la voce del segnalibro si espanderà, altrimenti si chiuderà.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSubEntry(ArrayList value) {#setSubEntry-java.util.ArrayList-}
```
public void setSubEntry(ArrayList value)
```


Sotto voce di un segnalibro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.ArrayList |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Titolo di un segnalibro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

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

