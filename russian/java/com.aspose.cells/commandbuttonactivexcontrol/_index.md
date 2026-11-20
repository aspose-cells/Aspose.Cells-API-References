---
title: "CommandButtonActiveXControl"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет кнопку команды."
type: docs
url: /ru/java/com.aspose.cells/commandbuttonactivexcontrol/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ActiveXControlBase](../../com.aspose.cells/activexcontrolbase), [com.aspose.cells.ActiveXControl](../../com.aspose.cells/activexcontrol)
```
public class CommandButtonActiveXControl extends ActiveXControl
```

Представляет кнопку команды.
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAccelerator()](#getAccelerator--) | Получает клавишу ускорителя для элемента управления. |
| [getBackOleColor()](#getBackOleColor--) | Получает OLE‑цвет фона. |
| [getCaption()](#getCaption--) | Получает описательный текст, отображаемый на элементе управления. |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | Получает двоичные данные элемента управления. |
| [getFont()](#getFont--) | Представляет шрифт элемента управления. |
| [getForeOleColor()](#getForeOleColor--) | Получает OLE‑цвет переднего плана. |
| [getHeight()](#getHeight--) | Получает высоту элемента управления в пунктах. |
| [getIMEMode()](#getIMEMode--) | Получает режим выполнения по умолчанию редактора методов ввода для элемента управления при получении им фокуса. |
| [getLinkedCell()](#getLinkedCell--) | Получает связанную ячейку. |
| [getListFillRange()](#getListFillRange--) | Получает диапазон заполнения списка. |
| [getMouseIcon()](#getMouseIcon--) | Получает пользовательский значок, отображаемый в качестве указателя мыши для элемента управления. |
| [getMousePointer()](#getMousePointer--) | Получает тип значка, отображаемого в качестве указателя мыши для элемента управления. |
| [getPicture()](#getPicture--) | Получает данные изображения. |
| [getPicturePosition()](#getPicturePosition--) | Получает расположение изображения элемента управления относительно его подписи. |
| [getShadow()](#getShadow--) | Указывает, отображать ли тень. |
| [getTakeFocusOnClick()](#getTakeFocusOnClick--) | Указывает, получает ли элемент управления фокус при щелчке. |
| [getTextAlign()](#getTextAlign--) | Представляет способ выравнивания текста, используемого элементом управления. |
| [getType()](#getType--) | Получает тип ActiveX‑элемента управления. |
| [getWidth()](#getWidth--) | Получает ширину элемента управления в единицах точек. |
| [getWorkbook()](#getWorkbook--) | Получает объект [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--). |
| [hashCode()](#hashCode--) |  |
| [isAutoSize()](#isAutoSize--) | Указывает, будет ли элемент управления автоматически изменять размер для отображения всего содержимого. |
| [isEnabled()](#isEnabled--) | Указывает, может ли элемент управления получать фокус и реагировать на события, генерируемые пользователем. |
| [isLocked()](#isLocked--) | Указывает, заблокированы ли данные в элементе управления для редактирования. |
| [isTransparent()](#isTransparent--) | Указывает, является ли элемент управления прозрачным. |
| [isVisible()](#isVisible--) | Указывает, видим ли этот элемент управления. |
| [isWordWrapped()](#isWordWrapped--) | Указывает, будет ли содержимое элемента управления автоматически переноситься в конце строки. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAccelerator(char value)](#setAccelerator-char-) | Устанавливает клавишу ускорителя для элемента управления. |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Указывает, будет ли элемент управления автоматически изменять размер для отображения всего содержимого. |
| [setBackOleColor(int value)](#setBackOleColor-int-) | Устанавливает OLE‑цвет фона. |
| [setCaption(String value)](#setCaption-java.lang.String-) | Устанавливает описательный текст, отображаемый на элементе управления. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | Указывает, может ли элемент управления получать фокус и реагировать на события, генерируемые пользователем. |
| [setForeOleColor(int value)](#setForeOleColor-int-) | Устанавливает OLE‑цвет переднего плана. |
| [setHeight(double value)](#setHeight-double-) | Устанавливает высоту элемента управления в единицах точек. |
| [setIMEMode(int value)](#setIMEMode-int-) | Устанавливает режим выполнения по умолчанию для Input Method Editor элемента управления при получении фокуса. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Устанавливает связанную ячейку. |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | Устанавливает диапазон заполнения списка. |
| [setLocked(boolean value)](#setLocked-boolean-) | Указывает, заблокированы ли данные в элементе управления для редактирования. |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | Устанавливает пользовательский значок, отображаемый в качестве указателя мыши для элемента управления. |
| [setMousePointer(int value)](#setMousePointer-int-) | Устанавливает тип значка, отображаемого в качестве указателя мыши для элемента управления. |
| [setPicture(byte[] value)](#setPicture-byte---) | Устанавливает данные изображения. |
| [setPicturePosition(int value)](#setPicturePosition-int-) | Устанавливает расположение изображения элемента управления относительно его подписи. |
| [setShadow(boolean value)](#setShadow-boolean-) | Указывает, отображать ли тень. |
| [setTakeFocusOnClick(boolean value)](#setTakeFocusOnClick-boolean-) | Указывает, получает ли элемент управления фокус при щелчке. |
| [setTextAlign(int value)](#setTextAlign-int-) | Представляет способ выравнивания текста, используемого элементом управления. |
| [setTransparent(boolean value)](#setTransparent-boolean-) | Указывает, является ли элемент управления прозрачным. |
| [setVisible(boolean value)](#setVisible-boolean-) | Указывает, видим ли этот элемент управления. |
| [setWidth(double value)](#setWidth-double-) | Устанавливает ширину элемента управления в единицах пунктов. |
| [setWordWrapped(boolean value)](#setWordWrapped-boolean-) | Указывает, будет ли содержимое элемента управления автоматически переноситься в конце строки. |
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
### getAccelerator() {#getAccelerator--}
```
public char getAccelerator()
```


Получает клавишу ускорителя для элемента управления.

**Returns:**
char
### getBackOleColor() {#getBackOleColor--}
```
public int getBackOleColor()
```


Получает OLE‑цвет фона.

**Returns:**
int
### getCaption() {#getCaption--}
```
public String getCaption()
```


Получает описательный текст, отображаемый на элементе управления.

**Returns:**
java.lang.String
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
### getFont() {#getFont--}
```
public Font getFont()
```


Представляет шрифт элемента управления.

**Returns:**
[Font](../../com.aspose.cells/font)
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
### getIMEMode() {#getIMEMode--}
```
public int getIMEMode()
```


Получает режим выполнения по умолчанию редактора методов ввода для элемента управления при получении им фокуса.

См. [InputMethodEditorMode](../../com.aspose.cells/inputmethodeditormode).

**Returns:**
int
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
### getPicture() {#getPicture--}
```
public byte[] getPicture()
```


Получает данные изображения.

**Returns:**
byte[]
### getPicturePosition() {#getPicturePosition--}
```
public int getPicturePosition()
```


Получает расположение изображения элемента управления относительно его подписи.

См. [ControlPicturePositionType](../../com.aspose.cells/controlpicturepositiontype).

**Returns:**
int
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Указывает, отображать ли тень.

**Returns:**
boolean
### getTakeFocusOnClick() {#getTakeFocusOnClick--}
```
public boolean getTakeFocusOnClick()
```


Указывает, получает ли элемент управления фокус при щелчке.

**Returns:**
boolean
### getTextAlign() {#getTextAlign--}
```
public int getTextAlign()
```


Представляет способ выравнивания текста, используемого элементом управления.

См. [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getType() {#getType--}
```
public int getType()
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
### isAutoSize() {#isAutoSize--}
```
public boolean isAutoSize()
```


Указывает, будет ли элемент управления автоматически изменять размер для отображения всего содержимого.

**Returns:**
boolean
### isEnabled() {#isEnabled--}
```
public boolean isEnabled()
```


Указывает, может ли элемент управления получать фокус и реагировать на события, генерируемые пользователем.

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


Указывает, заблокированы ли данные в элементе управления для редактирования.

**Returns:**
boolean
### isTransparent() {#isTransparent--}
```
public boolean isTransparent()
```


Указывает, является ли элемент управления прозрачным.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Указывает, видим ли этот элемент управления.

**Returns:**
boolean
### isWordWrapped() {#isWordWrapped--}
```
public boolean isWordWrapped()
```


Указывает, будет ли содержимое элемента управления автоматически переноситься в конце строки.

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




### setAccelerator(char value) {#setAccelerator-char-}
```
public void setAccelerator(char value)
```


Устанавливает клавишу ускорителя для элемента управления.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | char |  |

### setAutoSize(boolean value) {#setAutoSize-boolean-}
```
public void setAutoSize(boolean value)
```


Указывает, будет ли элемент управления автоматически изменять размер для отображения всего содержимого.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setBackOleColor(int value) {#setBackOleColor-int-}
```
public void setBackOleColor(int value)
```


Устанавливает OLE‑цвет фона.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setCaption(String value) {#setCaption-java.lang.String-}
```
public void setCaption(String value)
```


Устанавливает описательный текст, отображаемый на элементе управления.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public void setEnabled(boolean value)
```


Указывает, может ли элемент управления получать фокус и реагировать на события, генерируемые пользователем.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

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

### setIMEMode(int value) {#setIMEMode-int-}
```
public void setIMEMode(int value)
```


Устанавливает режим выполнения по умолчанию для Input Method Editor элемента управления при получении фокуса.

См. [InputMethodEditorMode](../../com.aspose.cells/inputmethodeditormode).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

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

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Указывает, заблокированы ли данные в элементе управления для редактирования.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

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

### setPicture(byte[] value) {#setPicture-byte---}
```
public void setPicture(byte[] value)
```


Устанавливает данные изображения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | byte[] |  |

### setPicturePosition(int value) {#setPicturePosition-int-}
```
public void setPicturePosition(int value)
```


Устанавливает расположение изображения элемента управления относительно его подписи.

См. [ControlPicturePositionType](../../com.aspose.cells/controlpicturepositiontype).

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

### setTakeFocusOnClick(boolean value) {#setTakeFocusOnClick-boolean-}
```
public void setTakeFocusOnClick(boolean value)
```


Указывает, получает ли элемент управления фокус при щелчке.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setTextAlign(int value) {#setTextAlign-int-}
```
public void setTextAlign(int value)
```


Представляет способ выравнивания текста, используемого элементом управления.

См. [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setTransparent(boolean value) {#setTransparent-boolean-}
```
public void setTransparent(boolean value)
```


Указывает, является ли элемент управления прозрачным.

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

### setWordWrapped(boolean value) {#setWordWrapped-boolean-}
```
public void setWordWrapped(boolean value)
```


Указывает, будет ли содержимое элемента управления автоматически переноситься в конце строки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

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

