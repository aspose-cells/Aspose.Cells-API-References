---
title: "LabelActiveXControl"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente le contrôle ActiveX d'étiquette."
type: docs
url: /fr/java/com.aspose.cells/labelactivexcontrol/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ActiveXControlBase](../../com.aspose.cells/activexcontrolbase), [com.aspose.cells.ActiveXControl](../../com.aspose.cells/activexcontrol)
```
public class LabelActiveXControl extends ActiveXControl
```

Représente le contrôle ActiveX d'étiquette.
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAccelerator()](#getAccelerator--) | Obtient la touche d'accélérateur pour le contrôle. |
| [getBackOleColor()](#getBackOleColor--) | Obtient la couleur ole de l'arrière-plan. |
| [getBorderOleColor()](#getBorderOleColor--) | Obtient la couleur ole de l'arrière-plan. |
| [getBorderStyle()](#getBorderStyle--) | Obtient le type de bordure utilisé par le contrôle. |
| [getCaption()](#getCaption--) | Obtient le texte descriptif qui apparaît sur un contrôle. |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | Obtient les données binaires du contrôle. |
| [getFont()](#getFont--) | Représente la police du contrôle. |
| [getForeOleColor()](#getForeOleColor--) | Obtient la couleur OLE du premier plan. |
| [getHeight()](#getHeight--) | Obtient la hauteur du contrôle en points. |
| [getIMEMode()](#getIMEMode--) | Obtient le mode d'exécution par défaut de l'éditeur de méthode d'entrée pour le contrôle lorsqu'il reçoit le focus. |
| [getLinkedCell()](#getLinkedCell--) | Obtient la cellule liée. |
| [getListFillRange()](#getListFillRange--) | Obtient la plage de remplissage de la liste. |
| [getMouseIcon()](#getMouseIcon--) | Obtient une icône personnalisée à afficher comme pointeur de la souris pour le contrôle. |
| [getMousePointer()](#getMousePointer--) | Obtient le type d'icône affiché comme pointeur de la souris pour le contrôle. |
| [getPicture()](#getPicture--) | Obtient les données de l'image. |
| [getPicturePosition()](#getPicturePosition--) | Obtient l'emplacement de l'image du contrôle par rapport à sa légende. |
| [getShadow()](#getShadow--) | Indique s'il faut afficher une ombre. |
| [getSpecialEffect()](#getSpecialEffect--) | Obtient l'effet spécial du contrôle. |
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
| [isWordWrapped()](#isWordWrapped--) | Indique si le contenu du contrôle passe automatiquement à la ligne à la fin d'une ligne. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAccelerator(char value)](#setAccelerator-char-) | Définit la touche d'accélérateur pour le contrôle. |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Indique si le contrôle redimensionnera automatiquement pour afficher tout son contenu. |
| [setBackOleColor(int value)](#setBackOleColor-int-) | Définit la couleur ole de l'arrière-plan. |
| [setBorderOleColor(int value)](#setBorderOleColor-int-) | Définit la couleur ole de l'arrière-plan. |
| [setBorderStyle(int value)](#setBorderStyle-int-) | Définit le type de bordure utilisé par le contrôle. |
| [setCaption(String value)](#setCaption-java.lang.String-) | Définit le texte descriptif qui apparaît sur un contrôle. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | Indique si le contrôle peut recevoir le focus et répondre aux événements générés par l'utilisateur. |
| [setForeOleColor(int value)](#setForeOleColor-int-) | Définit la couleur ole du premier plan. |
| [setHeight(double value)](#setHeight-double-) | Définit la hauteur du contrôle en unités de points. |
| [setIMEMode(int value)](#setIMEMode-int-) | Définit le mode d'exécution par défaut de l'Input Method Editor pour le contrôle lorsqu'il reçoit le focus. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Définit la cellule liée. |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | Définit la plage de remplissage de la liste. |
| [setLocked(boolean value)](#setLocked-boolean-) | Indique si les données du contrôle sont verrouillées pour l'édition. |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | Définit une icône personnalisée à afficher comme pointeur de la souris pour le contrôle. |
| [setMousePointer(int value)](#setMousePointer-int-) | Définit le type d'icône affichée comme pointeur de la souris pour le contrôle. |
| [setPicture(byte[] value)](#setPicture-byte---) | Définit les données de l'image. |
| [setPicturePosition(int value)](#setPicturePosition-int-) | Définit l'emplacement de l'image du contrôle par rapport à sa légende. |
| [setShadow(boolean value)](#setShadow-boolean-) | Indique s'il faut afficher une ombre. |
| [setSpecialEffect(int value)](#setSpecialEffect-int-) | Définit l'effet spécial du contrôle. |
| [setTextAlign(int value)](#setTextAlign-int-) | Représente la façon d'aligner le texte utilisé par le contrôle. |
| [setTransparent(boolean value)](#setTransparent-boolean-) | Indique si le contrôle est transparent. |
| [setVisible(boolean value)](#setVisible-boolean-) | Indique si ce contrôle est visible. |
| [setWidth(double value)](#setWidth-double-) | Définit la largeur du contrôle en unité de points. |
| [setWordWrapped(boolean value)](#setWordWrapped-boolean-) | Indique si le contenu du contrôle passe automatiquement à la ligne à la fin d'une ligne. |
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
### getAccelerator() {#getAccelerator--}
```
public char getAccelerator()
```


Obtient la touche d'accélérateur pour le contrôle.

**Returns:**
char
### getBackOleColor() {#getBackOleColor--}
```
public int getBackOleColor()
```


Obtient la couleur ole de l'arrière-plan.

**Returns:**
int
### getBorderOleColor() {#getBorderOleColor--}
```
public int getBorderOleColor()
```


Obtient la couleur ole de l'arrière-plan.

**Returns:**
int
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```


Obtient le type de bordure utilisé par le contrôle.

Voir [ControlBorderType](../../com.aspose.cells/controlbordertype).

**Returns:**
int
### getCaption() {#getCaption--}
```
public String getCaption()
```


Obtient le texte descriptif qui apparaît sur un contrôle.

**Returns:**
java.lang.String
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
### getPicture() {#getPicture--}
```
public byte[] getPicture()
```


Obtient les données de l'image.

**Returns:**
byte[]
### getPicturePosition() {#getPicturePosition--}
```
public int getPicturePosition()
```


Obtient l'emplacement de l'image du contrôle par rapport à sa légende.

Voir [ControlPicturePositionType](../../com.aspose.cells/controlpicturepositiontype).

**Returns:**
int
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Indique s'il faut afficher une ombre.

**Returns:**
boolean
### getSpecialEffect() {#getSpecialEffect--}
```
public int getSpecialEffect()
```


Obtient l'effet spécial du contrôle.

Voir [ControlSpecialEffectType](../../com.aspose.cells/controlspecialeffecttype).

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
### isWordWrapped() {#isWordWrapped--}
```
public boolean isWordWrapped()
```


Indique si le contenu du contrôle passe automatiquement à la ligne à la fin d'une ligne.

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




### setAccelerator(char value) {#setAccelerator-char-}
```
public void setAccelerator(char value)
```


Définit la touche d'accélérateur pour le contrôle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | char |  |

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

### setBorderOleColor(int value) {#setBorderOleColor-int-}
```
public void setBorderOleColor(int value)
```


Définit la couleur ole de l'arrière-plan.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setBorderStyle(int value) {#setBorderStyle-int-}
```
public void setBorderStyle(int value)
```


Définit le type de bordure utilisé par le contrôle.

Voir [ControlBorderType](../../com.aspose.cells/controlbordertype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setCaption(String value) {#setCaption-java.lang.String-}
```
public void setCaption(String value)
```


Définit le texte descriptif qui apparaît sur un contrôle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

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

### setPicture(byte[] value) {#setPicture-byte---}
```
public void setPicture(byte[] value)
```


Définit les données de l'image.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | byte[] |  |

### setPicturePosition(int value) {#setPicturePosition-int-}
```
public void setPicturePosition(int value)
```


Définit l'emplacement de l'image du contrôle par rapport à sa légende.

Voir [ControlPicturePositionType](../../com.aspose.cells/controlpicturepositiontype).

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

### setSpecialEffect(int value) {#setSpecialEffect-int-}
```
public void setSpecialEffect(int value)
```


Définit l'effet spécial du contrôle.

Voir [ControlSpecialEffectType](../../com.aspose.cells/controlspecialeffecttype).

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

### setWordWrapped(boolean value) {#setWordWrapped-boolean-}
```
public void setWordWrapped(boolean value)
```


Indique si le contenu du contrôle passe automatiquement à la ligne à la fin d'une ligne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

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

