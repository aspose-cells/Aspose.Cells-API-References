---
title: "PdfBookmarkEntry"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "PdfBookmarkEntry est une entrée dans le signet PDF."
type: docs
url: /fr/java/com.aspose.cells/pdfbookmarkentry/
---

**Inheritance:**
java.lang.Object
```
public class PdfBookmarkEntry
```

PdfBookmarkEntry est une entrée dans le signet PDF. Si la propriété Text de l'instance actuelle est null ou \"\", l'instance actuelle sera masquée et les enfants seront insérés au même niveau.

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
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [PdfBookmarkEntry()](#PdfBookmarkEntry--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDestination()](#getDestination--) | La cellule à laquelle le lien du signet pointe. |
| [getDestinationName()](#getDestinationName--) | Obtient le nom de la destination. |
| [getSubEntry()](#getSubEntry--) | Sous-entrée d'un signet. |
| [getText()](#getText--) | Titre d'un signet. |
| [hashCode()](#hashCode--) |  |
| [isCollapse()](#isCollapse--) | Lorsque cette propriété est true, l'entrée du signet se repliera, sinon elle s'étendra. |
| [isOpen()](#isOpen--) | Lorsque cette propriété est true, l'entrée du signet s'étendra, sinon elle se repliera. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCollapse(boolean value)](#setCollapse-boolean-) | Lorsque cette propriété est true, l'entrée du signet se repliera, sinon elle s'étendra. |
| [setDestination(Cell value)](#setDestination-com.aspose.cells.Cell-) | La cellule à laquelle le lien du signet pointe. |
| [setDestinationName(String value)](#setDestinationName-java.lang.String-) | Définit le nom de la destination. |
| [setOpen(boolean value)](#setOpen-boolean-) | Lorsque cette propriété est true, l'entrée du signet s'étendra, sinon elle se repliera. |
| [setSubEntry(ArrayList value)](#setSubEntry-java.util.ArrayList-) | Sous-entrée d'un signet. |
| [setText(String value)](#setText-java.lang.String-) | Titre d'un signet. |
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
### getDestination() {#getDestination--}
```
public Cell getDestination()
```


La cellule à laquelle le lien du signet pointe.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getDestinationName() {#getDestinationName--}
```
public String getDestinationName()
```


Obtient le nom de la destination.

**Remarks**

Si le nom de destination est défini, la destination sera définie comme une destination nommée avec ce nom.

**Returns:**
java.lang.String
### getSubEntry() {#getSubEntry--}
```
public ArrayList getSubEntry()
```


Sous-entrée d'un signet.

**Returns:**
java.util.ArrayList
### getText() {#getText--}
```
public String getText()
```


Titre d'un signet.

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


Lorsque cette propriété est true, l'entrée du signet se repliera, sinon elle s'étendra.

**Returns:**
boolean
### isOpen() {#isOpen--}
```
public boolean isOpen()
```


Lorsque cette propriété est true, l'entrée du signet s'étendra, sinon elle se repliera.

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


Lorsque cette propriété est true, l'entrée du signet se repliera, sinon elle s'étendra.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setDestination(Cell value) {#setDestination-com.aspose.cells.Cell-}
```
public void setDestination(Cell value)
```


La cellule à laquelle le lien du signet pointe.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Cell](../../com.aspose.cells/cell) |  |

### setDestinationName(String value) {#setDestinationName-java.lang.String-}
```
public void setDestinationName(String value)
```


Définit le nom de la destination.

**Remarks**

Si le nom de destination est défini, la destination sera définie comme une destination nommée avec ce nom.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setOpen(boolean value) {#setOpen-boolean-}
```
public void setOpen(boolean value)
```


Lorsque cette propriété est true, l'entrée du signet s'étendra, sinon elle se repliera.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSubEntry(ArrayList value) {#setSubEntry-java.util.ArrayList-}
```
public void setSubEntry(ArrayList value)
```


Sous-entrée d'un signet.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.ArrayList |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Titre d'un signet.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

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

