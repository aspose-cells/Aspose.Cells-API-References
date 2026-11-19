---
title: "SpinButtonActiveXControl"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente le contrôle SpinButton."
type: docs
url: /fr/java/com.aspose.cells/spinbuttonactivexcontrol/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ActiveXControlBase](../../com.aspose.cells/activexcontrolbase), [com.aspose.cells.ActiveXControl](../../com.aspose.cells/activexcontrol)
```
public class SpinButtonActiveXControl extends ActiveXControl
```

Représente le contrôle SpinButton.

**Example**

```
         //Initialize a new workbook.
         Workbook book = new Workbook();
 
         //Add a ToggleButtonActiveXControl.
         Shape shape = book.getWorksheets().get(0).getShapes().addActiveXControl(ControlType.SPIN_BUTTON, 1, 0, 1, 0, 100, 50);
         SpinButtonActiveXControl activeXControl = (SpinButtonActiveXControl)shape.getActiveXControl();
 
         //do your business
 
         //Save the excel file.
         book.save("exmaple.xlsx");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackOleColor()](#getBackOleColor--) | Obtient la couleur ole de l'arrière-plan. |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | Obtient les données binaires du contrôle. |
| [getFont()](#getFont--) | Représente la police du contrôle. |
| [getForeOleColor()](#getForeOleColor--) | Obtient la couleur OLE du premier plan. |
| [getHeight()](#getHeight--) | Obtient la hauteur du contrôle en points. |
| [getIMEMode()](#getIMEMode--) | Obtient le mode d'exécution par défaut de l'éditeur de méthode d'entrée pour le contrôle lorsqu'il reçoit le focus. |
| [getLinkedCell()](#getLinkedCell--) | Obtient la cellule liée. |
| [getListFillRange()](#getListFillRange--) | Obtient la plage de remplissage de la liste. |
| [getMax()](#getMax--) | Obtient la valeur maximale acceptable. |
| [getMin()](#getMin--) | Obtient la valeur minimale acceptable. |
| [getMouseIcon()](#getMouseIcon--) | Obtient une icône personnalisée à afficher comme pointeur de la souris pour le contrôle. |
| [getMousePointer()](#getMousePointer--) | Obtient le type d'icône affiché comme pointeur de la souris pour le contrôle. |
| [getOrientation()](#getOrientation--) | Obtient si le SpinButton ou le ScrollBar est orienté verticalement ou horizontalement. |
| [getPosition()](#getPosition--) | Obtient la valeur. |
| [getShadow()](#getShadow--) | Indique s'il faut afficher une ombre. |
| [getSmallChange()](#getSmallChange--) | Obtient la quantité par laquelle la propriété Position change |
| [getTextAlign()](#getTextAlign--) | Représente la façon d'aligner le texte utilisé par le contrôle. |
| [getType()](#getType--) | Obtient le type du contrôle ActiveX. |
| [getWidth()](#getWidth--) | Obtient la largeur du contrôle en unités de points. |
| [getWorkbook()](#getWorkbook--) | Obtient l'objet [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--). |
| [hashCode()](#hashCode--) |  |
| [isAutoSize()](#isAutoSize--) | Indique si le contrôle redimensionnera automatiquement pour afficher tout son contenu. |
| [isEnabled()](#isEnabled--) | Indique si le contrôle peut recevoir le focus et répondre aux événements générés par l'utilisateur. |
| [isLocked()](#isLocked--) | Indique si les données du contrôle sont verrouillées pour l'édition. |
| [isTransparent()](#isTransparent--) | Indique si le contrôle est transparent. |
| [isVisible()](#isVisible--) | Indique si ce contrôle est visible. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Indique si le contrôle redimensionnera automatiquement pour afficher tout son contenu. |
| [setBackOleColor(int value)](#setBackOleColor-int-) | Définit la couleur ole de l'arrière-plan. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | Indique si le contrôle peut recevoir le focus et répondre aux événements générés par l'utilisateur. |
| [setForeOleColor(int value)](#setForeOleColor-int-) | Définit la couleur ole du premier plan. |
| [setHeight(double value)](#setHeight-double-) | Définit la hauteur du contrôle en unités de points. |
| [setIMEMode(int value)](#setIMEMode-int-) | Définit le mode d'exécution par défaut de l'Input Method Editor pour le contrôle lorsqu'il reçoit le focus. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Définit la cellule liée. |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | Définit la plage de remplissage de la liste. |
| [setLocked(boolean value)](#setLocked-boolean-) | Indique si les données du contrôle sont verrouillées pour l'édition. |
| [setMax(int value)](#setMax-int-) | Définit la valeur maximale acceptable. |
| [setMin(int value)](#setMin-int-) | Définit la valeur minimale acceptable. |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | Définit une icône personnalisée à afficher comme pointeur de la souris pour le contrôle. |
| [setMousePointer(int value)](#setMousePointer-int-) | Définit le type d'icône affichée comme pointeur de la souris pour le contrôle. |
| [setOrientation(int value)](#setOrientation-int-) | Définit si le SpinButton ou le ScrollBar est orienté verticalement ou horizontalement. |
| [setPosition(int value)](#setPosition-int-) | Définit la valeur. |
| [setShadow(boolean value)](#setShadow-boolean-) | Indique s'il faut afficher une ombre. |
| [setSmallChange(int value)](#setSmallChange-int-) | Définit la quantité par laquelle la propriété Position change |
| [setTextAlign(int value)](#setTextAlign-int-) | Représente la façon d'aligner le texte utilisé par le contrôle. |
| [setTransparent(boolean value)](#setTransparent-boolean-) | Indique si le contrôle est transparent. |
| [setVisible(boolean value)](#setVisible-boolean-) | Indique si ce contrôle est visible. |
| [setWidth(double value)](#setWidth-double-) | Définit la largeur du contrôle en unité de points. |
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
### getBackOleColor() {#getBackOleColor--}
```
public int getBackOleColor()
```


Obtient la couleur ole de l'arrière-plan.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getData() {#getData--}
```
public byte[] getData()
```


Obtient les données binaires du contrôle.

**Returns:**
byte[]
### getFont() {#getFont--}
```
public Font getFont()
```


Représente la police du contrôle.

**Returns:**
[Font](../../com.aspose.cells/font)
### getForeOleColor() {#getForeOleColor--}
```
public int getForeOleColor()
```


Obtient la couleur OLE du premier plan.

**Remarks**

Ne s'applique pas au contrôle Image.

**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```


