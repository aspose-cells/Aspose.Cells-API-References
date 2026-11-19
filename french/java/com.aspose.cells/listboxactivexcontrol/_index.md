---
title: "ListBoxActiveXControl"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente un contrôle ActiveX ListBox."
type: docs
url: /fr/java/com.aspose.cells/listboxactivexcontrol/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ActiveXControlBase](../../com.aspose.cells/activexcontrolbase), [com.aspose.cells.ActiveXControl](../../com.aspose.cells/activexcontrol)
```
public class ListBoxActiveXControl extends ActiveXControl
```

Représente un contrôle ActiveX ListBox.
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackOleColor()](#getBackOleColor--) | Obtient la couleur ole de l'arrière-plan. |
| [getBorderOleColor()](#getBorderOleColor--) | Obtient la couleur ole de l'arrière-plan. |
| [getBorderStyle()](#getBorderStyle--) | Obtient le type de bordure utilisé par le contrôle. |
| [getBoundColumn()](#getBoundColumn--) | Représente la façon dont la propriété Value est déterminée pour une ComboBox ou ListBox lorsque la valeur de la propriété MultiSelect est (fmMultiSelectSingle). |
| [getClass()](#getClass--) |  |
| [getColumnCount()](#getColumnCount--) | Représente le nombre de colonnes à afficher dans une ComboBox ou ListBox. |
| [getColumnWidths()](#getColumnWidths--) | Obtient la largeur de la colonne. |
| [getData()](#getData--) | Obtient les données binaires du contrôle. |
| [getFont()](#getFont--) | Représente la police du contrôle. |
| [getForeOleColor()](#getForeOleColor--) | Obtient la couleur OLE du premier plan. |
| [getHeight()](#getHeight--) | Obtient la hauteur du contrôle en points. |
| [getIMEMode()](#getIMEMode--) | Obtient le mode d'exécution par défaut de l'éditeur de méthode d'entrée pour le contrôle lorsqu'il reçoit le focus. |
| [getIntegralHeight()](#getIntegralHeight--) | Indique si le contrôle n'affichera que des lignes complètes de texte sans afficher de lignes partielles. |
| [getLinkedCell()](#getLinkedCell--) | Obtient la cellule liée. |
| [getListFillRange()](#getListFillRange--) | Obtient la plage de remplissage de la liste. |
| [getListStyle()](#getListStyle--) | Obtient l'apparence visuelle. |
| [getListWidth()](#getListWidth--) | Obtient la largeur en points. |
| [getMatchEntry()](#getMatchEntry--) | Indique comment une ListBox ou une ComboBox recherche dans sa liste pendant que l'utilisateur tape. |
| [getMouseIcon()](#getMouseIcon--) | Obtient une icône personnalisée à afficher comme pointeur de la souris pour le contrôle. |
| [getMousePointer()](#getMousePointer--) | Obtient le type d'icône affiché comme pointeur de la souris pour le contrôle. |
| [getScrollBars()](#getScrollBars--) | Indique si le contrôle possède des barres de défilement verticales, des barres de défilement horizontales, les deux ou aucune. |
| [getSelectionType()](#getSelectionType--) | Indique si le contrôle autorise plusieurs sélections. |
| [getShadow()](#getShadow--) | Indique s'il faut afficher une ombre. |
| [getShowColumnHeads()](#getShowColumnHeads--) | Indique si les en-têtes de colonne sont affichés. |
| [getSpecialEffect()](#getSpecialEffect--) | Obtient l'effet spécial du contrôle. |
| [getTextAlign()](#getTextAlign--) | Représente la façon d'aligner le texte utilisé par le contrôle. |
| [getTextColumn()](#getTextColumn--) | Représente la colonne d'une ComboBox ou d'une ListBox à afficher à l'utilisateur. |
| [getType()](#getType--) | Obtient le type du contrôle ActiveX. |
| [getValue()](#getValue--) | Obtient la valeur du contrôle. |
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
| [setBorderOleColor(int value)](#setBorderOleColor-int-) | Définit la couleur ole de l'arrière-plan. |
| [setBorderStyle(int value)](#setBorderStyle-int-) | Définit le type de bordure utilisé par le contrôle. |
| [setBoundColumn(int value)](#setBoundColumn-int-) | Représente la façon dont la propriété Value est déterminée pour une ComboBox ou ListBox lorsque la valeur de la propriété MultiSelect est (fmMultiSelectSingle). |
| [setColumnCount(int value)](#setColumnCount-int-) | Représente le nombre de colonnes à afficher dans une ComboBox ou ListBox. |
| [setColumnWidths(double value)](#setColumnWidths-double-) | Définit la largeur de la colonne. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | Indique si le contrôle peut recevoir le focus et répondre aux événements générés par l'utilisateur. |
| [setForeOleColor(int value)](#setForeOleColor-int-) | Définit la couleur ole du premier plan. |
| [setHeight(double value)](#setHeight-double-) | Définit la hauteur du contrôle en unités de points. |
| [setIMEMode(int value)](#setIMEMode-int-) | Définit le mode d'exécution par défaut de l'Input Method Editor pour le contrôle lorsqu'il reçoit le focus. |
| [setIntegralHeight(boolean value)](#setIntegralHeight-boolean-) | Indique si le contrôle n'affichera que des lignes complètes de texte sans afficher de lignes partielles. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Définit la cellule liée. |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | Définit la plage de remplissage de la liste. |
| [setListStyle(int value)](#setListStyle-int-) | Définit l'apparence visuelle. |
| [setListWidth(double value)](#setListWidth-double-) | Définit la largeur en unités de points. |
| [setLocked(boolean value)](#setLocked-boolean-) | Indique si les données du contrôle sont verrouillées pour l'édition. |
| [setMatchEntry(int value)](#setMatchEntry-int-) | Indique comment une ListBox ou une ComboBox recherche dans sa liste pendant que l'utilisateur tape. |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | Définit une icône personnalisée à afficher comme pointeur de la souris pour le contrôle. |
| [setMousePointer(int value)](#setMousePointer-int-) | Définit le type d'icône affichée comme pointeur de la souris pour le contrôle. |
| [setScrollBars(int value)](#setScrollBars-int-) | Indique si le contrôle possède des barres de défilement verticales, des barres de défilement horizontales, les deux ou aucune. |
| [setSelectionType(int value)](#setSelectionType-int-) | Indique si le contrôle autorise plusieurs sélections. |
| [setShadow(boolean value)](#setShadow-boolean-) | Indique s'il faut afficher une ombre. |
| [setShowColumnHeads(boolean value)](#setShowColumnHeads-boolean-) | Indique si les en-têtes de colonne sont affichés. |
| [setSpecialEffect(int value)](#setSpecialEffect-int-) | Définit l'effet spécial du contrôle. |
| [setTextAlign(int value)](#setTextAlign-int-) | Représente la façon d'aligner le texte utilisé par le contrôle. |
| [setTextColumn(int value)](#setTextColumn-int-) | Représente la colonne d'une ComboBox ou d'une ListBox à afficher à l'utilisateur. |
| [setTransparent(boolean value)](#setTransparent-boolean-) | Indique si le contrôle est transparent. |
| [setValue(String value)](#setValue-java.lang.String-) | Définit la valeur du contrôle. |
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
### getBoundColumn() {#getBoundColumn--}
```
public int getBoundColumn()
```


Représente la façon dont la propriété Value est déterminée pour une ComboBox ou ListBox lorsque la valeur de la propriété MultiSelect est (fmMultiSelectSingle).

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


Représente le nombre de colonnes à afficher dans une ComboBox ou ListBox.

**Returns:**
int
### getColumnWidths() {#getColumnWidths--}
```
public double getColumnWidths()
```


Obtient la largeur de la colonne.

**Returns:**
double
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
### getIntegralHeight() {#getIntegralHeight--}
```
public boolean getIntegralHeight()
```


Indique si le contrôle n'affichera que des lignes complètes de texte sans afficher de lignes partielles.

**Returns:**
boolean
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
### getListStyle() {#getListStyle--}
```
public int getListStyle()
```


Obtient l'apparence visuelle.

Voir [ControlListStyle](../../com.aspose.cells/controlliststyle).

**Returns:**
int
### getListWidth() {#getListWidth--}
```
public double getListWidth()
```


Obtient la largeur en points.

**Returns:**
double
### getMatchEntry() {#getMatchEntry--}
```
public int getMatchEntry()
```


Indique comment une ListBox ou une ComboBox recherche dans sa liste pendant que l'utilisateur tape.

Voir [ControlMatchEntryType](../../com.aspose.cells/controlmatchentrytype).

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
### getScrollBars() {#getScrollBars--}
```
public int getScrollBars()
```


Indique si le contrôle possède des barres de défilement verticales, des barres de défilement horizontales, les deux ou aucune.

Voir [ControlScrollBarType](../../com.aspose.cells/controlscrollbartype).

**Returns:**
int
### getSelectionType() {#getSelectionType--}
```
public int getSelectionType()
```


Indique si le contrôle autorise plusieurs sélections.

Voir [SelectionType](../../com.aspose.cells/selectiontype).

**Returns:**
int
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Indique s'il faut afficher une ombre.

**Returns:**
boolean
### getShowColumnHeads() {#getShowColumnHeads--}
```
public boolean getShowColumnHeads()
```


Indique si les en-têtes de colonne sont affichés.

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
### getTextColumn() {#getTextColumn--}
```
public int getTextColumn()
```


Représente la colonne d'une ComboBox ou d'une ListBox à afficher à l'utilisateur.

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
### getValue() {#getValue--}
```
public String getValue()
```


Obtient la valeur du contrôle.

**Remarks**

N'affecte que lorsque [getSelectionType()](../../com.aspose.cells/listboxactivexcontrol\#getSelectionType--) est SelectionType.Single;

**Returns:**
java.lang.String
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

### setBoundColumn(int value) {#setBoundColumn-int-}
```
public void setBoundColumn(int value)
```


Représente la façon dont la propriété Value est déterminée pour une ComboBox ou ListBox lorsque la valeur de la propriété MultiSelect est (fmMultiSelectSingle).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setColumnCount(int value) {#setColumnCount-int-}
```
public void setColumnCount(int value)
```


Représente le nombre de colonnes à afficher dans une ComboBox ou ListBox.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setColumnWidths(double value) {#setColumnWidths-double-}
```
public void setColumnWidths(double value)
```


Définit la largeur de la colonne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

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

### setIntegralHeight(boolean value) {#setIntegralHeight-boolean-}
```
public void setIntegralHeight(boolean value)
```


Indique si le contrôle n'affichera que des lignes complètes de texte sans afficher de lignes partielles.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

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

### setListStyle(int value) {#setListStyle-int-}
```
public void setListStyle(int value)
```


Définit l'apparence visuelle.

Voir [ControlListStyle](../../com.aspose.cells/controlliststyle).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setListWidth(double value) {#setListWidth-double-}
```
public void setListWidth(double value)
```


Définit la largeur en unités de points.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Indique si les données du contrôle sont verrouillées pour l'édition.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setMatchEntry(int value) {#setMatchEntry-int-}
```
public void setMatchEntry(int value)
```


Indique comment une ListBox ou une ComboBox recherche dans sa liste pendant que l'utilisateur tape.

Voir [ControlMatchEntryType](../../com.aspose.cells/controlmatchentrytype).

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

### setScrollBars(int value) {#setScrollBars-int-}
```
public void setScrollBars(int value)
```


Indique si le contrôle possède des barres de défilement verticales, des barres de défilement horizontales, les deux ou aucune.

Voir [ControlScrollBarType](../../com.aspose.cells/controlscrollbartype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setSelectionType(int value) {#setSelectionType-int-}
```
public void setSelectionType(int value)
```


Indique si le contrôle autorise plusieurs sélections.

Voir [SelectionType](../../com.aspose.cells/selectiontype).

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

### setShowColumnHeads(boolean value) {#setShowColumnHeads-boolean-}
```
public void setShowColumnHeads(boolean value)
```


Indique si les en-têtes de colonne sont affichés.

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

### setTextColumn(int value) {#setTextColumn-int-}
```
public void setTextColumn(int value)
```


Représente la colonne d'une ComboBox ou d'une ListBox à afficher à l'utilisateur.

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

### setValue(String value) {#setValue-java.lang.String-}
```
public void setValue(String value)
```


Définit la valeur du contrôle.

**Remarks**

N'affecte que lorsque [getSelectionType()](../../com.aspose.cells/listboxactivexcontrol\#getSelectionType--) est SelectionType.Single;

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

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

