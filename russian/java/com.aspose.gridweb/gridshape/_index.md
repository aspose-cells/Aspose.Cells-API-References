---
title: "GridShape"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет объект формы."
type: docs
url: /ru/java/com.aspose.gridweb/gridshape/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.gridweb.IGridSave
```
public class GridShape implements IGridSave
```

Представляет объект формы.
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBuffer()](#getBuffer--) | Получает буфер объекта. |
| [getClass()](#getClass--) |  |
| [getID()](#getID--) | Получает ID набора для фигуры. |
| [getLeft()](#getLeft--) | Представляет горизонтальное смещение фигуры от её левого столбца в пикселях. |
| [getLeftToCorner()](#getLeftToCorner--) | Представляет горизонтальное смещение фигуры от левого края листа, в пикселях. |
| [getMsoDrawingType()](#getMsoDrawingType--) | Получает тип mso-рисования. |
| [getName()](#getName--) | Получает имя фигуры. |
| [getText()](#getText--) | Представляет строку в этом объекте TextBox. |
| [getTop()](#getTop--) | Представляет вертикальное смещение фигуры от её верхней строки, в пикселях. |
| [getTopToCorner()](#getTopToCorner--) | Представляет вертикальное смещение фигуры от верхнего края листа, в пикселях. |
| [getUpperLeftColumn()](#getUpperLeftColumn--) | Представляет индекс столбца левого верхнего угла. |
| [getUpperLeftRow()](#getUpperLeftRow--) | Представляет индекс строки верхнего левого угла. |
| [getZOrderPosition()](#getZOrderPosition--) | Возвращает позицию фигуры в порядке Z. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [saveToImage(InputStream s)](#saveToImage-java.io.InputStream-) | Создаёт изображение и сохраняет его в поток в указанном формате PNG. |
| [setID(String value)](#setID-java.lang.String-) | Получает ID набора для фигуры. |
| [setLeftToCorner(int value)](#setLeftToCorner-int-) | Представляет горизонтальное смещение фигуры от левого края листа, в пикселях. |
| [setText(String value)](#setText-java.lang.String-) | Представляет строку в этом объекте TextBox. |
| [setTopToCorner(int value)](#setTopToCorner-int-) | Представляет вертикальное смещение фигуры от верхнего края листа, в пикселях. |
| [setZOrderPosition(int value)](#setZOrderPosition-int-) | Возвращает позицию фигуры в порядке Z. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getBuffer() {#getBuffer--}
```
public byte[] getBuffer()
```


Получает буфер объекта.

**Returns:**
byte[]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getID() {#getID--}
```
public String getID()
```


Получает ID набора для фигуры.

**Returns:**
java.lang.String
### getLeft() {#getLeft--}
```
public int getLeft()
```


Представляет горизонтальное смещение фигуры от её левого столбца в пикселях.

**Returns:**
int
### getLeftToCorner() {#getLeftToCorner--}
```
public int getLeftToCorner()
```


Представляет горизонтальное смещение фигуры от левого края листа, в пикселях.

**Returns:**
int
### getMsoDrawingType() {#getMsoDrawingType--}
```
public int getMsoDrawingType()
```


Получает тип mso-рисования.

Смотрите [GridMsoDrawingType](../../com.aspose.gridweb/gridmsodrawingtype).

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Получает имя фигуры.

**Returns:**
java.lang.String
### getText() {#getText--}
```
public String getText()
```


Представляет строку в этом объекте TextBox.

**Returns:**
java.lang.String
### getTop() {#getTop--}
```
public int getTop()
```


Представляет вертикальное смещение фигуры от её верхней строки, в пикселях.

**Remarks**

Если форма находится в диаграмме, представляет вертикальное смещение формы от её верхней границы.

**Returns:**
int
### getTopToCorner() {#getTopToCorner--}
```
public int getTopToCorner()
```


Представляет вертикальное смещение фигуры от верхнего края листа, в пикселях.

**Returns:**
int
### getUpperLeftColumn() {#getUpperLeftColumn--}
```
public int getUpperLeftColumn()
```


Представляет индекс столбца левого верхнего угла.

**Returns:**
int
### getUpperLeftRow() {#getUpperLeftRow--}
```
public int getUpperLeftRow()
```


Представляет индекс строки верхнего левого угла.

**Remarks**

Если форма находится в другой форме или в группе, UpperLeftRow будет игнорироваться.

**Returns:**
int
### getZOrderPosition() {#getZOrderPosition--}
```
public int getZOrderPosition()
```


Возвращает позицию фигуры в порядке Z.

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




### saveToImage(InputStream s) {#saveToImage-java.io.InputStream-}
```
public void saveToImage(InputStream s)
```


Создаёт изображение и сохраняет его в поток в указанном формате PNG.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| s | java.io.InputStream |  |

### setID(String value) {#setID-java.lang.String-}
```
public void setID(String value)
```


Получает ID набора для фигуры.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setLeftToCorner(int value) {#setLeftToCorner-int-}
```
public void setLeftToCorner(int value)
```


Представляет горизонтальное смещение фигуры от левого края листа, в пикселях.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Представляет строку в этом объекте TextBox.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setTopToCorner(int value) {#setTopToCorner-int-}
```
public void setTopToCorner(int value)
```


Представляет вертикальное смещение фигуры от верхнего края листа, в пикселях.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setZOrderPosition(int value) {#setZOrderPosition-int-}
```
public void setZOrderPosition(int value)
```


Возвращает позицию фигуры в порядке Z.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

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

