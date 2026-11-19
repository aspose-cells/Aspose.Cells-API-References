---
title: "CustomCommandButton"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente un bouton de commande personnalisé dans la barre d'onglets du contrôle GridWeb."
type: docs
url: /fr/java/com.aspose.gridweb/customcommandbutton/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.Control](../../com.aspose.gridweb/control)
```
public class CustomCommandButton extends Control
```

Représente un bouton de commande personnalisé dans la barre d'onglets du contrôle GridWeb.

**Example**

```
         GridWebBean GridWeb1=ExtPage.getInstance().getBean();
         CustomCommandButton button = new CustomCommandButton();
         button.setCommand("MyCommand");
         button.setImageUrl("images/button1.gif");
         GridWeb1.getCustomCommandButtons().add(button);
```
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [CustomCommandButton()](#CustomCommandButton--) | Constructeur par défaut. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getClientClickEvent()](#getClientClickEvent--) | Obtient le gestionnaire d'événement de clic côté client. |
| [getCommand()](#getCommand--) | Obtient le nom de la commande. |
| [getCommandType()](#getCommandType--) | Obtient le type de rendu de la commande. |
| [getDiscardInput()](#getDiscardInput--) | Indique s'il faut ignorer l'entrée utilisateur dans le navigateur client lorsque l'utilisateur clique sur ce bouton. |
| [getImageUrl()](#getImageUrl--) | Obtient l'URL de l'image du bouton de commande. |
| [getText()](#getText--) | Obtient le texte alternatif du bouton de commande. |
| [getToolTip()](#getToolTip--) | Obtient l'infobulle du bouton de commande. |
| [getUniqueID()](#getUniqueID--) | Obtient l'UniqueID dans le Contrôle |
| [getVisible()](#getVisible--) | Obtient le Visible dans le Control |
| [getWidth()](#getWidth--) | Largeur du bouton. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setClientClickEvent(String value)](#setClientClickEvent-java.lang.String-) | Définit le gestionnaire d'événement de clic côté client. |
| [setCommand(String value)](#setCommand-java.lang.String-) | Définit le nom de la commande. |
| [setCommandType(int value)](#setCommandType-int-) | Définit le type de rendu de la commande. |
| [setDiscardInput(boolean value)](#setDiscardInput-boolean-) | Indique s'il faut ignorer l'entrée utilisateur dans le navigateur client lorsque l'utilisateur clique sur ce bouton. |
| [setImageUrl(String value)](#setImageUrl-java.lang.String-) | Définit l'URL de l'image du bouton de commande. |
| [setText(String value)](#setText-java.lang.String-) | Définit le texte alternatif du bouton de commande. |
| [setToolTip(String value)](#setToolTip-java.lang.String-) | Définit l'infobulle du bouton de commande. |
| [setVisible(boolean value)](#setVisible-boolean-) | Définit le Visible dans le Control |
| [setWidth(Unit value)](#setWidth-com.aspose.gridweb.Unit-) | Largeur du bouton. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CustomCommandButton() {#CustomCommandButton--}
```
public CustomCommandButton()
```


Constructeur par défaut.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Paramètre | Type | Description |
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


Obtient le gestionnaire d'événement de clic côté client.

**Returns:**
java.lang.String
### getCommand() {#getCommand--}
```
public String getCommand()
```


Obtient le nom de la commande.

**Returns:**
java.lang.String
### getCommandType() {#getCommandType--}
```
public int getCommandType()
```


Obtient le type de rendu de la commande. Le type peut être un bouton de commande ou un élément de menu contextuel.

Voir [CustomCommandButtonType](../../com.aspose.gridweb/customcommandbuttontype).

**Returns:**
int
### getDiscardInput() {#getDiscardInput--}
```
public boolean getDiscardInput()
```


Indique s'il faut ignorer l'entrée utilisateur dans le navigateur client lorsque l'utilisateur clique sur ce bouton. Peut être utilisé comme une action "annuler".

**Returns:**
boolean
### getImageUrl() {#getImageUrl--}
```
public String getImageUrl()
```


Obtient l'URL de l'image du bouton de commande. Si elle est définie sur null ou une chaîne vide, le bouton n'affichera que son texte.

**Returns:**
java.lang.String
### getText() {#getText--}
```
public String getText()
```


Obtient le texte alternatif du bouton de commande.

**Returns:**
java.lang.String
### getToolTip() {#getToolTip--}
```
public String getToolTip()
```


Obtient l'infobulle du bouton de commande.

**Returns:**
java.lang.String
### getUniqueID() {#getUniqueID--}
```
public String getUniqueID()
```


Obtient l'UniqueID dans le Contrôle

**Returns:**
java.lang.String
### getVisible() {#getVisible--}
```
public boolean getVisible()
```


Obtient le Visible dans le Control

**Returns:**
boolean
### getWidth() {#getWidth--}
```
public Unit getWidth()
```


Largeur du bouton.

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


Définit le gestionnaire d'événement de clic côté client.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setCommand(String value) {#setCommand-java.lang.String-}
```
public void setCommand(String value)
```


Définit le nom de la commande.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setCommandType(int value) {#setCommandType-int-}
```
public void setCommandType(int value)
```


Définit le type de rendu de la commande. Le type peut être un bouton de commande ou un élément de menu contextuel.

Voir [CustomCommandButtonType](../../com.aspose.gridweb/customcommandbuttontype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setDiscardInput(boolean value) {#setDiscardInput-boolean-}
```
public void setDiscardInput(boolean value)
```


Indique s'il faut ignorer l'entrée utilisateur dans le navigateur client lorsque l'utilisateur clique sur ce bouton. Peut être utilisé comme une action "annuler".

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setImageUrl(String value) {#setImageUrl-java.lang.String-}
```
public void setImageUrl(String value)
```


Définit l'URL de l'image du bouton de commande. Si elle est définie sur null ou une chaîne vide, le bouton n'affichera que son texte.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Définit le texte alternatif du bouton de commande.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setToolTip(String value) {#setToolTip-java.lang.String-}
```
public void setToolTip(String value)
```


Définit l'infobulle du bouton de commande.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Définit le Visible dans le Control

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setWidth(Unit value) {#setWidth-com.aspose.gridweb.Unit-}
```
public void setWidth(Unit value)
```


Largeur du bouton.

**Parameters:**
| Paramètre | Type | Description |
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
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

