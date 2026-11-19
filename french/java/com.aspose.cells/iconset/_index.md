---
title: "IconSet"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Décrit la règle de mise en forme conditionnelle IconSet."
type: docs
url: /fr/java/com.aspose.cells/iconset/
---

**Inheritance:**
java.lang.Object
```
public class IconSet
```

Décrivez la règle de mise en forme conditionnelle IconSet. Cette règle de mise en forme conditionnelle applique des icônes aux cellules en fonction de leurs valeurs.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         Worksheet sheet = workbook.getWorksheets().get(0);
 
         //Adds an empty conditional formatting
         int index = sheet.getConditionalFormattings().add();
 
         FormatConditionCollection fcs = sheet.getConditionalFormattings().get(index);
 
         //Sets the conditional format range.
         CellArea ca = new CellArea();
 
         ca.StartRow = 0;
 
         ca.EndRow = 2;
 
         ca.StartColumn = 0;
 
         ca.EndColumn = 0;
 
         fcs.addArea(ca);
 
         //Adds condition.
         int idx = fcs.addCondition(FormatConditionType.ICON_SET);
 
         fcs.addArea(ca);
 
         FormatCondition cond = fcs.get(idx);
 
         //Get Icon Set
         IconSet iconSet = cond.getIconSet();
 
         //Set Icon Type
         iconSet.setType(IconSetType.ARROWS_3);
 
         //Put Cell Values
         Cell cell1 = sheet.getCells().get("A1");
 
         cell1.putValue(10);
 
         Cell cell2 = sheet.getCells().get("A2");
 
         cell2.putValue(120);
 
         Cell cell3 = sheet.getCells().get("A3");
 
         cell3.putValue(260);
 
         //Saving the Excel file
         workbook.save("book1.xlsx");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCfIcons()](#getCfIcons--) | Obtenez le[ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) de la collection |
| [getCfvos()](#getCfvos--) | Obtenez l'instance CFValueObjects. |
| [getClass()](#getClass--) |  |
| [getReverse()](#getReverse--) | Obtient le drapeau indiquant s'il faut inverser l'ordre par défaut des icônes dans cet ensemble d'icônes. |
| [getShowValue()](#getShowValue--) | Obtient le drapeau indiquant s'il faut afficher les valeurs des cellules auxquelles cet ensemble d'icônes est appliqué. |
| [getType()](#getType--) | Obtient le type d'ensemble d'icônes à afficher. |
| [hashCode()](#hashCode--) |  |
| [isCustom()](#isCustom--) | Indique si l'ensemble d'icônes est personnalisé. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setReverse(boolean value)](#setReverse-boolean-) | Définit le drapeau indiquant s'il faut inverser l'ordre par défaut des icônes dans cet ensemble d'icônes. |
| [setShowValue(boolean value)](#setShowValue-boolean-) | Définit le drapeau indiquant s'il faut afficher les valeurs des cellules auxquelles cet ensemble d'icônes est appliqué. |
| [setType(int value)](#setType-int-) | Définit le type d'ensemble d'icônes à afficher. |
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
### getCfIcons() {#getCfIcons--}
```
public ConditionalFormattingIconCollection getCfIcons()
```


Obtenez le[ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) de la collection

**Returns:**
[ConditionalFormattingIconCollection](../../com.aspose.cells/conditionalformattingiconcollection)
### getCfvos() {#getCfvos--}
```
public ConditionalFormattingValueCollection getCfvos()
```


Obtenez l'instance CFValueObjects.

**Returns:**
[ConditionalFormattingValueCollection](../../com.aspose.cells/conditionalformattingvaluecollection)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getReverse() {#getReverse--}
```
public boolean getReverse()
```


Obtient le drapeau indiquant s'il faut inverser l'ordre par défaut des icônes dans cet ensemble d'icônes. La valeur par défaut est false.

**Returns:**
boolean
### getShowValue() {#getShowValue--}
```
public boolean getShowValue()
```


Obtient le drapeau indiquant s'il faut afficher les valeurs des cellules auxquelles cet ensemble d'icônes est appliqué. La valeur par défaut est true.

**Returns:**
boolean
### getType() {#getType--}
```
public int getType()
```


Obtient le type d'ensemble d'icônes à afficher. La définition du type vérifiera automatiquement si le nombre actuel de Cfvos correspond au nouveau type. Si ce n'est pas le cas, les anciens Cfvos seront supprimés et des Cfvos par défaut seront ajoutés.

Voir [IconSetType](../../com.aspose.cells/iconsettype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCustom() {#isCustom--}
```
public boolean isCustom()
```


Indique si l'ensemble d'icônes est personnalisé. La valeur par défaut est false.

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




### setReverse(boolean value) {#setReverse-boolean-}
```
public void setReverse(boolean value)
```


Définit le drapeau indiquant s'il faut inverser l'ordre par défaut des icônes dans cet ensemble d'icônes. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowValue(boolean value) {#setShowValue-boolean-}
```
public void setShowValue(boolean value)
```


Définit le drapeau indiquant s'il faut afficher les valeurs des cellules auxquelles cet ensemble d'icônes est appliqué. La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Définit le type de jeu d’icônes à afficher. Le réglage du type vérifiera automatiquement si le nombre actuel de Cfvos est conforme au nouveau type. Si ce n’est pas le cas, les anciens Cfvos seront nettoyés et des Cfvos par défaut seront ajoutés.

Voir [IconSetType](../../com.aspose.cells/iconsettype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

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

