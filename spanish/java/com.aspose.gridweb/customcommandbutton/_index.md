---
title: "CustomCommandButton"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa un botón de comando personalizado en la barra de pestañas del control GridWeb."
type: docs
url: /es/java/com.aspose.gridweb/customcommandbutton/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.Control](../../com.aspose.gridweb/control)
```
public class CustomCommandButton extends Control
```

Representa un botón de comando personalizado en la barra de pestañas del control GridWeb.

**Example**

```
         GridWebBean GridWeb1=ExtPage.getInstance().getBean();
         CustomCommandButton button = new CustomCommandButton();
         button.setCommand("MyCommand");
         button.setImageUrl("images/button1.gif");
         GridWeb1.getCustomCommandButtons().add(button);
```
## Constructores

| Constructor | Descripción |
| --- | --- |
| [CustomCommandButton()](#CustomCommandButton--) | Constructor predeterminado. |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getClientClickEvent()](#getClientClickEvent--) | Obtiene el controlador del evento de clic en el lado del cliente. |
| [getCommand()](#getCommand--) | Obtiene el nombre del comando. |
| [getCommandType()](#getCommandType--) | Obtiene el tipo de renderizado del comando. |
| [getDiscardInput()](#getDiscardInput--) | Indica si se debe descartar la entrada del usuario en el navegador cliente cuando el usuario hace clic en este botón. |
| [getImageUrl()](#getImageUrl--) | Obtiene la URL de la imagen del botón de comando. |
| [getText()](#getText--) | Obtiene el texto alternativo del botón de comando. |
| [getToolTip()](#getToolTip--) | Obtiene la información sobre herramienta del botón de comando. |
| [getUniqueID()](#getUniqueID--) | Obtiene el UniqueID en el Control |
| [getVisible()](#getVisible--) | Obtiene la propiedad Visible en el Control |
| [getWidth()](#getWidth--) | Ancho del botón. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setClientClickEvent(String value)](#setClientClickEvent-java.lang.String-) | Establece el controlador del evento de clic en el lado del cliente. |
| [setCommand(String value)](#setCommand-java.lang.String-) | Establece el nombre del comando. |
| [setCommandType(int value)](#setCommandType-int-) | Establece el tipo de renderizado del comando. |
| [setDiscardInput(boolean value)](#setDiscardInput-boolean-) | Indica si se debe descartar la entrada del usuario en el navegador cliente cuando el usuario hace clic en este botón. |
| [setImageUrl(String value)](#setImageUrl-java.lang.String-) | Establece la URL de la imagen del botón de comando. |
| [setText(String value)](#setText-java.lang.String-) | Establece el texto alternativo del botón de comando. |
| [setToolTip(String value)](#setToolTip-java.lang.String-) | Establece la información emergente del botón de comando. |
| [setVisible(boolean value)](#setVisible-boolean-) | Establece la propiedad Visible en el Control |
| [setWidth(Unit value)](#setWidth-com.aspose.gridweb.Unit-) | Ancho del botón. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CustomCommandButton() {#CustomCommandButton--}
```
public CustomCommandButton()
```


Constructor predeterminado.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
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


Obtiene el controlador del evento de clic en el lado del cliente.

**Returns:**
java.lang.String
### getCommand() {#getCommand--}
```
public String getCommand()
```


Obtiene el nombre del comando.

**Returns:**
java.lang.String
### getCommandType() {#getCommandType--}
```
public int getCommandType()
```


Obtiene el tipo de renderizado del comando. El tipo puede ser botón de comando o elemento de menú contextual.

Ver [CustomCommandButtonType](../../com.aspose.gridweb/customcommandbuttontype).

**Returns:**
int
### getDiscardInput() {#getDiscardInput--}
```
public boolean getDiscardInput()
```


Indica si se debe descartar la entrada del usuario en el navegador cliente cuando el usuario hace clic en este botón. Puede usarse como una acción de "deshacer".

**Returns:**
boolean
### getImageUrl() {#getImageUrl--}
```
public String getImageUrl()
```


Obtiene la URL de la imagen del botón de comando. Si se establece en null o cadena vacía, el botón solo mostrará su texto.

**Returns:**
java.lang.String
### getText() {#getText--}
```
public String getText()
```


Obtiene el texto alternativo del botón de comando.

**Returns:**
java.lang.String
### getToolTip() {#getToolTip--}
```
public String getToolTip()
```


Obtiene la información sobre herramienta del botón de comando.

**Returns:**
java.lang.String
### getUniqueID() {#getUniqueID--}
```
public String getUniqueID()
```


Obtiene el UniqueID en el Control

**Returns:**
java.lang.String
### getVisible() {#getVisible--}
```
public boolean getVisible()
```


Obtiene la propiedad Visible en el Control

**Returns:**
boolean
### getWidth() {#getWidth--}
```
public Unit getWidth()
```


Ancho del botón.

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


Establece el controlador del evento de clic en el lado del cliente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setCommand(String value) {#setCommand-java.lang.String-}
```
public void setCommand(String value)
```


Establece el nombre del comando.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setCommandType(int value) {#setCommandType-int-}
```
public void setCommandType(int value)
```


Establece el tipo de renderizado del comando. El tipo puede ser botón de comando o elemento de menú contextual.

Ver [CustomCommandButtonType](../../com.aspose.gridweb/customcommandbuttontype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setDiscardInput(boolean value) {#setDiscardInput-boolean-}
```
public void setDiscardInput(boolean value)
```


Indica si se debe descartar la entrada del usuario en el navegador cliente cuando el usuario hace clic en este botón. Puede usarse como una acción de "deshacer".

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setImageUrl(String value) {#setImageUrl-java.lang.String-}
```
public void setImageUrl(String value)
```


Establece la URL de la imagen del botón de comando. Si se establece en null o cadena vacía, el botón solo mostrará su texto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Establece el texto alternativo del botón de comando.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setToolTip(String value) {#setToolTip-java.lang.String-}
```
public void setToolTip(String value)
```


Establece la información emergente del botón de comando.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Establece la propiedad Visible en el Control

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setWidth(Unit value) {#setWidth-com.aspose.gridweb.Unit-}
```
public void setWidth(Unit value)
```


Ancho del botón.

**Parameters:**
| Parámetro | Tipo | Descripción |
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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

