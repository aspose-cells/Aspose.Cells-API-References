---
title: "PdfBookmarkEntry"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "PdfBookmarkEntry es una entrada en el marcador PDF."
type: docs
url: /es/java/com.aspose.cells/pdfbookmarkentry/
---

**Inheritance:**
java.lang.Object
```
public class PdfBookmarkEntry
```

PdfBookmarkEntry es una entrada en el marcador PDF. Si la propiedad Text de la instancia actual es null o \"\", la instancia actual se ocultará y los hijos se insertarán en el nivel actual.

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
## Constructores

| Constructor | Descripción |
| --- | --- |
| [PdfBookmarkEntry()](#PdfBookmarkEntry--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDestination()](#getDestination--) | La celda a la que enlaza el marcador. |
| [getDestinationName()](#getDestinationName--) | Obtiene el nombre del destino. |
| [getSubEntry()](#getSubEntry--) | Subentrada de un marcador. |
| [getText()](#getText--) | Título de un marcador. |
| [hashCode()](#hashCode--) |  |
| [isCollapse()](#isCollapse--) | Cuando esta propiedad es true, la entrada del marcador se colapsará; de lo contrario se expandirá. |
| [isOpen()](#isOpen--) | Cuando esta propiedad es true, la entrada del marcador se expandirá; de lo contrario se colapsará. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCollapse(boolean value)](#setCollapse-boolean-) | Cuando esta propiedad es true, la entrada del marcador se colapsará; de lo contrario se expandirá. |
| [setDestination(Cell value)](#setDestination-com.aspose.cells.Cell-) | La celda a la que enlaza el marcador. |
| [setDestinationName(String value)](#setDestinationName-java.lang.String-) | Establece el nombre del destino. |
| [setOpen(boolean value)](#setOpen-boolean-) | Cuando esta propiedad es true, la entrada del marcador se expandirá; de lo contrario se colapsará. |
| [setSubEntry(ArrayList value)](#setSubEntry-java.util.ArrayList-) | Subentrada de un marcador. |
| [setText(String value)](#setText-java.lang.String-) | Título de un marcador. |
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
### getDestination() {#getDestination--}
```
public Cell getDestination()
```


La celda a la que enlaza el marcador.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getDestinationName() {#getDestinationName--}
```
public String getDestinationName()
```


Obtiene el nombre del destino.

**Remarks**

Si se establece el nombre del destino, el destino se definirá como un destino nombrado con este nombre.

**Returns:**
java.lang.String
### getSubEntry() {#getSubEntry--}
```
public ArrayList getSubEntry()
```


Subentrada de un marcador.

**Returns:**
java.util.ArrayList
### getText() {#getText--}
```
public String getText()
```


Título de un marcador.

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


Cuando esta propiedad es true, la entrada del marcador se colapsará; de lo contrario se expandirá.

**Returns:**
boolean
### isOpen() {#isOpen--}
```
public boolean isOpen()
```


Cuando esta propiedad es true, la entrada del marcador se expandirá; de lo contrario se colapsará.

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


Cuando esta propiedad es true, la entrada del marcador se colapsará; de lo contrario se expandirá.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setDestination(Cell value) {#setDestination-com.aspose.cells.Cell-}
```
public void setDestination(Cell value)
```


La celda a la que enlaza el marcador.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Cell](../../com.aspose.cells/cell) |  |

### setDestinationName(String value) {#setDestinationName-java.lang.String-}
```
public void setDestinationName(String value)
```


Establece el nombre del destino.

**Remarks**

Si se establece el nombre del destino, el destino se definirá como un destino nombrado con este nombre.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setOpen(boolean value) {#setOpen-boolean-}
```
public void setOpen(boolean value)
```


Cuando esta propiedad es true, la entrada del marcador se expandirá; de lo contrario se colapsará.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSubEntry(ArrayList value) {#setSubEntry-java.util.ArrayList-}
```
public void setSubEntry(ArrayList value)
```


Subentrada de un marcador.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.ArrayList |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Título de un marcador.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

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

