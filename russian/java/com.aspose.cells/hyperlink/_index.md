---
title: "Гиперссылка"
second_title: "Справочник API Aspose.Cells for Java"
description: "Инкапсулирует объект, представляющий гиперссылку."
type: docs
url: /ru/java/com.aspose.cells/hyperlink/
---

**Inheritance:**
java.lang.Object
```
public class Hyperlink
```

Инкапсулирует объект, представляющий гиперссылку.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Adding a new worksheet to the Workbook object
         workbook.getWorksheets().add();
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Adding a hyperlink to a URL at "A1" cell
         int index = worksheet.getHyperlinks().add("A1", 1, 1, "http://www.aspose.com");
         //Getting a Hyperlink by index.
         Hyperlink hyperlink = worksheet.getHyperlinks().get(index);
         //Setting display text of this hyperlink.
         hyperlink.setTextToDisplay("Aspose");
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Методы

| Метод | Описание |
| --- | --- |
| [delete()](#delete--) | Удаляет эту гиперссылку |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAddress()](#getAddress--) | Представляет адрес гиперссылки. |
| [getArea()](#getArea--) | Получает диапазон гиперссылки. |
| [getClass()](#getClass--) |  |
| [getLinkType()](#getLinkType--) | Получает тип ссылки. |
| [getScreenTip()](#getScreenTip--) | Возвращает или задает текст подсказки ScreenTip для указанной гиперссылки. |
| [getTextToDisplay()](#getTextToDisplay--) | Представляет текст, отображаемый для указанной гиперссылки. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAddress(String value)](#setAddress-java.lang.String-) | Представляет адрес гиперссылки. |
| [setScreenTip(String value)](#setScreenTip-java.lang.String-) | Возвращает или задает текст подсказки ScreenTip для указанной гиперссылки. |
| [setTextToDisplay(String value)](#setTextToDisplay-java.lang.String-) | Представляет текст, отображаемый для указанной гиперссылки. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### delete() {#delete--}
```
public void delete()
```


Удаляет эту гиперссылку

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
### getAddress() {#getAddress--}
```
public String getAddress()
```


Представляет адрес гиперссылки.

**Returns:**
java.lang.String
### getArea() {#getArea--}
```
public CellArea getArea()
```


Получает диапазон гиперссылки.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getLinkType() {#getLinkType--}
```
public int getLinkType()
```


Получает тип ссылки.

Смотрите [TargetModeType](../../com.aspose.cells/targetmodetype).

**Returns:**
int
### getScreenTip() {#getScreenTip--}
```
public String getScreenTip()
```


Возвращает или задает текст подсказки ScreenTip для указанной гиперссылки.

**Returns:**
java.lang.String
### getTextToDisplay() {#getTextToDisplay--}
```
public String getTextToDisplay()
```


Представляет текст, отображаемый для указанной гиперссылки. Значение по умолчанию — адрес гиперссылки.

**Returns:**
java.lang.String
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




### setAddress(String value) {#setAddress-java.lang.String-}
```
public void setAddress(String value)
```


Представляет адрес гиперссылки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setScreenTip(String value) {#setScreenTip-java.lang.String-}
```
public void setScreenTip(String value)
```


Возвращает или задает текст подсказки ScreenTip для указанной гиперссылки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setTextToDisplay(String value) {#setTextToDisplay-java.lang.String-}
```
public void setTextToDisplay(String value)
```


Представляет текст, отображаемый для указанной гиперссылки. Значение по умолчанию — адрес гиперссылки.

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

