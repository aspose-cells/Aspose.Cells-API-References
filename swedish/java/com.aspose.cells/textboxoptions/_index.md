---
title: "TextBoxOptions"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar textalternativen för formen"
type: docs
url: /sv/java/com.aspose.cells/textboxoptions/
---

**Inheritance:**
java.lang.Object
```
public class TextBoxOptions
```

Representerar textalternativen för formen

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
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowTextToOverflow()](#getAllowTextToOverflow--) | Om text får flöda över formen. |
| [getBottomMarginPt()](#getBottomMarginPt--) | Returnerar den nedre marginalen i enheten Points. |
| [getClass()](#getClass--) |  |
| [getLeftMarginPt()](#getLeftMarginPt--) | Hämtar vänster marginal i enheten punkter. |
| [getResizeToFitText()](#getResizeToFitText--) | Anger om formen ska ändras storlek för att passa texten |
| [getRightMarginPt()](#getRightMarginPt--) | Hämtar höger marginal i enheten punkter. |
| [getShapeTextDirection()](#getShapeTextDirection--) | Hämtar textriktning inom en given textkropp. |
| [getShapeTextVerticalAlignment()](#getShapeTextVerticalAlignment--) | Den motsvarar "Format Shape - Text Options - Text Box - Vertical Alignment" i Excel. |
| [getTopMarginPt()](#getTopMarginPt--) | Hämtar överkantsmarginal i enheten punkter. |
| [getWrapTextInShape()](#getWrapTextInShape--) | Anger radbrytning av text inom en form. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowTextToOverflow(boolean value)](#setAllowTextToOverflow-boolean-) | Om text får flöda över formen. |
| [setBottomMarginPt(double value)](#setBottomMarginPt-double-) | Returnerar den nedre marginalen i enheten Points. |
| [setLeftMarginPt(double value)](#setLeftMarginPt-double-) | Ställer in vänster marginal i enheten punkter. |
| [setResizeToFitText(boolean value)](#setResizeToFitText-boolean-) | Anger om formen ska ändras storlek för att passa texten |
| [setRightMarginPt(double value)](#setRightMarginPt-double-) | Ställer in höger marginal i enheten punkter. |
| [setShapeTextDirection(int value)](#setShapeTextDirection-int-) | Ställer in textriktning inom en given textkropp. |
| [setShapeTextVerticalAlignment(int value)](#setShapeTextVerticalAlignment-int-) | Den motsvarar "Format Shape - Text Options - Text Box - Vertical Alignment" i Excel. |
| [setTopMarginPt(double value)](#setTopMarginPt-double-) | Ställer in överkantsmarginal i enheten punkter. |
| [setWrapTextInShape(boolean value)](#setWrapTextInShape-boolean-) | Anger radbrytning av text inom en form. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAllowTextToOverflow() {#getAllowTextToOverflow--}
```
public boolean getAllowTextToOverflow()
```


Om text får flöda över formen.

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


Returnerar den nedre marginalen i enheten Points.

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


Hämtar vänster marginal i enheten punkter.

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


Anger om formen ska ändras storlek för att passa texten

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


Hämtar höger marginal i enheten punkter.

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


Hämtar textriktning inom en given textkropp. Det motsvarar "Format Shape - Text Options - Text Box - Text direction" i Excel

Se [TextVerticalType](../../com.aspose.cells/textverticaltype).

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


Den motsvarar "Format Shape - Text Options - Text Box - Vertical Alignment" i Excel.

Se [ShapeTextVerticalAlignmentType](../../com.aspose.cells/shapetextverticalalignmenttype).

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


Hämtar överkantsmarginal i enheten punkter.

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


Anger radbrytning av text inom en form. Falskt - Ingen radbrytning kommer att ske i textkroppen. Sant - Radbrytning kommer att ske i textkroppen.

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


Om text får flöda över formen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setBottomMarginPt(double value) {#setBottomMarginPt-double-}
```
public void setBottomMarginPt(double value)
```


Returnerar den nedre marginalen i enheten Points.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setLeftMarginPt(double value) {#setLeftMarginPt-double-}
```
public void setLeftMarginPt(double value)
```


Ställer in vänster marginal i enheten punkter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setResizeToFitText(boolean value) {#setResizeToFitText-boolean-}
```
public void setResizeToFitText(boolean value)
```


Anger om formen ska ändras storlek för att passa texten

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setRightMarginPt(double value) {#setRightMarginPt-double-}
```
public void setRightMarginPt(double value)
```


Ställer in höger marginal i enheten punkter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setShapeTextDirection(int value) {#setShapeTextDirection-int-}
```
public void setShapeTextDirection(int value)
```


Ställer in textriktning inom en given textkropp. Det motsvarar "Format Shape - Text Options - Text Box - Text direction" i Excel

Se [TextVerticalType](../../com.aspose.cells/textverticaltype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setShapeTextVerticalAlignment(int value) {#setShapeTextVerticalAlignment-int-}
```
public void setShapeTextVerticalAlignment(int value)
```


Den motsvarar "Format Shape - Text Options - Text Box - Vertical Alignment" i Excel.

Se [ShapeTextVerticalAlignmentType](../../com.aspose.cells/shapetextverticalalignmenttype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setTopMarginPt(double value) {#setTopMarginPt-double-}
```
public void setTopMarginPt(double value)
```


Ställer in överkantsmarginal i enheten punkter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setWrapTextInShape(boolean value) {#setWrapTextInShape-boolean-}
```
public void setWrapTextInShape(boolean value)
```


Anger radbrytning av text inom en form. Falskt - Ingen radbrytning kommer att ske i textkroppen. Sant - Radbrytning kommer att ske i textkroppen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

