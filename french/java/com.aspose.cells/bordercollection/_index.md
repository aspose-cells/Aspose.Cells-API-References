---
title: "BorderCollection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Encapsule une collection d'objets."
type: docs
url: /fr/java/com.aspose.cells/bordercollection/
---

**Inheritance:**
java.lang.Object
```
public class BorderCollection
```

Encapsule une collection d'objets [Border](../../com.aspose.cells/border).

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Adding a new worksheet to the Excel object
         workbook.getWorksheets().add();
 
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         //Accessing the "A1" cell from the worksheet
         Cell cell = worksheet.getCells().get("A1");
 
         //Adding some value to the "A1" cell
         cell.putValue("Visit Aspose!");
 
         Style style = cell.getStyle();
 
         //Setting the line style of the top border
         style.getBorders().getByBorderType(BorderType.TOP_BORDER).setLineStyle(CellBorderType.THICK);
 
         //Setting the color of the top border
         style.getBorders().getByBorderType(BorderType.TOP_BORDER).setColor(Color.getBlack());
 
         //Setting the line style of the bottom border
         style.getBorders().getByBorderType(BorderType.BOTTOM_BORDER).setLineStyle(CellBorderType.THICK);
 
         //Setting the color of the bottom border
         style.getBorders().getByBorderType(BorderType.BOTTOM_BORDER).setColor(Color.getBlack());
 
         //Setting the line style of the left border
         style.getBorders().getByBorderType(BorderType.LEFT_BORDER).setLineStyle(CellBorderType.THICK);
 
         //Setting the color of the left border
         style.getBorders().getByBorderType(BorderType.LEFT_BORDER).setColor(Color.getBlack());
 
         //Setting the line style of the right border
         style.getBorders().getByBorderType(BorderType.RIGHT_BORDER).setLineStyle(CellBorderType.THICK);
 
         //Setting the color of the right border
         style.getBorders().getByBorderType(BorderType.RIGHT_BORDER).setColor(Color.getBlack());
 
         cell.setStyle(style);
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getByBorderType(int borderType)](#getByBorderType-int-) | Obtient l'élément [Border](../../com.aspose.cells/border) à l'index spécifié. |
| [getClass()](#getClass--) |  |
| [getDiagonalColor()](#getDiagonalColor--) | Obtient la [Color](../../com.aspose.cells/color) des lignes diagonales. |
| [getDiagonalStyle()](#getDiagonalStyle--) | Obtient le style des lignes diagonales. |
| [hashCode()](#hashCode--) |  |
| [isOutline()](#isOutline--) | Indique si les bordures gauche, droite, supérieure et inférieure doivent être appliquées uniquement aux bordures extérieures d'une plage de cellules. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setColor(Color color)](#setColor-com.aspose.cells.Color-) | Définit la [Color](../../com.aspose.cells/color) de toutes les bordures de la collection. |
| [setDiagonalColor(Color value)](#setDiagonalColor-com.aspose.cells.Color-) | Définit la [Color](../../com.aspose.cells/color) des lignes diagonales. |
| [setDiagonalStyle(int value)](#setDiagonalStyle-int-) | Définit le style des lignes diagonales. |
| [setOutline(boolean value)](#setOutline-boolean-) | Indique si les bordures gauche, droite, supérieure et inférieure doivent être appliquées uniquement aux bordures extérieures d'une plage de cellules. |
| [setStyle(int style)](#setStyle-int-) | Définit le style de toutes les bordures de la collection. |
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
### getByBorderType(int borderType) {#getByBorderType-int-}
```
public Border getByBorderType(int borderType)
```


Obtient l'élément [Border](../../com.aspose.cells/border) à l'index spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| borderType | int | [BorderType](../../com.aspose.cells/bordertype). La bordure à récupérer. |

**Returns:**
[Border](../../com.aspose.cells/border) - The element at the specified index.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDiagonalColor() {#getDiagonalColor--}
```
public Color getDiagonalColor()
```


Obtient la [Color](../../com.aspose.cells/color) des lignes diagonales.

**Returns:**
[Color](../../com.aspose.cells/color)
### getDiagonalStyle() {#getDiagonalStyle--}
```
public int getDiagonalStyle()
```


Obtient le style des lignes diagonales.

Voir [CellBorderType](../../com.aspose.cells/cellbordertype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isOutline() {#isOutline--}
```
public boolean isOutline()
```


Indique si les bordures gauche, droite, supérieure et inférieure doivent être appliquées uniquement aux bordures extérieures d'une plage de cellules. La valeur par défaut est true.

**Remarks**

Fonctionne uniquement lors de l'application à une plage pour les mises en forme conditionnelles, les tableaux croisés dynamiques. Si false, les bordures gauche, droite, supérieure et inférieure seront appliquées à chaque cellule, sinon uniquement aux bordures extérieures d'une plage de cellules. Si true, veuillez définir les bordures horizontales et verticales des bordures internes de la plage pour les mises en forme conditionnelles, les tableaux croisés dynamiques.

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




### setColor(Color color) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color color)
```


Définit la [Color](../../com.aspose.cells/color) de toutes les bordures de la collection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Couleur des bordures [Color](../../com.aspose.cells/color). |

### setDiagonalColor(Color value) {#setDiagonalColor-com.aspose.cells.Color-}
```
public void setDiagonalColor(Color value)
```


Définit la [Color](../../com.aspose.cells/color) des lignes diagonales.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setDiagonalStyle(int value) {#setDiagonalStyle-int-}
```
public void setDiagonalStyle(int value)
```


Définit le style des lignes diagonales.

Voir [CellBorderType](../../com.aspose.cells/cellbordertype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setOutline(boolean value) {#setOutline-boolean-}
```
public void setOutline(boolean value)
```


Indique si les bordures gauche, droite, supérieure et inférieure doivent être appliquées uniquement aux bordures extérieures d'une plage de cellules. La valeur par défaut est true.

**Remarks**

Fonctionne uniquement lors de l'application à une plage pour les mises en forme conditionnelles, les tableaux croisés dynamiques. Si false, les bordures gauche, droite, supérieure et inférieure seront appliquées à chaque cellule, sinon uniquement aux bordures extérieures d'une plage de cellules. Si true, veuillez définir les bordures horizontales et verticales des bordures internes de la plage pour les mises en forme conditionnelles, les tableaux croisés dynamiques.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setStyle(int style) {#setStyle-int-}
```
public void setStyle(int style)
```


Définit le style de toutes les bordures de la collection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| style | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Style des bordures |

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