Obtient la hauteur du contrôle en points.

**Returns:**
double
### getIMEMode() {#getIMEMode--}
```
public int getIMEMode()
```


Obtient le mode d'exécution par défaut de l'éditeur de méthode d'entrée pour le contrôle lorsqu'il reçoit le focus.

Voir [InputMethodEditorMode](../../com.aspose.cells/inputmethodeditormode).

**Returns:**
int
### getLinkedCell() {#getLinkedCell--}
```
public String getLinkedCell()
```


Obtient la cellule liée.

**Returns:**
java.lang.String
### getListFillRange() {#getListFillRange--}
```
public String getListFillRange()
```


Obtient la plage de remplissage de la liste.

**Returns:**
java.lang.String
### getMax() {#getMax--}
```
public int getMax()
```


Obtient la valeur maximale acceptable.

**Example**

```
         activeXControl.setMax(100);
```

**Returns:**
int
### getMin() {#getMin--}
```
public int getMin()
```


Obtient la valeur minimale acceptable.

**Example**

```
         activeXControl.setMin(0);
```

**Returns:**
int
### getMouseIcon() {#getMouseIcon--}
```
public byte[] getMouseIcon()
```


Obtient une icône personnalisée à afficher comme pointeur de la souris pour le contrôle.

**Returns:**
byte[]
### getMousePointer() {#getMousePointer--}
```
public int getMousePointer()
```


Obtient le type d'icône affiché comme pointeur de la souris pour le contrôle.

Voir [ControlMousePointerType](../../com.aspose.cells/controlmousepointertype).

**Returns:**
int
### getOrientation() {#getOrientation--}
```
public int getOrientation()
```


Obtient si le SpinButton ou le ScrollBar est orienté verticalement ou horizontalement.

Voir [ControlScrollOrientation](../../com.aspose.cells/controlscrollorientation).

**Example**

```
         if(activeXControl.getOrientation() == com.aspose.cells.ControlScrollOrientation.AUTO)
         {
             activeXControl.setOrientation(com.aspose.cells.ControlScrollOrientation.HORIZONTAL);
         }
```

**Returns:**
int
### getPosition() {#getPosition--}
```
public int getPosition()
```


Obtient la valeur.

**Example**

```
         activeXControl.setPosition(30);
```

**Returns:**
int
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Indique s'il faut afficher une ombre.

**Returns:**
boolean
### getSmallChange() {#getSmallChange--}
```
public int getSmallChange()
```


Obtient la quantité par laquelle la propriété Position change

