---
title: "PlotArea"
second_title: "Справочник API Aspose.Cells for Java"
description: "Инкапсулирует объект, представляющий область построения в диаграмме."
type: docs
url: /ru/java/com.aspose.cells/plotarea/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ChartFrame](../../com.aspose.cells/chartframe)
```
public class PlotArea extends ChartFrame
```

Инкапсулирует объект, представляющий область построения в диаграмме.
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | Получает [getArea()](../../com.aspose.cells/chartframe\\#getArea--). |
| [getAutoScaleFont()](#getAutoScaleFont--) | True, если текст в объекте изменяет размер шрифта при изменении размера объекта. |
| [getBackground()](#getBackground--) | Получает режим отображения фона. |
| [getBackgroundMode()](#getBackgroundMode--) | Получает режим отображения фона. |
| [getBorder()](#getBorder--) | Получает [Line](../../com.aspose.cells/line). |
| [getChart()](#getChart--) | Получает диаграмму, к которой принадлежит этот объект. |
| [getClass()](#getClass--) |  |
| [getDefaultHeight()](#getDefaultHeight--) | Представляет высоту позиции по умолчанию в единицах 1/4000 области диаграммы. |
| [getDefaultHeightRatioToChart()](#getDefaultHeightRatioToChart--) | Представляет высоту позиции по умолчанию в долях области диаграммы. |
| [getDefaultWidth()](#getDefaultWidth--) | Представляет ширину позиции по умолчанию в единицах 1/4000 области диаграммы. |
| [getDefaultWidthRatioToChart()](#getDefaultWidthRatioToChart--) | Представляет ширину позиции по умолчанию в единицах доли области диаграммы. |
| [getDefaultX()](#getDefaultX--) | Представляет координату x позиции по умолчанию в единицах 1/4000 области диаграммы. |
| [getDefaultXRatioToChart()](#getDefaultXRatioToChart--) | Представляет координату x позиции по умолчанию в единицах доли области диаграммы. |
| [getDefaultY()](#getDefaultY--) | Представляет координату y позиции по умолчанию в единицах 1/4000 области диаграммы. |
| [getDefaultYRatioToChart()](#getDefaultYRatioToChart--) | Представляет координату y позиции по умолчанию в единицах доли области диаграммы. |
| [getFont()](#getFont--) | Получает объект [getFont()](../../com.aspose.cells/chartframe\#getFont--) указанного объекта ChartFrame. |
| [getHeight()](#getHeight--) | Получает высоту ограничивающего прямоугольника области построения в единицах 1/4000 площади диаграммы. |
| [getHeightPixel()](#getHeightPixel--) | Получает высоту кадра в пикселях. |
| [getHeightRatioToChart()](#getHeightRatioToChart--) | Получает высоту ограничивающего прямоугольника области построения в единицах отношения к площади диаграммы. |
| [getInnerHeight()](#getInnerHeight--) | Получает высоту области построения в единицах 1/4000 площади диаграммы. |
| [getInnerHeightRatioToChart()](#getInnerHeightRatioToChart--) | Получает высоту области построения в единицах отношения к площади диаграммы. |
| [getInnerWidth()](#getInnerWidth--) | Получает ширину области построения в единицах 1/4000 площади диаграммы. |
| [getInnerWidthRatioToChart()](#getInnerWidthRatioToChart--) | Получает ширину области построения в единицах отношения к площади диаграммы. |
| [getInnerX()](#getInnerX--) | Получает координату x верхнего левого угла области построения в единицах 1/4000 площади диаграммы. |
| [getInnerXRatioToChart()](#getInnerXRatioToChart--) | Получает координату x верхнего левого угла области построения в единицах отношения к площади диаграммы. |
| [getInnerY()](#getInnerY--) | Получает координату x верхнего верхнего угла области построения в единицах 1/4000 области диаграммы. |
| [getInnerYRatioToChart()](#getInnerYRatioToChart--) | Получает координату x верхнего левого угла области построения в единицах отношения к площади диаграммы. |
| [getShadow()](#getShadow--) | Истина, если у кадра есть тень. |
| [getShapeProperties()](#getShapeProperties--) | Получает объект [getShapeProperties()](../../com.aspose.cells/chartframe\#getShapeProperties--). |
| [getTextFont()](#getTextFont--) | Получает объект [getFont()](../../com.aspose.cells/chartframe\#getFont--) указанного объекта ChartFrame. |
| [getTextOptions()](#getTextOptions--) | Получает параметры текста. |
| [getWidth()](#getWidth--) | Получает ширину ограничивающего прямоугольника области построения в единицах 1/4000 области диаграммы. |
| [getWidthPixel()](#getWidthPixel--) | Получает ширину кадра в пикселях. |
| [getWidthRatioToChart()](#getWidthRatioToChart--) | Получает ширину ограничивающего прямоугольника области построения в единицах отношения к области диаграммы. |
| [getX()](#getX--) | Получает координату x верхнего левого угла ограничивающего прямоугольника области построения в единицах 1/4000 области диаграммы. |
| [getXPixel()](#getXPixel--) | Получает координату x верхнего левого угла в пикселях. |
| [getXRatioToChart()](#getXRatioToChart--) | Получает координату x верхнего левого угла ограничивающего прямоугольника области построения как отношение к области диаграммы. |
| [getY()](#getY--) | Получает координату y верхнего верхнего угла ограничивающего прямоугольника области построения в единицах 1/4000 области диаграммы. |
| [getYPixel()](#getYPixel--) | Получает координату y верхнего левого угла в пикселях. |
| [getYRatioToChart()](#getYRatioToChart--) | Получает координату y верхнего верхнего угла ограничивающего прямоугольника области построения как отношение к области диаграммы. |
| [hashCode()](#hashCode--) |  |
| [isAutomaticSize()](#isAutomaticSize--) | Указывает, автоматически ли задаются размеры области построения. |
| [isDefaultPosBeSet()](#isDefaultPosBeSet--) | Указывает, установлена ли позиция по умолчанию (DefaultX, DefaultY, DefaultWidth и DefaultHeight). |
| [isInnerMode()](#isInnerMode--) | Указывает, включает ли размер области построения отметки делений и подписи осей. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | True, если текст в объекте изменяет размер шрифта при изменении размера объекта. |
| [setAutomaticSize(boolean value)](#setAutomaticSize-boolean-) | Указывает, автоматически ли задаются размеры области построения. |
| [setBackground(int value)](#setBackground-int-) | Устанавливает режим отображения фона. |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | Устанавливает режим отображения фона. |
| [setHeight(int value)](#setHeight-int-) | Устанавливает высоту ограничивающего прямоугольника области построения в единицах 1/4000 области диаграммы. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Устанавливает высоту рамки в пикселях. |
| [setHeightRatioToChart(double value)](#setHeightRatioToChart-double-) | Устанавливает высоту ограничивающего прямоугольника области построения в единицах отношения к области диаграммы. |
| [setInnerHeight(int value)](#setInnerHeight-int-) | Устанавливает высоту области построения в единицах 1/4000 области диаграммы. |
| [setInnerHeightRatioToChart(double value)](#setInnerHeightRatioToChart-double-) | Устанавливает высоту области построения в единицах отношения к области диаграммы. |
| [setInnerMode(boolean value)](#setInnerMode-boolean-) | Указывает, включает ли размер области построения отметки делений и подписи осей. |
| [setInnerWidth(int value)](#setInnerWidth-int-) | Устанавливает ширину области построения в единицах 1/4000 области диаграммы. |
| [setInnerWidthRatioToChart(double value)](#setInnerWidthRatioToChart-double-) | Устанавливает ширину области построения в единицах отношения к области диаграммы. |
| [setInnerX(int value)](#setInnerX-int-) | Устанавливает координату x верхнего верхнего угла области построения в единицах 1/4000 области диаграммы. |
| [setInnerXRatioToChart(double value)](#setInnerXRatioToChart-double-) | Получает координату x верхнего левого угла области построения в единицах отношения к площади диаграммы. |
| [setInnerY(int value)](#setInnerY-int-) | Устанавливает координату x верхнего верхнего угла области построения в единицах 1/4000 области диаграммы. |
| [setInnerYRatioToChart(double value)](#setInnerYRatioToChart-double-) | Получает координату x верхнего левого угла области построения в единицах отношения к площади диаграммы. |
| [setPositionAuto()](#setPositionAuto--) | Установите позицию области построения в автоматический режим. |
| [setShadow(boolean value)](#setShadow-boolean-) | Истина, если у кадра есть тень. |
| [setWidth(int value)](#setWidth-int-) | Устанавливает ширину ограничивающего прямоугольника области построения в единицах 1/4000 области диаграммы. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Устанавливает ширину рамки в пикселях. |
| [setWidthRatioToChart(double value)](#setWidthRatioToChart-double-) | Устанавливает ширину ограничивающего прямоугольника области построения в единицах отношения к области диаграммы. |
| [setX(int value)](#setX-int-) | Устанавливает координату x верхнего левого угла ограничивающего прямоугольника области построения в единицах 1/4000 области диаграммы. |
| [setXPixel(int value)](#setXPixel-int-) | Устанавливает координату x верхнего левого угла в пикселях. |
| [setXRatioToChart(double value)](#setXRatioToChart-double-) | Устанавливает координату x верхнего левого угла ограничивающего прямоугольника области построения как отношение к области диаграммы. |
| [setY(int value)](#setY-int-) | Устанавливает координату y верхнего верхнего угла ограничивающего прямоугольника области построения в единицах 1/4000 области диаграммы. |
| [setYPixel(int value)](#setYPixel-int-) | Устанавливает координату y верхнего левого угла в пикселях. |
| [setYRatioToChart(double value)](#setYRatioToChart-double-) | Устанавливает координату y верхнего верхнего угла ограничивающего прямоугольника области построения как отношение к области диаграммы. |
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
### getArea() {#getArea--}
```
public Area getArea()
```


Получает [getArea()](../../com.aspose.cells/chartframe\\#getArea--).

**Returns:**
[Area](../../com.aspose.cells/area)
### getAutoScaleFont() {#getAutoScaleFont--}
```
public boolean getAutoScaleFont()
```


True, если текст в объекте изменяет размер шрифта при изменении размера объекта. Значение по умолчанию — True.

**Returns:**
boolean
### getBackground() {#getBackground--}
```
public int getBackground()
```


Получает режим отображения фона. Это свойство действительно только в Excel 2003 и более ранних версиях.

Смотрите [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Remarks**

ПРИМЕЧАНИЕ: Этот элемент теперь устарел. Вместо этого, пожалуйста, используйте свойство ChartFrame.Area.FillFormat.FillType. Например, если вам нужно установить BackgroundMode в Opaque, вы можете использовать следующий код: Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; Это свойство будет удалено через 12 месяцев, начиная с ЯНВАРЯ 2012 г. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
int
### getBackgroundMode() {#getBackgroundMode--}
```
public int getBackgroundMode()
```


Получает режим отображения фона. Это свойство действительно только в Excel 2003 и более ранних версиях.

Смотрите [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Remarks**

ПРИМЕЧАНИЕ: Этот элемент теперь устарел. Вместо этого, пожалуйста, используйте свойство ChartFrame.Area.FillFormat.FillType. Например, если вам нужно установить BackgroundMode в Opaque, вы можете использовать следующий код: Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; Это свойство будет удалено через 12 месяцев, начиная с ФЕВРАЛЯ 2026 г. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
int
### getBorder() {#getBorder--}
```
public Line getBorder()
```


Получает [Line](../../com.aspose.cells/line).

**Returns:**
[Line](../../com.aspose.cells/line)
### getChart() {#getChart--}
```
public Chart getChart()
```


Получает диаграмму, к которой принадлежит этот объект.

**Returns:**
[Chart](../../com.aspose.cells/chart)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDefaultHeight() {#getDefaultHeight--}
```
public int getDefaultHeight()
```


Представляет высоту позиции по умолчанию в единицах 1/4000 области диаграммы.

**Remarks**

ПРИМЕЧАНИЕ: Этот элемент теперь устарел. Пожалуйста, используйте свойство ChartFrame.DefaultHeightRatioToChart вместо него. DefaultHeight = (int)(DefaultHeightRatioToChart \* 4000); Это свойство будет удалено через 12 месяцев, начиная с ФЕВРАЛЯ 2025 г. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
int
### getDefaultHeightRatioToChart() {#getDefaultHeightRatioToChart--}
```
public double getDefaultHeightRatioToChart()
```


Представляет высоту позиции по умолчанию в долях области диаграммы.

**Returns:**
double
### getDefaultWidth() {#getDefaultWidth--}
```
public int getDefaultWidth()
```


Представляет ширину позиции по умолчанию в единицах 1/4000 области диаграммы.

**Remarks**

ПРИМЕЧАНИЕ: Этот элемент теперь устарел. Пожалуйста, используйте свойство ChartFrame.DefaultWidthRatioToChart вместо него. DefaultWidth = (int)(DefaultWidthRatioToChart \* 4000); Это свойство будет удалено через 12 месяцев, начиная с ФЕВРАЛЯ 2025 г. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
int
### getDefaultWidthRatioToChart() {#getDefaultWidthRatioToChart--}
```
public double getDefaultWidthRatioToChart()
```


Представляет ширину позиции по умолчанию в единицах доли области диаграммы.

**Returns:**
double
### getDefaultX() {#getDefaultX--}
```
public int getDefaultX()
```


Представляет координату x позиции по умолчанию в единицах 1/4000 области диаграммы.

**Remarks**

ПРИМЕЧАНИЕ: Этот элемент теперь устарел. Пожалуйста, используйте свойство ChartFrame.DefaultXRatioToChart вместо него. DefaultX = (int)(DefaultXRatioToChart \* 4000); Это свойство будет удалено через 12 месяцев, начиная с ФЕВРАЛЯ 2025 г. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
int
### getDefaultXRatioToChart() {#getDefaultXRatioToChart--}
```
public double getDefaultXRatioToChart()
```


Представляет координату x позиции по умолчанию в единицах доли области диаграммы.

**Returns:**
double
### getDefaultY() {#getDefaultY--}
```
public int getDefaultY()
```


Представляет координату y позиции по умолчанию в единицах 1/4000 области диаграммы.

**Remarks**

ПРИМЕЧАНИЕ: Этот элемент теперь устарел. Пожалуйста, используйте свойство ChartFrame.DefaultYRatioToChart вместо него. DefaultY = (int)(DefaultYRatioToChart \* 4000); Это свойство будет удалено через 12 месяцев, начиная с ФЕВРАЛЯ 2025 г. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
int
### getDefaultYRatioToChart() {#getDefaultYRatioToChart--}
```
public double getDefaultYRatioToChart()
```


Представляет координату y позиции по умолчанию в единицах доли области диаграммы.

**Returns:**
double
### getFont() {#getFont--}
```
public Font getFont()
```


Получает объект [getFont()](../../com.aspose.cells/chartframe\#getFont--) указанного объекта ChartFrame.

**Returns:**
[Font](../../com.aspose.cells/font)
### getHeight() {#getHeight--}
```
public int getHeight()
```


Получает высоту ограничивающего прямоугольника области построения в единицах 1/4000 площади диаграммы.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Пожалуйста, используйте свойство PlotArea.HeightRatioToChart вместо него. Height = HeightRatioToChart \* 4000. Это свойство будет удалено через 12 месяцев, начиная с февраля 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
int
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```


Получает высоту кадра в пикселях.

**Returns:**
int
### getHeightRatioToChart() {#getHeightRatioToChart--}
```
public double getHeightRatioToChart()
```


Получает высоту ограничивающего прямоугольника области построения в единицах отношения к площади диаграммы.

**Remarks**

Ограничивающий прямоугольник области построения включает область построения, деления (метки делений) и небольшую границу вокруг делений. Если значение не было создано MS Excel, пожалуйста, вызовите метод Chart.Calculate() перед вызовом этого метода.

The **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** и **HeightRatioToChart** объекта **PlotArea** представляют ограничивающий прямоугольник области графика, который включает область графика, деления (метки делений) и небольшую границу вокруг делений. Если вы хотите получить фактический размер области графика, следует вызвать свойства **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** и **InnerHeightRatioToChart**.

Для Excel 2007 и более новых версий значение по умолчанию равно нулю. Вы должны получить значение после вызова Chart.Calculate().

HeightPixel = HeightRatioToChart \* chart.ChartObject.Width. Примечание: Когда HeightRatioToChart задаётся, свойство IsInnerMode автоматически устанавливается в false.

**Returns:**
double
### getInnerHeight() {#getInnerHeight--}
```
public int getInnerHeight()
```


Получает высоту области построения в единицах 1/4000 площади диаграммы.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте свойство PlotArea.InnerHeightRatioToChart. InnerHeight = InnerHeightRatioToChart \* 4000; Это свойство будет удалено через 12 месяцев, начиная с февраля 2025 года. Aspose приносит извинения за любые причинённые неудобства.

**Returns:**
int
### getInnerHeightRatioToChart() {#getInnerHeightRatioToChart--}
```
public double getInnerHeightRatioToChart()
```


Получает высоту области построения в единицах отношения к площади диаграммы.

**Remarks**

Ограничивающий прямоугольник области построения включает область построения, деления (метки делений) и небольшую границу вокруг делений. Если значение не было создано MS Excel, пожалуйста, вызовите метод Chart.Calculate() перед вызовом этого метода.

The **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** и **HeightRatioToChart** объекта **PlotArea** представляют ограничивающий прямоугольник области графика, который включает область графика, деления (метки делений) и небольшую границу вокруг делений. Если вы хотите получить фактический размер области графика, следует вызвать свойства **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** и **InnerHeightRatioToChart**.

Для Excel 2007 и более новых версий значение по умолчанию равно нулю. Вы должны получить значение после вызова Chart.Calculate().

InnerHeight в пикселях = InnerXRatioToChart \* chart.ChartObject.Width. Примечание: Когда InnerHeightRatioToChart задаётся, свойство IsInnerMode автоматически устанавливается в True.

**Returns:**
double
### getInnerWidth() {#getInnerWidth--}
```
public int getInnerWidth()
```


Получает ширину области построения в единицах 1/4000 площади диаграммы.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте свойство PlotArea.InnerWidthRatioToChart. InnerWidth = InnerWidthRatioToChart \* 4000; Это свойство будет удалено через 12 месяцев, начиная с февраля 2025 года. Aspose приносит извинения за любые причинённые неудобства.

**Returns:**
int
### getInnerWidthRatioToChart() {#getInnerWidthRatioToChart--}
```
public double getInnerWidthRatioToChart()
```


Получает ширину области построения в единицах отношения к площади диаграммы.

**Remarks**

Ограничивающий прямоугольник области построения включает область построения, деления (метки делений) и небольшую границу вокруг делений. Если значение не было создано MS Excel, пожалуйста, вызовите метод Chart.Calculate() перед вызовом этого метода.

The **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** и **HeightRatioToChart** объекта **PlotArea** представляют ограничивающий прямоугольник области графика, который включает область графика, деления (метки делений) и небольшую границу вокруг делений. Если вы хотите получить фактический размер области графика, следует вызвать свойства **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** и **InnerHeightRatioToChart**.

Для Excel 2007 и более новых версий значение по умолчанию равно нулю. Вы должны получить значение после вызова Chart.Calculate().

InnerWidth в пикселях = InnerXRatioToChart \* chart.ChartObject.Width. Примечание: Когда InnerWidthRatioToChart задаётся, свойство IsInnerMode автоматически устанавливается в True.

**Returns:**
double
### getInnerX() {#getInnerX--}
```
public int getInnerX()
```


Получает координату x верхнего левого угла области построения в единицах 1/4000 площади диаграммы.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте свойство PlotArea.InnerXRatioToChart. InnerX = InnerXRatioToChart \* 4000. Это свойство будет удалено через 12 месяцев, начиная с февраля 2025 года. Aspose приносит извинения за любые причинённые неудобства.

**Returns:**
int
### getInnerXRatioToChart() {#getInnerXRatioToChart--}
```
public double getInnerXRatioToChart()
```


Получает координату x верхнего левого угла области построения в единицах отношения к площади диаграммы.

**Remarks**

Ограничивающий прямоугольник области построения включает область построения, деления (метки делений) и небольшую границу вокруг делений. Если значение не было создано MS Excel, пожалуйста, вызовите метод Chart.Calculate() перед вызовом этого метода.

The **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** и **HeightRatioToChart** объекта **PlotArea** представляют ограничивающий прямоугольник области графика, который включает область графика, деления (метки делений) и небольшую границу вокруг делений. Если вы хотите получить фактический размер области графика, следует вызвать свойства **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** и **InnerHeightRatioToChart**.

Для Excel 2007 и более новых версий значение по умолчанию равно нулю. Вы должны получить значение после вызова Chart.Calculate().

InnerX в пикселях = InnerXRatioToChart \* chart.ChartObject.Width. Примечание: Когда InnerXRatioToChart задаётся, свойство IsInnerMode автоматически устанавливается в True.

**Returns:**
double
### getInnerY() {#getInnerY--}
```
public int getInnerY()
```


Получает координату x верхнего верхнего угла области построения в единицах 1/4000 области диаграммы.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте свойство PlotArea.InnerYRatioToChart. InnerY = InnerYRatioToChart \* 4000. Это свойство будет удалено через 12 месяцев, начиная с февраля 2025 года. Aspose приносит извинения за любые причинённые неудобства.

**Returns:**
int
### getInnerYRatioToChart() {#getInnerYRatioToChart--}
```
public double getInnerYRatioToChart()
```


Получает координату x верхнего левого угла области построения в единицах отношения к площади диаграммы.

**Remarks**

Ограничивающий прямоугольник области построения включает область построения, деления (метки делений) и небольшую границу вокруг делений. Если значение не было создано MS Excel, пожалуйста, вызовите метод Chart.Calculate() перед вызовом этого метода.

The **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** и **HeightRatioToChart** объекта **PlotArea** представляют ограничивающий прямоугольник области графика, который включает область графика, деления (метки делений) и небольшую границу вокруг делений. Если вы хотите получить фактический размер области графика, следует вызвать свойства **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** и **InnerHeightRatioToChart**.

Для Excel 2007 и более новых версий значение по умолчанию равно нулю. Вы должны получить значение после вызова Chart.Calculate().

InnerY в пикселях = InnerYRatioToChart \* chart.ChartObject.Width. Примечание: Когда InnerYRatioToChart задаётся, свойство IsInnerMode автоматически устанавливается в True.

**Returns:**
double
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Истина, если у кадра есть тень.

**Remarks**

Только для диаграмм в файле xls.

**Returns:**
boolean
### getShapeProperties() {#getShapeProperties--}
```
public ShapePropertyCollection getShapeProperties()
```


Получает объект [getShapeProperties()](../../com.aspose.cells/chartframe\#getShapeProperties--).

**Returns:**
[ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection)
### getTextFont() {#getTextFont--}
```
public Font getTextFont()
```


Получает объект [getFont()](../../com.aspose.cells/chartframe\#getFont--) указанного объекта ChartFrame.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство ChartFrame.Font. Это свойство будет удалено через 12 месяцев, начиная с ЯНВАРЯ 2012 года. Aspose извиняется за любые неудобства, которые вы могли испытать.

**Returns:**
[Font](../../com.aspose.cells/font)
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


Получает параметры текста.

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getWidth() {#getWidth--}
```
public int getWidth()
```


Получает ширину ограничивающего прямоугольника области построения в единицах 1/4000 области диаграммы.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте свойство PlotArea.WidthRatioToChart. Width = WidthRatioToChart \* 4000. Это свойство будет удалено через 12 месяцев, начиная с февраля 2025 года. Aspose приносит извинения за любые причинённые неудобства.

**Returns:**
int
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```


Получает ширину кадра в пикселях.

**Returns:**
int
### getWidthRatioToChart() {#getWidthRatioToChart--}
```
public double getWidthRatioToChart()
```


Получает ширину ограничивающего прямоугольника области построения в единицах отношения к области диаграммы.

**Remarks**

Ограничивающий прямоугольник области построения включает область построения, деления (метки делений) и небольшую границу вокруг делений. Если значение не было создано MS Excel, пожалуйста, вызовите метод Chart.Calculate() перед вызовом этого метода.

The **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** и **HeightRatioToChart** объекта **PlotArea** представляют ограничивающий прямоугольник области графика, который включает область графика, деления (метки делений) и небольшую границу вокруг делений. Если вы хотите получить фактический размер области графика, следует вызвать свойства **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** и **InnerHeightRatioToChart**.

Для Excel 2007 и более новых версий значение по умолчанию равно нулю. Вы должны получить значение после вызова Chart.Calculate().

WidthPixel = WidthRatioToChart \* chart.ChartObject.Width. Примечание: Когда WidthRatioToChart задаётся, свойство IsInnerMode автоматически устанавливается в false.

**Returns:**
double
### getX() {#getX--}
```
public int getX()
```


Получает координату x верхнего левого угла ограничивающего прямоугольника области построения в единицах 1/4000 области диаграммы.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте свойство PlotArea.XRatioToChart. X = XRatioToChart \* 4000. Это свойство будет удалено через 12 месяцев, начиная с февраля 2025 года. Aspose приносит извинения за любые причинённые неудобства.

**Returns:**
int
### getXPixel() {#getXPixel--}
```
public int getXPixel()
```


Получает координату x верхнего левого угла в пикселях.

**Returns:**
int
### getXRatioToChart() {#getXRatioToChart--}
```
public double getXRatioToChart()
```


Получает координату x верхнего левого угла ограничивающего прямоугольника области построения как отношение к области диаграммы.

**Remarks**

Ограничивающий прямоугольник области построения включает область построения, деления (метки делений) и небольшую границу вокруг делений. Если значение не было создано MS Excel, пожалуйста, вызовите метод Chart.Calculate() перед вызовом этого метода.

The **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** и **HeightRatioToChart** объекта **PlotArea** представляют ограничивающий прямоугольник области графика, который включает область графика, деления (метки делений) и небольшую границу вокруг делений. Если вы хотите получить фактический размер области графика, следует вызвать свойства **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** и **InnerHeightRatioToChart**.

Для Excel 2007 и более новых версий значение по умолчанию равно нулю. Вы должны получить значение после вызова Chart.Calculate().

XPixel = XRatioToChart \* chart.ChartObject.Width. Примечание: Когда XRatioToChart задаётся, свойство IsInnerMode автоматически устанавливается в false.

**Returns:**
double
### getY() {#getY--}
```
public int getY()
```


Получает координату y верхнего верхнего угла ограничивающего прямоугольника области построения в единицах 1/4000 области диаграммы.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте свойство PlotArea.YRatioToChart. Y = YRatioToChart \* 4000. Это свойство будет удалено через 12 месяцев, начиная с февраля 2025 года. Aspose приносит извинения за любые причинённые неудобства.

**Returns:**
int
### getYPixel() {#getYPixel--}
```
public int getYPixel()
```


Получает координату y верхнего левого угла в пикселях.

**Returns:**
int
### getYRatioToChart() {#getYRatioToChart--}
```
public double getYRatioToChart()
```


Получает координату y верхнего верхнего угла ограничивающего прямоугольника области построения как отношение к области диаграммы.

**Remarks**

Ограничивающий прямоугольник области построения включает область построения, деления (метки делений) и небольшую границу вокруг делений. Если значение не было создано MS Excel, пожалуйста, вызовите метод Chart.Calculate() перед вызовом этого метода.

The **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** и **HeightRatioToChart** объекта **PlotArea** представляют ограничивающий прямоугольник области графика, который включает область графика, деления (метки делений) и небольшую границу вокруг делений. Если вы хотите получить фактический размер области графика, следует вызвать свойства **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** и **InnerHeightRatioToChart**.

Для Excel 2007 и более новых версий значение по умолчанию равно нулю. Вы должны получить значение после вызова Chart.Calculate().

YPixel = YRatioToChart \* chart.ChartObject.Width. Примечание: Когда YRatioToChart задаётся, свойство IsInnerMode автоматически устанавливается в false.

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutomaticSize() {#isAutomaticSize--}
```
public boolean isAutomaticSize()
```


Указывает, автоматически ли задаются размеры области построения.

**Remarks**

ПРИМЕЧАНИЕ: Когда IsAutomaticSize устанавливается в True, значения, которые вы вручную задаёте для Width и Height, будут отключены.

**Returns:**
boolean
### isDefaultPosBeSet() {#isDefaultPosBeSet--}
```
public boolean isDefaultPosBeSet()
```


Указывает, установлена ли позиция по умолчанию (DefaultX, DefaultY, DefaultWidth и DefaultHeight).

**Returns:**
boolean
### isInnerMode() {#isInnerMode--}
```
public boolean isInnerMode()
```


Указывает, включает ли размер области построения отметки делений и подписи осей. Значение False указывает, что размер определяет только размер области построения, без отметок делений и подписей осей.

**Remarks**

Только для файла Xlsx.

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




### setAutoScaleFont(boolean value) {#setAutoScaleFont-boolean-}
```
public void setAutoScaleFont(boolean value)
```


True, если текст в объекте изменяет размер шрифта при изменении размера объекта. Значение по умолчанию — True.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAutomaticSize(boolean value) {#setAutomaticSize-boolean-}
```
public void setAutomaticSize(boolean value)
```


Указывает, автоматически ли задаются размеры области построения.

**Remarks**

ПРИМЕЧАНИЕ: Когда IsAutomaticSize устанавливается в True, значения, которые вы вручную задаёте для Width и Height, будут отключены.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setBackground(int value) {#setBackground-int-}
```
public void setBackground(int value)
```


Устанавливает режим отображения фона. Это свойство действительно только в Excel 2003 и более ранних версиях.

Смотрите [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Remarks**

ПРИМЕЧАНИЕ: Этот элемент теперь устарел. Вместо этого, пожалуйста, используйте свойство ChartFrame.Area.FillFormat.FillType. Например, если вам нужно установить BackgroundMode в Opaque, вы можете использовать следующий код: Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; Это свойство будет удалено через 12 месяцев, начиная с ЯНВАРЯ 2012 г. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setBackgroundMode(int value) {#setBackgroundMode-int-}
```
public void setBackgroundMode(int value)
```


Устанавливает режим отображения фона. Это свойство действительно только в Excel 2003 и более ранних версиях.

Смотрите [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Remarks**

ПРИМЕЧАНИЕ: Этот элемент теперь устарел. Вместо этого, пожалуйста, используйте свойство ChartFrame.Area.FillFormat.FillType. Например, если вам нужно установить BackgroundMode в Opaque, вы можете использовать следующий код: Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; Это свойство будет удалено через 12 месяцев, начиная с ФЕВРАЛЯ 2026 г. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


Устанавливает высоту ограничивающего прямоугольника области построения в единицах 1/4000 области диаграммы.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Пожалуйста, используйте свойство PlotArea.HeightRatioToChart вместо него. Height = HeightRatioToChart \* 4000. Это свойство будет удалено через 12 месяцев, начиная с февраля 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setHeightPixel(int value) {#setHeightPixel-int-}
```
public void setHeightPixel(int value)
```


Устанавливает высоту рамки в пикселях.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setHeightRatioToChart(double value) {#setHeightRatioToChart-double-}
```
public void setHeightRatioToChart(double value)
```


Устанавливает высоту ограничивающего прямоугольника области построения в единицах отношения к области диаграммы.

**Remarks**

Ограничивающий прямоугольник области построения включает область построения, деления (метки делений) и небольшую границу вокруг делений. Если значение не было создано MS Excel, пожалуйста, вызовите метод Chart.Calculate() перед вызовом этого метода.

The **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** и **HeightRatioToChart** объекта **PlotArea** представляют ограничивающий прямоугольник области графика, который включает область графика, деления (метки делений) и небольшую границу вокруг делений. Если вы хотите получить фактический размер области графика, следует вызвать свойства **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** и **InnerHeightRatioToChart**.

Для Excel 2007 и более новых версий значение по умолчанию равно нулю. Вы должны получить значение после вызова Chart.Calculate().

HeightPixel = HeightRatioToChart \* chart.ChartObject.Width. Примечание: Когда HeightRatioToChart задаётся, свойство IsInnerMode автоматически устанавливается в false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setInnerHeight(int value) {#setInnerHeight-int-}
```
public void setInnerHeight(int value)
```


Устанавливает высоту области построения в единицах 1/4000 области диаграммы.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте свойство PlotArea.InnerHeightRatioToChart. InnerHeight = InnerHeightRatioToChart \* 4000; Это свойство будет удалено через 12 месяцев, начиная с февраля 2025 года. Aspose приносит извинения за любые причинённые неудобства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setInnerHeightRatioToChart(double value) {#setInnerHeightRatioToChart-double-}
```
public void setInnerHeightRatioToChart(double value)
```


Устанавливает высоту области построения в единицах отношения к области диаграммы.

**Remarks**

Ограничивающий прямоугольник области построения включает область построения, деления (метки делений) и небольшую границу вокруг делений. Если значение не было создано MS Excel, пожалуйста, вызовите метод Chart.Calculate() перед вызовом этого метода.

The **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** и **HeightRatioToChart** объекта **PlotArea** представляют ограничивающий прямоугольник области графика, который включает область графика, деления (метки делений) и небольшую границу вокруг делений. Если вы хотите получить фактический размер области графика, следует вызвать свойства **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** и **InnerHeightRatioToChart**.

Для Excel 2007 и более новых версий значение по умолчанию равно нулю. Вы должны получить значение после вызова Chart.Calculate().

InnerHeight в пикселях = InnerXRatioToChart \* chart.ChartObject.Width. Примечание: Когда InnerHeightRatioToChart задаётся, свойство IsInnerMode автоматически устанавливается в True.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setInnerMode(boolean value) {#setInnerMode-boolean-}
```
public void setInnerMode(boolean value)
```


Указывает, включает ли размер области построения отметки делений и подписи осей. Значение False указывает, что размер определяет только размер области построения, без отметок делений и подписей осей.

**Remarks**

Только для файла Xlsx.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setInnerWidth(int value) {#setInnerWidth-int-}
```
public void setInnerWidth(int value)
```


Устанавливает ширину области построения в единицах 1/4000 области диаграммы.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте свойство PlotArea.InnerWidthRatioToChart. InnerWidth = InnerWidthRatioToChart \* 4000; Это свойство будет удалено через 12 месяцев, начиная с февраля 2025 года. Aspose приносит извинения за любые причинённые неудобства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setInnerWidthRatioToChart(double value) {#setInnerWidthRatioToChart-double-}
```
public void setInnerWidthRatioToChart(double value)
```


Устанавливает ширину области построения в единицах отношения к области диаграммы.

**Remarks**

Ограничивающий прямоугольник области построения включает область построения, деления (метки делений) и небольшую границу вокруг делений. Если значение не было создано MS Excel, пожалуйста, вызовите метод Chart.Calculate() перед вызовом этого метода.

The **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** и **HeightRatioToChart** объекта **PlotArea** представляют ограничивающий прямоугольник области графика, который включает область графика, деления (метки делений) и небольшую границу вокруг делений. Если вы хотите получить фактический размер области графика, следует вызвать свойства **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** и **InnerHeightRatioToChart**.

Для Excel 2007 и более новых версий значение по умолчанию равно нулю. Вы должны получить значение после вызова Chart.Calculate().

InnerWidth в пикселях = InnerXRatioToChart \* chart.ChartObject.Width. Примечание: Когда InnerWidthRatioToChart задаётся, свойство IsInnerMode автоматически устанавливается в True.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setInnerX(int value) {#setInnerX-int-}
```
public void setInnerX(int value)
```


Устанавливает координату x верхнего верхнего угла области построения в единицах 1/4000 области диаграммы.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте свойство PlotArea.InnerXRatioToChart. InnerX = InnerXRatioToChart \* 4000. Это свойство будет удалено через 12 месяцев, начиная с февраля 2025 года. Aspose приносит извинения за любые причинённые неудобства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setInnerXRatioToChart(double value) {#setInnerXRatioToChart-double-}
```
public void setInnerXRatioToChart(double value)
```


Получает координату x верхнего левого угла области построения в единицах отношения к площади диаграммы.

**Remarks**

Ограничивающий прямоугольник области построения включает область построения, деления (метки делений) и небольшую границу вокруг делений. Если значение не было создано MS Excel, пожалуйста, вызовите метод Chart.Calculate() перед вызовом этого метода.

The **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** и **HeightRatioToChart** объекта **PlotArea** представляют ограничивающий прямоугольник области графика, который включает область графика, деления (метки делений) и небольшую границу вокруг делений. Если вы хотите получить фактический размер области графика, следует вызвать свойства **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** и **InnerHeightRatioToChart**.

Для Excel 2007 и более новых версий значение по умолчанию равно нулю. Вы должны получить значение после вызова Chart.Calculate().

InnerX в пикселях = InnerXRatioToChart \* chart.ChartObject.Width. Примечание: Когда InnerXRatioToChart задаётся, свойство IsInnerMode автоматически устанавливается в True.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setInnerY(int value) {#setInnerY-int-}
```
public void setInnerY(int value)
```


Устанавливает координату x верхнего верхнего угла области построения в единицах 1/4000 области диаграммы.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте свойство PlotArea.InnerYRatioToChart. InnerY = InnerYRatioToChart \* 4000. Это свойство будет удалено через 12 месяцев, начиная с февраля 2025 года. Aspose приносит извинения за любые причинённые неудобства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setInnerYRatioToChart(double value) {#setInnerYRatioToChart-double-}
```
public void setInnerYRatioToChart(double value)
```


Получает координату x верхнего левого угла области построения в единицах отношения к площади диаграммы.

**Remarks**

Ограничивающий прямоугольник области построения включает область построения, деления (метки делений) и небольшую границу вокруг делений. Если значение не было создано MS Excel, пожалуйста, вызовите метод Chart.Calculate() перед вызовом этого метода.

The **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** и **HeightRatioToChart** объекта **PlotArea** представляют ограничивающий прямоугольник области графика, который включает область графика, деления (метки делений) и небольшую границу вокруг делений. Если вы хотите получить фактический размер области графика, следует вызвать свойства **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** и **InnerHeightRatioToChart**.

Для Excel 2007 и более новых версий значение по умолчанию равно нулю. Вы должны получить значение после вызова Chart.Calculate().

InnerY в пикселях = InnerYRatioToChart \* chart.ChartObject.Width. Примечание: Когда InnerYRatioToChart задаётся, свойство IsInnerMode автоматически устанавливается в True.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setPositionAuto() {#setPositionAuto--}
```
public void setPositionAuto()
```


Установите позицию области построения в автоматический режим.

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


Истина, если у кадра есть тень.

**Remarks**

Только для диаграмм в файле xls.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


Устанавливает ширину ограничивающего прямоугольника области построения в единицах 1/4000 области диаграммы.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте свойство PlotArea.WidthRatioToChart. Width = WidthRatioToChart \* 4000. Это свойство будет удалено через 12 месяцев, начиная с февраля 2025 года. Aspose приносит извинения за любые причинённые неудобства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```


Устанавливает ширину рамки в пикселях.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setWidthRatioToChart(double value) {#setWidthRatioToChart-double-}
```
public void setWidthRatioToChart(double value)
```


Устанавливает ширину ограничивающего прямоугольника области построения в единицах отношения к области диаграммы.

**Remarks**

Ограничивающий прямоугольник области построения включает область построения, деления (метки делений) и небольшую границу вокруг делений. Если значение не было создано MS Excel, пожалуйста, вызовите метод Chart.Calculate() перед вызовом этого метода.

The **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** и **HeightRatioToChart** объекта **PlotArea** представляют ограничивающий прямоугольник области графика, который включает область графика, деления (метки делений) и небольшую границу вокруг делений. Если вы хотите получить фактический размер области графика, следует вызвать свойства **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** и **InnerHeightRatioToChart**.

Для Excel 2007 и более новых версий значение по умолчанию равно нулю. Вы должны получить значение после вызова Chart.Calculate().

WidthPixel = WidthRatioToChart \* chart.ChartObject.Width. Примечание: Когда WidthRatioToChart задаётся, свойство IsInnerMode автоматически устанавливается в false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setX(int value) {#setX-int-}
```
public void setX(int value)
```


Устанавливает координату x верхнего левого угла ограничивающего прямоугольника области построения в единицах 1/4000 области диаграммы.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте свойство PlotArea.XRatioToChart. X = XRatioToChart \* 4000. Это свойство будет удалено через 12 месяцев, начиная с февраля 2025 года. Aspose приносит извинения за любые причинённые неудобства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setXPixel(int value) {#setXPixel-int-}
```
public void setXPixel(int value)
```


Устанавливает координату x верхнего левого угла в пикселях.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setXRatioToChart(double value) {#setXRatioToChart-double-}
```
public void setXRatioToChart(double value)
```


Устанавливает координату x верхнего левого угла ограничивающего прямоугольника области построения как отношение к области диаграммы.

**Remarks**

Ограничивающий прямоугольник области построения включает область построения, деления (метки делений) и небольшую границу вокруг делений. Если значение не было создано MS Excel, пожалуйста, вызовите метод Chart.Calculate() перед вызовом этого метода.

The **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** и **HeightRatioToChart** объекта **PlotArea** представляют ограничивающий прямоугольник области графика, который включает область графика, деления (метки делений) и небольшую границу вокруг делений. Если вы хотите получить фактический размер области графика, следует вызвать свойства **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** и **InnerHeightRatioToChart**.

Для Excel 2007 и более новых версий значение по умолчанию равно нулю. Вы должны получить значение после вызова Chart.Calculate().

XPixel = XRatioToChart \* chart.ChartObject.Width. Примечание: Когда XRatioToChart задаётся, свойство IsInnerMode автоматически устанавливается в false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


Устанавливает координату y верхнего верхнего угла ограничивающего прямоугольника области построения в единицах 1/4000 области диаграммы.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте свойство PlotArea.YRatioToChart. Y = YRatioToChart \* 4000. Это свойство будет удалено через 12 месяцев, начиная с февраля 2025 года. Aspose приносит извинения за любые причинённые неудобства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setYPixel(int value) {#setYPixel-int-}
```
public void setYPixel(int value)
```


Устанавливает координату y верхнего левого угла в пикселях.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setYRatioToChart(double value) {#setYRatioToChart-double-}
```
public void setYRatioToChart(double value)
```


Устанавливает координату y верхнего верхнего угла ограничивающего прямоугольника области построения как отношение к области диаграммы.

**Remarks**

Ограничивающий прямоугольник области построения включает область построения, деления (метки делений) и небольшую границу вокруг делений. Если значение не было создано MS Excel, пожалуйста, вызовите метод Chart.Calculate() перед вызовом этого метода.

The **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** и **HeightRatioToChart** объекта **PlotArea** представляют ограничивающий прямоугольник области графика, который включает область графика, деления (метки делений) и небольшую границу вокруг делений. Если вы хотите получить фактический размер области графика, следует вызвать свойства **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** и **InnerHeightRatioToChart**.

Для Excel 2007 и более новых версий значение по умолчанию равно нулю. Вы должны получить значение после вызова Chart.Calculate().

YPixel = YRatioToChart \* chart.ChartObject.Width. Примечание: Когда YRatioToChart задаётся, свойство IsInnerMode автоматически устанавливается в false.

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

