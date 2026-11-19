---
title: "TextBoxActiveXControl"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente un contrôle ActiveX de zone de texte."
type: docs
url: /fr/java/com.aspose.cells/textboxactivexcontrol/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ActiveXControlBase](../../com.aspose.cells/activexcontrolbase), [com.aspose.cells.ActiveXControl](../../com.aspose.cells/activexcontrol)
```
public class TextBoxActiveXControl extends ActiveXControl
```

Représente un contrôle ActiveX de zone de texte.

**Example**

```
         //Initialize a new workbook.
         Workbook book = new Workbook();
 
         //Add a TextBoxActiveXControl.
         Shape shape = book.getWorksheets().get(0).getShapes().addActiveXControl(ControlType.TEXT_BOX, 1, 0, 1, 0, 100, 50);
         TextBoxActiveXControl activeXControl = (TextBoxActiveXControl)shape.getActiveXControl();
 
         //do your business
 
         //Save the excel file.
         book.save("exmaple.xlsx");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackOleColor()](#getBackOleColor--) | Obtient la couleur ole de l'arrière-plan. |
| [getBorderOleColor()](#getBorderOleColor--) | Obtient la couleur ole de l'arrière-plan. |
| [getBorderStyle()](#getBorderStyle--) | Obtient le type de bordure utilisé par le contrôle. |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | Obtient les données binaires du contrôle. |
| [getDropButtonStyle()](#getDropButtonStyle--) | Spécifie le symbole affiché sur le bouton déroulant |
| [getEnterFieldBehavior()](#getEnterFieldBehavior--) | Spécifie le comportement de sélection lors de l'entrée dans le contrôle. |
| [getEnterKeyBehavior()](#getEnterKeyBehavior--) | Spécifie le comportement de la touche ENTER. |
| [getFont()](#getFont--) | Représente la police du contrôle. |
| [getForeOleColor()](#getForeOleColor--) | Obtient la couleur OLE du premier plan. |
| [getHeight()](#getHeight--) | Obtient la hauteur du contrôle en points. |
| [getHideSelection()](#getHideSelection--) | Indique si le texte sélectionné dans le contrôle apparaît en surbrillance lorsque le contrôle n'a pas le focus. |
| [getIMEMode()](#getIMEMode--) | Obtient le mode d'exécution par défaut de l'éditeur de méthode d'entrée pour le contrôle lorsqu'il reçoit le focus. |
| [getIntegralHeight()](#getIntegralHeight--) | Indique si le contrôle n'affichera que des lignes complètes de texte sans afficher de lignes partielles. |
| [getLinkedCell()](#getLinkedCell--) | Obtient la cellule liée. |
| [getListFillRange()](#getListFillRange--) | Obtient la plage de remplissage de la liste. |
| [getMaxLength()](#getMaxLength--) | Obtient le nombre maximal de caractères |
| [getMouseIcon()](#getMouseIcon--) | Obtient une icône personnalisée à afficher comme pointeur de la souris pour le contrôle. |
| [getMousePointer()](#getMousePointer--) | Obtient le type d'icône affiché comme pointeur de la souris pour le contrôle. |
| [getPasswordChar()](#getPasswordChar--) | Obtient un caractère à afficher à la place des caractères saisis. |
| [getScrollBars()](#getScrollBars--) | Indique si le contrôle possède des barres de défilement verticales, des barres de défilement horizontales, les deux ou aucune. |
| [getShadow()](#getShadow--) | Indique s'il faut afficher une ombre. |
| [getShowDropButtonTypeWhen()](#getShowDropButtonTypeWhen--) | Spécifie le symbole affiché sur le bouton déroulant |
| [getSpecialEffect()](#getSpecialEffect--) | Obtient l'effet spécial du contrôle. |
| [getTabKeyBehavior()](#getTabKeyBehavior--) | Indique si les caractères de tabulation sont autorisés dans le texte du contrôle. |
| [getText()](#getText--) | Obtient le texte du contrôle. |
| [getTextAlign()](#getTextAlign--) | Représente la façon d'aligner le texte utilisé par le contrôle. |
| [getType()](#getType--) | Obtient le type du contrôle ActiveX. |
| [getWidth()](#getWidth--) | Obtient la largeur du contrôle en unités de points. |
| [getWorkbook()](#getWorkbook--) | Obtient l'objet [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--). |
| [hashCode()](#hashCode--) |  |
| [isAutoSize()](#isAutoSize--) | Indique si le contrôle redimensionnera automatiquement pour afficher tout son contenu. |
| [isAutoTab()](#isAutoTab--) | Indique si le focus se déplacera automatiquement vers le contrôle suivant lorsque l'utilisateur saisit le nombre maximal de caractères. |
| [isAutoWordSelected()](#isAutoWordSelected--) | Spécifie l'unité de base utilisée pour étendre une sélection. |
| [isDragBehaviorEnabled()](#isDragBehaviorEnabled--) | Indique si le glisser-déposer est activé pour le contrôle. |
| [isEditable()](#isEditable--) | Indique si l'utilisateur peut saisir du texte dans le contrôle. |
| [isEnabled()](#isEnabled--) | Indique si le contrôle peut recevoir le focus et répondre aux événements générés par l'utilisateur. |
| [isLocked()](#isLocked--) | Indique si les données du contrôle sont verrouillées pour l'édition. |
| [isMultiLine()](#isMultiLine--) | Indique si le contrôle peut afficher plus d'une ligne de texte. |
| [isTransparent()](#isTransparent--) | Indique si le contrôle est transparent. |
| [isVisible()](#isVisible--) | Indique si ce contrôle est visible. |
| [isWordWrapped()](#isWordWrapped--) | Indique si le contenu du contrôle passe automatiquement à la ligne à la fin d'une ligne. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Indique si le contrôle redimensionnera automatiquement pour afficher tout son contenu. |
| [setAutoTab(boolean value)](#setAutoTab-boolean-) | Indique si le focus se déplacera automatiquement vers le contrôle suivant lorsque l'utilisateur saisit le nombre maximal de caractères. |
| [setAutoWordSelected(boolean value)](#setAutoWordSelected-boolean-) | Spécifie l'unité de base utilisée pour étendre une sélection. |
| [setBackOleColor(int value)](#setBackOleColor-int-) | Définit la couleur ole de l'arrière-plan. |
| [setBorderOleColor(int value)](#setBorderOleColor-int-) | Définit la couleur ole de l'arrière-plan. |
| [setBorderStyle(int value)](#setBorderStyle-int-) | Définit le type de bordure utilisé par le contrôle. |
| [setDragBehaviorEnabled(boolean value)](#setDragBehaviorEnabled-boolean-) | Indique si le glisser-déposer est activé pour le contrôle. |
| [setDropButtonStyle(int value)](#setDropButtonStyle-int-) | Spécifie le symbole affiché sur le bouton déroulant |
| [setEditable(boolean value)](#setEditable-boolean-) | Indique si l'utilisateur peut saisir du texte dans le contrôle. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | Indique si le contrôle peut recevoir le focus et répondre aux événements générés par l'utilisateur. |
| [setEnterFieldBehavior(boolean value)](#setEnterFieldBehavior-boolean-) | Spécifie le comportement de sélection lors de l'entrée dans le contrôle. |
| [setEnterKeyBehavior(boolean value)](#setEnterKeyBehavior-boolean-) | Spécifie le comportement de la touche ENTER. |
| [setForeOleColor(int value)](#setForeOleColor-int-) | Définit la couleur ole du premier plan. |
| [setHeight(double value)](#setHeight-double-) | Définit la hauteur du contrôle en unités de points. |
| [setHideSelection(boolean value)](#setHideSelection-boolean-) | Indique si le texte sélectionné dans le contrôle apparaît en surbrillance lorsque le contrôle n'a pas le focus. |
| [setIMEMode(int value)](#setIMEMode-int-) | Définit le mode d'exécution par défaut de l'Input Method Editor pour le contrôle lorsqu'il reçoit le focus. |
| [setIntegralHeight(boolean value)](#setIntegralHeight-boolean-) | Indique si le contrôle n'affichera que des lignes complètes de texte sans afficher de lignes partielles. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Définit la cellule liée. |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | Définit la plage de remplissage de la liste. |
| [setLocked(boolean value)](#setLocked-boolean-) | Indique si les données du contrôle sont verrouillées pour l'édition. |
| [setMaxLength(int value)](#setMaxLength-int-) | Définit le nombre maximal de caractères |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | Définit une icône personnalisée à afficher comme pointeur de la souris pour le contrôle. |
| [setMousePointer(int value)](#setMousePointer-int-) | Définit le type d'icône affichée comme pointeur de la souris pour le contrôle. |
| [setMultiLine(boolean value)](#setMultiLine-boolean-) | Indique si le contrôle peut afficher plus d'une ligne de texte. |
| [setPasswordChar(char value)](#setPasswordChar-char-) | Définit un caractère à afficher à la place des caractères saisis. |
| [setScrollBars(int value)](#setScrollBars-int-) | Indique si le contrôle possède des barres de défilement verticales, des barres de défilement horizontales, les deux ou aucune. |
| [setShadow(boolean value)](#setShadow-boolean-) | Indique s'il faut afficher une ombre. |
| [setShowDropButtonTypeWhen(int value)](#setShowDropButtonTypeWhen-int-) | Spécifie le symbole affiché sur le bouton déroulant |
| [setSpecialEffect(int value)](#setSpecialEffect-int-) | Définit l'effet spécial du contrôle. |
| [setTabKeyBehavior(boolean value)](#setTabKeyBehavior-boolean-) | Indique si les caractères de tabulation sont autorisés dans le texte du contrôle. |
| [setText(String value)](#setText-java.lang.String-) | Définit le texte du contrôle. |
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

**Example**

```
         //excel default color system 12 or green(0x0000FF00)
         activeXControl.setBorderOleColor(/*unchecked*/((int)0x80000012L));
