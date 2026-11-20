---
title: "CustomCommandButton"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет пользовательскую кнопку команды на панели вкладок контроля GridWeb."
type: docs
url: /ru/java/com.aspose.gridweb/customcommandbutton/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.Control](../../com.aspose.gridweb/control)
```
public class CustomCommandButton extends Control
```

Представляет пользовательскую кнопку команды на панели вкладок контроля GridWeb.

**Example**

```
         GridWebBean GridWeb1=ExtPage.getInstance().getBean();
         CustomCommandButton button = new CustomCommandButton();
         button.setCommand("MyCommand");
         button.setImageUrl("images/button1.gif");
         GridWeb1.getCustomCommandButtons().add(button);
```
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [CustomCommandButton()](#CustomCommandButton--) | Конструктор по умолчанию. |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getClientClickEvent()](#getClientClickEvent--) | Получает обработчик события клика на стороне клиента. |
| [getCommand()](#getCommand--) | Получает имя команды. |
| [getCommandType()](#getCommandType--) | Получает тип рендеринга команды. |
| [getDiscardInput()](#getDiscardInput--) | Указывает, следует ли отбрасывать ввод пользователя в браузере клиента, когда пользователь нажимает эту кнопку. |
| [getImageUrl()](#getImageUrl--) | Получает URL изображения кнопки команды. |
| [getText()](#getText--) | Получает альтернативный текст кнопки команды. |
| [getToolTip()](#getToolTip--) | Получает всплывающую подсказку кнопки команды. |
| [getUniqueID()](#getUniqueID--) | Получает UniqueID в элементе управления. |
| [getVisible()](#getVisible--) | Получает свойство Visible в Control |
| [getWidth()](#getWidth--) | Ширина кнопки. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setClientClickEvent(String value)](#setClientClickEvent-java.lang.String-) | Устанавливает обработчик события клика на клиентской стороне. |
| [setCommand(String value)](#setCommand-java.lang.String-) | Устанавливает имя команды. |
| [setCommandType(int value)](#setCommandType-int-) | Устанавливает тип отображения команды. |
| [setDiscardInput(boolean value)](#setDiscardInput-boolean-) | Указывает, следует ли отбрасывать ввод пользователя в браузере клиента, когда пользователь нажимает эту кнопку. |
| [setImageUrl(String value)](#setImageUrl-java.lang.String-) | Устанавливает URL изображения кнопки команды. |
| [setText(String value)](#setText-java.lang.String-) | Устанавливает альтернативный текст кнопки команды. |
| [setToolTip(String value)](#setToolTip-java.lang.String-) | Устанавливает всплывающую подсказку кнопки команды. |
| [setVisible(boolean value)](#setVisible-boolean-) | Устанавливает свойство Visible в Control |
| [setWidth(Unit value)](#setWidth-com.aspose.gridweb.Unit-) | Ширина кнопки. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CustomCommandButton() {#CustomCommandButton--}
```
public CustomCommandButton()
```


Конструктор по умолчанию.

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
### getClientClickEvent() {#getClientClickEvent--}
```
public String getClientClickEvent()
```


Получает обработчик события клика на стороне клиента.

**Returns:**
java.lang.String
### getCommand() {#getCommand--}
```
public String getCommand()
```


Получает имя команды.

**Returns:**
java.lang.String
### getCommandType() {#getCommandType--}
```
public int getCommandType()
```


Получает тип отображения команды. Тип может быть кнопкой команды или элементом контекстного меню.

Смотрите [CustomCommandButtonType](../../com.aspose.gridweb/customcommandbuttontype).

**Returns:**
int
### getDiscardInput() {#getDiscardInput--}
```
public boolean getDiscardInput()
```


Указывает, следует ли отбрасывать ввод пользователя в браузере клиента, когда пользователь нажимает эту кнопку. Может использоваться как действие "undo".

**Returns:**
boolean
### getImageUrl() {#getImageUrl--}
```
public String getImageUrl()
```


Получает URL изображения кнопки команды. Если установить значение null или пустую строку, кнопка будет отображать только свой текст.

**Returns:**
java.lang.String
### getText() {#getText--}
```
public String getText()
```


Получает альтернативный текст кнопки команды.

**Returns:**
java.lang.String
### getToolTip() {#getToolTip--}
```
public String getToolTip()
```


Получает всплывающую подсказку кнопки команды.

**Returns:**
java.lang.String
### getUniqueID() {#getUniqueID--}
```
public String getUniqueID()
```


Получает UniqueID в элементе управления.

**Returns:**
java.lang.String
### getVisible() {#getVisible--}
```
public boolean getVisible()
```


Получает свойство Visible в Control

**Returns:**
boolean
### getWidth() {#getWidth--}
```
public Unit getWidth()
```


Ширина кнопки.

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
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




### setClientClickEvent(String value) {#setClientClickEvent-java.lang.String-}
```
public void setClientClickEvent(String value)
```


Устанавливает обработчик события клика на клиентской стороне.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setCommand(String value) {#setCommand-java.lang.String-}
```
public void setCommand(String value)
```


Устанавливает имя команды.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setCommandType(int value) {#setCommandType-int-}
```
public void setCommandType(int value)
```


Устанавливает тип отображения команды. Тип может быть кнопкой команды или элементом контекстного меню.

Смотрите [CustomCommandButtonType](../../com.aspose.gridweb/customcommandbuttontype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setDiscardInput(boolean value) {#setDiscardInput-boolean-}
```
public void setDiscardInput(boolean value)
```


Указывает, следует ли отбрасывать ввод пользователя в браузере клиента, когда пользователь нажимает эту кнопку. Может использоваться как действие "undo".

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setImageUrl(String value) {#setImageUrl-java.lang.String-}
```
public void setImageUrl(String value)
```


Устанавливает URL изображения кнопки команды. Если установить значение null или пустую строку, кнопка будет отображать только свой текст.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Устанавливает альтернативный текст кнопки команды.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setToolTip(String value) {#setToolTip-java.lang.String-}
```
public void setToolTip(String value)
```


Устанавливает всплывающую подсказку кнопки команды.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Устанавливает свойство Visible в Control

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setWidth(Unit value) {#setWidth-com.aspose.gridweb.Unit-}
```
public void setWidth(Unit value)
```


Ширина кнопки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

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

