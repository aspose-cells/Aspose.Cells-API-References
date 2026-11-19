---
title: "GridHyperlink"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Encapsule l'objet qui représente un hyperlien."
type: docs
url: /fr/java/com.aspose.gridweb/gridhyperlink/
---

**Inheritance:**
java.lang.Object
```
public class GridHyperlink
```

Encapsule l'objet qui représente un hyperlien.
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAddress()](#getAddress--) | Représente l'adresse d'un lien hypertexte. |
| [getAltText()](#getAltText--) | Obtient le texte alternatif pour le lien image, veuillez noter qu'il s'agit d'un attribut d'extension qui ne peut pas être conservé dans le fichier Excel. |
| [getArea()](#getArea--) | Obtient la plage du lien hypertexte. |
| [getClass()](#getClass--) |  |
| [getCommand()](#getCommand--) | Renvoie ou définit le texte de valeur de commande défini par l'utilisateur pour le lien hypertexte spécifié. |
| [getDiscardInput()](#getDiscardInput--) | Indique s'il faut ignorer l'entrée utilisateur dans le navigateur client lorsque l'utilisateur clique sur ce lien hypertexte CellCommand. |
| [getImageURL()](#getImageURL--) | Obtient l'URL de l'image pour le lien, il n'existe pas de propriété imageurl dans le lien hypertexte, donc on utilise en fait TextToDisplay pour enregistrer cette valeur. TextToDisplay sera défini sur <img src=valeur> ce qui modifiera la valeur de TextToDisplay. |
| [getScreenTip()](#getScreenTip--) | Renvoie ou définit le texte d'infobulle pour le lien hypertexte spécifié. |
| [getTarget()](#getTarget--) | Obtient le type de cible du lien web, veuillez noter qu'il s'agit d'un attribut d'extension qui ne peut pas être conservé dans le fichier Excel. |
| [getTextToDisplay()](#getTextToDisplay--) | Représente le texte à afficher pour le lien hypertexte spécifié. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAddress(String value)](#setAddress-java.lang.String-) | Représente l'adresse d'un lien hypertexte. |
| [setAltText(String value)](#setAltText-java.lang.String-) | Définit le texte alternatif pour le lien image, veuillez noter qu'il s'agit d'un attribut d'extension qui ne peut pas être conservé dans le fichier Excel. |
| [setCommand(String value)](#setCommand-java.lang.String-) | Renvoie ou définit le texte de valeur de commande défini par l'utilisateur pour le lien hypertexte spécifié. |
| [setDiscardInput(boolean value)](#setDiscardInput-boolean-) | Indique s'il faut ignorer l'entrée utilisateur dans le navigateur client lorsque l'utilisateur clique sur ce lien hypertexte CellCommand. |
| [setImageURL(String value)](#setImageURL-java.lang.String-) | Définit l'URL de l'image pour le lien, il n'existe pas de propriété imageurl dans le lien hypertexte, donc on utilise en fait TextToDisplay pour enregistrer cette valeur. TextToDisplay sera défini sur <img src=valeur> ce qui modifiera la valeur de TextToDisplay. |
| [setScreenTip(String value)](#setScreenTip-java.lang.String-) | Renvoie ou définit le texte d'infobulle pour le lien hypertexte spécifié. |
| [setTarget(String value)](#setTarget-java.lang.String-) | Définit le type de cible du lien web, veuillez noter qu'il s'agit d'un attribut d'extension qui ne peut pas être conservé dans le fichier Excel. |
| [setTextToDisplay(String value)](#setTextToDisplay-java.lang.String-) | Représente le texte à afficher pour le lien hypertexte spécifié. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getAddress() {#getAddress--}
```
public String getAddress()
```


Représente l'adresse d'un lien hypertexte.

**Returns:**
java.lang.String
### getAltText() {#getAltText--}
```
public String getAltText()
```


Obtient le texte alternatif pour le lien image, veuillez noter qu'il s'agit d'un attribut d'extension qui ne peut pas être conservé dans le fichier Excel.

**Returns:**
java.lang.String
### getArea() {#getArea--}
```
public GridCellArea getArea()
```


Obtient la plage du lien hypertexte.

**Returns:**
[GridCellArea](../../com.aspose.gridweb/gridcellarea)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCommand() {#getCommand--}
```
public String getCommand()
```


Renvoie ou définit le texte de valeur de commande défini par l'utilisateur pour le lien hypertexte spécifié.

**Returns:**
java.lang.String
### getDiscardInput() {#getDiscardInput--}
```
public boolean getDiscardInput()
```


Indique s'il faut ignorer l'entrée utilisateur dans le navigateur client lorsque l'utilisateur clique sur ce lien hypertexte CellCommand. Peut être utilisé comme une action "undo".

**Returns:**
boolean
### getImageURL() {#getImageURL--}
```
public String getImageURL()
```


Obtient l'URL de l'image pour le lien, il n'existe pas de propriété imageurl dans le lien hypertexte, donc on utilise en fait TextToDisplay pour enregistrer cette valeur. TextToDisplay sera défini sur <img src=valeur> ce qui modifiera la valeur de TextToDisplay.

**Returns:**
java.lang.String
### getScreenTip() {#getScreenTip--}
```
public String getScreenTip()
```


Renvoie ou définit le texte d'infobulle pour le lien hypertexte spécifié.

**Returns:**
java.lang.String
### getTarget() {#getTarget--}
```
public String getTarget()
```


Obtient le type de cible du lien web, veuillez noter qu'il s'agit d'un attribut d'extension qui ne peut pas être conservé dans le fichier Excel.

**Returns:**
java.lang.String
### getTextToDisplay() {#getTextToDisplay--}
```
public String getTextToDisplay()
```


Représente le texte à afficher pour le lien hypertexte spécifié. La valeur par défaut est l'adresse du lien hypertexte.

**Returns:**
java.lang.String
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




### setAddress(String value) {#setAddress-java.lang.String-}
```
public void setAddress(String value)
```


Représente l'adresse d'un lien hypertexte.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setAltText(String value) {#setAltText-java.lang.String-}
```
public void setAltText(String value)
```


Définit le texte alternatif pour le lien image, veuillez noter qu'il s'agit d'un attribut d'extension qui ne peut pas être conservé dans le fichier Excel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setCommand(String value) {#setCommand-java.lang.String-}
```
public void setCommand(String value)
```


Renvoie ou définit le texte de valeur de commande défini par l'utilisateur pour le lien hypertexte spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setDiscardInput(boolean value) {#setDiscardInput-boolean-}
```
public void setDiscardInput(boolean value)
```


Indique s'il faut ignorer l'entrée utilisateur dans le navigateur client lorsque l'utilisateur clique sur ce lien hypertexte CellCommand. Peut être utilisé comme une action "undo".

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setImageURL(String value) {#setImageURL-java.lang.String-}
```
public void setImageURL(String value)
```


Définit l'URL de l'image pour le lien, il n'existe pas de propriété imageurl dans le lien hypertexte, donc on utilise en fait TextToDisplay pour enregistrer cette valeur. TextToDisplay sera défini sur <img src=valeur> ce qui modifiera la valeur de TextToDisplay.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setScreenTip(String value) {#setScreenTip-java.lang.String-}
```
public void setScreenTip(String value)
```


Renvoie ou définit le texte d'infobulle pour le lien hypertexte spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setTarget(String value) {#setTarget-java.lang.String-}
```
public void setTarget(String value)
```


Définit le type de cible du lien web, veuillez noter qu'il s'agit d'un attribut d'extension qui ne peut pas être conservé dans le fichier Excel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setTextToDisplay(String value) {#setTextToDisplay-java.lang.String-}
```
public void setTextToDisplay(String value)
```


Représente le texte à afficher pour le lien hypertexte spécifié. La valeur par défaut est l'adresse du lien hypertexte.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

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