```

**Returns:**
int
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```


Obtient le type de bordure utilisé par le contrôle.

Voir [ControlBorderType](../../com.aspose.cells/controlbordertype).

**Example**

```
         activeXControl.setBorderStyle(com.aspose.cells.ControlBorderType.SINGLE);
```

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
### getDropButtonStyle() {#getDropButtonStyle--}
```
public int getDropButtonStyle()
```


Spécifie le symbole affiché sur le bouton déroulant

Voir [DropButtonStyle](../../com.aspose.cells/dropbuttonstyle).

**Example**

```
         activeXControl.setDropButtonStyle(com.aspose.cells.DropButtonStyle.ARROW);
```

**Returns:**
int
### getEnterFieldBehavior() {#getEnterFieldBehavior--}
```
public boolean getEnterFieldBehavior()
```


Spécifie le comportement de sélection lors de l'entrée dans le contrôle. True indique que la sélection reste inchangée depuis la dernière fois que le contrôle était actif. False indique que tout le texte du contrôle sera sélectionné lors de l'entrée dans le contrôle.

**Example**

```
         if(!activeXControl.getEnterFieldBehavior())
         {
             activeXControl.setEnterFieldBehavior(true);
         }
```

**Returns:**
boolean
### getEnterKeyBehavior() {#getEnterKeyBehavior--}
```
public boolean getEnterKeyBehavior()
```


