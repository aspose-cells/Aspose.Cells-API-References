---
title: "ShapeTextAlignment"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente le paramètre d'alignement du texte des formes"
type: docs
url: /fr/java/com.aspose.cells/shapetextalignment/
---

**Inheritance:**
java.lang.Object
```
public class ShapeTextAlignment
```

Représente le paramètre d'alignement du texte de la forme ;

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Shape shape = workbook.getWorksheets().get(0).getShapes().addRectangle(1, 0, 1, 0, 50, 100);
         ShapeTextAlignment shapeTextAlignment = shape.getTextBody().getTextAlignment();
 
         //do your business
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | Détermine si cette instance a la même valeur qu'un autre objet [ShapeTextAlignment](../../com.aspose.cells/shapetextalignment) spécifié. |
| [getAutoSize()](#getAutoSize--) | Indique si la taille de la forme est ajustée automatiquement en fonction de son contenu. |
| [getBottomMarginPt()](#getBottomMarginPt--) | Renvoie la marge inférieure en unité de Points |
| [getClass()](#getClass--) |  |
| [getLeftMarginPt()](#getLeftMarginPt--) | Renvoie la marge gauche en unité de Points |
| [getNumberOfColumns()](#getNumberOfColumns--) | Obtient le nombre de colonnes de texte dans le rectangle englobant. |
| [getRightMarginPt()](#getRightMarginPt--) | Renvoie la marge droite en unité de Points |
| [getRotateTextWithShape()](#getRotateTextWithShape--) | Indique si le texte est tourné avec la forme. |
| [getRotationAngle()](#getRotationAngle--) | Obtient la rotation de la forme. |
| [getTextHorizontalOverflow()](#getTextHorizontalOverflow--) | Obtient le type de dépassement horizontal du texte de la zone de texte. |
| [getTextShapeType()](#getTextShapeType--) | Obtient le type de transformation du texte. |
| [getTextVerticalOverflow()](#getTextVerticalOverflow--) | Obtient le type de dépassement vertical du texte de la zone de texte. |
| [getTextVerticalType()](#getTextVerticalType--) | Obtient la direction du texte. |
| [getTopMarginPt()](#getTopMarginPt--) | Renvoie la marge supérieure en unité de Points |
| [hashCode()](#hashCode--) |  |
| [isAutoMargin()](#isAutoMargin--) | Indique si la marge du cadre de texte est automatique. |
| [isLockedText()](#isLockedText--) | Indique si la forme est verrouillée lorsque la feuille de calcul est protégée. |
| [isTextWrapped()](#isTextWrapped--) | Obtient le type d'habillage du texte de la forme qui contient du texte. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoMargin(boolean value)](#setAutoMargin-boolean-) | Indique si la marge du cadre de texte est automatique. |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Indique si la taille de la forme est ajustée automatiquement en fonction de son contenu. |
| [setBottomMarginPt(double value)](#setBottomMarginPt-double-) | Renvoie la marge inférieure en unité de Points |
| [setLeftMarginPt(double value)](#setLeftMarginPt-double-) | Renvoie la marge gauche en unité de Points |
| [setLockedText(boolean value)](#setLockedText-boolean-) | Indique si la forme est verrouillée lorsque la feuille de calcul est protégée. |
| [setNumberOfColumns(int value)](#setNumberOfColumns-int-) | Définit le nombre de colonnes de texte dans le rectangle englobant. |
| [setRightMarginPt(double value)](#setRightMarginPt-double-) | Renvoie la marge droite en unité de Points |
| [setRotateTextWithShape(boolean value)](#setRotateTextWithShape-boolean-) | Indique si le texte est tourné avec la forme. |
| [setRotationAngle(double value)](#setRotationAngle-double-) | Définit la rotation de la forme. |
| [setTextHorizontalOverflow(int value)](#setTextHorizontalOverflow-int-) | Définit le type de dépassement horizontal du texte de la zone de texte. |
| [setTextShapeType(int value)](#setTextShapeType-int-) | Définit le type de transformation du texte. |
| [setTextVerticalOverflow(int value)](#setTextVerticalOverflow-int-) | Définit le type de dépassement vertical du texte de la zone de texte. |
| [setTextVerticalType(int value)](#setTextVerticalType-int-) | Définit la direction du texte. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Définit le type d'habillage du texte de la forme contenant du texte. |
| [setTopMarginPt(double value)](#setTopMarginPt-double-) | Renvoie la marge supérieure en unité de Points |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Détermine si cette instance a la même valeur qu'un autre objet [ShapeTextAlignment](../../com.aspose.cells/shapetextalignment) spécifié.

**Example**

```
         //You have to make sure that the index value in this line of code exists
         ShapeTextAlignment obj = workbook.getWorksheets().get(0).getShapes().get(0).getTextBody().getTextAlignment();
         if (shapeTextAlignment.equals(obj))
         {
             //do what you want
         }
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | L'objet [ShapeTextAlignment](../../com.aspose.cells/shapetextalignment) à comparer avec cette instance. |

**Returns:**
booléen - true si la valeur du paramètre obj est la même que la valeur de cette instance ; sinon, false. Si obj est null, cette méthode renvoie false.
### getAutoSize() {#getAutoSize--}
```
public boolean getAutoSize()
```


Indique si la taille de la forme est ajustée automatiquement en fonction de son contenu.

**Example**

```
         shapeTextAlignment.setAutoSize(false);
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
         shapeTextAlignment.setBottomMarginPt(2.0d);
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


Renvoie la marge gauche en unité de Points

**Example**

```
         shapeTextAlignment.setLeftMarginPt(2.0d);
```

**Returns:**
double
### getNumberOfColumns() {#getNumberOfColumns--}
```
public int getNumberOfColumns()
```


Obtient le nombre de colonnes de texte dans le rectangle englobant.

**Returns:**
int
### getRightMarginPt() {#getRightMarginPt--}
```
public double getRightMarginPt()
```


Renvoie la marge droite en unité de Points

**Example**

```
         shapeTextAlignment.setRightMarginPt(2.0d);
```

**Returns:**
double
### getRotateTextWithShape() {#getRotateTextWithShape--}
```
public boolean getRotateTextWithShape()
```


Indique si le texte est tourné avec la forme.

**Example**

```
         shapeTextAlignment.setRotateTextWithShape(true);
```

**Returns:**
boolean
### getRotationAngle() {#getRotationAngle--}
```
public double getRotationAngle()
```


Obtient la rotation de la forme.

**Example**

```
         shapeTextAlignment.setRotationAngle(90);
```

**Returns:**
double
### getTextHorizontalOverflow() {#getTextHorizontalOverflow--}
```
public int getTextHorizontalOverflow()
```


Obtient le type de dépassement horizontal du texte de la zone de texte.

Voir [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Example**

```
         shapeTextAlignment.setTextHorizontalOverflow(TextOverflowType.CLIP);
```

**Returns:**
int
### getTextShapeType() {#getTextShapeType--}
```
public int getTextShapeType()
```


Obtient le type de transformation du texte.

Voir [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Example**

```
         //Usually do not modify this value unless you know exactly what the modification will result in
         shapeTextAlignment.setTextShapeType(AutoShapeType.TEXT_BOX);
```

**Returns:**
int
### getTextVerticalOverflow() {#getTextVerticalOverflow--}
```
public int getTextVerticalOverflow()
```


Obtient le type de dépassement vertical du texte de la zone de texte.

Voir [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Example**

```
         shapeTextAlignment.setTextVerticalOverflow(TextOverflowType.CLIP);
```

**Returns:**
int
### getTextVerticalType() {#getTextVerticalType--}
```
public int getTextVerticalType()
```


Obtient la direction du texte.

Voir [TextVerticalType](../../com.aspose.cells/textverticaltype).

**Example**

```
         shapeTextAlignment.setTextVerticalType(com.aspose.cells.TextVerticalType.HORIZONTAL);
```

**Returns:**
int
### getTopMarginPt() {#getTopMarginPt--}
```
public double getTopMarginPt()
```


Renvoie la marge supérieure en unité de Points

**Example**

```
         shapeTextAlignment.setTopMarginPt(2.0d);
```

**Returns:**
double
### hashCode() {#hashCode--}
```
public int hashCode()
```




**Returns:**
int -
### isAutoMargin() {#isAutoMargin--}
```
public boolean isAutoMargin()
```


Indique si la marge du cadre de texte est automatique.

**Example**

```
         shapeTextAlignment.setAutoMargin(true);
```

**Returns:**
boolean
### isLockedText() {#isLockedText--}
```
public boolean isLockedText()
```


Indique si la forme est verrouillée lorsque la feuille de calcul est protégée.

**Remarks**

Fonctionne uniquement lorsque la feuille de calcul est protégée.

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


Obtient le type d'habillage du texte de la forme qui contient du texte.

**Example**

```
         shapeTextAlignment.setTextWrapped(true);
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




### setAutoMargin(boolean value) {#setAutoMargin-boolean-}
```
public void setAutoMargin(boolean value)
```


Indique si la marge du cadre de texte est automatique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAutoSize(boolean value) {#setAutoSize-boolean-}
```
public void setAutoSize(boolean value)
```


Indique si la taille de la forme est ajustée automatiquement en fonction de son contenu.

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


Renvoie la marge gauche en unité de Points

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setLockedText(boolean value) {#setLockedText-boolean-}
```
public void setLockedText(boolean value)
```


Indique si la forme est verrouillée lorsque la feuille de calcul est protégée.

**Remarks**

Fonctionne uniquement lorsque la feuille de calcul est protégée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setNumberOfColumns(int value) {#setNumberOfColumns-int-}
```
public void setNumberOfColumns(int value)
```


Définit le nombre de colonnes de texte dans le rectangle englobant.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setRightMarginPt(double value) {#setRightMarginPt-double-}
```
public void setRightMarginPt(double value)
```


Renvoie la marge droite en unité de Points

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setRotateTextWithShape(boolean value) {#setRotateTextWithShape-boolean-}
```
public void setRotateTextWithShape(boolean value)
```


Indique si le texte est tourné avec la forme.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setRotationAngle(double value) {#setRotationAngle-double-}
```
public void setRotationAngle(double value)
```


Définit la rotation de la forme.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setTextHorizontalOverflow(int value) {#setTextHorizontalOverflow-int-}
```
public void setTextHorizontalOverflow(int value)
```


Définit le type de dépassement horizontal du texte de la zone de texte.

Voir [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setTextShapeType(int value) {#setTextShapeType-int-}
```
public void setTextShapeType(int value)
```


Définit le type de transformation du texte.

Voir [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setTextVerticalOverflow(int value) {#setTextVerticalOverflow-int-}
```
public void setTextVerticalOverflow(int value)
```


Définit le type de dépassement vertical du texte de la zone de texte.

Voir [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setTextVerticalType(int value) {#setTextVerticalType-int-}
```
public void setTextVerticalType(int value)
```


Définit la direction du texte.

Voir [TextVerticalType](../../com.aspose.cells/textverticaltype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


Définit le type d'habillage du texte de la forme contenant du texte.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setTopMarginPt(double value) {#setTopMarginPt-double-}
```
public void setTopMarginPt(double value)
```


Renvoie la marge supérieure en unité de Points

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

