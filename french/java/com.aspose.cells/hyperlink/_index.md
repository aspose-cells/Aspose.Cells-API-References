---
title: "Lien hypertexte"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Encapsule l'objet qui représente un hyperlien."
type: docs
url: /fr/java/com.aspose.cells/hyperlink/
---

**Inheritance:**
java.lang.Object
```
public class Hyperlink
```

Encapsule l'objet qui représente un hyperlien.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Adding a new worksheet to the Workbook object
         workbook.getWorksheets().add();
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Adding a hyperlink to a URL at "A1" cell
         int index = worksheet.getHyperlinks().add("A1", 1, 1, "http://www.aspose.com");
         //Getting a Hyperlink by index.
         Hyperlink hyperlink = worksheet.getHyperlinks().get(index);
         //Setting display text of this hyperlink.
         hyperlink.setTextToDisplay("Aspose");
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [delete()](#delete--) | Supprime ce lien hypertexte |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAddress()](#getAddress--) | Représente l'adresse d'un lien hypertexte. |
| [getArea()](#getArea--) | Obtient la plage du lien hypertexte. |
| [getClass()](#getClass--) |  |
| [getLinkType()](#getLinkType--) | Obtient le type de lien. |
| [getScreenTip()](#getScreenTip--) | Renvoie ou définit le texte d'infobulle pour le lien hypertexte spécifié. |
| [getTextToDisplay()](#getTextToDisplay--) | Représente le texte à afficher pour le lien hypertexte spécifié. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAddress(String value)](#setAddress-java.lang.String-) | Représente l'adresse d'un lien hypertexte. |
| [setScreenTip(String value)](#setScreenTip-java.lang.String-) | Renvoie ou définit le texte d'infobulle pour le lien hypertexte spécifié. |
| [setTextToDisplay(String value)](#setTextToDisplay-java.lang.String-) | Représente le texte à afficher pour le lien hypertexte spécifié. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### delete() {#delete--}
```
public void delete()
```


Supprime ce lien hypertexte

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
### getArea() {#getArea--}
```
public CellArea getArea()
```


Obtient la plage du lien hypertexte.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getLinkType() {#getLinkType--}
```
public int getLinkType()
```


Obtient le type de lien.

Voir [TargetModeType](../../com.aspose.cells/targetmodetype).

**Returns:**
int
### getScreenTip() {#getScreenTip--}
```
public String getScreenTip()
```


Renvoie ou définit le texte d'infobulle pour le lien hypertexte spécifié.

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

### setScreenTip(String value) {#setScreenTip-java.lang.String-}
```
public void setScreenTip(String value)
```


Renvoie ou définit le texte d'infobulle pour le lien hypertexte spécifié.

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