Spécifie le comportement de la touche ENTER. True indique que la pression sur ENTER créera une nouvelle ligne. False indique que la pression sur ENTER déplacera le focus vers l'objet suivant dans l'ordre de tabulation.

**Example**

```
         if(!activeXControl.getEnterKeyBehavior())
         {
             activeXControl.setEnterKeyBehavior(true);
         }
```

**Returns:**
boolean
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
### getHideSelection() {#getHideSelection--}
```
public boolean getHideSelection()
```


Indique si le texte sélectionné dans le contrôle apparaît en surbrillance lorsque le contrôle n'a pas le focus.

**Example**

```
         if(!activeXControl.getHideSelection())
         {
             activeXControl.setHideSelection(true);
         }
```

**Returns:**
boolean
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

**Example**

```
         if(!activeXControl.getIntegralHeight())
         {
             activeXControl.setIntegralHeight(true);
         }
```

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
### getMaxLength() {#getMaxLength--}
```
public int getMaxLength()
```


Obtient le nombre maximal de caractères

**Example**

```
         if(activeXControl.getMaxLength() == 0)
         {
             activeXControl.setMaxLength(30);
         }
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
### getPasswordChar() {#getPasswordChar--}
```
public char getPasswordChar()
```


Obtient un caractère à afficher à la place des caractères saisis.

**Example**

```
         activeXControl.setPasswordChar('a');