**Example**

```
         activeXControl.setSmallChange(5);
```

**Returns:**
int
### getTextAlign() {#getTextAlign--}
```
public int getTextAlign()
```


Représente la façon d'aligner le texte utilisé par le contrôle.

Voir [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Obtient le type du contrôle ActiveX.

Voir [ControlType](../../com.aspose.cells/controltype).

**Example**

```
         if(activeXControl.getType() == com.aspose.cells.ControlType.SPIN_BUTTON)
         {
             //do something
         }
```

**Returns:**
int
### getWidth() {#getWidth--}
```
public double getWidth()
```


Obtient la largeur du contrôle en unités de points.

**Returns:**
double
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


Obtient l'objet [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--).

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoSize() {#isAutoSize--}
```
public boolean isAutoSize()
```


Indique si le contrôle redimensionnera automatiquement pour afficher tout son contenu.

**Returns:**
boolean
### isEnabled() {#isEnabled--}
```
public boolean isEnabled()
```


Indique si le contrôle peut recevoir le focus et répondre aux événements générés par l'utilisateur.

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


Indique si les données du contrôle sont verrouillées pour l'édition.

**Returns:**
boolean
### isTransparent() {#isTransparent--}
```
public boolean isTransparent()
```


Indique si le contrôle est transparent.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Indique si ce contrôle est visible.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAutoSize(boolean value) {#setAutoSize-boolean-}
```
public void setAutoSize(boolean value)
```


Indique si le contrôle redimensionnera automatiquement pour afficher tout son contenu.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setBackOleColor(int value) {#setBackOleColor-int-}
```
public void setBackOleColor(int value)
```


Définit la couleur ole de l'arrière-plan.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public void setEnabled(boolean value)
```


Indique si le contrôle peut recevoir le focus et répondre aux événements générés par l'utilisateur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setForeOleColor(int value) {#setForeOleColor-int-}
```
public void setForeOleColor(int value)
```


Définit la couleur ole du premier plan.

**Remarks**

Ne s'applique pas au contrôle Image.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


Définit la hauteur du contrôle en unités de points.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setIMEMode(int value) {#setIMEMode-int-}
```
public void setIMEMode(int value)
```


Définit le mode d'exécution par défaut de l'Input Method Editor pour le contrôle lorsqu'il reçoit le focus.

Voir [InputMethodEditorMode](../../com.aspose.cells/inputmethodeditormode).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setLinkedCell(String value) {#setLinkedCell-java.lang.String-}
```
public void setLinkedCell(String value)
```


Définit la cellule liée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setListFillRange(String value) {#setListFillRange-java.lang.String-}
```
public void setListFillRange(String value)
```


Définit la plage de remplissage de la liste.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Indique si les données du contrôle sont verrouillées pour l'édition.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setMax(int value) {#setMax-int-}
```
public void setMax(int value)
```


Définit la valeur maximale acceptable.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setMin(int value) {#setMin-int-}
```
public void setMin(int value)
```


Définit la valeur minimale acceptable.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setMouseIcon(byte[] value) {#setMouseIcon-byte---}
```
public void setMouseIcon(byte[] value)
```


Définit une icône personnalisée à afficher comme pointeur de la souris pour le contrôle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | byte[] |  |

### setMousePointer(int value) {#setMousePointer-int-}
```
public void setMousePointer(int value)
```


Définit le type d'icône affichée comme pointeur de la souris pour le contrôle.

Voir [ControlMousePointerType](../../com.aspose.cells/controlmousepointertype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setOrientation(int value) {#setOrientation-int-}
```
public void setOrientation(int value)
```


Définit si le SpinButton ou le ScrollBar est orienté verticalement ou horizontalement.

Voir [ControlScrollOrientation](../../com.aspose.cells/controlscrollorientation).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setPosition(int value) {#setPosition-int-}
```
public void setPosition(int value)
```


Définit la valeur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


Indique s'il faut afficher une ombre.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSmallChange(int value) {#setSmallChange-int-}
```
public void setSmallChange(int value)
```


Définit la quantité par laquelle la propriété Position change

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setTextAlign(int value) {#setTextAlign-int-}
```
public void setTextAlign(int value)
```


Représente la façon d'aligner le texte utilisé par le contrôle.

Voir [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setTransparent(boolean value) {#setTransparent-boolean-}
```
public void setTransparent(boolean value)
```


Indique si le contrôle est transparent.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Indique si ce contrôle est visible.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```


Définit la largeur du contrôle en unité de points.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

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

