---
title: "ChartPoint"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет отдельную точку в серии диаграммы."
type: docs
url: /ru/java/com.aspose.cells/chartpoint/
---

**Inheritance:**
java.lang.Object
```
public class ChartPoint
```

Представляет отдельную точку в серии диаграммы.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         //Adding a sample value to "A1" cell
         worksheet.getCells().get("A1").putValue(50);
 
         //Adding a sample value to "A2" cell
         worksheet.getCells().get("A2").putValue(100);
 
         //Adding a sample value to "A3" cell
         worksheet.getCells().get("A3").putValue(150);
 
         //Adding a sample value to "B1" cell
         worksheet.getCells().get("B1").putValue(60);
 
         //Adding a sample value to "B2" cell
         worksheet.getCells().get("B2").putValue(32);
 
         //Adding a sample value to "B3" cell
         worksheet.getCells().get("B3").putValue(50);
 
         //Adding a chart to the worksheet
         int chartIndex = worksheet.getCharts().add(ChartType.PIE_EXPLODED, 5, 0, 25, 10);
 
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
 
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
         chart.getNSeries().add("A1:B3", true);
 
         //Show Data Labels 
         chart.getNSeries().get(0).getDataLabels().setShowValue(true);
 
         for (int i = 0; i  <chart.getNSeries().get(0).getPoints().getCount(); i++)
         {
             //Get Data Point
             ChartPoint point = chart.getNSeries().get(0).getPoints().get(i);
             //Set Pir Explosion
             point.setExplosion(15);
             //Set Border Color
             point.getBorder().setColor(com.aspose.cells.Color.getRed());
         }
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArcEndPointXPx()](#getArcEndPointXPx--) | Получает координату x конечной точки секции пирога после вызова метода Chart.Calculate(). |
| [getArcEndPointYPx()](#getArcEndPointYPx--) | Получает координату y конечной точки секции пирога после вызова метода Chart.Calculate(). |
| [getArcStartPointXPx()](#getArcStartPointXPx--) | Получает координату x начальной точки секции пирога после вызова метода Chart.Calculate(). |
| [getArcStartPointYPx()](#getArcStartPointYPx--) | Получает координату y начальной точки секции пирога после вызова метода Chart.Calculate(). |
| [getArea()](#getArea--) | Получает [getArea()](../../com.aspose.cells/chartpoint\#getArea--). |
| [getBorder()](#getBorder--) | Получает [Line](../../com.aspose.cells/line). |
| [getBorderWidthPx()](#getBorderWidthPx--) | Получает ширину границы в пикселях после вызова метода Chart.Calculate(). |
| [getBottomPointCount()](#getBottomPointCount--) | Получает количество нижних точек после вызова метода Chart.Calculate(). |
| [getBottomPointXPx(int index)](#getBottomPointXPx-int-) | Получает координату x нижней точки формы после вызова метода Chart.Calculate(). |
| [getBottomPointYPx(int index)](#getBottomPointYPx-int-) | Получает координату y нижней точки формы после вызова метода Chart.Calculate(). |
| [getClass()](#getClass--) |  |
| [getDataLabels()](#getDataLabels--) | Возвращает объект [getDataLabels()](../../com.aspose.cells/chartpoint\#getDataLabels--), представляющий метку данных, связанную с этой точкой диаграммы. |
| [getDoughnutInnerRadius()](#getDoughnutInnerRadius--) | Получает внутренний радиус сектора кольцевой диаграммы в пикселях после вызова метода Chart.Calculate(). |
| [getEndAngle()](#getEndAngle--) | Получает конечный угол секции пирога, измеряемый в градусах по часовой стрелке от оси x после вызова метода Chart.Calculate(). |
| [getExplosion()](#getExplosion--) | Расстояние открытого сектора пирога от центра круговой диаграммы выражается в процентах от диаметра пирога. |
| [getInnerArcEndPointXPx()](#getInnerArcEndPointXPx--) | Получает координату x конечной точки секции пирога после вызова метода Chart.Calculate(). |
| [getInnerArcEndPointYPx()](#getInnerArcEndPointYPx--) | Получает координату y конечной точки секции пирога после вызова метода Chart.Calculate(). |
| [getInnerArcStartPointXPx()](#getInnerArcStartPointXPx--) | Получает координату x начальной точки секции пирога после вызова метода Chart.Calculate(). |
| [getInnerArcStartPointYPx()](#getInnerArcStartPointYPx--) | Получает координату y начальной точки секции пирога после вызова метода Chart.Calculate(). |
| [getInnerRadiusPx()](#getInnerRadiusPx--) | Получает внутренний радиус сектора кольцевой диаграммы в пикселях после вызова метода Chart.Calculate(). |
| [getMarker()](#getMarker--) | Получает [getMarker()](../../com.aspose.cells/chartpoint\#getMarker--). |
| [getOnCategoryAxisPointCount()](#getOnCategoryAxisPointCount--) | Получает количество точек на оси категорий после вызова метода Chart.Calculate(). |
| [getOnCategoryAxisPointXPx(int index)](#getOnCategoryAxisPointXPx-int-) | Получает координату x точки на оси категорий после вызова метода Chart.Calculate(). |
| [getOnCategoryAxisPointYPx(int index)](#getOnCategoryAxisPointYPx-int-) | Получает координату y точки на оси категорий после вызова метода Chart.Calculate(). |
| [getRadiusPx()](#getRadiusPx--) | Получает радиус пузыря, сектора пирога или кольцевой диаграммы в пикселях после вызова метода Chart.Calculate(). |
| [getShadow()](#getShadow--) | Истина, если у точки диаграммы есть тень. |
| [getShapeHeight()](#getShapeHeight--) | Получает высоту в единицах 1/4000 высоты диаграммы после вызова метода Chart.Calculate(). |
| [getShapeHeightPx()](#getShapeHeightPx--) | Получает высоту в пикселях после вызова метода Chart.Calculate(). |
| [getShapeProperties()](#getShapeProperties--) | Получает объект [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection), содержащий визуальные свойства формы ChartPoint. |
| [getShapeWidth()](#getShapeWidth--) | Получает ширину в единицах 1/4000 ширины диаграммы после вызова метода Chart.Calculate(). |
| [getShapeWidthPx()](#getShapeWidthPx--) | Получает ширину в пикселях после вызова метода Chart.Calculate(). |
| [getShapeX()](#getShapeX--) | Получает координату x верхнего левого угла в единицах 1/4000 ширины диаграммы после вызова метода Chart.Calculate(). |
| [getShapeXPx()](#getShapeXPx--) | Получает координату x верхнего левого угла в пикселях после вызова метода Chart.Calculate(). |
| [getShapeY()](#getShapeY--) | Получает координату y верхнего левого угла в единицах 1/4000 высоты диаграммы после вызова метода Chart.Calculate(). |
| [getShapeYPx()](#getShapeYPx--) | Получает координату y верхнего левого угла в пикселях после вызова метода Chart.Calculate(). |
| [getStartAngle()](#getStartAngle--) | Получает начальный угол секции круговой диаграммы, измеряемый в градусах по часовой стрелке от оси x после вызова метода Chart.Calculate(). |
| [getTopPointCount()](#getTopPointCount--) | Получает количество верхних точек после вызова метода Chart.Calculate(). |
| [getTopPointXPx(int index)](#getTopPointXPx-int-) | Получает координату x верхней точки формы после вызова метода Chart.Calculate(). |
| [getTopPointYPx(int index)](#getTopPointYPx-int-) | Получает координату y верхней точки формы после вызова метода Chart.Calculate(). |
| [getXValue()](#getXValue--) | Получает значение X точки диаграммы. |
| [getXValueType()](#getXValueType--) | Получает тип значения X точки диаграммы. |
| [getYValue()](#getYValue--) | Получает значение Y точки диаграммы. |
| [getYValueType()](#getYValueType--) | Получает тип значения Y точки диаграммы. |
| [hashCode()](#hashCode--) |  |
| [isInSecondaryPlot()](#isInSecondaryPlot--) | Получает значение, указывающее, находится ли эта точка данных во втором круге или столбце на диаграмме pie of pie или bar of pie. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setExplosion(int value)](#setExplosion-int-) | Расстояние открытого сектора пирога от центра круговой диаграммы выражается в процентах от диаметра пирога. |
| [setInSecondaryPlot(boolean value)](#setInSecondaryPlot-boolean-) | Устанавливает значение, указывающее, находится ли эта точка данных во втором круге или столбце на диаграмме pie of pie или bar of pie. |
| [setShadow(boolean value)](#setShadow-boolean-) | Истина, если у точки диаграммы есть тень. |
| [setXValue(Object value)](#setXValue-java.lang.Object-) | Устанавливает значение X точки диаграммы. |
| [setYValue(Object value)](#setYValue-java.lang.Object-) | Устанавливает значение Y точки диаграммы. |
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
### getArcEndPointXPx() {#getArcEndPointXPx--}
```
public float getArcEndPointXPx()
```


Получает координату x конечной точки секции круговой диаграммы после вызова метода Chart.Calculate(). Применяется к диаграммам Pie и Doughnut.

**Returns:**
float
### getArcEndPointYPx() {#getArcEndPointYPx--}
```
public float getArcEndPointYPx()
```


Получает координату y конечной точки секции круговой диаграммы после вызова метода Chart.Calculate(). Применяется к диаграммам Pie и Doughnut.

**Returns:**
float
### getArcStartPointXPx() {#getArcStartPointXPx--}
```
public float getArcStartPointXPx()
```


Получает координату x начальной точки секции круговой диаграммы после вызова метода Chart.Calculate(). Применяется к диаграммам Pie и Doughnut.

**Returns:**
float
### getArcStartPointYPx() {#getArcStartPointYPx--}
```
public float getArcStartPointYPx()
```


Получает координату y начальной точки секции круговой диаграммы после вызова метода Chart.Calculate(). Применяется к диаграммам Pie и Doughnut.

**Returns:**
float
### getArea() {#getArea--}
```
public Area getArea()
```


Получает [getArea()](../../com.aspose.cells/chartpoint\#getArea--).

**Returns:**
[Area](../../com.aspose.cells/area)
### getBorder() {#getBorder--}
```
public Line getBorder()
```


Получает [Line](../../com.aspose.cells/line).

**Returns:**
[Line](../../com.aspose.cells/line)
### getBorderWidthPx() {#getBorderWidthPx--}
```
public int getBorderWidthPx()
```


Получает ширину границы в пикселях после вызова метода Chart.Calculate().

**Returns:**
int
### getBottomPointCount() {#getBottomPointCount--}
```
public int getBottomPointCount()
```


Получает количество нижних точек после вызова метода Chart.Calculate().

**Returns:**
int
### getBottomPointXPx(int index) {#getBottomPointXPx-int-}
```
public float getBottomPointXPx(int index)
```


Получает координату x нижней точки формы после вызова метода Chart.Calculate(). Применяется к 3D-диаграммам: Column3D, Bar3D, Cone, Cylinder, Pyramid.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int |  |

**Returns:**
float
### getBottomPointYPx(int index) {#getBottomPointYPx-int-}
```
public float getBottomPointYPx(int index)
```


Получает координату y нижней точки формы после вызова метода Chart.Calculate(). Применяется к 3D-диаграммам: Column3D, Bar3D, Cone, Cylinder, Pyramid.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int |  |

**Returns:**
float
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDataLabels() {#getDataLabels--}
```
public DataLabels getDataLabels()
```


Возвращает объект [getDataLabels()](../../com.aspose.cells/chartpoint\#getDataLabels--), представляющий метку данных, связанную с этой точкой диаграммы.

**Returns:**
[DataLabels](../../com.aspose.cells/datalabels)
### getDoughnutInnerRadius() {#getDoughnutInnerRadius--}
```
public int getDoughnutInnerRadius()
```


Получает внутренний радиус сектора кольцевой диаграммы в пикселях после вызова метода Chart.Calculate(). Применяется к диаграмме Doughnut.

**Returns:**
int
### getEndAngle() {#getEndAngle--}
```
public float getEndAngle()
```


Получает конечный угол секции круговой диаграммы, измеряемый в градусах по часовой стрелке от оси x после вызова метода Chart.Calculate(). Применяется к диаграмме Pie.

**Returns:**
float
### getExplosion() {#getExplosion--}
```
public int getExplosion()
```


Расстояние открытого сектора пирога от центра круговой диаграммы выражается в процентах от диаметра пирога.

**Returns:**
int
### getInnerArcEndPointXPx() {#getInnerArcEndPointXPx--}
```
public float getInnerArcEndPointXPx()
```


Получает координату x конечной точки секции круговой диаграммы после вызова метода Chart.Calculate(). Применяется к диаграммам Doughnut.

**Returns:**
float
### getInnerArcEndPointYPx() {#getInnerArcEndPointYPx--}
```
public float getInnerArcEndPointYPx()
```


Получает координату y конечной точки секции круговой диаграммы после вызова метода Chart.Calculate(). Применяется к диаграмме Doughnut.

**Returns:**
float
### getInnerArcStartPointXPx() {#getInnerArcStartPointXPx--}
```
public float getInnerArcStartPointXPx()
```


Получает координату x начальной точки секции круговой диаграммы после вызова метода Chart.Calculate(). Применяется к диаграмме Doughnut.

**Returns:**
float
### getInnerArcStartPointYPx() {#getInnerArcStartPointYPx--}
```
public float getInnerArcStartPointYPx()
```


Получает координату y начальной точки сектора после вызова метода Chart.Calculate(). Применяется к диаграмме Doughnut.

**Returns:**
float
### getInnerRadiusPx() {#getInnerRadiusPx--}
```
public int getInnerRadiusPx()
```


Получает внутренний радиус сегмента кольцевой диаграммы в пикселях после вызова метода Chart.Calculate(). Применяется к диаграмме Doughnut.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство ChartPoint.DoughnutInnerRadius. Это свойство будет удалено через 12 месяцев, начиная с июня 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
int
### getMarker() {#getMarker--}
```
public Marker getMarker()
```


Получает [getMarker()](../../com.aspose.cells/chartpoint\#getMarker--).

**Returns:**
[Marker](../../com.aspose.cells/marker)
### getOnCategoryAxisPointCount() {#getOnCategoryAxisPointCount--}
```
public int getOnCategoryAxisPointCount()
```


Получает количество точек на категориальной оси после вызова метода Chart.Calculate(). Применяется только к диаграммам области.

**Remarks**

Диаграмма области 2D возвращает 1, диаграмма области 3D возвращает 2.

**Returns:**
int
### getOnCategoryAxisPointXPx(int index) {#getOnCategoryAxisPointXPx-int-}
```
public float getOnCategoryAxisPointXPx(int index)
```


Получает координату x точки на категориальной оси после вызова метода Chart.Calculate(). Применяется только к диаграмме области.

**Remarks**

Диаграмма области 2D: индекс 0. Диаграмма области 3D: индекс 0 или 1.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int |  |

**Returns:**
float
### getOnCategoryAxisPointYPx(int index) {#getOnCategoryAxisPointYPx-int-}
```
public float getOnCategoryAxisPointYPx(int index)
```


Получает координату y точки на категориальной оси после вызова метода Chart.Calculate(). Применяется только к диаграмме области.

**Remarks**

Диаграмма области 2D: индекс 0. Диаграмма области 3D: индекс 0 или 1.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int |  |

**Returns:**
float
### getRadiusPx() {#getRadiusPx--}
```
public int getRadiusPx()
```


Получает радиус пузыря, сектора пирога или кольцевой диаграммы в пикселях после вызова метода Chart.Calculate().

**Returns:**
int
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Истина, если у точки диаграммы есть тень.

**Returns:**
boolean
### getShapeHeight() {#getShapeHeight--}
```
public int getShapeHeight()
```


Получает высоту в единицах 1/4000 высоты диаграммы после вызова метода Chart.Calculate().

**Returns:**
int
### getShapeHeightPx() {#getShapeHeightPx--}
```
public int getShapeHeightPx()
```


Получает высоту в пикселях после вызова метода Chart.Calculate().

**Returns:**
int
### getShapeProperties() {#getShapeProperties--}
```
public ShapePropertyCollection getShapeProperties()
```


Получает объект [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection), содержащий визуальные свойства формы ChartPoint.

**Returns:**
[ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection)
### getShapeWidth() {#getShapeWidth--}
```
public int getShapeWidth()
```


Получает ширину в единицах 1/4000 ширины диаграммы после вызова метода Chart.Calculate().

**Returns:**
int
### getShapeWidthPx() {#getShapeWidthPx--}
```
public int getShapeWidthPx()
```


Получает ширину в пикселях после вызова метода Chart.Calculate().

**Returns:**
int
### getShapeX() {#getShapeX--}
```
public int getShapeX()
```


Получает координату x верхнего левого угла в единицах 1/4000 ширины диаграммы после вызова метода Chart.Calculate().

**Returns:**
int
### getShapeXPx() {#getShapeXPx--}
```
public int getShapeXPx()
```


Получает координату x верхнего левого угла в пикселях после вызова метода Chart.Calculate().

**Returns:**
int
### getShapeY() {#getShapeY--}
```
public int getShapeY()
```


Получает координату y верхнего левого угла в единицах 1/4000 высоты диаграммы после вызова метода Chart.Calculate().

**Returns:**
int
### getShapeYPx() {#getShapeYPx--}
```
public int getShapeYPx()
```


Получает координату y верхнего левого угла в пикселях после вызова метода Chart.Calculate().

**Returns:**
int
### getStartAngle() {#getStartAngle--}
```
public float getStartAngle()
```


Получает начальный угол секции пирога, измеряемый в градусах по часовой стрелке от оси x после вызова метода Chart.Calculate(). Применяется к диаграмме Pie.

**Returns:**
float
### getTopPointCount() {#getTopPointCount--}
```
public int getTopPointCount()
```


Получает количество верхних точек после вызова метода Chart.Calculate().

**Returns:**
int
### getTopPointXPx(int index) {#getTopPointXPx-int-}
```
public float getTopPointXPx(int index)
```


Получает координату x верхней точки формы после вызова метода Chart.Calculate(). Применяется к 3D‑диаграммам: Column3D, Bar3D, Cone, Cylinder, Pyramid и Area3D.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int |  |

**Returns:**
float
### getTopPointYPx(int index) {#getTopPointYPx-int-}
```
public float getTopPointYPx(int index)
```


Получает координату y верхней точки формы после вызова метода Chart.Calculate(). Применяется к 3D‑диаграммам: Column3D, Bar3D, Cone, Cylinder, Pyramid, и Area3D.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int |  |

**Returns:**
float
### getXValue() {#getXValue--}
```
public Object getXValue()
```


Получает значение X точки диаграммы.

**Returns:**
java.lang.Object
### getXValueType() {#getXValueType--}
```
public int getXValueType()
```


Получает тип значения X точки диаграммы.

Смотрите [CellValueType](../../com.aspose.cells/cellvaluetype).

**Returns:**
int
### getYValue() {#getYValue--}
```
public Object getYValue()
```


Получает значение Y точки диаграммы.

**Returns:**
java.lang.Object
### getYValueType() {#getYValueType--}
```
public int getYValueType()
```


Получает тип значения Y точки диаграммы.

Смотрите [CellValueType](../../com.aspose.cells/cellvaluetype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isInSecondaryPlot() {#isInSecondaryPlot--}
```
public boolean isInSecondaryPlot()
```


Получает значение, указывающее, находится ли эта точка данных во втором круге или столбце на диаграмме pie of pie или bar of pie.

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




### setExplosion(int value) {#setExplosion-int-}
```
public void setExplosion(int value)
```


Расстояние открытого сектора пирога от центра круговой диаграммы выражается в процентах от диаметра пирога.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setInSecondaryPlot(boolean value) {#setInSecondaryPlot-boolean-}
```
public void setInSecondaryPlot(boolean value)
```


Устанавливает значение, указывающее, находится ли эта точка данных во втором круге или столбце на диаграмме pie of pie или bar of pie.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


Истина, если у точки диаграммы есть тень.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setXValue(Object value) {#setXValue-java.lang.Object-}
```
public void setXValue(Object value)
```


Устанавливает значение X точки диаграммы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.Object |  |

### setYValue(Object value) {#setYValue-java.lang.Object-}
```
public void setYValue(Object value)
```


Устанавливает значение Y точки диаграммы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.Object |  |

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