```

**Returns:**
char
### getScrollBars() {#getScrollBars--}
```
public int getScrollBars()
```


Indique si le contrôle possède des barres de défilement verticales, des barres de défilement horizontales, les deux ou aucune.

Voir [ControlScrollBarType](../../com.aspose.cells/controlscrollbartype).

**Example**

```
         activeXControl.setScrollBars(com.aspose.cells.ControlScrollBarType.BARS_VERTICAL);
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
### getShowDropButtonTypeWhen() {#getShowDropButtonTypeWhen--}
```
public int getShowDropButtonTypeWhen()
```


Spécifie le symbole affiché sur le bouton déroulant

Voir [ShowDropButtonType](../../com.aspose.cells/showdropbuttontype).

**Example**

```
         activeXControl.setShowDropButtonTypeWhen(com.aspose.cells.ShowDropButtonType.FOCUS);
```

**Returns:**
int
### getSpecialEffect() {#getSpecialEffect--}
```
public int getSpecialEffect()
```


Obtient l'effet spécial du contrôle.

Voir [ControlSpecialEffectType](../../com.aspose.cells/controlspecialeffecttype).

**Example**

```
         activeXControl.setSpecialEffect(com.aspose.cells.ControlSpecialEffectType.BUMP);
```

**Returns:**
int
### getTabKeyBehavior() {#getTabKeyBehavior--}
```
public boolean getTabKeyBehavior()
```


Indique si les caractères de tabulation sont autorisés dans le texte du contrôle.

**Example**

```
         if(!activeXControl.getTabKeyBehavior())
         {
             activeXControl.setTabKeyBehavior(true);
         }
```

**Returns:**
boolean
### getText() {#getText--}
```
public String getText()
```


Obtient le texte du contrôle.

**Example**

```
         activeXControl.setText("This is a test.");
```

**Returns:**
java.lang.String
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
         /*Aspose.Cells.Drawing.ActiveXControls.ControlType*/int type = activeXControl.getType();
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
### isAutoTab() {#isAutoTab--}
```
public boolean isAutoTab()
```


Indique si le focus se déplacera automatiquement vers le contrôle suivant lorsque l'utilisateur saisit le nombre maximal de caractères.

**Example**

```
         if(!activeXControl.isAutoTab())
         {
             activeXControl.setAutoTab(true);
         }
```

**Returns:**
boolean
### isAutoWordSelected() {#isAutoWordSelected--}
```
public boolean isAutoWordSelected()
```


Spécifie l'unité de base utilisée pour étendre une sélection. True indique que l'unité de base est un caractère unique. false indique que l'unité de base est un mot entier.

**Example**

```
         if(!activeXControl.isAutoWordSelected())
         {
             activeXControl.setAutoWordSelected(true);
         }
```

**Returns:**
boolean
### isDragBehaviorEnabled() {#isDragBehaviorEnabled--}
```
public boolean isDragBehaviorEnabled()
```


Indique si le glisser-déposer est activé pour le contrôle.

**Example**

```
         if(!activeXControl.isDragBehaviorEnabled())
         {
             activeXControl.setDragBehaviorEnabled(true);
         }
```

**Returns:**
boolean
### isEditable() {#isEditable--}
```
public boolean isEditable()
```


Indique si l'utilisateur peut saisir du texte dans le contrôle.

**Example**

