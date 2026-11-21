---
title: "CustomCommandButton"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar en anpassad kommandoknapp i flikfältet för GridWeb‑kontrollen."
type: docs
url: /sv/java/com.aspose.gridweb/customcommandbutton/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.Control](../../com.aspose.gridweb/control)
```
public class CustomCommandButton extends Control
```

Representerar en anpassad kommandoknapp i flikfältet för GridWeb‑kontrollen.

**Example**

```
         GridWebBean GridWeb1=ExtPage.getInstance().getBean();
         CustomCommandButton button = new CustomCommandButton();
         button.setCommand("MyCommand");
         button.setImageUrl("images/button1.gif");
         GridWeb1.getCustomCommandButtons().add(button);
```
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [CustomCommandButton()](#CustomCommandButton--) | Standardkonstruktor. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getClientClickEvent()](#getClientClickEvent--) | Hämtar klickhändelsehanteraren på klientsidan. |
| [getCommand()](#getCommand--) | Hämtar kommandonamnet. |
| [getCommandType()](#getCommandType--) | Hämtar renderingstypen för kommandot. |
| [getDiscardInput()](#getDiscardInput--) | Indikerar om användarens inmatning i webbläsaren ska förkastas när användaren klickar på den här knappen. |
| [getImageUrl()](#getImageUrl--) | Hämtar bild‑URL:en för kommandoknappen. |
| [getText()](#getText--) | Hämtar den alternativa texten för kommandoknappen. |
| [getToolTip()](#getToolTip--) | Hämtar verktygstipset för kommandoknappen. |
| [getUniqueID()](#getUniqueID--) | Hämtar UniqueID i kontrollen |
| [getVisible()](#getVisible--) | Hämtar Visible i Control |
| [getWidth()](#getWidth--) | Knappens bredd. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setClientClickEvent(String value)](#setClientClickEvent-java.lang.String-) | Ställer in klickhändelsehanteraren på klientsidan. |
| [setCommand(String value)](#setCommand-java.lang.String-) | Ställer in kommandots namn. |
| [setCommandType(int value)](#setCommandType-int-) | Ställer in renderings typen för kommandot. |
| [setDiscardInput(boolean value)](#setDiscardInput-boolean-) | Indikerar om användarens inmatning i webbläsaren ska förkastas när användaren klickar på den här knappen. |
| [setImageUrl(String value)](#setImageUrl-java.lang.String-) | Ställer in kommandoknappens bild‑URL. |
| [setText(String value)](#setText-java.lang.String-) | Ställer in den alternativa texten för kommandoknappen. |
| [setToolTip(String value)](#setToolTip-java.lang.String-) | Ställer in verktygstipset för kommandoknappen. |
| [setVisible(boolean value)](#setVisible-boolean-) | Sätter Visible i Control |
| [setWidth(Unit value)](#setWidth-com.aspose.gridweb.Unit-) | Knappens bredd. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CustomCommandButton() {#CustomCommandButton--}
```
public CustomCommandButton()
```


Standardkonstruktor.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
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


Hämtar klickhändelsehanteraren på klientsidan.

**Returns:**
java.lang.String
### getCommand() {#getCommand--}
```
public String getCommand()
```


Hämtar kommandonamnet.

**Returns:**
java.lang.String
### getCommandType() {#getCommandType--}
```
public int getCommandType()
```


Hämtar renderings typen för kommandot. Typen kan vara kommandoknapp eller kontextmenyobjekt.

Se [CustomCommandButtonType](../../com.aspose.gridweb/customcommandbuttontype).

**Returns:**
int
### getDiscardInput() {#getDiscardInput--}
```
public boolean getDiscardInput()
```


Anger om användarinmatning ska förkastas i klientens webbläsare när användaren klickar på den här knappen. Kan användas som en "ångra"‑åtgärd.

**Returns:**
boolean
### getImageUrl() {#getImageUrl--}
```
public String getImageUrl()
```


Hämtar kommandoknappens bild‑URL. Om den sätts till null eller en tom sträng visas bara knappens text.

**Returns:**
java.lang.String
### getText() {#getText--}
```
public String getText()
```


Hämtar den alternativa texten för kommandoknappen.

**Returns:**
java.lang.String
### getToolTip() {#getToolTip--}
```
public String getToolTip()
```


Hämtar verktygstipset för kommandoknappen.

**Returns:**
java.lang.String
### getUniqueID() {#getUniqueID--}
```
public String getUniqueID()
```


Hämtar UniqueID i kontrollen

**Returns:**
java.lang.String
### getVisible() {#getVisible--}
```
public boolean getVisible()
```


Hämtar Visible i Control

**Returns:**
boolean
### getWidth() {#getWidth--}
```
public Unit getWidth()
```


Knappens bredd.

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


Ställer in klickhändelsehanteraren på klientsidan.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setCommand(String value) {#setCommand-java.lang.String-}
```
public void setCommand(String value)
```


Ställer in kommandots namn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setCommandType(int value) {#setCommandType-int-}
```
public void setCommandType(int value)
```


Ställer in renderings typen för kommandot. Typen kan vara kommandoknapp eller kontextmenyobjekt.

Se [CustomCommandButtonType](../../com.aspose.gridweb/customcommandbuttontype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setDiscardInput(boolean value) {#setDiscardInput-boolean-}
```
public void setDiscardInput(boolean value)
```


Anger om användarinmatning ska förkastas i klientens webbläsare när användaren klickar på den här knappen. Kan användas som en "ångra"‑åtgärd.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setImageUrl(String value) {#setImageUrl-java.lang.String-}
```
public void setImageUrl(String value)
```


Ställer in kommandoknappens bild‑URL. Om den sätts till null eller en tom sträng visas bara knappens text.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Ställer in den alternativa texten för kommandoknappen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setToolTip(String value) {#setToolTip-java.lang.String-}
```
public void setToolTip(String value)
```


Ställer in verktygstipset för kommandoknappen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Sätter Visible i Control

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setWidth(Unit value) {#setWidth-com.aspose.gridweb.Unit-}
```
public void setWidth(Unit value)
```


Knappens bredd.

**Parameters:**
| Parameter | Typ | Beskrivning |
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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

