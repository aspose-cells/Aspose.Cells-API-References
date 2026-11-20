---
title: "ShapeTextAlignment"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет настройку выравнивания текста фигур"
type: docs
url: /ru/java/com.aspose.cells/shapetextalignment/
---

**Inheritance:**
java.lang.Object
```
public class ShapeTextAlignment
```

Представляет настройку выравнивания текста формы;

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Shape shape = workbook.getWorksheets().get(0).getShapes().addRectangle(1, 0, 1, 0, 50, 100);
         ShapeTextAlignment shapeTextAlignment = shape.getTextBody().getTextAlignment();
 
         //do your business
```
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | Определяет, имеет ли данный экземпляр то же значение, что и другой указанный объект [ShapeTextAlignment](../../com.aspose.cells/shapetextalignment). |
| [getAutoSize()](#getAutoSize--) | Указывает, автоматически ли размер фигуры корректируется в соответствии с её содержимым. |
| [getBottomMarginPt()](#getBottomMarginPt--) | Возвращает нижнее поле в единицах Points. |
| [getClass()](#getClass--) |  |
| [getLeftMarginPt()](#getLeftMarginPt--) | Возвращает левое поле в единицах Points. |
| [getNumberOfColumns()](#getNumberOfColumns--) | Получает количество колонок текста в ограничивающем прямоугольнике. |
| [getRightMarginPt()](#getRightMarginPt--) | Возвращает правое поле в единицах Points. |
| [getRotateTextWithShape()](#getRotateTextWithShape--) | Указывает, вращается ли текст вместе с фигурой. |
| [getRotationAngle()](#getRotationAngle--) | Получает вращение фигуры. |
| [getTextHorizontalOverflow()](#getTextHorizontalOverflow--) | Получает тип горизонтального переполнения текста в текстовом поле. |
| [getTextShapeType()](#getTextShapeType--) | Получает тип трансформации текста. |
| [getTextVerticalOverflow()](#getTextVerticalOverflow--) | Получает тип вертикального переполнения текста в текстовом поле. |
| [getTextVerticalType()](#getTextVerticalType--) | Получает направление текста. |
| [getTopMarginPt()](#getTopMarginPt--) | Возвращает верхнее поле в единицах Points. |
| [hashCode()](#hashCode--) |  |
| [isAutoMargin()](#isAutoMargin--) | Указывает, является ли отступ текстовой рамки автоматическим. |
| [isLockedText()](#isLockedText--) | Указывает, заблокирована ли фигура, когда лист защищён. |
| [isTextWrapped()](#isTextWrapped--) | Получает тип переноса текста у объекта, содержащего текст. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoMargin(boolean value)](#setAutoMargin-boolean-) | Указывает, является ли отступ текстовой рамки автоматическим. |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Указывает, автоматически ли размер фигуры корректируется в соответствии с её содержимым. |
| [setBottomMarginPt(double value)](#setBottomMarginPt-double-) | Возвращает нижнее поле в единицах Points. |
| [setLeftMarginPt(double value)](#setLeftMarginPt-double-) | Возвращает левое поле в единицах Points. |
| [setLockedText(boolean value)](#setLockedText-boolean-) | Указывает, заблокирована ли фигура, когда лист защищён. |
| [setNumberOfColumns(int value)](#setNumberOfColumns-int-) | Устанавливает количество колонок текста в ограничивающем прямоугольнике. |
| [setRightMarginPt(double value)](#setRightMarginPt-double-) | Возвращает правое поле в единицах Points. |
| [setRotateTextWithShape(boolean value)](#setRotateTextWithShape-boolean-) | Указывает, вращается ли текст вместе с фигурой. |
| [setRotationAngle(double value)](#setRotationAngle-double-) | Устанавливает вращение объекта. |
| [setTextHorizontalOverflow(int value)](#setTextHorizontalOverflow-int-) | Устанавливает тип горизонтального переполнения текста в текстовом поле. |
| [setTextShapeType(int value)](#setTextShapeType-int-) | Устанавливает тип трансформации текста. |
| [setTextVerticalOverflow(int value)](#setTextVerticalOverflow-int-) | Устанавливает тип вертикального переполнения текста в текстовом поле. |
| [setTextVerticalType(int value)](#setTextVerticalType-int-) | Устанавливает направление текста. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Устанавливает тип переноса текста в фигуре, содержащей текст. |
| [setTopMarginPt(double value)](#setTopMarginPt-double-) | Возвращает верхнее поле в единицах Points. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Определяет, имеет ли данный экземпляр то же значение, что и другой указанный объект [ShapeTextAlignment](../../com.aspose.cells/shapetextalignment).

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | java.lang.Object | Объект [ShapeTextAlignment](../../com.aspose.cells/shapetextalignment) для сравнения с этим экземпляром. |

**Returns:**
boolean — true, если значение параметра obj совпадает со значением этого экземпляра; иначе — false. Если obj равен null, этот метод возвращает false.
### getAutoSize() {#getAutoSize--}
```
public boolean getAutoSize()
```


Указывает, автоматически ли размер фигуры корректируется в соответствии с её содержимым.

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


Возвращает нижнее поле в единицах Points.

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


Возвращает левое поле в единицах Points.

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


Получает количество колонок текста в ограничивающем прямоугольнике.

**Returns:**
int
### getRightMarginPt() {#getRightMarginPt--}
```
public double getRightMarginPt()
```


Возвращает правое поле в единицах Points.

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


Указывает, вращается ли текст вместе с фигурой.

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


Получает вращение фигуры.

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


Получает тип горизонтального переполнения текста в текстовом поле.

См. [TextOverflowType](../../com.aspose.cells/textoverflowtype).

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


Получает тип трансформации текста.

См. [AutoShapeType](../../com.aspose.cells/autoshapetype).

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


Получает тип вертикального переполнения текста в текстовом поле.

См. [TextOverflowType](../../com.aspose.cells/textoverflowtype).

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


Получает направление текста.

См. [TextVerticalType](../../com.aspose.cells/textverticaltype).

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


Возвращает верхнее поле в единицах Points.

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


Указывает, является ли отступ текстовой рамки автоматическим.

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


Указывает, заблокирована ли фигура, когда лист защищён.

**Remarks**

Работает только когда лист защищён.

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


Получает тип переноса текста у объекта, содержащего текст.

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


Указывает, является ли отступ текстовой рамки автоматическим.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAutoSize(boolean value) {#setAutoSize-boolean-}
```
public void setAutoSize(boolean value)
```


Указывает, автоматически ли размер фигуры корректируется в соответствии с её содержимым.

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


Возвращает левое поле в единицах Points.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setLockedText(boolean value) {#setLockedText-boolean-}
```
public void setLockedText(boolean value)
```


Указывает, заблокирована ли фигура, когда лист защищён.

**Remarks**

Работает только когда лист защищён.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setNumberOfColumns(int value) {#setNumberOfColumns-int-}
```
public void setNumberOfColumns(int value)
```


Устанавливает количество колонок текста в ограничивающем прямоугольнике.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setRightMarginPt(double value) {#setRightMarginPt-double-}
```
public void setRightMarginPt(double value)
```


Возвращает правое поле в единицах Points.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setRotateTextWithShape(boolean value) {#setRotateTextWithShape-boolean-}
```
public void setRotateTextWithShape(boolean value)
```


Указывает, вращается ли текст вместе с фигурой.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setRotationAngle(double value) {#setRotationAngle-double-}
```
public void setRotationAngle(double value)
```


Устанавливает вращение объекта.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setTextHorizontalOverflow(int value) {#setTextHorizontalOverflow-int-}
```
public void setTextHorizontalOverflow(int value)
```


Устанавливает тип горизонтального переполнения текста в текстовом поле.

См. [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setTextShapeType(int value) {#setTextShapeType-int-}
```
public void setTextShapeType(int value)
```


Устанавливает тип трансформации текста.

См. [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setTextVerticalOverflow(int value) {#setTextVerticalOverflow-int-}
```
public void setTextVerticalOverflow(int value)
```


Устанавливает тип вертикального переполнения текста в текстовом поле.

См. [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setTextVerticalType(int value) {#setTextVerticalType-int-}
```
public void setTextVerticalType(int value)
```


Устанавливает направление текста.

См. [TextVerticalType](../../com.aspose.cells/textverticaltype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


Устанавливает тип переноса текста в фигуре, содержащей текст.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setTopMarginPt(double value) {#setTopMarginPt-double-}
```
public void setTopMarginPt(double value)
```


Возвращает верхнее поле в единицах Points.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

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

