---
title: "CustomCommandButton"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل زر أمر مخصص في شريط علامات التبويب لعنصر التحكم GridWeb."
type: docs
url: /ar/java/com.aspose.gridweb/customcommandbutton/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.Control](../../com.aspose.gridweb/control)
```
public class CustomCommandButton extends Control
```

يمثل زر أمر مخصص في شريط علامات التبويب لعنصر التحكم GridWeb.

**Example**

```
         GridWebBean GridWeb1=ExtPage.getInstance().getBean();
         CustomCommandButton button = new CustomCommandButton();
         button.setCommand("MyCommand");
         button.setImageUrl("images/button1.gif");
         GridWeb1.getCustomCommandButtons().add(button);
```
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [CustomCommandButton()](#CustomCommandButton--) | المنشئ الافتراضي. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getClientClickEvent()](#getClientClickEvent--) | يحصل على معالج حدث النقر على جانب العميل. |
| [getCommand()](#getCommand--) | يحصل على اسم الأمر. |
| [getCommandType()](#getCommandType--) | يحصل على نوع العرض للأمر. |
| [getDiscardInput()](#getDiscardInput--) | يشير إلى ما إذا كان يجب تجاهل إدخال المستخدم في متصفح العميل عندما ينقر المستخدم على هذا الزر. |
| [getImageUrl()](#getImageUrl--) | يحصل على عنوان URL لصورة زر الأمر. |
| [getText()](#getText--) | يحصل على النص البديل لزر الأمر. |
| [getToolTip()](#getToolTip--) | يحصل على تلميح الأداة لزر الأمر. |
| [getUniqueID()](#getUniqueID--) | يحصل على UniqueID في التحكم |
| [getVisible()](#getVisible--) | يحصل على Visible في الـ Control |
| [getWidth()](#getWidth--) | عرض الزر. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setClientClickEvent(String value)](#setClientClickEvent-java.lang.String-) | يضبط معالج حدث النقر على جانب العميل. |
| [setCommand(String value)](#setCommand-java.lang.String-) | يضبط اسم الأمر. |
| [setCommandType(int value)](#setCommandType-int-) | يضبط نوع العرض للأمر. |
| [setDiscardInput(boolean value)](#setDiscardInput-boolean-) | يشير إلى ما إذا كان يجب تجاهل إدخال المستخدم في متصفح العميل عندما ينقر المستخدم على هذا الزر. |
| [setImageUrl(String value)](#setImageUrl-java.lang.String-) | يضبط عنوان URL لصورة زر الأمر. |
| [setText(String value)](#setText-java.lang.String-) | يضبط النص البديل لزر الأمر. |
| [setToolTip(String value)](#setToolTip-java.lang.String-) | يضبط تلميح الأداة لزر الأمر. |
| [setVisible(boolean value)](#setVisible-boolean-) | يضبط Visible في الـ Control |
| [setWidth(Unit value)](#setWidth-com.aspose.gridweb.Unit-) | عرض الزر. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CustomCommandButton() {#CustomCommandButton--}
```
public CustomCommandButton()
```


المنشئ الافتراضي.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
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


يحصل على معالج حدث النقر على جانب العميل.

**Returns:**
java.lang.String
### getCommand() {#getCommand--}
```
public String getCommand()
```


يحصل على اسم الأمر.

**Returns:**
java.lang.String
### getCommandType() {#getCommandType--}
```
public int getCommandType()
```


يحصل على نوع العرض للأمر. يمكن أن يكون النوع زر أمر أو عنصر قائمة سياقية.

انظر [CustomCommandButtonType](../../com.aspose.gridweb/customcommandbuttontype).

**Returns:**
int
### getDiscardInput() {#getDiscardInput--}
```
public boolean getDiscardInput()
```


يشير إلى ما إذا كان يجب تجاهل إدخال المستخدم في متصفح العميل عندما ينقر المستخدم هذا الزر. يمكن استخدامه كإجراء "تراجع".

**Returns:**
boolean
### getImageUrl() {#getImageUrl--}
```
public String getImageUrl()
```


يحصل على عنوان URL لصورة زر الأمر. إذا تم تعيينه إلى null أو سلسلة فارغة، سيعرض الزر نصه فقط.

**Returns:**
java.lang.String
### getText() {#getText--}
```
public String getText()
```


يحصل على النص البديل لزر الأمر.

**Returns:**
java.lang.String
### getToolTip() {#getToolTip--}
```
public String getToolTip()
```


يحصل على تلميح الأداة لزر الأمر.

**Returns:**
java.lang.String
### getUniqueID() {#getUniqueID--}
```
public String getUniqueID()
```


يحصل على UniqueID في التحكم

**Returns:**
java.lang.String
### getVisible() {#getVisible--}
```
public boolean getVisible()
```


يحصل على Visible في الـ Control

**Returns:**
boolean
### getWidth() {#getWidth--}
```
public Unit getWidth()
```


عرض الزر.

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


يضبط معالج حدث النقر على جانب العميل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setCommand(String value) {#setCommand-java.lang.String-}
```
public void setCommand(String value)
```


يضبط اسم الأمر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setCommandType(int value) {#setCommandType-int-}
```
public void setCommandType(int value)
```


يضبط نوع العرض للأمر. يمكن أن يكون النوع زر أمر أو عنصر قائمة سياقية.

انظر [CustomCommandButtonType](../../com.aspose.gridweb/customcommandbuttontype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setDiscardInput(boolean value) {#setDiscardInput-boolean-}
```
public void setDiscardInput(boolean value)
```


يشير إلى ما إذا كان يجب تجاهل إدخال المستخدم في متصفح العميل عندما ينقر المستخدم هذا الزر. يمكن استخدامه كإجراء "تراجع".

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setImageUrl(String value) {#setImageUrl-java.lang.String-}
```
public void setImageUrl(String value)
```


يضبط عنوان URL لصورة زر الأمر. إذا تم تعيينه إلى null أو سلسلة فارغة، سيعرض الزر نصه فقط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


يضبط النص البديل لزر الأمر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setToolTip(String value) {#setToolTip-java.lang.String-}
```
public void setToolTip(String value)
```


يضبط تلميح الأداة لزر الأمر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


يضبط Visible في الـ Control

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setWidth(Unit value) {#setWidth-com.aspose.gridweb.Unit-}
```
public void setWidth(Unit value)
```


عرض الزر.

**Parameters:**
| معامل | نوع | الوصف |
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
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