```
         if(!activeXControl.isEditable())
         {
             activeXControl.setEditable(true);
         }
```

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
### isMultiLine() {#isMultiLine--}
```
public boolean isMultiLine()
```


Indique si le contrôle peut afficher plus d'une ligne de texte.

**Example**

```
         if(!activeXControl.isMultiLine())
         {
             activeXControl.setMultiLine(true);
         }
```

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

**Example**

```
         if(!activeXControl.isWordWrapped())
         {
             activeXControl.setWordWrapped(true);
         }
```

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

### setAutoTab(boolean value) {#setAutoTab-boolean-}
```
public void setAutoTab(boolean value)
```


Indique si le focus se déplacera automatiquement vers le contrôle suivant lorsque l'utilisateur saisit le nombre maximal de caractères.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAutoWordSelected(boolean value) {#setAutoWordSelected-boolean-}
```
public void setAutoWordSelected(boolean value)
```


Spécifie l'unité de base utilisée pour étendre une sélection. True indique que l'unité de base est un caractère unique. false indique que l'unité de base est un mot entier.

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

### setDragBehaviorEnabled(boolean value) {#setDragBehaviorEnabled-boolean-}
```
public void setDragBehaviorEnabled(boolean value)
```


Indique si le glisser-déposer est activé pour le contrôle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setDropButtonStyle(int value) {#setDropButtonStyle-int-}
```
public void setDropButtonStyle(int value)
```


Spécifie le symbole affiché sur le bouton déroulant

Voir [DropButtonStyle](../../com.aspose.cells/dropbuttonstyle).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setEditable(boolean value) {#setEditable-boolean-}
```
public void setEditable(boolean value)
```


Indique si l'utilisateur peut saisir du texte dans le contrôle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public void setEnabled(boolean value)
```


Indique si le contrôle peut recevoir le focus et répondre aux événements générés par l'utilisateur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEnterFieldBehavior(boolean value) {#setEnterFieldBehavior-boolean-}
```
public void setEnterFieldBehavior(boolean value)
```


Spécifie le comportement de sélection lors de l'entrée dans le contrôle. True indique que la sélection reste inchangée depuis la dernière fois que le contrôle était actif. False indique que tout le texte du contrôle sera sélectionné lors de l'entrée dans le contrôle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEnterKeyBehavior(boolean value) {#setEnterKeyBehavior-boolean-}
```
public void setEnterKeyBehavior(boolean value)
```


Spécifie le comportement de la touche ENTER. True indique que la pression sur ENTER créera une nouvelle ligne. False indique que la pression sur ENTER déplacera le focus vers l'objet suivant dans l'ordre de tabulation.

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

### setHideSelection(boolean value) {#setHideSelection-boolean-}
```
public void setHideSelection(boolean value)
```


Indique si le texte sélectionné dans le contrôle apparaît en surbrillance lorsque le contrôle n'a pas le focus.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

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

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Indique si les données du contrôle sont verrouillées pour l'édition.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setMaxLength(int value) {#setMaxLength-int-}
```
public void setMaxLength(int value)
```


Définit le nombre maximal de caractères

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

### setMultiLine(boolean value) {#setMultiLine-boolean-}
```
public void setMultiLine(boolean value)
```


Indique si le contrôle peut afficher plus d'une ligne de texte.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setPasswordChar(char value) {#setPasswordChar-char-}
```
public void setPasswordChar(char value)
```


Définit un caractère à afficher à la place des caractères saisis.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | char |  |

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

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


Indique s'il faut afficher une ombre.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowDropButtonTypeWhen(int value) {#setShowDropButtonTypeWhen-int-}
```
public void setShowDropButtonTypeWhen(int value)
```


Spécifie le symbole affiché sur le bouton déroulant

Voir [ShowDropButtonType](../../com.aspose.cells/showdropbuttontype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

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

### setTabKeyBehavior(boolean value) {#setTabKeyBehavior-boolean-}
```
public void setTabKeyBehavior(boolean value)
```


Indique si les caractères de tabulation sont autorisés dans le texte du contrôle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Définit le texte du contrôle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

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

