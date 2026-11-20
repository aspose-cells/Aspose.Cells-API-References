---
title: "DisplayUnitLabel"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет метку единицы отображения."
type: docs
url: /ru/java/com.aspose.cells/displayunitlabel/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ChartFrame](../../com.aspose.cells/chartframe), [com.aspose.cells.ChartTextFrame](../../com.aspose.cells/charttextframe)
```
public class DisplayUnitLabel extends ChartTextFrame
```

Представляет метку единицы отображения.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Adding a new worksheet to the Excel object
         int sheetIndex = workbook.getWorksheets().add();
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(sheetIndex);
         //Adding a sample value to "A1" cell
         worksheet.getCells().get("A1").putValue(50);
         //Adding a sample value to "A2" cell
         worksheet.getCells().get("A2").putValue(100);
         //Adding a sample value to "A3" cell
         worksheet.getCells().get("A3").putValue(150);
         //Adding a sample value to "A4" cell
         worksheet.getCells().get("A4").putValue(200);
         //Adding a sample value to "B1" cell
         worksheet.getCells().get("B1").putValue(60);
         //Adding a sample value to "B2" cell
         worksheet.getCells().get("B2").putValue(32);
         //Adding a sample value to "B3" cell
         worksheet.getCells().get("B3").putValue(50);
         //Adding a sample value to "B4" cell
         worksheet.getCells().get("B4").putValue(40);
         //Adding a sample value to "C1" cell as category data
         worksheet.getCells().get("C1").putValue("Q1");
         //Adding a sample value to "C2" cell as category data
         worksheet.getCells().get("C2").putValue("Q2");
         //Adding a sample value to "C3" cell as category data
         worksheet.getCells().get("C3").putValue("Y1");
         //Adding a sample value to "C4" cell as category data
         worksheet.getCells().get("C4").putValue("Y2");
         //Adding a chart to the worksheet
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 15, 5);
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
         chart.getNSeries().add("A1:B4", true);
         //Setting the data source for the category data of NSeries
         chart.getNSeries().setCategoryData("C1:C4");
         //Setting the display unit of value(Y) axis.
         chart.getValueAxis().setDisplayUnit(DisplayUnitType.HUNDREDS);
         DisplayUnitLabel displayUnitLabel = chart.getValueAxis().getDisplayUnitLabel();
         //Setting the custom display unit label
         displayUnitLabel.setText("100");
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Методы

