---
title: "DataBar"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Décrit la règle de mise en forme conditionnelle DataBar."
type: docs
url: /fr/java/com.aspose.cells/databar/
---

**Inheritance:**
java.lang.Object
```
public class DataBar
```

Décrivez la règle de mise en forme conditionnelle DataBar. Cette règle de mise en forme conditionnelle affiche une barre de données graduée dans la plage de cellules.

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
         int idx = fcs.addCondition(FormatConditionType.DATA_BAR);
 
         fcs.addArea(ca);
 
         FormatCondition cond = fcs.get(idx);
 
         //Get Databar
         DataBar dataBar = cond.getDataBar();
 
         dataBar.setColor(Color.getOrange());
 
         //Set Databar properties
         dataBar.getMinCfvo().setType(FormatConditionValueType.PERCENTILE);
 
         dataBar.getMinCfvo().setValue(30);
 
         dataBar.setShowValue(false);
 
         dataBar.getBarBorder().setType(DataBarBorderType.SOLID);
 
         dataBar.getBarBorder().setColor(Color.getPlum());
 
          dataBar.setBarFillType(DataBarFillType.SOLID);
 
          dataBar.setAxisColor(Color.getRed());
 
          dataBar.setAxisPosition(DataBarAxisPosition.MIDPOINT);
 
          dataBar.getNegativeBarFormat().setColorType(DataBarNegativeColorType.COLOR);
 
          dataBar.getNegativeBarFormat().setColor(Color.getWhite());
 
          dataBar.getNegativeBarFormat().setBorderColorType(DataBarNegativeColorType.COLOR);
 
          dataBar.getNegativeBarFormat().setBorderColor(Color.getYellow());
 
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
| [getAxisColor()](#getAxisColor--) | Obtient la couleur de l'axe pour les cellules avec une mise en forme conditionnelle sous forme de barres de données. |
| [getAxisPosition()](#getAxisPosition--) | Obtient la position de l'axe des barres de données spécifiées par une règle de mise en forme conditionnelle. |
| [getBarBorder()](#getBarBorder--) | Obtient un objet qui spécifie la bordure d'une barre de données. |
| [getBarFillType()](#getBarFillType--) | Obtient la façon dont une barre de données est remplie de couleur. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Obtient la couleur de ce DataBar. |
| [getDirection()](#getDirection--) | Obtient la direction dans laquelle la barre de données est affichée. |
| [getMaxCfvo()](#getMaxCfvo--) | Obtient l'objet de valeur maximale de ce DataBar. |
| [getMaxLength()](#getMaxLength--) | Représente la longueur maximale de la barre de données. |
| [getMinCfvo()](#getMinCfvo--) | Obtient l'objet de valeur minimale de ce DataBar. |
| [getMinLength()](#getMinLength--) | Représente la longueur minimale de la barre de données. |
| [getNegativeBarFormat()](#getNegativeBarFormat--) | Obtient l'objet NegativeBarFormat associé à une règle de mise en forme conditionnelle de barre de données. |
| [getShowValue()](#getShowValue--) | Obtient le drapeau indiquant s'il faut afficher les valeurs des cellules sur lesquelles cette barre de données est appliquée. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAxisColor(Color value)](#setAxisColor-com.aspose.cells.Color-) | Obtient la couleur de l'axe pour les cellules avec une mise en forme conditionnelle sous forme de barres de données. |
| [setAxisPosition(int value)](#setAxisPosition-int-) | Définit la position de l'axe des barres de données spécifiées par une règle de mise en forme conditionnelle. |
| [setBarFillType(int value)](#setBarFillType-int-) | Définit la façon dont une barre de données est remplie de couleur. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Définit la couleur de ce DataBar. |
| [setDirection(int value)](#setDirection-int-) | Définit la direction dans laquelle la barre de données est affichée. |
| [setMaxLength(int value)](#setMaxLength-int-) | Représente la longueur maximale de la barre de données. |
| [setMinLength(int value)](#setMinLength-int-) | Représente la longueur minimale de la barre de données. |
| [setShowValue(boolean value)](#setShowValue-boolean-) | Définit le drapeau indiquant s'il faut afficher les valeurs des cellules sur lesquelles cette barre de données est appliquée. |
| [toImage(Cell cell, ImageOrPrintOptions imgOpts)](#toImage-com.aspose.cells.Cell-com.aspose.cells.ImageOrPrintOptions-) | Rendu de la barre de données dans la cellule en tableau d'octets d'image. |
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
### getAxisColor() {#getAxisColor--}
```
public Color getAxisColor()
```


Obtient la couleur de l'axe pour les cellules avec une mise en forme conditionnelle sous forme de barres de données.

**Returns:**
[Color](../../com.aspose.cells/color)
### getAxisPosition() {#getAxisPosition--}
```
public int getAxisPosition()
```


Obtient la position de l'axe des barres de données spécifiées par une règle de mise en forme conditionnelle.

Voir [DataBarAxisPosition](../../com.aspose.cells/databaraxisposition).

**Returns:**
int
### getBarBorder() {#getBarBorder--}
```
public DataBarBorder getBarBorder()
```


Obtient un objet qui spécifie la bordure d'une barre de données.

**Returns:**
[DataBarBorder](../../com.aspose.cells/databarborder)
### getBarFillType() {#getBarFillType--}
```
public int getBarFillType()
```


Obtient la façon dont une barre de données est remplie de couleur.

Voir [DataBarFillType](../../com.aspose.cells/databarfilltype).

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColor() {#getColor--}
```
public Color getColor()
```


Obtient la couleur de ce DataBar.

**Returns:**
[Color](../../com.aspose.cells/color)
### getDirection() {#getDirection--}
```
public int getDirection()
```


Obtient la direction dans laquelle la barre de données est affichée.

Voir [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Returns:**
int
### getMaxCfvo() {#getMaxCfvo--}
```
public ConditionalFormattingValue getMaxCfvo()
```


Obtient l'objet de valeur maximale de ce DataBar. Impossible de définir null ou CFValueObject avec le type FormatConditionValueType.Min.

**Returns:**
[ConditionalFormattingValue](../../com.aspose.cells/conditionalformattingvalue)
### getMaxLength() {#getMaxLength--}
```
public int getMaxLength()
```


Représente la longueur maximale de la barre de données.

**Returns:**
int
### getMinCfvo() {#getMinCfvo--}
```
public ConditionalFormattingValue getMinCfvo()
```


Obtient l'objet de valeur minimale de ce DataBar. Impossible de définir null ou CFValueObject avec le type FormatConditionValueType.Max.

**Returns:**
[ConditionalFormattingValue](../../com.aspose.cells/conditionalformattingvalue)
### getMinLength() {#getMinLength--}
```
public int getMinLength()
```


Représente la longueur minimale de la barre de données.

**Returns:**
int
### getNegativeBarFormat() {#getNegativeBarFormat--}
```
public NegativeBarFormat getNegativeBarFormat()
```


Obtient l'objet NegativeBarFormat associé à une règle de mise en forme conditionnelle de barre de données.

**Returns:**
[NegativeBarFormat](../../com.aspose.cells/negativebarformat)
### getShowValue() {#getShowValue--}
```
public boolean getShowValue()
```


Obtient le drapeau indiquant s'il faut afficher les valeurs des cellules sur lesquelles cette barre de données est appliquée. La valeur par défaut est true.

**Returns:**
boolean
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




### setAxisColor(Color value) {#setAxisColor-com.aspose.cells.Color-}
```
public void setAxisColor(Color value)
```


Obtient la couleur de l'axe pour les cellules avec une mise en forme conditionnelle sous forme de barres de données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setAxisPosition(int value) {#setAxisPosition-int-}
```
public void setAxisPosition(int value)
```


Définit la position de l'axe des barres de données spécifiées par une règle de mise en forme conditionnelle.

Voir [DataBarAxisPosition](../../com.aspose.cells/databaraxisposition).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setBarFillType(int value) {#setBarFillType-int-}
```
public void setBarFillType(int value)
```


Définit la façon dont une barre de données est remplie de couleur.

Voir [DataBarFillType](../../com.aspose.cells/databarfilltype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


Définit la couleur de ce DataBar.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setDirection(int value) {#setDirection-int-}
```
public void setDirection(int value)
```


Définit la direction dans laquelle la barre de données est affichée.

Voir [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setMaxLength(int value) {#setMaxLength-int-}
```
public void setMaxLength(int value)
```


Représente la longueur maximale de la barre de données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setMinLength(int value) {#setMinLength-int-}
```
public void setMinLength(int value)
```


Représente la longueur minimale de la barre de données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setShowValue(boolean value) {#setShowValue-boolean-}
```
public void setShowValue(boolean value)
```


Définit le drapeau indiquant s'il faut afficher les valeurs des cellules sur lesquelles cette barre de données est appliquée. La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### toImage(Cell cell, ImageOrPrintOptions imgOpts) {#toImage-com.aspose.cells.Cell-com.aspose.cells.ImageOrPrintOptions-}
```
public byte[] toImage(Cell cell, ImageOrPrintOptions imgOpts)
```


Rendu de la barre de données dans la cellule en tableau d'octets d'image.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | Indique la barre de données dans laquelle la cellule doit être rendue. |
| imgOpts | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | ImageOrPrintOptions contient certaines propriétés de l'image de sortie |

**Returns:**
byte[] -
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

