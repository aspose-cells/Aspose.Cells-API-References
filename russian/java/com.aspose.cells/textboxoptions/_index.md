---
title: "TextBoxOptions"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет параметры текста формы"
type: docs
url: /ru/java/com.aspose.cells/textboxoptions/
---

**Inheritance:**
java.lang.Object
```
public class TextBoxOptions
```

Представляет параметры текста формы

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
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowTextToOverflow()](#getAllowTextToOverflow--) | Разрешать ли текст выходить за пределы фигуры. |
| [getBottomMarginPt()](#getBottomMarginPt--) | Возвращает нижнее поле в единицах Points. |
| [getClass()](#getClass--) |  |
| [getLeftMarginPt()](#getLeftMarginPt--) | Получает левый отступ в единицах Points. |
| [getResizeToFitText()](#getResizeToFitText--) | Указывает, следует ли изменять размер фигуры, чтобы соответствовать тексту |
| [getRightMarginPt()](#getRightMarginPt--) | Получает правый отступ в единицах Points. |
| [getShapeTextDirection()](#getShapeTextDirection--) | Получает направление отображения текста внутри заданного текстового блока. |
| [getShapeTextVerticalAlignment()](#getShapeTextVerticalAlignment--) | It corresponds to "Format Shape - Text Options - Text Box - Vertical Alignment" in Excel. |
| [getTopMarginPt()](#getTopMarginPt--) | Получает верхний отступ в единицах Points. |
| [getWrapTextInShape()](#getWrapTextInShape--) | Указывает перенос текста внутри фигуры. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowTextToOverflow(boolean value)](#setAllowTextToOverflow-boolean-) | Разрешать ли текст выходить за пределы фигуры. |
| [setBottomMarginPt(double value)](#setBottomMarginPt-double-) | Возвращает нижнее поле в единицах Points. |
| [setLeftMarginPt(double value)](#setLeftMarginPt-double-) | Устанавливает левый отступ в единицах Points. |
| [setResizeToFitText(boolean value)](#setResizeToFitText-boolean-) | Указывает, следует ли изменять размер фигуры, чтобы соответствовать тексту |
| [setRightMarginPt(double value)](#setRightMarginPt-double-) | Устанавливает правый отступ в единицах Points. |
| [setShapeTextDirection(int value)](#setShapeTextDirection-int-) | Устанавливает направление отображения текста внутри заданного текстового блока. |
| [setShapeTextVerticalAlignment(int value)](#setShapeTextVerticalAlignment-int-) | It corresponds to "Format Shape - Text Options - Text Box - Vertical Alignment" in Excel. |
| [setTopMarginPt(double value)](#setTopMarginPt-double-) | Устанавливает верхний отступ в единицах Points. |
| [setWrapTextInShape(boolean value)](#setWrapTextInShape-boolean-) | Указывает перенос текста внутри фигуры. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAllowTextToOverflow() {#getAllowTextToOverflow--}
```
public boolean getAllowTextToOverflow()
```


Разрешать ли текст выходить за пределы фигуры.

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


Возвращает нижнее поле в единицах Points.

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


Получает левый отступ в единицах Points.

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


Указывает, следует ли изменять размер фигуры, чтобы соответствовать тексту

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


Получает правый отступ в единицах Points.

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


Получает направление отображения текста внутри заданного текстового блока. It corresponds to "Format Shape - Text Options - Text Box - Text direction" in Excel

См. [TextVerticalType](../../com.aspose.cells/textverticaltype).

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


It corresponds to "Format Shape - Text Options - Text Box - Vertical Alignment" in Excel.

См. [ShapeTextVerticalAlignmentType](../../com.aspose.cells/shapetextverticalalignmenttype).

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


Получает верхний отступ в единицах Points.

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


Указывает перенос текста внутри фигуры. False - Перенос не будет происходить в текстовом блоке. True - Перенос будет происходить в текстовом блоке.

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


Разрешать ли текст выходить за пределы фигуры.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setBottomMarginPt(double value) {#setBottomMarginPt-double-}
```
public void setBottomMarginPt(double value)
```


Возвращает нижнее поле в единицах Points.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setLeftMarginPt(double value) {#setLeftMarginPt-double-}
```
public void setLeftMarginPt(double value)
```


Устанавливает левый отступ в единицах Points.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setResizeToFitText(boolean value) {#setResizeToFitText-boolean-}
```
public void setResizeToFitText(boolean value)
```


Указывает, следует ли изменять размер фигуры, чтобы соответствовать тексту

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setRightMarginPt(double value) {#setRightMarginPt-double-}
```
public void setRightMarginPt(double value)
```


Устанавливает правый отступ в единицах Points.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setShapeTextDirection(int value) {#setShapeTextDirection-int-}
```
public void setShapeTextDirection(int value)
```


Устанавливает направление отображения текста внутри заданного текстового блока. It corresponds to "Format Shape - Text Options - Text Box - Text direction" in Excel

См. [TextVerticalType](../../com.aspose.cells/textverticaltype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setShapeTextVerticalAlignment(int value) {#setShapeTextVerticalAlignment-int-}
```
public void setShapeTextVerticalAlignment(int value)
```


It corresponds to "Format Shape - Text Options - Text Box - Vertical Alignment" in Excel.

См. [ShapeTextVerticalAlignmentType](../../com.aspose.cells/shapetextverticalalignmenttype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setTopMarginPt(double value) {#setTopMarginPt-double-}
```
public void setTopMarginPt(double value)
```


Устанавливает верхний отступ в единицах Points.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setWrapTextInShape(boolean value) {#setWrapTextInShape-boolean-}
```
public void setWrapTextInShape(boolean value)
```


Указывает перенос текста внутри фигуры. False - Перенос не будет происходить в текстовом блоке. True - Перенос будет происходить в текстовом блоке.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