| Метод | Описание |
| --- | --- |
| [characters(int startIndex, int length)](#characters-int-int-) | Возвращает объект Characters, представляющий диапазон символов в тексте. |
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
| [getDirectionType()](#getDirectionType--) | Получает направление текста. |
| [getFont()](#getFont--) | Получает объект [getFont()](../../com.aspose.cells/displayunitlabel\#getFont--) указанного объекта ChartFrame. |
| [getHeight()](#getHeight--) | Получает высоту кадра в единицах 1/4000 области диаграммы. |
| [getHeightPixel()](#getHeightPixel--) | Получает высоту кадра в пикселях. |
| [getHeightRatioToChart()](#getHeightRatioToChart--) | Получает высоту кадра в единицах отношения к области диаграммы. |
| [getLinkedSource()](#getLinkedSource--) | Получает ссылку на лист. |
| [getReadingOrder()](#getReadingOrder--) | Представляет порядок чтения текста. |
| [getRotationAngle()](#getRotationAngle--) | Представляет угол поворота текста. |
| [getShadow()](#getShadow--) | Истина, если у кадра есть тень. |
| [getShapeProperties()](#getShapeProperties--) | Получает объект [getShapeProperties()](../../com.aspose.cells/chartframe\#getShapeProperties--). |
| [getText()](#getText--) | Получает текст метки единицы отображения. |
| [getTextDirection()](#getTextDirection--) | Представляет порядок чтения текста. |
| [getTextFont()](#getTextFont--) | Получает объект [getFont()](../../com.aspose.cells/chartframe\#getFont--) указанного объекта ChartFrame. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--) | Получает горизонтальное выравнивание текста. |
| [getTextOptions()](#getTextOptions--) | Получает параметры текста. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--) | Получает вертикальное выравнивание текста. |
| [getWidth()](#getWidth--) | Получает ширину кадра в единицах 1/4000 области диаграммы. |
| [getWidthPixel()](#getWidthPixel--) | Получает ширину кадра в пикселях. |
| [getWidthRatioToChart()](#getWidthRatioToChart--) | Получает ширину кадра в единицах отношения к области диаграммы. |
| [getX()](#getX--) | Возвращает координату x верхнего левого угла в единицах 1/4000 области диаграммы. |
| [getXPixel()](#getXPixel--) | Получает координату x верхнего левого угла в пикселях. |
| [getXRatioToChart()](#getXRatioToChart--) | Возвращает координату x верхнего левого угла в относительных единицах области диаграммы. |
| [getY()](#getY--) | Получает координату y верхнего левого угла в единицах 1/4000 области диаграммы. |
| [getYPixel()](#getYPixel--) | Получает координату y верхнего левого угла в пикселях. |
| [getYRatioToChart()](#getYRatioToChart--) | Возвращает координату y верхнего левого угла в относительных единицах области диаграммы. |
| [hashCode()](#hashCode--) |  |
| [isAutoText()](#isAutoText--) | Указывает, что текст сгенерирован автоматически. |
| [isAutomaticRotation()](#isAutomaticRotation--) | Указывает, автоматически ли вращается текст диаграммы. |
| [isAutomaticSize()](#isAutomaticSize--) | Указывает, автоматически ли задаются размеры рамки диаграммы. |
| [isDefaultPosBeSet()](#isDefaultPosBeSet--) | Указывает, установлена ли позиция по умолчанию (DefaultX, DefaultY, DefaultWidth и DefaultHeight). |
| [isDeleted()](#isDeleted--) | Указывает, удалена ли эта метка данных. |
| [isInnerMode()](#isInnerMode--) | Указывает, включает ли размер области построения отметки делений и подписи осей. |
| [isResizeShapeToFitText()](#isResizeShapeToFitText--) | Получает, должна ли форма автоматически подгоняться, чтобы полностью содержать описанный в ней текст. |
| [isTextWrapped()](#isTextWrapped--) | Получает значение, указывающее, переносится ли текст. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | True, если текст в объекте изменяет размер шрифта при изменении размера объекта. |
| [setAutoText(boolean value)](#setAutoText-boolean-) | Указывает, что текст сгенерирован автоматически. |
| [setAutomaticSize(boolean value)](#setAutomaticSize-boolean-) | Указывает, автоматически ли задаются размеры рамки диаграммы. |
| [setBackground(int value)](#setBackground-int-) | Устанавливает режим отображения фона. |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | Устанавливает режим отображения фона. |
| [setDeleted(boolean value)](#setDeleted-boolean-) | Указывает, удалена ли эта метка данных. |
| [setDirectionType(int value)](#setDirectionType-int-) | Устанавливает направление текста. |
| [setHeight(int value)](#setHeight-int-) | Устанавливает высоту рамки в единицах 1/4000 области диаграммы. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Устанавливает высоту рамки в пикселях. |
| [setHeightRatioToChart(double value)](#setHeightRatioToChart-double-) | Устанавливает высоту рамки в единицах отношения к области диаграммы. |
| [setInnerMode(boolean value)](#setInnerMode-boolean-) | Указывает, включает ли размер области построения отметки делений и подписи осей. |
| [setLinkedSource(String value)](#setLinkedSource-java.lang.String-) | Устанавливает ссылку на лист. |
| [setPositionAuto()](#setPositionAuto--) | Установить позицию рамки в автоматический режим |
| [setReadingOrder(int value)](#setReadingOrder-int-) | Представляет порядок чтения текста. |
| [setResizeShapeToFitText(boolean value)](#setResizeShapeToFitText-boolean-) | Устанавливает, должна ли форма автоматически подгоняться, чтобы полностью содержать описанный в ней текст. |
| [setRotationAngle(int value)](#setRotationAngle-int-) | Представляет угол поворота текста. |
| [setShadow(boolean value)](#setShadow-boolean-) | Истина, если у кадра есть тень. |
| [setText(String value)](#setText-java.lang.String-) | Устанавливает текст метки единицы отображения. |
| [setTextDirection(int value)](#setTextDirection-int-) | Представляет порядок чтения текста. |
| [setTextHorizontalAlignment(int value)](#setTextHorizontalAlignment-int-) | Устанавливает горизонтальное выравнивание текста. |
| [setTextVerticalAlignment(int value)](#setTextVerticalAlignment-int-) | Устанавливает вертикальное выравнивание текста. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Устанавливает значение, указывающее, переносится ли текст. |
| [setWidth(int value)](#setWidth-int-) | Устанавливает ширину рамки в единицах 1/4000 области диаграммы. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Устанавливает ширину рамки в пикселях. |
| [setWidthRatioToChart(double value)](#setWidthRatioToChart-double-) | Устанавливает ширину рамки в единицах отношения к области диаграммы. |
| [setX(int value)](#setX-int-) | Устанавливает координату x верхнего левого угла в единицах 1/4000 области диаграммы. |
| [setXPixel(int value)](#setXPixel-int-) | Устанавливает координату x верхнего левого угла в пикселях. |
| [setXRatioToChart(double value)](#setXRatioToChart-double-) | Устанавливает координату x верхнего левого угла в относительных единицах области диаграммы. |
| [setY(int value)](#setY-int-) | Устанавливает координату y верхнего левого угла в единицах 1/4000 области диаграммы. |
| [setYPixel(int value)](#setYPixel-int-) | Устанавливает координату y верхнего левого угла в пикселях. |
| [setYRatioToChart(double value)](#setYRatioToChart-double-) | Устанавливает координату y верхнего левого угла в относительных единицах области диаграммы. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```


Возвращает объект Characters, представляющий диапазон символов в тексте.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startIndex | int | Индекс начала символа. |
| length | int | Количество символов. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - Characters object.
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
### getDirectionType() {#getDirectionType--}
```
public int getDirectionType()
```


Получает направление текста.

Смотрите [ChartTextDirectionType](../../com.aspose.cells/charttextdirectiontype).

**Returns:**
int
### getFont() {#getFont--}
```
public Font getFont()
```


Получает объект [getFont()](../../com.aspose.cells/displayunitlabel\#getFont--) указанного объекта ChartFrame.

**Returns:**
[Font](../../com.aspose.cells/font)
### getHeight() {#getHeight--}
```
public int getHeight()
```


Получает высоту кадра в единицах 1/4000 области диаграммы.

**Remarks**

ПРИМЕЧАНИЕ: Этот элемент теперь устарел. Пожалуйста, используйте свойство ChartFrame.HeightRatioToChart вместо него. Height = HeightRatioToChart \* 4000. Это свойство будет удалено через 12 месяцев, начиная с ФЕВРАЛЯ 2025 г. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

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


Получает высоту кадра в единицах отношения к области диаграммы.

**Remarks**

Это дробное значение, допустимый диапазон от 0 до 1. Как преобразовать единицы отношения в пиксели? HeightPixel = HeightRatioToChart \* Chart.ChartObject.Height;

**Returns:**
double
### getLinkedSource() {#getLinkedSource--}
```
public String getLinkedSource()
```


Получает ссылку на лист.

**Returns:**
java.lang.String
### getReadingOrder() {#getReadingOrder--}
```
public int getReadingOrder()
```


Представляет порядок чтения текста.

См. [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Returns:**
int
### getRotationAngle() {#getRotationAngle--}
```
public int getRotationAngle()
```


Представляет угол поворота текста.

**Remarks**


0: Не повернут.

255: Сверху вниз.

\-90: Вниз.

90: Вверх.


**Returns:**
int
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
### getText() {#getText--}
```
public String getText()
```


Получает текст метки единицы отображения.

**Returns:**
java.lang.String
### getTextDirection() {#getTextDirection--}
```
public int getTextDirection()
```


Представляет порядок чтения текста.

См. [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство ChartTextFrame.ReadingOrder. Это свойство будет удалено через 12 месяцев, начиная с марта 2020 года. Aspose извиняется за любые неудобства, которые вы могли испытать.

**Returns:**
int
### getTextFont() {#getTextFont--}
```
public Font getTextFont()
```


Получает объект [getFont()](../../com.aspose.cells/chartframe\#getFont--) указанного объекта ChartFrame.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство ChartFrame.Font. Это свойство будет удалено через 12 месяцев, начиная с ЯНВАРЯ 2012 года. Aspose извиняется за любые неудобства, которые вы могли испытать.

**Returns:**
[Font](../../com.aspose.cells/font)
### getTextHorizontalAlignment() {#getTextHorizontalAlignment--}
```
public int getTextHorizontalAlignment()
```


Получает горизонтальное выравнивание текста.

См. [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


Получает параметры текста.

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getTextVerticalAlignment() {#getTextVerticalAlignment--}
```
public int getTextVerticalAlignment()
```


Получает вертикальное выравнивание текста.

См. [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getWidth() {#getWidth--}
```
public int getWidth()
```


Получает ширину кадра в единицах 1/4000 области диаграммы.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Пожалуйста, используйте свойство ChartFrame.WidthRatioToChart вместо него. Width = WidthRatioToChart \* 4000; Это свойство будет удалено через 12 месяцев, начиная с февраля 2025 года. Aspose извиняется за любые неудобства, которые вы могли испытать.

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


Получает ширину кадра в единицах отношения к области диаграммы.

**Remarks**

Это дробное значение, его допустимый диапазон от 0 до 1. Как преобразовать единицы отношения в пиксели? WidthPixel = WidthRatioToChart \* Chart.ChartObject.Width;

**Returns:**
double
### getX() {#getX--}
```
public int getX()
```


Возвращает координату x верхнего левого угла в единицах 1/4000 области диаграммы.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Пожалуйста, используйте свойство ChartFrame.XRatioToChart вместо него. X = XRatioToChart \\* 4000. Это свойство будет удалено через 12 месяцев, начиная с февраля 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

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


Возвращает координату x верхнего левого угла в относительных единицах области диаграммы.

**Remarks**

Это дробное значение, допустимый диапазон от 0 до 1. Как преобразовать единицы отношения в пиксели? XPixel = XRatioToChart \\* Chart.ChartObject.Width;

**Returns:**
double
### getY() {#getY--}
```
public int getY()
```


Получает координату y верхнего левого угла в единицах 1/4000 области диаграммы.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Пожалуйста, используйте свойство ChartFrame.YRatioToChart вместо него. Y = YRatioToChart \\* 4000. Это свойство будет удалено через 12 месяцев, начиная с февраля 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

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


Возвращает координату y верхнего левого угла в относительных единицах области диаграммы.

**Remarks**

Это дробное значение, допустимый диапазон от 0 до 1. Как преобразовать единицы отношения в пиксели? YPixel = YRatioToChart \\* Chart.ChartObject.Height;

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoText() {#isAutoText--}
```
public boolean isAutoText()
```


Указывает, что текст сгенерирован автоматически.

**Returns:**
boolean
### isAutomaticRotation() {#isAutomaticRotation--}
```
public boolean isAutomaticRotation()
```


Указывает, автоматически ли вращается текст диаграммы.

**Returns:**
boolean
### isAutomaticSize() {#isAutomaticSize--}
```
public boolean isAutomaticSize()
```


Указывает, автоматически ли задаются размеры рамки диаграммы.

**Returns:**
boolean
### isDefaultPosBeSet() {#isDefaultPosBeSet--}
```
public boolean isDefaultPosBeSet()
```


Указывает, установлена ли позиция по умолчанию (DefaultX, DefaultY, DefaultWidth и DefaultHeight).

**Returns:**
boolean
### isDeleted() {#isDeleted--}
```
public boolean isDeleted()
```


Указывает, удалена ли эта метка данных.

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
### isResizeShapeToFitText() {#isResizeShapeToFitText--}
```
public boolean isResizeShapeToFitText()
```


Получает, следует ли автоматически подгонять форму, чтобы полностью вместить описанный в ней текст. Автоподгонка происходит, когда текст внутри формы масштабируется, чтобы вместить весь текст.

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


Получает значение, указывающее, переносится ли текст.

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

### setAutoText(boolean value) {#setAutoText-boolean-}
```
public void setAutoText(boolean value)
```


Указывает, что текст сгенерирован автоматически.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAutomaticSize(boolean value) {#setAutomaticSize-boolean-}
```
public void setAutomaticSize(boolean value)
```


Указывает, автоматически ли задаются размеры рамки диаграммы.

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

### setDeleted(boolean value) {#setDeleted-boolean-}
```
public void setDeleted(boolean value)
```


Указывает, удалена ли эта метка данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setDirectionType(int value) {#setDirectionType-int-}
```
public void setDirectionType(int value)
```


Устанавливает направление текста.

Смотрите [ChartTextDirectionType](../../com.aspose.cells/charttextdirectiontype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


Устанавливает высоту рамки в единицах 1/4000 области диаграммы.

**Remarks**

ПРИМЕЧАНИЕ: Этот элемент теперь устарел. Пожалуйста, используйте свойство ChartFrame.HeightRatioToChart вместо него. Height = HeightRatioToChart \* 4000. Это свойство будет удалено через 12 месяцев, начиная с ФЕВРАЛЯ 2025 г. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

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


Устанавливает высоту рамки в единицах отношения к области диаграммы.

**Remarks**

Это дробное значение, допустимый диапазон от 0 до 1. Как преобразовать единицы отношения в пиксели? HeightPixel = HeightRatioToChart \* Chart.ChartObject.Height;

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

### setLinkedSource(String value) {#setLinkedSource-java.lang.String-}
```
public void setLinkedSource(String value)
```


Устанавливает ссылку на лист.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setPositionAuto() {#setPositionAuto--}
```
public void setPositionAuto()
```


Установить позицию рамки в автоматический режим

### setReadingOrder(int value) {#setReadingOrder-int-}
```
public void setReadingOrder(int value)
```


Представляет порядок чтения текста.

См. [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setResizeShapeToFitText(boolean value) {#setResizeShapeToFitText-boolean-}
```
public void setResizeShapeToFitText(boolean value)
```


Устанавливает, следует ли автоматически подгонять форму, чтобы полностью вместить описанный в ней текст. Автоподгонка происходит, когда текст внутри формы масштабируется, чтобы вместить весь текст.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setRotationAngle(int value) {#setRotationAngle-int-}
```
public void setRotationAngle(int value)
```


Представляет угол поворота текста.

**Remarks**


0: Не повернут.

255: Сверху вниз.

\-90: Вниз.

90: Вверх.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

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

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Устанавливает текст метки единицы отображения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setTextDirection(int value) {#setTextDirection-int-}
```
public void setTextDirection(int value)
```


Представляет порядок чтения текста.

См. [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство ChartTextFrame.ReadingOrder. Это свойство будет удалено через 12 месяцев, начиная с марта 2020 года. Aspose извиняется за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setTextHorizontalAlignment(int value) {#setTextHorizontalAlignment-int-}
```
public void setTextHorizontalAlignment(int value)
```


Устанавливает горизонтальное выравнивание текста.

См. [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setTextVerticalAlignment(int value) {#setTextVerticalAlignment-int-}
```
public void setTextVerticalAlignment(int value)
```


Устанавливает вертикальное выравнивание текста.

См. [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


Устанавливает значение, указывающее, переносится ли текст.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


Устанавливает ширину рамки в единицах 1/4000 области диаграммы.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Пожалуйста, используйте свойство ChartFrame.WidthRatioToChart вместо него. Width = WidthRatioToChart \* 4000; Это свойство будет удалено через 12 месяцев, начиная с февраля 2025 года. Aspose извиняется за любые неудобства, которые вы могли испытать.

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


Устанавливает ширину рамки в единицах отношения к области диаграммы.

**Remarks**

Это дробное значение, его допустимый диапазон от 0 до 1. Как преобразовать единицы отношения в пиксели? WidthPixel = WidthRatioToChart \* Chart.ChartObject.Width;

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setX(int value) {#setX-int-}
```
public void setX(int value)
```


Устанавливает координату x верхнего левого угла в единицах 1/4000 области диаграммы.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Пожалуйста, используйте свойство ChartFrame.XRatioToChart вместо него. X = XRatioToChart \\* 4000. Это свойство будет удалено через 12 месяцев, начиная с февраля 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

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


Устанавливает координату x верхнего левого угла в относительных единицах области диаграммы.

**Remarks**

Это дробное значение, допустимый диапазон от 0 до 1. Как преобразовать единицы отношения в пиксели? XPixel = XRatioToChart \\* Chart.ChartObject.Width;

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


Устанавливает координату y верхнего левого угла в единицах 1/4000 области диаграммы.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Пожалуйста, используйте свойство ChartFrame.YRatioToChart вместо него. Y = YRatioToChart \\* 4000. Это свойство будет удалено через 12 месяцев, начиная с февраля 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

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


Устанавливает координату y верхнего левого угла в относительных единицах области диаграммы.

**Remarks**

Это дробное значение, допустимый диапазон от 0 до 1. Как преобразовать единицы отношения в пиксели? YPixel = YRatioToChart \\* Chart.ChartObject.Height;

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

