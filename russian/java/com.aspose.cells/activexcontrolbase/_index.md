---
title: "ActiveXControlBase"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет элемент управления ActiveX."
type: docs
url: /ru/java/com.aspose.cells/activexcontrolbase/
---

**Inheritance:**
java.lang.Object
```
public abstract class ActiveXControlBase
```

Представляет элемент управления ActiveX.
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackOleColor()](#getBackOleColor--) | Получает OLE‑цвет фона. |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | Получает двоичные данные элемента управления. |
| [getForeOleColor()](#getForeOleColor--) | Получает OLE‑цвет переднего плана. |
| [getHeight()](#getHeight--) | Получает высоту элемента управления в пунктах. |
| [getLinkedCell()](#getLinkedCell--) | Получает связанную ячейку. |
| [getListFillRange()](#getListFillRange--) | Получает диапазон заполнения списка. |
| [getMouseIcon()](#getMouseIcon--) | Получает пользовательский значок, отображаемый в качестве указателя мыши для элемента управления. |
| [getMousePointer()](#getMousePointer--) | Получает тип значка, отображаемого в качестве указателя мыши для элемента управления. |
| [getShadow()](#getShadow--) | Указывает, отображать ли тень. |
| [getType()](#getType--) | Получает тип ActiveX‑элемента управления. |
| [getWidth()](#getWidth--) | Получает ширину элемента управления в единицах точек. |
| [getWorkbook()](#getWorkbook--) | Получает объект [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--). |
| [hashCode()](#hashCode--) |  |
| [isVisible()](#isVisible--) | Указывает, видим ли этот элемент управления. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackOleColor(int value)](#setBackOleColor-int-) | Устанавливает OLE‑цвет фона. |
| [setForeOleColor(int value)](#setForeOleColor-int-) | Устанавливает OLE‑цвет переднего плана. |
| [setHeight(double value)](#setHeight-double-) | Устанавливает высоту элемента управления в единицах точек. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Устанавливает связанную ячейку. |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | Устанавливает диапазон заполнения списка. |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | Устанавливает пользовательский значок, отображаемый в качестве указателя мыши для элемента управления. |
| [setMousePointer(int value)](#setMousePointer-int-) | Устанавливает тип значка, отображаемого в качестве указателя мыши для элемента управления. |
| [setShadow(boolean value)](#setShadow-boolean-) | Указывает, отображать ли тень. |
| [setVisible(boolean value)](#setVisible-boolean-) | Указывает, видим ли этот элемент управления. |
| [setWidth(double value)](#setWidth-double-) | Устанавливает ширину элемента управления в единицах пунктов. |
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
### getBackOleColor() {#getBackOleColor--}
```
public int getBackOleColor()
```


Получает OLE‑цвет фона.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getData() {#getData--}
```
public byte[] getData()
```


Получает двоичные данные элемента управления.

**Returns:**
byte[]
### getForeOleColor() {#getForeOleColor--}
```
public int getForeOleColor()
```


Получает OLE‑цвет переднего плана.

**Remarks**

Не применяется к элементу управления Image.

**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```


Получает высоту элемента управления в пунктах.

**Returns:**
double
### getLinkedCell() {#getLinkedCell--}
```
public String getLinkedCell()
```


Получает связанную ячейку.

**Returns:**
java.lang.String
### getListFillRange() {#getListFillRange--}
```
public String getListFillRange()
```


Получает диапазон заполнения списка.

**Returns:**
java.lang.String
### getMouseIcon() {#getMouseIcon--}
```
public byte[] getMouseIcon()
```


Получает пользовательский значок, отображаемый в качестве указателя мыши для элемента управления.

**Returns:**
byte[]
### getMousePointer() {#getMousePointer--}
```
public int getMousePointer()
```


Получает тип значка, отображаемого в качестве указателя мыши для элемента управления.

См. [ControlMousePointerType](../../com.aspose.cells/controlmousepointertype).

**Returns:**
int
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Указывает, отображать ли тень.

**Returns:**
boolean
### getType() {#getType--}
```
public abstract int getType()
```


Получает тип ActiveX‑элемента управления.

См. [ControlType](../../com.aspose.cells/controltype).

**Returns:**
int
### getWidth() {#getWidth--}
```
public double getWidth()
```


Получает ширину элемента управления в единицах точек.

**Returns:**
double
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


Получает объект [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--).

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Указывает, видим ли этот элемент управления.

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




### setBackOleColor(int value) {#setBackOleColor-int-}
```
public void setBackOleColor(int value)
```


Устанавливает OLE‑цвет фона.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setForeOleColor(int value) {#setForeOleColor-int-}
```
public void setForeOleColor(int value)
```


Устанавливает OLE‑цвет переднего плана.

**Remarks**

Не применяется к элементу управления Image.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


Устанавливает высоту элемента управления в единицах точек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setLinkedCell(String value) {#setLinkedCell-java.lang.String-}
```
public void setLinkedCell(String value)
```


Устанавливает связанную ячейку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setListFillRange(String value) {#setListFillRange-java.lang.String-}
```
public void setListFillRange(String value)
```


Устанавливает диапазон заполнения списка.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setMouseIcon(byte[] value) {#setMouseIcon-byte---}
```
public void setMouseIcon(byte[] value)
```


Устанавливает пользовательский значок, отображаемый в качестве указателя мыши для элемента управления.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | byte[] |  |

### setMousePointer(int value) {#setMousePointer-int-}
```
public void setMousePointer(int value)
```


Устанавливает тип значка, отображаемого в качестве указателя мыши для элемента управления.

См. [ControlMousePointerType](../../com.aspose.cells/controlmousepointertype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


Указывает, отображать ли тень.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Указывает, видим ли этот элемент управления.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```


Устанавливает ширину элемента управления в единицах пунктов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

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

