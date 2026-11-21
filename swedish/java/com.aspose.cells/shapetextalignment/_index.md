---
title: "ShapeTextAlignment"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar inställningen för formers textjustering"
type: docs
url: /sv/java/com.aspose.cells/shapetextalignment/
---

**Inheritance:**
java.lang.Object
```
public class ShapeTextAlignment
```

Representerar inställningen för formens textjustering;

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Shape shape = workbook.getWorksheets().get(0).getShapes().addRectangle(1, 0, 1, 0, 50, 100);
         ShapeTextAlignment shapeTextAlignment = shape.getTextBody().getTextAlignment();
 
         //do your business
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | Bestämmer om detta objekt har samma värde som ett annat specificerat [ShapeTextAlignment](../../com.aspose.cells/shapetextalignment)-objekt. |
| [getAutoSize()](#getAutoSize--) | Indikerar om storleken på formen justeras automatiskt enligt dess innehåll. |
| [getBottomMarginPt()](#getBottomMarginPt--) | Returnerar den nedre marginalen i enheten Points. |
| [getClass()](#getClass--) |  |
| [getLeftMarginPt()](#getLeftMarginPt--) | Returnerar den vänstra marginalen i enheten Points. |
| [getNumberOfColumns()](#getNumberOfColumns--) | Hämtar antalet textkolumner i den omgivande rektangeln. |
| [getRightMarginPt()](#getRightMarginPt--) | Returnerar den högra marginalen i enheten Points. |
| [getRotateTextWithShape()](#getRotateTextWithShape--) | Indikerar om text roteras med formen. |
| [getRotationAngle()](#getRotationAngle--) | Hämtar rotationen av formen. |
| [getTextHorizontalOverflow()](#getTextHorizontalOverflow--) | Hämtar den horisontella översvämningstypen för texten i textrutan. |
| [getTextShapeType()](#getTextShapeType--) | Hämtar transformeringstypen för texten. |
| [getTextVerticalOverflow()](#getTextVerticalOverflow--) | Hämtar den vertikala översvämningstypen för texten i textrutan. |
| [getTextVerticalType()](#getTextVerticalType--) | Hämtar textens riktning. |
| [getTopMarginPt()](#getTopMarginPt--) | Returnerar den övre marginalen i enheten Points. |
| [hashCode()](#hashCode--) |  |
| [isAutoMargin()](#isAutoMargin--) | Anger om marginalen för textramen är automatisk. |
| [isLockedText()](#isLockedText--) | Anger om formen är låst när kalkylbladet är skyddat. |
| [isTextWrapped()](#isTextWrapped--) | Hämtar den typ av textomslag för formen som innehåller text. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoMargin(boolean value)](#setAutoMargin-boolean-) | Anger om marginalen för textramen är automatisk. |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Indikerar om storleken på formen justeras automatiskt enligt dess innehåll. |
| [setBottomMarginPt(double value)](#setBottomMarginPt-double-) | Returnerar den nedre marginalen i enheten Points. |
| [setLeftMarginPt(double value)](#setLeftMarginPt-double-) | Returnerar den vänstra marginalen i enheten Points. |
| [setLockedText(boolean value)](#setLockedText-boolean-) | Anger om formen är låst när kalkylbladet är skyddat. |
| [setNumberOfColumns(int value)](#setNumberOfColumns-int-) | Ställer in antalet textkolumner i den omgivande rektangeln. |
| [setRightMarginPt(double value)](#setRightMarginPt-double-) | Returnerar den högra marginalen i enheten Points. |
| [setRotateTextWithShape(boolean value)](#setRotateTextWithShape-boolean-) | Indikerar om text roteras med formen. |
| [setRotationAngle(double value)](#setRotationAngle-double-) | Ställer in rotationen av formen. |
| [setTextHorizontalOverflow(int value)](#setTextHorizontalOverflow-int-) | Ställer in den horisontella översvämningstypen för texten i textrutan. |
| [setTextShapeType(int value)](#setTextShapeType-int-) | Ställer in transformeringstypen för texten. |
| [setTextVerticalOverflow(int value)](#setTextVerticalOverflow-int-) | Ställer in den vertikala översvämningstypen för texten i textrutan. |
| [setTextVerticalType(int value)](#setTextVerticalType-int-) | Ställer in textens riktning. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Ställer in typen av textbrytning för formen som innehåller text. |
| [setTopMarginPt(double value)](#setTopMarginPt-double-) | Returnerar den övre marginalen i enheten Points. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Bestämmer om detta objekt har samma värde som ett annat specificerat [ShapeTextAlignment](../../com.aspose.cells/shapetextalignment)-objekt.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | java.lang.Object | Det [ShapeTextAlignment](../../com.aspose.cells/shapetextalignment)-objektet att jämföra med detta objekt. |

**Returns:**
boolean - sant om värdet på parametern obj är samma som värdet på detta objekt; annars falskt. Om obj är null returnerar denna metod falskt.
### getAutoSize() {#getAutoSize--}
```
public boolean getAutoSize()
```


Indikerar om storleken på formen justeras automatiskt enligt dess innehåll.

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


Returnerar den nedre marginalen i enheten Points.

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


Returnerar den vänstra marginalen i enheten Points.

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


Hämtar antalet textkolumner i den omgivande rektangeln.

**Returns:**
int
### getRightMarginPt() {#getRightMarginPt--}
```
public double getRightMarginPt()
```


Returnerar den högra marginalen i enheten Points.

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


Indikerar om text roteras med formen.

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


Hämtar rotationen av formen.

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


Hämtar den horisontella översvämningstypen för texten i textrutan.

Se [TextOverflowType](../../com.aspose.cells/textoverflowtype).

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


Hämtar transformeringstypen för texten.

Se [AutoShapeType](../../com.aspose.cells/autoshapetype).

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


Hämtar den vertikala översvämningstypen för texten i textrutan.

Se [TextOverflowType](../../com.aspose.cells/textoverflowtype).

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


Hämtar textens riktning.

Se [TextVerticalType](../../com.aspose.cells/textverticaltype).

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


Returnerar den övre marginalen i enheten Points.

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


Anger om marginalen för textramen är automatisk.

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


Anger om formen är låst när kalkylbladet är skyddat.

**Remarks**

Fungerar endast när kalkylbladet är skyddat.

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


Hämtar den typ av textomslag för formen som innehåller text.

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


Anger om marginalen för textramen är automatisk.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAutoSize(boolean value) {#setAutoSize-boolean-}
```
public void setAutoSize(boolean value)
```


Indikerar om storleken på formen justeras automatiskt enligt dess innehåll.

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


Returnerar den vänstra marginalen i enheten Points.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setLockedText(boolean value) {#setLockedText-boolean-}
```
public void setLockedText(boolean value)
```


Anger om formen är låst när kalkylbladet är skyddat.

**Remarks**

Fungerar endast när kalkylbladet är skyddat.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setNumberOfColumns(int value) {#setNumberOfColumns-int-}
```
public void setNumberOfColumns(int value)
```


Ställer in antalet textkolumner i den omgivande rektangeln.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setRightMarginPt(double value) {#setRightMarginPt-double-}
```
public void setRightMarginPt(double value)
```


Returnerar den högra marginalen i enheten Points.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setRotateTextWithShape(boolean value) {#setRotateTextWithShape-boolean-}
```
public void setRotateTextWithShape(boolean value)
```


Indikerar om text roteras med formen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setRotationAngle(double value) {#setRotationAngle-double-}
```
public void setRotationAngle(double value)
```


Ställer in rotationen av formen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setTextHorizontalOverflow(int value) {#setTextHorizontalOverflow-int-}
```
public void setTextHorizontalOverflow(int value)
```


Ställer in den horisontella översvämningstypen för texten i textrutan.

Se [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setTextShapeType(int value) {#setTextShapeType-int-}
```
public void setTextShapeType(int value)
```


Ställer in transformeringstypen för texten.

Se [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setTextVerticalOverflow(int value) {#setTextVerticalOverflow-int-}
```
public void setTextVerticalOverflow(int value)
```


Ställer in den vertikala översvämningstypen för texten i textrutan.

Se [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setTextVerticalType(int value) {#setTextVerticalType-int-}
```
public void setTextVerticalType(int value)
```


Ställer in textens riktning.

Se [TextVerticalType](../../com.aspose.cells/textverticaltype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


Ställer in typen av textbrytning för formen som innehåller text.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setTopMarginPt(double value) {#setTopMarginPt-double-}
```
public void setTopMarginPt(double value)
```


Returnerar den övre marginalen i enheten Points.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

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

