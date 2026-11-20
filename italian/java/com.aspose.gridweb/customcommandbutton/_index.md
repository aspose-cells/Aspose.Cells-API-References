---
title: "CustomCommandButton"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta un pulsante di comando personalizzato nella barra delle schede del controllo GridWeb."
type: docs
url: /it/java/com.aspose.gridweb/customcommandbutton/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.Control](../../com.aspose.gridweb/control)
```
public class CustomCommandButton extends Control
```

Rappresenta un pulsante di comando personalizzato nella barra delle schede del controllo GridWeb.

**Example**

```
         GridWebBean GridWeb1=ExtPage.getInstance().getBean();
         CustomCommandButton button = new CustomCommandButton();
         button.setCommand("MyCommand");
         button.setImageUrl("images/button1.gif");
         GridWeb1.getCustomCommandButtons().add(button);
```
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [CustomCommandButton()](#CustomCommandButton--) | Costruttore predefinito. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getClientClickEvent()](#getClientClickEvent--) | Ottiene il gestore dell'evento click lato client. |
| [getCommand()](#getCommand--) | Ottiene il nome del comando. |
| [getCommandType()](#getCommandType--) | Ottiene il tipo di rendering del comando. |
| [getDiscardInput()](#getDiscardInput--) | Indica se scartare l'input dell'utente nel browser client quando l'utente fa clic su questo pulsante. |
| [getImageUrl()](#getImageUrl--) | Ottiene l'URL dell'immagine del pulsante di comando. |
| [getText()](#getText--) | Ottiene il testo alternativo del pulsante di comando. |
| [getToolTip()](#getToolTip--) | Ottiene il tooltip del pulsante di comando. |
| [getUniqueID()](#getUniqueID--) | Ottiene l'UniqueID nel Control |
| [getVisible()](#getVisible--) | Ottiene il Visible nel Control |
| [getWidth()](#getWidth--) | Larghezza del pulsante. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setClientClickEvent(String value)](#setClientClickEvent-java.lang.String-) | Imposta il gestore dell'evento click lato client. |
| [setCommand(String value)](#setCommand-java.lang.String-) | Imposta il nome del comando. |
| [setCommandType(int value)](#setCommandType-int-) | Imposta il tipo di rendering del comando. |
| [setDiscardInput(boolean value)](#setDiscardInput-boolean-) | Indica se scartare l'input dell'utente nel browser client quando l'utente fa clic su questo pulsante. |
| [setImageUrl(String value)](#setImageUrl-java.lang.String-) | Imposta l'URL dell'immagine del pulsante di comando. |
| [setText(String value)](#setText-java.lang.String-) | Imposta il testo alternativo del pulsante di comando. |
| [setToolTip(String value)](#setToolTip-java.lang.String-) | Imposta il tooltip del pulsante di comando. |
| [setVisible(boolean value)](#setVisible-boolean-) | Imposta il Visible nel Control |
| [setWidth(Unit value)](#setWidth-com.aspose.gridweb.Unit-) | Larghezza del pulsante. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CustomCommandButton() {#CustomCommandButton--}
```
public CustomCommandButton()
```


Costruttore predefinito.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
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


Ottiene il gestore dell'evento click lato client.

**Returns:**
java.lang.String
### getCommand() {#getCommand--}
```
public String getCommand()
```


Ottiene il nome del comando.

**Returns:**
java.lang.String
### getCommandType() {#getCommandType--}
```
public int getCommandType()
```


Restituisce il tipo di rendering del comando. Il tipo può essere pulsante di comando o voce di menu contestuale.

Vedi [CustomCommandButtonType](../../com.aspose.gridweb/customcommandbuttontype).

**Returns:**
int
### getDiscardInput() {#getDiscardInput--}
```
public boolean getDiscardInput()
```


Indica se scartare l'input dell'utente nel browser client quando l'utente clicca questo pulsante. Può essere usato come azione di "annullamento".

**Returns:**
boolean
### getImageUrl() {#getImageUrl--}
```
public String getImageUrl()
```


Restituisce l'URL dell'immagine del pulsante di comando. Se impostato a null o stringa vuota, il pulsante mostrerà solo il suo testo.

**Returns:**
java.lang.String
### getText() {#getText--}
```
public String getText()
```


Ottiene il testo alternativo del pulsante di comando.

**Returns:**
java.lang.String
### getToolTip() {#getToolTip--}
```
public String getToolTip()
```


Ottiene il tooltip del pulsante di comando.

**Returns:**
java.lang.String
### getUniqueID() {#getUniqueID--}
```
public String getUniqueID()
```


Ottiene l'UniqueID nel Control

**Returns:**
java.lang.String
### getVisible() {#getVisible--}
```
public boolean getVisible()
```


Ottiene il Visible nel Control

**Returns:**
boolean
### getWidth() {#getWidth--}
```
public Unit getWidth()
```


Larghezza del pulsante.

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


Imposta il gestore dell'evento click lato client.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setCommand(String value) {#setCommand-java.lang.String-}
```
public void setCommand(String value)
```


Imposta il nome del comando.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setCommandType(int value) {#setCommandType-int-}
```
public void setCommandType(int value)
```


Imposta il tipo di rendering del comando. Il tipo può essere pulsante di comando o voce di menu contestuale.

Vedi [CustomCommandButtonType](../../com.aspose.gridweb/customcommandbuttontype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setDiscardInput(boolean value) {#setDiscardInput-boolean-}
```
public void setDiscardInput(boolean value)
```


Indica se scartare l'input dell'utente nel browser client quando l'utente clicca questo pulsante. Può essere usato come azione di "annullamento".

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setImageUrl(String value) {#setImageUrl-java.lang.String-}
```
public void setImageUrl(String value)
```


Imposta l'URL dell'immagine del pulsante di comando. Se impostato a null o stringa vuota, il pulsante mostrerà solo il suo testo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Imposta il testo alternativo del pulsante di comando.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setToolTip(String value) {#setToolTip-java.lang.String-}
```
public void setToolTip(String value)
```


Imposta il tooltip del pulsante di comando.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Imposta il Visible nel Control

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setWidth(Unit value) {#setWidth-com.aspose.gridweb.Unit-}
```
public void setWidth(Unit value)
```


Larghezza del pulsante.

**Parameters:**
| Parametro | Tipo | Descrizione |
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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

