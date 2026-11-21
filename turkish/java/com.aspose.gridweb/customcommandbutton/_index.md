---
title: "CustomCommandButton"
second_title: "Aspose.Cells for Java API Referansı"
description: "GridWeb kontrolünün sekme çubuğunda özel bir komut düğmesini temsil eder."
type: docs
url: /tr/java/com.aspose.gridweb/customcommandbutton/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.Control](../../com.aspose.gridweb/control)
```
public class CustomCommandButton extends Control
```

GridWeb kontrolünün sekme çubuğunda özel bir komut düğmesini temsil eder.

**Example**

```
         GridWebBean GridWeb1=ExtPage.getInstance().getBean();
         CustomCommandButton button = new CustomCommandButton();
         button.setCommand("MyCommand");
         button.setImageUrl("images/button1.gif");
         GridWeb1.getCustomCommandButtons().add(button);
```
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [CustomCommandButton()](#CustomCommandButton--) | Varsayılan yapıcı. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getClientClickEvent()](#getClientClickEvent--) | İstemci tarafındaki tıklama olayı işleyicisini alır. |
| [getCommand()](#getCommand--) | Komut adını alır. |
| [getCommandType()](#getCommandType--) | Komutun renderleme tipini alır. |
| [getDiscardInput()](#getDiscardInput--) | Kullanıcı bu düğmeye tıkladığında istemci tarayıcısındaki kullanıcı girişinin atlanıp atlanmayacağını gösterir. |
| [getImageUrl()](#getImageUrl--) | Komut düğmesinin resim URL'sini alır. |
| [getText()](#getText--) | Komut düğmesinin alternatif metnini alır. |
| [getToolTip()](#getToolTip--) | Komut düğmesinin araç ipucunu alır. |
| [getUniqueID()](#getUniqueID--) | Denetimde UniqueID'yi alır |
| [getVisible()](#getVisible--) | Control içindeki Visible özelliğini alır |
| [getWidth()](#getWidth--) | Düğmenin genişliği. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setClientClickEvent(String value)](#setClientClickEvent-java.lang.String-) | İstemci tarafında tıklama olayı işleyicisini ayarlar. |
| [setCommand(String value)](#setCommand-java.lang.String-) | Komut adını ayarlar. |
| [setCommandType(int value)](#setCommandType-int-) | Komutun renderleme türünü ayarlar. |
| [setDiscardInput(boolean value)](#setDiscardInput-boolean-) | Kullanıcı bu düğmeye tıkladığında istemci tarayıcısındaki kullanıcı girişinin atlanıp atlanmayacağını gösterir. |
| [setImageUrl(String value)](#setImageUrl-java.lang.String-) | Komut düğmesinin resim URL'sini ayarlar. |
| [setText(String value)](#setText-java.lang.String-) | Komut düğmesinin alternatif metnini ayarlar. |
| [setToolTip(String value)](#setToolTip-java.lang.String-) | Komut düğmesinin araç ipucunu ayarlar. |
| [setVisible(boolean value)](#setVisible-boolean-) | Control içindeki Visible özelliğini ayarlar |
| [setWidth(Unit value)](#setWidth-com.aspose.gridweb.Unit-) | Düğmenin genişliği. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CustomCommandButton() {#CustomCommandButton--}
```
public CustomCommandButton()
```


Varsayılan yapıcı.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
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


İstemci tarafındaki tıklama olayı işleyicisini alır.

**Returns:**
java.lang.String
### getCommand() {#getCommand--}
```
public String getCommand()
```


Komut adını alır.

**Returns:**
java.lang.String
### getCommandType() {#getCommandType--}
```
public int getCommandType()
```


Komutun renderleme türünü alır. Tür, komut düğmesi veya bağlam menüsü öğesi olabilir.

Bakın [CustomCommandButtonType](../../com.aspose.gridweb/customcommandbuttontype).

**Returns:**
int
### getDiscardInput() {#getDiscardInput--}
```
public boolean getDiscardInput()
```


Kullanıcı bu düğmeye tıkladığında istemci tarayıcısındaki kullanıcı girdisinin atılıp atılmayacağını gösterir. "undo" eylemi olarak kullanılabilir.

**Returns:**
boolean
### getImageUrl() {#getImageUrl--}
```
public String getImageUrl()
```


Komut düğmesinin resim URL'sini alır. Null veya boş dizeye ayarlanırsa, düğme yalnızca metnini gösterir.

**Returns:**
java.lang.String
### getText() {#getText--}
```
public String getText()
```


Komut düğmesinin alternatif metnini alır.

**Returns:**
java.lang.String
### getToolTip() {#getToolTip--}
```
public String getToolTip()
```


Komut düğmesinin araç ipucunu alır.

**Returns:**
java.lang.String
### getUniqueID() {#getUniqueID--}
```
public String getUniqueID()
```


Denetimde UniqueID'yi alır

**Returns:**
java.lang.String
### getVisible() {#getVisible--}
```
public boolean getVisible()
```


Control içindeki Visible özelliğini alır

**Returns:**
boolean
### getWidth() {#getWidth--}
```
public Unit getWidth()
```


Düğmenin genişliği.

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


İstemci tarafında tıklama olayı işleyicisini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setCommand(String value) {#setCommand-java.lang.String-}
```
public void setCommand(String value)
```


Komut adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setCommandType(int value) {#setCommandType-int-}
```
public void setCommandType(int value)
```


Komutun renderleme türünü ayarlar. Tür, komut düğmesi veya bağlam menüsü öğesi olabilir.

Bakın [CustomCommandButtonType](../../com.aspose.gridweb/customcommandbuttontype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setDiscardInput(boolean value) {#setDiscardInput-boolean-}
```
public void setDiscardInput(boolean value)
```


Kullanıcı bu düğmeye tıkladığında istemci tarayıcısındaki kullanıcı girdisinin atılıp atılmayacağını gösterir. "undo" eylemi olarak kullanılabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setImageUrl(String value) {#setImageUrl-java.lang.String-}
```
public void setImageUrl(String value)
```


Komut düğmesinin resim URL'sini ayarlar. Null veya boş dizeye ayarlanırsa, düğme yalnızca metnini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Komut düğmesinin alternatif metnini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setToolTip(String value) {#setToolTip-java.lang.String-}
```
public void setToolTip(String value)
```


Komut düğmesinin araç ipucunu ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Control içindeki Visible özelliğini ayarlar

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setWidth(Unit value) {#setWidth-com.aspose.gridweb.Unit-}
```
public void setWidth(Unit value)
```


Düğmenin genişliği.

**Parameters:**
| Parametre | Tür | Açıklama |
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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

