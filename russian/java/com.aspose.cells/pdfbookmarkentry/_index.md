---
title: "PdfBookmarkEntry"
second_title: "Справочник API Aspose.Cells for Java"
description: "PdfBookmarkEntry — это запись в закладке PDF."
type: docs
url: /ru/java/com.aspose.cells/pdfbookmarkentry/
---

**Inheritance:**
java.lang.Object
```
public class PdfBookmarkEntry
```

PdfBookmarkEntry — это запись в закладках PDF. Если свойство Text текущего экземпляра равно null или "", текущий экземпляр будет скрыт, а дочерние элементы будут вставлены на текущем уровне.

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
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [PdfBookmarkEntry()](#PdfBookmarkEntry--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDestination()](#getDestination--) | Ячейка, к которой привязана ссылка закладки. |
| [getDestinationName()](#getDestinationName--) | Получает имя назначения. |
| [getSubEntry()](#getSubEntry--) | Подзапись закладки. |
| [getText()](#getText--) | Заголовок закладки. |
| [hashCode()](#hashCode--) |  |
| [isCollapse()](#isCollapse--) | Когда это свойство равно true, запись закладки будет свернута, иначе она будет развернута. |
| [isOpen()](#isOpen--) | Когда это свойство равно true, запись закладки будет развернута, иначе она будет свернута. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCollapse(boolean value)](#setCollapse-boolean-) | Когда это свойство равно true, запись закладки будет свернута, иначе она будет развернута. |
| [setDestination(Cell value)](#setDestination-com.aspose.cells.Cell-) | Ячейка, к которой привязана ссылка закладки. |
| [setDestinationName(String value)](#setDestinationName-java.lang.String-) | Устанавливает имя назначения. |
| [setOpen(boolean value)](#setOpen-boolean-) | Когда это свойство равно true, запись закладки будет развернута, иначе она будет свернута. |
| [setSubEntry(ArrayList value)](#setSubEntry-java.util.ArrayList-) | Подзапись закладки. |
| [setText(String value)](#setText-java.lang.String-) | Заголовок закладки. |
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
| Параметр | Тип | Описание |
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


Ячейка, к которой привязана ссылка закладки.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getDestinationName() {#getDestinationName--}
```
public String getDestinationName()
```


Получает имя назначения.

**Remarks**

Если имя назначения задано, оно будет определено как именованное назначение с этим именем.

**Returns:**
java.lang.String
### getSubEntry() {#getSubEntry--}
```
public ArrayList getSubEntry()
```


Подзапись закладки.

**Returns:**
java.util.ArrayList
### getText() {#getText--}
```
public String getText()
```


Заголовок закладки.

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


Когда это свойство равно true, запись закладки будет свернута, иначе она будет развернута.

**Returns:**
boolean
### isOpen() {#isOpen--}
```
public boolean isOpen()
```


Когда это свойство равно true, запись закладки будет развернута, иначе она будет свернута.

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


Когда это свойство равно true, запись закладки будет свернута, иначе она будет развернута.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setDestination(Cell value) {#setDestination-com.aspose.cells.Cell-}
```
public void setDestination(Cell value)
```


Ячейка, к которой привязана ссылка закладки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Cell](../../com.aspose.cells/cell) |  |

### setDestinationName(String value) {#setDestinationName-java.lang.String-}
```
public void setDestinationName(String value)
```


Устанавливает имя назначения.

**Remarks**

Если имя назначения задано, оно будет определено как именованное назначение с этим именем.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setOpen(boolean value) {#setOpen-boolean-}
```
public void setOpen(boolean value)
```


Когда это свойство равно true, запись закладки будет развернута, иначе она будет свернута.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSubEntry(ArrayList value) {#setSubEntry-java.util.ArrayList-}
```
public void setSubEntry(ArrayList value)
```


Подзапись закладки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.util.ArrayList |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Заголовок закладки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

