---
title: "Линия"
second_title: "Справочник API Aspose.Cells for Java"
description: "Инкапсулирует объект, представляющий формат линии."
type: docs
url: /ru/java/com.aspose.cells/line/
---

**Inheritance:**
java.lang.Object
```
public class Line
```

Инкапсулирует объект, представляющий формат линии.

**Example**

```
         Workbook workbook = new Workbook();
         	Worksheet sheet = workbook.getWorksheets().get(0);
 
         	Cells cells = sheet.getCells();
         	cells.get(0,1).putValue("Income");
         	cells.get(1,0).putValue("Company A");
         	cells.get(2,0).putValue("Company B");
         	cells.get(3,0).putValue("Company C");
         	cells.get(1,1).putValue(10000);
         	cells.get(2,1).putValue(20000);
         	cells.get(3,1).putValue(30000);
 
         	int chartIndex = sheet.getCharts().add(ChartType.LINE, 9, 9, 21, 15);
         Chart chart = sheet.getCharts().get(chartIndex);
         //Add series
         chart.getNSeries().add("A2:B4", true);
         //Set category data
         chart.getNSeries().setCategoryData("=Sheet1!$A$2:$A$4");
         //Applying a dotted line style on the lines of an NSeries
         chart.getNSeries().get(0).getBorder().setStyle(LineType.DOT);
         chart.getNSeries().get(0).getBorder().setColor(Color.getRed());
         //Applying a triangular marker style on the data markers of an NSeries
         chart.getNSeries().get(0).getMarker().setMarkerStyle(ChartMarkerType.TRIANGLE);
         //Setting the weight of all lines in an NSeries to medium
         chart.getNSeries().get(0).getBorder().setWeight(WeightType.MEDIUM_LINE);
```
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBeginArrowLength()](#getBeginArrowLength--) | Указывает длину наконечника стрелки для начала линии. |
| [getBeginArrowWidth()](#getBeginArrowWidth--) | Указывает ширину наконечника стрелки для начала линии. |
| [getBeginType()](#getBeginType--) | Указывает наконечник стрелки для начала линии. |
| [getCapType()](#getCapType--) | Указывает конечные заглушки. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Представляет [Color](../../com.aspose.cells/color) линии. |
| [getCompoundType()](#getCompoundType--) | Указывает составной тип линии |
| [getDashType()](#getDashType--) | Указывает тип пунктирной линии |
| [getEndArrowLength()](#getEndArrowLength--) | Указывает длину наконечника стрелки для конца линии. |
| [getEndArrowWidth()](#getEndArrowWidth--) | Указывает ширину наконечника стрелки для конца линии. |
| [getEndType()](#getEndType--) | Указывает тип наконечника стрелки для конца линии. |
| [getFormattingType()](#getFormattingType--) | Получает тип формата. |
| [getGradientFill()](#getGradientFill--) | Представляет градиентную заливку. |
| [getJoinType()](#getJoinType--) | Указывает соединительные заглушки. |
| [getStyle()](#getStyle--) | Представляет стиль линии. |
| [getThemeColor()](#getThemeColor--) | Получает цвет темы. |
| [getTransparency()](#getTransparency--) | Возвращает или задает степень прозрачности линии значением от 0,0 (непрозрачный) до 1,0 (прозрачный). |
| [getWeight()](#getWeight--) | Получает [WeightType](../../com.aspose.cells/weighttype) линии. |
| [getWeightPt()](#getWeightPt--) | Получает толщину линии в единицах пунктов. |
| [getWeightPx()](#getWeightPx--) | Получает толщину линии в пикселях. |
| [hashCode()](#hashCode--) |  |
| [isAuto()](#isAuto--) | Указывает, автоматически ли назначен этот стиль линии. |
| [isAutomaticColor()](#isAutomaticColor--) | Указывает, автоматически ли назначен цвет линии. |
| [isVisible()](#isVisible--) | Отображает, видима ли линия. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuto(boolean value)](#setAuto-boolean-) | Указывает, автоматически ли назначен этот стиль линии. |
| [setBeginArrowLength(int value)](#setBeginArrowLength-int-) | Указывает длину наконечника стрелки для начала линии. |
| [setBeginArrowWidth(int value)](#setBeginArrowWidth-int-) | Указывает ширину наконечника стрелки для начала линии. |
| [setBeginType(int value)](#setBeginType-int-) | Указывает наконечник стрелки для начала линии. |
| [setCapType(int value)](#setCapType-int-) | Указывает конечные заглушки. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Представляет [Color](../../com.aspose.cells/color) линии. |
| [setCompoundType(int value)](#setCompoundType-int-) | Указывает составной тип линии |
| [setDashType(int value)](#setDashType-int-) | Указывает тип пунктирной линии |
| [setEndArrowLength(int value)](#setEndArrowLength-int-) | Указывает длину наконечника стрелки для конца линии. |
| [setEndArrowWidth(int value)](#setEndArrowWidth-int-) | Указывает ширину наконечника стрелки для конца линии. |
| [setEndType(int value)](#setEndType-int-) | Указывает тип наконечника стрелки для конца линии. |
| [setFormattingType(int value)](#setFormattingType-int-) | Устанавливает тип формата. |
| [setJoinType(int value)](#setJoinType-int-) | Указывает соединительные заглушки. |
| [setStyle(int value)](#setStyle-int-) | Представляет стиль линии. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Устанавливает цвет темы. |
| [setTransparency(double value)](#setTransparency-double-) | Возвращает или задает степень прозрачности линии значением от 0,0 (непрозрачный) до 1,0 (прозрачный). |
| [setVisible(boolean value)](#setVisible-boolean-) | Отображает, видима ли линия. |
| [setWeight(int value)](#setWeight-int-) | Устанавливает [WeightType](../../com.aspose.cells/weighttype) линии. |
| [setWeightPt(double value)](#setWeightPt-double-) | Устанавливает толщину линии в пунктах. |
| [setWeightPx(double value)](#setWeightPx-double-) | Устанавливает толщину линии в пикселях. |
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
### getBeginArrowLength() {#getBeginArrowLength--}
```
public int getBeginArrowLength()
```


Указывает длину наконечника стрелки для начала линии.

См. [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Returns:**
int
### getBeginArrowWidth() {#getBeginArrowWidth--}
```
public int getBeginArrowWidth()
```


Указывает ширину наконечника стрелки для начала линии.

См. [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Returns:**
int
### getBeginType() {#getBeginType--}
```
public int getBeginType()
```


Указывает наконечник стрелки для начала линии.

См. [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Returns:**
int
### getCapType() {#getCapType--}
```
public int getCapType()
```


Указывает конечные заглушки.

См. [LineCapType](../../com.aspose.cells/linecaptype).

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


Представляет [Color](../../com.aspose.cells/color) линии.

**Returns:**
[Color](../../com.aspose.cells/color)
### getCompoundType() {#getCompoundType--}
```
public int getCompoundType()
```


Указывает составной тип линии

См. [MsoLineStyle](../../com.aspose.cells/msolinestyle).

**Returns:**
int
### getDashType() {#getDashType--}
```
public int getDashType()
```


Указывает тип пунктирной линии

См. [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle).

**Returns:**
int
### getEndArrowLength() {#getEndArrowLength--}
```
public int getEndArrowLength()
```


Указывает длину наконечника стрелки для конца линии.

См. [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Returns:**
int
### getEndArrowWidth() {#getEndArrowWidth--}
```
public int getEndArrowWidth()
```


Указывает ширину наконечника стрелки для конца линии.

См. [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Returns:**
int
### getEndType() {#getEndType--}
```
public int getEndType()
```


Указывает тип наконечника стрелки для конца линии.

См. [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Returns:**
int
### getFormattingType() {#getFormattingType--}
```
public int getFormattingType()
```


Получает тип формата.

См. [ChartLineFormattingType](../../com.aspose.cells/chartlineformattingtype).

**Returns:**
int
### getGradientFill() {#getGradientFill--}
```
public GradientFill getGradientFill()
```


Представляет градиентную заливку.

**Returns:**
[GradientFill](../../com.aspose.cells/gradientfill)
### getJoinType() {#getJoinType--}
```
public int getJoinType()
```


Указывает соединительные заглушки.

См. [LineJoinType](../../com.aspose.cells/linejointype).

**Returns:**
int
### getStyle() {#getStyle--}
```
public int getStyle()
```


Представляет стиль линии.

Смотрите [LineType](../../com.aspose.cells/linetype).

**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```


Получает цвет темы.

**Remarks**

Если цвет переднего плана не является цветом темы, будет возвращено NULL.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


Возвращает или задает степень прозрачности линии значением от 0,0 (непрозрачный) до 1,0 (прозрачный).

**Returns:**
double
### getWeight() {#getWeight--}
```
public int getWeight()
```


Получает [WeightType](../../com.aspose.cells/weighttype) линии.

Смотрите [WeightType](../../com.aspose.cells/weighttype).

**Returns:**
int
### getWeightPt() {#getWeightPt--}
```
public double getWeightPt()
```


Получает толщину линии в единицах пунктов.

**Returns:**
double
### getWeightPx() {#getWeightPx--}
```
public double getWeightPx()
```


Получает толщину линии в пикселях.

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAuto() {#isAuto--}
```
public boolean isAuto()
```


Указывает, автоматически ли назначен этот стиль линии.

**Returns:**
boolean
### isAutomaticColor() {#isAutomaticColor--}
```
public boolean isAutomaticColor()
```


Указывает, автоматически ли назначен цвет линии.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Отображает, видима ли линия.

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




### setAuto(boolean value) {#setAuto-boolean-}
```
public void setAuto(boolean value)
```


Указывает, автоматически ли назначен этот стиль линии.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setBeginArrowLength(int value) {#setBeginArrowLength-int-}
```
public void setBeginArrowLength(int value)
```


Указывает длину наконечника стрелки для начала линии.

См. [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setBeginArrowWidth(int value) {#setBeginArrowWidth-int-}
```
public void setBeginArrowWidth(int value)
```


Указывает ширину наконечника стрелки для начала линии.

См. [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setBeginType(int value) {#setBeginType-int-}
```
public void setBeginType(int value)
```


Указывает наконечник стрелки для начала линии.

См. [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setCapType(int value) {#setCapType-int-}
```
public void setCapType(int value)
```


Указывает конечные заглушки.

См. [LineCapType](../../com.aspose.cells/linecaptype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


Представляет [Color](../../com.aspose.cells/color) линии.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setCompoundType(int value) {#setCompoundType-int-}
```
public void setCompoundType(int value)
```


Указывает составной тип линии

См. [MsoLineStyle](../../com.aspose.cells/msolinestyle).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setDashType(int value) {#setDashType-int-}
```
public void setDashType(int value)
```


Указывает тип пунктирной линии

См. [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setEndArrowLength(int value) {#setEndArrowLength-int-}
```
public void setEndArrowLength(int value)
```


Указывает длину наконечника стрелки для конца линии.

См. [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setEndArrowWidth(int value) {#setEndArrowWidth-int-}
```
public void setEndArrowWidth(int value)
```


Указывает ширину наконечника стрелки для конца линии.

См. [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setEndType(int value) {#setEndType-int-}
```
public void setEndType(int value)
```


Указывает тип наконечника стрелки для конца линии.

См. [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setFormattingType(int value) {#setFormattingType-int-}
```
public void setFormattingType(int value)
```


Устанавливает тип формата.

См. [ChartLineFormattingType](../../com.aspose.cells/chartlineformattingtype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setJoinType(int value) {#setJoinType-int-}
```
public void setJoinType(int value)
```


Указывает соединительные заглушки.

См. [LineJoinType](../../com.aspose.cells/linejointype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setStyle(int value) {#setStyle-int-}
```
public void setStyle(int value)
```


Представляет стиль линии.

Смотрите [LineType](../../com.aspose.cells/linetype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


Устанавливает цвет темы.

**Remarks**

Если цвет переднего плана не является цветом темы, будет возвращено NULL.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


Возвращает или задает степень прозрачности линии значением от 0,0 (непрозрачный) до 1,0 (прозрачный).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Отображает, видима ли линия.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setWeight(int value) {#setWeight-int-}
```
public void setWeight(int value)
```


Устанавливает [WeightType](../../com.aspose.cells/weighttype) линии.

Смотрите [WeightType](../../com.aspose.cells/weighttype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setWeightPt(double value) {#setWeightPt-double-}
```
public void setWeightPt(double value)
```


Устанавливает толщину линии в пунктах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setWeightPx(double value) {#setWeightPx-double-}
```
public void setWeightPx(double value)
```


Устанавливает толщину линии в пикселях.

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

