---
title: "TextBoxOptions"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Textoptionen der Form dar"
type: docs
url: /de/java/com.aspose.cells/textboxoptions/
---

**Inheritance:**
java.lang.Object
```
public class TextBoxOptions
```

Stellt die Textoptionen der Form dar

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
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowTextToOverflow()](#getAllowTextToOverflow--) | Ob Text das Shape überlaufen darf. |
| [getBottomMarginPt()](#getBottomMarginPt--) | Gibt den unteren Rand in Punkten zurück. |
| [getClass()](#getClass--) |  |
| [getLeftMarginPt()](#getLeftMarginPt--) | Liefert den linken Rand in Einheit von Punkten. |
| [getResizeToFitText()](#getResizeToFitText--) | Gibt an, ob die Form an den Text angepasst werden soll. |
| [getRightMarginPt()](#getRightMarginPt--) | Liefert den rechten Rand in Einheit von Punkten. |
| [getShapeTextDirection()](#getShapeTextDirection--) | Liefert die Textanzeigerichtung innerhalb eines gegebenen Textkörpers. |
| [getShapeTextVerticalAlignment()](#getShapeTextVerticalAlignment--) | Sie entspricht "Format Shape - Text Options - Text Box - Vertical Alignment" in Excel. |
| [getTopMarginPt()](#getTopMarginPt--) | Liefert den oberen Rand in Einheit von Punkten. |
| [getWrapTextInShape()](#getWrapTextInShape--) | Gibt die Textumbruch innerhalb einer Form an. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowTextToOverflow(boolean value)](#setAllowTextToOverflow-boolean-) | Ob Text das Shape überlaufen darf. |
| [setBottomMarginPt(double value)](#setBottomMarginPt-double-) | Gibt den unteren Rand in Punkten zurück. |
| [setLeftMarginPt(double value)](#setLeftMarginPt-double-) | Setzt den linken Rand in Einheit von Punkten. |
| [setResizeToFitText(boolean value)](#setResizeToFitText-boolean-) | Gibt an, ob die Form an den Text angepasst werden soll. |
| [setRightMarginPt(double value)](#setRightMarginPt-double-) | Setzt den rechten Rand in Einheit von Punkten. |
| [setShapeTextDirection(int value)](#setShapeTextDirection-int-) | Setzt die Textanzeigerichtung innerhalb eines gegebenen Textkörpers. |
| [setShapeTextVerticalAlignment(int value)](#setShapeTextVerticalAlignment-int-) | Sie entspricht "Format Shape - Text Options - Text Box - Vertical Alignment" in Excel. |
| [setTopMarginPt(double value)](#setTopMarginPt-double-) | Setzt den oberen Rand in Einheit von Punkten. |
| [setWrapTextInShape(boolean value)](#setWrapTextInShape-boolean-) | Gibt die Textumbruch innerhalb einer Form an. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAllowTextToOverflow() {#getAllowTextToOverflow--}
```
public boolean getAllowTextToOverflow()
```


Ob Text das Shape überlaufen darf.

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


Gibt den unteren Rand in Punkten zurück.

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


Liefert den linken Rand in Einheit von Punkten.

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


Gibt an, ob die Form an den Text angepasst werden soll.

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


Liefert den rechten Rand in Einheit von Punkten.

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


Liefert die Textanzeigerichtung innerhalb eines gegebenen Textkörpers. Sie entspricht "Format Shape - Text Options - Text Box - Text direction" in Excel

Siehe [TextVerticalType](../../com.aspose.cells/textverticaltype).

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


Sie entspricht "Format Shape - Text Options - Text Box - Vertical Alignment" in Excel.

Siehe [ShapeTextVerticalAlignmentType](../../com.aspose.cells/shapetextverticalalignmenttype).

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


Liefert den oberen Rand in Einheit von Punkten.

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


Gibt die Textumbruch innerhalb einer Form an. False - Kein Umbruch erfolgt im Textkörper. True - Umbruch erfolgt im Textkörper.

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


Ob Text das Shape überlaufen darf.

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


Setzt den linken Rand in Einheit von Punkten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setResizeToFitText(boolean value) {#setResizeToFitText-boolean-}
```
public void setResizeToFitText(boolean value)
```


Gibt an, ob die Form an den Text angepasst werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setRightMarginPt(double value) {#setRightMarginPt-double-}
```
public void setRightMarginPt(double value)
```


Setzt den rechten Rand in Einheit von Punkten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setShapeTextDirection(int value) {#setShapeTextDirection-int-}
```
public void setShapeTextDirection(int value)
```


Setzt die Textanzeigerichtung innerhalb eines gegebenen Textkörpers. Sie entspricht "Format Shape - Text Options - Text Box - Text direction" in Excel

Siehe [TextVerticalType](../../com.aspose.cells/textverticaltype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setShapeTextVerticalAlignment(int value) {#setShapeTextVerticalAlignment-int-}
```
public void setShapeTextVerticalAlignment(int value)
```


Sie entspricht "Format Shape - Text Options - Text Box - Vertical Alignment" in Excel.

Siehe [ShapeTextVerticalAlignmentType](../../com.aspose.cells/shapetextverticalalignmenttype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setTopMarginPt(double value) {#setTopMarginPt-double-}
```
public void setTopMarginPt(double value)
```


Setzt den oberen Rand in Einheit von Punkten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setWrapTextInShape(boolean value) {#setWrapTextInShape-boolean-}
```
public void setWrapTextInShape(boolean value)
```


Gibt die Textumbruch innerhalb einer Form an. False - Kein Umbruch erfolgt im Textkörper. True - Umbruch erfolgt im Textkörper.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

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

