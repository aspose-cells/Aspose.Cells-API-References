---
title: "ShapeTextAlignment"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Einstellung der Textausrichtung von Formen dar"
type: docs
url: /de/java/com.aspose.cells/shapetextalignment/
---

**Inheritance:**
java.lang.Object
```
public class ShapeTextAlignment
```

Stellt die Einstellung der Textausrichtung der Form dar;

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Shape shape = workbook.getWorksheets().get(0).getShapes().addRectangle(1, 0, 1, 0, 50, 100);
         ShapeTextAlignment shapeTextAlignment = shape.getTextBody().getTextAlignment();
 
         //do your business
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | Bestimmt, ob diese Instanz denselben Wert wie ein anderes angegebenes [ShapeTextAlignment](../../com.aspose.cells/shapetextalignment)-Objekt hat. |
| [getAutoSize()](#getAutoSize--) | Gibt an, ob die Größe der Form automatisch an ihren Inhalt angepasst wird. |
| [getBottomMarginPt()](#getBottomMarginPt--) | Gibt den unteren Rand in Punkten zurück. |
| [getClass()](#getClass--) |  |
| [getLeftMarginPt()](#getLeftMarginPt--) | Gibt den linken Rand in Punkten zurück. |
| [getNumberOfColumns()](#getNumberOfColumns--) | Ruft die Anzahl der Textspalten im Begrenzungsrechteck ab. |
| [getRightMarginPt()](#getRightMarginPt--) | Gibt den rechten Rand in Punkten zurück. |
| [getRotateTextWithShape()](#getRotateTextWithShape--) | Gibt an, ob Text mit der Form rotiert wird. |
| [getRotationAngle()](#getRotationAngle--) | Ermittelt die Drehung der Form. |
| [getTextHorizontalOverflow()](#getTextHorizontalOverflow--) | Ruft den horizontalen Überlauftyp des Textes im Textfeld ab. |
| [getTextShapeType()](#getTextShapeType--) | Ruft den Transformationstyp des Textes ab. |
| [getTextVerticalOverflow()](#getTextVerticalOverflow--) | Ruft den vertikalen Überlauftyp des Textes im Textfeld ab. |
| [getTextVerticalType()](#getTextVerticalType--) | Ruft die Textrichtung ab. |
| [getTopMarginPt()](#getTopMarginPt--) | Gibt den oberen Rand in Punkten zurück. |
| [hashCode()](#hashCode--) |  |
| [isAutoMargin()](#isAutoMargin--) | Gibt an, ob der Rand des Textrahmens automatisch ist. |
| [isLockedText()](#isLockedText--) | Gibt an, ob die Form gesperrt ist, wenn das Arbeitsblatt geschützt ist. |
| [isTextWrapped()](#isTextWrapped--) | Ermittelt den Textumbruchtyp der Form, die Text enthält. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoMargin(boolean value)](#setAutoMargin-boolean-) | Gibt an, ob der Rand des Textrahmens automatisch ist. |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Gibt an, ob die Größe der Form automatisch an ihren Inhalt angepasst wird. |
| [setBottomMarginPt(double value)](#setBottomMarginPt-double-) | Gibt den unteren Rand in Punkten zurück. |
| [setLeftMarginPt(double value)](#setLeftMarginPt-double-) | Gibt den linken Rand in Punkten zurück. |
| [setLockedText(boolean value)](#setLockedText-boolean-) | Gibt an, ob die Form gesperrt ist, wenn das Arbeitsblatt geschützt ist. |
| [setNumberOfColumns(int value)](#setNumberOfColumns-int-) | Legt die Anzahl der Textspalten im Begrenzungsrechteck fest. |
| [setRightMarginPt(double value)](#setRightMarginPt-double-) | Gibt den rechten Rand in Punkten zurück. |
| [setRotateTextWithShape(boolean value)](#setRotateTextWithShape-boolean-) | Gibt an, ob Text mit der Form rotiert wird. |
| [setRotationAngle(double value)](#setRotationAngle-double-) | Legt die Drehung der Form fest. |
| [setTextHorizontalOverflow(int value)](#setTextHorizontalOverflow-int-) | Legt den horizontalen Überlauftyp des Textes im Textfeld fest. |
| [setTextShapeType(int value)](#setTextShapeType-int-) | Legt den Transformations­typ des Textes fest. |
| [setTextVerticalOverflow(int value)](#setTextVerticalOverflow-int-) | Legt den vertikalen Überlauftyp des Textes im Textfeld fest. |
| [setTextVerticalType(int value)](#setTextVerticalType-int-) | Legt die Textausrichtung fest. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Legt den Typ des umgebrochenen Textes der Form fest, die Text enthält. |
| [setTopMarginPt(double value)](#setTopMarginPt-double-) | Gibt den oberen Rand in Punkten zurück. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Bestimmt, ob diese Instanz denselben Wert wie ein anderes angegebenes [ShapeTextAlignment](../../com.aspose.cells/shapetextalignment)-Objekt hat.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | java.lang.Object | Das [ShapeTextAlignment](../../com.aspose.cells/shapetextalignment)-Objekt zum Vergleich mit dieser Instanz. |

**Returns:**
boolean - true, wenn der Wert des Parameters obj derselbe ist wie der Wert dieser Instanz; andernfalls false. Wenn obj null ist, gibt diese Methode false zurück.
### getAutoSize() {#getAutoSize--}
```
public boolean getAutoSize()
```


Gibt an, ob die Größe der Form automatisch an ihren Inhalt angepasst wird.

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


Gibt den unteren Rand in Punkten zurück.

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


Gibt den linken Rand in Punkten zurück.

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


Ruft die Anzahl der Textspalten im Begrenzungsrechteck ab.

**Returns:**
int
### getRightMarginPt() {#getRightMarginPt--}
```
public double getRightMarginPt()
```


Gibt den rechten Rand in Punkten zurück.

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


Gibt an, ob Text mit der Form rotiert wird.

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


Ermittelt die Drehung der Form.

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


Ruft den horizontalen Überlauftyp des Textes im Textfeld ab.

Siehe [TextOverflowType](../../com.aspose.cells/textoverflowtype).

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


Ruft den Transformationstyp des Textes ab.

Siehe [AutoShapeType](../../com.aspose.cells/autoshapetype).

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


Ruft den vertikalen Überlauftyp des Textes im Textfeld ab.

Siehe [TextOverflowType](../../com.aspose.cells/textoverflowtype).

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


Ruft die Textrichtung ab.

Siehe [TextVerticalType](../../com.aspose.cells/textverticaltype).

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


Gibt den oberen Rand in Punkten zurück.

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


Gibt an, ob der Rand des Textrahmens automatisch ist.

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


Gibt an, ob die Form gesperrt ist, wenn das Arbeitsblatt geschützt ist.

**Remarks**

Funktioniert nur, wenn das Arbeitsblatt geschützt ist.

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


Ermittelt den Textumbruchtyp der Form, die Text enthält.

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


Gibt an, ob der Rand des Textrahmens automatisch ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAutoSize(boolean value) {#setAutoSize-boolean-}
```
public void setAutoSize(boolean value)
```


Gibt an, ob die Größe der Form automatisch an ihren Inhalt angepasst wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setBottomMarginPt(double value) {#setBottomMarginPt-double-}
```
public void setBottomMarginPt(double value)
```


Gibt den unteren Rand in Punkten zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setLeftMarginPt(double value) {#setLeftMarginPt-double-}
```
public void setLeftMarginPt(double value)
```


Gibt den linken Rand in Punkten zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setLockedText(boolean value) {#setLockedText-boolean-}
```
public void setLockedText(boolean value)
```


Gibt an, ob die Form gesperrt ist, wenn das Arbeitsblatt geschützt ist.

**Remarks**

Funktioniert nur, wenn das Arbeitsblatt geschützt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setNumberOfColumns(int value) {#setNumberOfColumns-int-}
```
public void setNumberOfColumns(int value)
```


Legt die Anzahl der Textspalten im Begrenzungsrechteck fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setRightMarginPt(double value) {#setRightMarginPt-double-}
```
public void setRightMarginPt(double value)
```


Gibt den rechten Rand in Punkten zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setRotateTextWithShape(boolean value) {#setRotateTextWithShape-boolean-}
```
public void setRotateTextWithShape(boolean value)
```


Gibt an, ob Text mit der Form rotiert wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setRotationAngle(double value) {#setRotationAngle-double-}
```
public void setRotationAngle(double value)
```


Legt die Drehung der Form fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setTextHorizontalOverflow(int value) {#setTextHorizontalOverflow-int-}
```
public void setTextHorizontalOverflow(int value)
```


Legt den horizontalen Überlauftyp des Textes im Textfeld fest.

Siehe [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setTextShapeType(int value) {#setTextShapeType-int-}
```
public void setTextShapeType(int value)
```


Legt den Transformations­typ des Textes fest.

Siehe [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setTextVerticalOverflow(int value) {#setTextVerticalOverflow-int-}
```
public void setTextVerticalOverflow(int value)
```


Legt den vertikalen Überlauftyp des Textes im Textfeld fest.

Siehe [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setTextVerticalType(int value) {#setTextVerticalType-int-}
```
public void setTextVerticalType(int value)
```


Legt die Textausrichtung fest.

Siehe [TextVerticalType](../../com.aspose.cells/textverticaltype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


Legt den Typ des umgebrochenen Textes der Form fest, die Text enthält.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setTopMarginPt(double value) {#setTopMarginPt-double-}
```
public void setTopMarginPt(double value)
```


Gibt den oberen Rand in Punkten zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

