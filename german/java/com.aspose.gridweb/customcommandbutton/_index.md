---
title: "CustomCommandButton"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt einen benutzerdefinierten Befehls‑Button in der Registerkartenleiste des GridWeb‑Steuerelements dar."
type: docs
url: /de/java/com.aspose.gridweb/customcommandbutton/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.Control](../../com.aspose.gridweb/control)
```
public class CustomCommandButton extends Control
```

Stellt einen benutzerdefinierten Befehls‑Button in der Registerkartenleiste des GridWeb‑Steuerelements dar.

**Example**

```
         GridWebBean GridWeb1=ExtPage.getInstance().getBean();
         CustomCommandButton button = new CustomCommandButton();
         button.setCommand("MyCommand");
         button.setImageUrl("images/button1.gif");
         GridWeb1.getCustomCommandButtons().add(button);
```
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [CustomCommandButton()](#CustomCommandButton--) | Standardkonstruktor. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getClientClickEvent()](#getClientClickEvent--) | Gibt den Klick‑Ereignishandler auf der Client‑Seite zurück. |
| [getCommand()](#getCommand--) | Gibt den Befehlsnamen zurück. |
| [getCommandType()](#getCommandType--) | Gibt den Rendering‑Typ des Befehls zurück. |
| [getDiscardInput()](#getDiscardInput--) | Gibt an, ob Benutzereingaben im Client‑Browser verworfen werden sollen, wenn der Benutzer diesen Button anklickt. |
| [getImageUrl()](#getImageUrl--) | Ermittelt die Bild-URL des Befehlsbuttons. |
| [getText()](#getText--) | Ermittelt den Alternativtext der Befehls-Schaltfläche. |
| [getToolTip()](#getToolTip--) | Ermittelt den Tooltip der Befehls-Schaltfläche. |
| [getUniqueID()](#getUniqueID--) | Ruft die UniqueID im Steuerelement ab. |
| [getVisible()](#getVisible--) | Ermittelt die Visible im Control |
| [getWidth()](#getWidth--) | Breite der Schaltfläche. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setClientClickEvent(String value)](#setClientClickEvent-java.lang.String-) | Legt den Klick-Ereignishandler auf der Clientseite fest. |
| [setCommand(String value)](#setCommand-java.lang.String-) | Legt den Befehlsnamen fest. |
| [setCommandType(int value)](#setCommandType-int-) | Legt den Render-Typ des Befehls fest. |
| [setDiscardInput(boolean value)](#setDiscardInput-boolean-) | Gibt an, ob Benutzereingaben im Client‑Browser verworfen werden sollen, wenn der Benutzer diesen Button anklickt. |
| [setImageUrl(String value)](#setImageUrl-java.lang.String-) | Legt die Bild-URL der Befehls-Schaltfläche fest. |
| [setText(String value)](#setText-java.lang.String-) | Legt den Alternativtext der Befehls-Schaltfläche fest. |
| [setToolTip(String value)](#setToolTip-java.lang.String-) | Legt den Tooltip der Befehls-Schaltfläche fest. |
| [setVisible(boolean value)](#setVisible-boolean-) | Setzt die Visible im Control |
| [setWidth(Unit value)](#setWidth-com.aspose.gridweb.Unit-) | Breite der Schaltfläche. |
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
| Parameter | Typ | Beschreibung |
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


Gibt den Klick‑Ereignishandler auf der Client‑Seite zurück.

**Returns:**
java.lang.String
### getCommand() {#getCommand--}
```
public String getCommand()
```


Gibt den Befehlsnamen zurück.

**Returns:**
java.lang.String
### getCommandType() {#getCommandType--}
```
public int getCommandType()
```


Ermittelt den Render-Typ des Befehls. Der Typ kann Befehls-Schaltfläche oder Kontextmenüeintrag sein.

Siehe [CustomCommandButtonType](../../com.aspose.gridweb/customcommandbuttontype).

**Returns:**
int
### getDiscardInput() {#getDiscardInput--}
```
public boolean getDiscardInput()
```


Gibt an, ob Benutzereingaben im Client‑Browser verworfen werden sollen, wenn der Benutzer diese Schaltfläche klickt. Kann als "undo"-Aktion verwendet werden.

**Returns:**
boolean
### getImageUrl() {#getImageUrl--}
```
public String getImageUrl()
```


Ermittelt die Bild-URL der Befehls-Schaltfläche. Wenn sie auf null oder einen leeren String gesetzt wird, zeigt die Schaltfläche nur ihren Text an.

**Returns:**
java.lang.String
### getText() {#getText--}
```
public String getText()
```


Ermittelt den Alternativtext der Befehls-Schaltfläche.

**Returns:**
java.lang.String
### getToolTip() {#getToolTip--}
```
public String getToolTip()
```


Ermittelt den Tooltip der Befehls-Schaltfläche.

**Returns:**
java.lang.String
### getUniqueID() {#getUniqueID--}
```
public String getUniqueID()
```


Ruft die UniqueID im Steuerelement ab.

**Returns:**
java.lang.String
### getVisible() {#getVisible--}
```
public boolean getVisible()
```


Ermittelt die Visible im Control

**Returns:**
boolean
### getWidth() {#getWidth--}
```
public Unit getWidth()
```


Breite der Schaltfläche.

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


Legt den Klick-Ereignishandler auf der Clientseite fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setCommand(String value) {#setCommand-java.lang.String-}
```
public void setCommand(String value)
```


Legt den Befehlsnamen fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setCommandType(int value) {#setCommandType-int-}
```
public void setCommandType(int value)
```


Legt den Render-Typ des Befehls fest. Der Typ kann Befehls-Schaltfläche oder Kontextmenüeintrag sein.

Siehe [CustomCommandButtonType](../../com.aspose.gridweb/customcommandbuttontype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setDiscardInput(boolean value) {#setDiscardInput-boolean-}
```
public void setDiscardInput(boolean value)
```


Gibt an, ob Benutzereingaben im Client‑Browser verworfen werden sollen, wenn der Benutzer diese Schaltfläche klickt. Kann als "undo"-Aktion verwendet werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setImageUrl(String value) {#setImageUrl-java.lang.String-}
```
public void setImageUrl(String value)
```


Legt die Bild-URL der Befehls-Schaltfläche fest. Wenn sie auf null oder einen leeren String gesetzt wird, zeigt die Schaltfläche nur ihren Text an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Legt den Alternativtext der Befehls-Schaltfläche fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setToolTip(String value) {#setToolTip-java.lang.String-}
```
public void setToolTip(String value)
```


Legt den Tooltip der Befehls-Schaltfläche fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Setzt die Visible im Control

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setWidth(Unit value) {#setWidth-com.aspose.gridweb.Unit-}
```
public void setWidth(Unit value)
```


Breite der Schaltfläche.

**Parameters:**
| Parameter | Typ | Beschreibung |
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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

