---
title: "TextBoxOptions"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente les options de texte de la forme"
type: docs
url: /fr/java/com.aspose.cells/textboxoptions/
---

**Inheritance:**
java.lang.Object
```
public class TextBoxOptions
```

Représente les options de texte de la forme

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         int index = workbook.getWorksheets().get(0).getTextBoxes().add(0, 0, 350, 350);
         Shape shape = workbook.getWorksheets().get(0).getTextBoxes().get(index);
         shape.setText("This is test.");
 
         //do your business
 
         //Save the excel file.
         workbook.save("exmaple.xlsx");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowTextToOverflow()](#getAllowTextToOverflow--) | Indique si le texte peut dépasser la forme. |
| [getBottomMarginPt()](#getBottomMarginPt--) | Renvoie la marge inférieure en unité de Points |
| [getClass()](#getClass--) |  |
| [getLeftMarginPt()](#getLeftMarginPt--) | Obtient la marge gauche en unité de points. |
| [getResizeToFitText()](#getResizeToFitText--) | Indique s'il faut redimensionner la forme pour ajuster le texte |
| [getRightMarginPt()](#getRightMarginPt--) | Obtient la marge droite en unité de points. |
| [getShapeTextDirection()](#getShapeTextDirection--) | Obtient la direction d'affichage du texte dans un corps de texte donné. |
| [getShapeTextVerticalAlignment()](#getShapeTextVerticalAlignment--) | Il correspond à "Format Shape - Text Options - Text Box - Vertical Alignment" dans Excel. |
| [getTopMarginPt()](#getTopMarginPt--) | Obtient la marge supérieure en unité de points. |
| [getWrapTextInShape()](#getWrapTextInShape--) | Spécifie le retour à la ligne du texte dans une forme. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowTextToOverflow(boolean value)](#setAllowTextToOverflow-boolean-) | Indique si le texte peut dépasser la forme. |
| [setBottomMarginPt(double value)](#setBottomMarginPt-double-) | Renvoie la marge inférieure en unité de Points |
| [setLeftMarginPt(double value)](#setLeftMarginPt-double-) | Définit la marge gauche en unité de points. |
| [setResizeToFitText(boolean value)](#setResizeToFitText-boolean-) | Indique s'il faut redimensionner la forme pour ajuster le texte |
| [setRightMarginPt(double value)](#setRightMarginPt-double-) | Définit la marge droite en unité de points. |
| [setShapeTextDirection(int value)](#setShapeTextDirection-int-) | Définit la direction d'affichage du texte dans un corps de texte donné. |
| [setShapeTextVerticalAlignment(int value)](#setShapeTextVerticalAlignment-int-) | Il correspond à "Format Shape - Text Options - Text Box - Vertical Alignment" dans Excel. |
| [setTopMarginPt(double value)](#setTopMarginPt-double-) | Définit la marge supérieure en unité de points. |
| [setWrapTextInShape(boolean value)](#setWrapTextInShape-boolean-) | Spécifie le retour à la ligne du texte dans une forme. |
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
### getAllowTextToOverflow() {#getAllowTextToOverflow--}
```
public boolean getAllowTextToOverflow()
```


Indique si le texte peut dépasser la forme.

**Example**

```
         shape.getTextBoxOptions().setAllowTextToOverflow(true);
```

**Returns:**
boolean
### getBottomMarginPt() {#getBottomMarginPt--}
```
public double getBottomMarginPt()
```


Renvoie la marge inférieure en unité de Points

**Example**

```
         shape.getTextBoxOptions().setBottomMarginPt(0.2d);
```

**Returns:**
double
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getLeftMarginPt() {#getLeftMarginPt--}
```
public double getLeftMarginPt()
```


Obtient la marge gauche en unité de points.

**Example**

```
         shape.getTextBoxOptions().setLeftMarginPt(0.2d);
```

**Returns:**
double
### getResizeToFitText() {#getResizeToFitText--}
```
public boolean getResizeToFitText()
```


Indique s'il faut redimensionner la forme pour ajuster le texte

**Example**

```
         shape.getTextBoxOptions().setResizeToFitText(true);
```

**Returns:**
boolean
### getRightMarginPt() {#getRightMarginPt--}
```
public double getRightMarginPt()
```


Obtient la marge droite en unité de points.

**Example**

```
         shape.getTextBoxOptions().setRightMarginPt(0.2d);
```

**Returns:**
double
### getShapeTextDirection() {#getShapeTextDirection--}
```
public int getShapeTextDirection()
```


Obtient la direction d'affichage du texte dans un corps de texte donné. Il correspond à "Format Shape - Text Options - Text Box - Text direction" dans Excel

Voir [TextVerticalType](../../com.aspose.cells/textverticaltype).

**Example**

```
         shape.getTextBoxOptions().setShapeTextDirection(TextVerticalType.VERTICAL);
```

**Returns:**
int
### getShapeTextVerticalAlignment() {#getShapeTextVerticalAlignment--}
```
public int getShapeTextVerticalAlignment()
```


Il correspond à "Format Shape - Text Options - Text Box - Vertical Alignment" dans Excel.

Voir [ShapeTextVerticalAlignmentType](../../com.aspose.cells/shapetextverticalalignmenttype).

**Example**

```
         shape.getTextBoxOptions().setShapeTextVerticalAlignment(ShapeTextVerticalAlignmentType.LEFT);
```

**Returns:**
int
### getTopMarginPt() {#getTopMarginPt--}
```
public double getTopMarginPt()
```


Obtient la marge supérieure en unité de points.

**Example**

```
         shape.getTextBoxOptions().setTopMarginPt(0.2d);
```

**Returns:**
double
### getWrapTextInShape() {#getWrapTextInShape--}
```
public boolean getWrapTextInShape()
```


Spécifie le retour à la ligne du texte dans une forme. False - Aucun retour à la ligne ne se produira dans le corps du texte. True - Un retour à la ligne se produira dans le corps du texte.

**Example**

```
         shape.getTextBoxOptions().setWrapTextInShape(true);
```

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




### setAllowTextToOverflow(boolean value) {#setAllowTextToOverflow-boolean-}
```
public void setAllowTextToOverflow(boolean value)
```


Indique si le texte peut dépasser la forme.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setBottomMarginPt(double value) {#setBottomMarginPt-double-}
```
public void setBottomMarginPt(double value)
```


Renvoie la marge inférieure en unité de Points

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setLeftMarginPt(double value) {#setLeftMarginPt-double-}
```
public void setLeftMarginPt(double value)
```


Définit la marge gauche en unité de points.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setResizeToFitText(boolean value) {#setResizeToFitText-boolean-}
```
public void setResizeToFitText(boolean value)
```


Indique s'il faut redimensionner la forme pour ajuster le texte

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setRightMarginPt(double value) {#setRightMarginPt-double-}
```
public void setRightMarginPt(double value)
```


Définit la marge droite en unité de points.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setShapeTextDirection(int value) {#setShapeTextDirection-int-}
```
public void setShapeTextDirection(int value)
```


Définit la direction d'affichage du texte dans un corps de texte donné. Il correspond à "Format Shape - Text Options - Text Box - Text direction" dans Excel

Voir [TextVerticalType](../../com.aspose.cells/textverticaltype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setShapeTextVerticalAlignment(int value) {#setShapeTextVerticalAlignment-int-}
```
public void setShapeTextVerticalAlignment(int value)
```


Il correspond à "Format Shape - Text Options - Text Box - Vertical Alignment" dans Excel.

Voir [ShapeTextVerticalAlignmentType](../../com.aspose.cells/shapetextverticalalignmenttype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setTopMarginPt(double value) {#setTopMarginPt-double-}
```
public void setTopMarginPt(double value)
```


Définit la marge supérieure en unité de points.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setWrapTextInShape(boolean value) {#setWrapTextInShape-boolean-}
```
public void setWrapTextInShape(boolean value)
```


Spécifie le retour à la ligne du texte dans une forme. False - Aucun retour à la ligne ne se produira dans le corps du texte. True - Un retour à la ligne se produira dans le corps du texte.

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

