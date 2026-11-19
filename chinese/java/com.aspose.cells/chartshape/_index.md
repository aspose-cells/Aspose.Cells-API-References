---
title: "ChartShape"
second_title: "Aspose.Cells for Java API 参考"
description: "表示图表的形状。"
type: docs
url: /zh/java/com.aspose.cells/chartshape/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Shape](../../com.aspose.cells/shape)
```
public class ChartShape extends Shape
```

表示图表的形状。ChartObject 对象的属性和方法控制工作表中嵌入图表的外观和大小。

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
 
         //Getting Chart Shape
         ChartShape chartShape = chart.getChartObject();
 
         //Set Lower Right Column
         chartShape.setLowerRightColumn(10);
 
         //Set LowerDeltaX
         chartShape.setLowerDeltaX(1024);
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [addHyperlink(String address)](#addHyperlink-java.lang.String-) | 向形状添加超链接。 |
| [alignTopRightCorner(int topRow, int rightColumn)](#alignTopRightCorner-int-int-) | 将图片移动到右上角。 |
| [calculateTextSize()](#calculateTextSize--) | 重新计算文本区域 |
| [characters(int startIndex, int length)](#characters-int-int-) | 返回一个 Characters 对象，表示文本中的字符范围。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [fitToTextSize()](#fitToTextSize--) | 重新计算适合显示所有文本内容的文本区域。 |
| [formatCharacters(int startIndex, int length, Font font, StyleFlag flag)](#formatCharacters-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-) | 使用字体设置格式化部分字符。 |
| [getActiveXControl()](#getActiveXControl--) | 获取 ActiveX 控件。 |
| [getActualBox()](#getActualBox--) | 获取形状的实际位置和大小（在应用旋转、翻转等之后）。 |
| [getActualLowerRightRow()](#getActualLowerRightRow--) | 获取实际的底部行。 |
| [getAlternativeText()](#getAlternativeText--) | 返回或设置 [Shape](../../com.aspose.cells/shape) 对象的描述性（替代）文本字符串。 |
| [getAnchorType()](#getAnchorType--) | 获取形状锚点占位符的类型。 |
| [getAutoShapeType()](#getAutoShapeType--) | 获取自动形状类型。 |
| [getBottom()](#getBottom--) | 表示形状从其左下角行的垂直偏移宽度，单位为像素。 |
| [getCharacters()](#getCharacters--) | 返回表示文本中字符范围的所有 Characters 对象。 |
| [getChart()](#getChart--) | 返回一个表示对象中包含的图表的 Chart 对象。 |
| [getClass()](#getClass--) |  |
| [getConnectionPoints()](#getConnectionPoints--) | 获取连接点 |
| [getControlData()](#getControlData--) | 获取控件的数据。 |
| [getCreateId()](#getCreateId--) | 获取此形状的创建 ID。 |
| [getFill()](#getFill--) | 返回一个 [getFillFormat()](../../com.aspose.cells/shape\\#getFillFormat--) 对象，该对象包含指定形状的填充格式属性。 |
| [getFillFormat()](#getFillFormat--) | 返回一个 MsoFillFormat 对象，该对象包含指定形状的填充格式属性。 |
| [getFont()](#getFont--) | 表示形状的字体。 |
| [getFormatPicture()](#getFormatPicture--) | 获取图片格式的选项。 |
| [getGeometry()](#getGeometry--) | 获取几何形状 |
| [getGlow()](#getGlow--) | 表示一个 [GlowEffect](../../com.aspose.cells/gloweffect) 对象，用于指定图表元素或形状的发光效果。 |
| [getGroup()](#getGroup--) | 获取包含此形状的组形状。 |
| [getHeight()](#getHeight--) | 表示形状的高度，单位为像素。 |
| [getHeightCM()](#getHeightCM--) | 表示形状的高度，单位为厘米。 |
| [getHeightInShape()](#getHeightInShape--) | 表示形状相对于父形状顶部边界的垂直偏移，单位为父形状高度的 1/4000。 |
| [getHeightInch()](#getHeightInch--) | 表示形状的高度，单位为英寸。 |
| [getHeightPt()](#getHeightPt--) | 表示形状的高度，单位为点。 |
| [getHeightScale()](#getHeightScale--) | 获取高度比例，单位为原始图片高度的百分比。 |
| [getHtmlText()](#getHtmlText--) | 获取包含此文本框中数据和部分格式的 HTML 字符串。 |
| [getHyperlink()](#getHyperlink--) | 获取形状的超链接。 |
| [getId()](#getId--) | 获取此形状的标识符。 |
| [getInputRange()](#getInputRange--) | 获取用于填充指定组合框的工作表范围。 |
| [getInputRange(boolean isR1C1, boolean isLocal)](#getInputRange-boolean-boolean-) | 获取用于填充控件的范围。 |
| [getLeft()](#getLeft--) | 表示形状相对于其左列的水平偏移，单位为像素。 |
| [getLeftCM()](#getLeftCM--) | 表示形状相对于其左列的水平偏移，单位为厘米。 |
| [getLeftInShape()](#getLeftInShape--) | 表示形状相对于父形状左边框的水平偏移，单位为父形状宽度的 1/4000。 |
| [getLeftInch()](#getLeftInch--) | 表示形状相对于其左列的水平偏移，单位为英寸。 |
| [getLeftToCorner()](#getLeftToCorner--) | 获取形状相对于工作表左边框的水平偏移。 |
| [getLine()](#getLine--) | 获取线条样式 |
| [getLineFormat()](#getLineFormat--) | 返回一个 MsoLineFormat 对象，其中包含指定形状的线条格式属性。 |
| [getLinkedCell()](#getLinkedCell--) | 获取与控件值关联的工作表范围。 |
| [getLinkedCell(boolean isR1C1, boolean isLocal)](#getLinkedCell-boolean-boolean-) | 获取与控件值关联的范围。 |
| [getLockedProperty(int type)](#getLockedProperty-int-) | 获取 locked 属性的值。 |
| [getLowerDeltaX()](#getLowerDeltaX--) | 获取形状相对于其右下角列的水平偏移。 |
| [getLowerDeltaY()](#getLowerDeltaY--) | 获取形状相对于其右下角行的垂直偏移。 |
| [getLowerRightColumn()](#getLowerRightColumn--) | 表示右下角列索引。 |
| [getLowerRightRow()](#getLowerRightRow--) | 表示右下角行索引。 |
| [getMacroName()](#getMacroName--) | 获取宏的名称。 |
| [getMsoDrawingType()](#getMsoDrawingType--) | 获取绘图类型。 |
| [getName()](#getName--) | 获取形状的名称。 |
| [getPaths()](#getPaths--) | 获取自定义几何形状的路径。 |
| [getPlacement()](#getPlacement--) | 表示绘图对象附着在其下方单元格的方式。 |
| [getReflection()](#getReflection--) | 表示一个 [ReflectionEffect](../../com.aspose.cells/reflectioneffect) 对象，用于指定图表元素或形状的反射效果。 |
| [getRelativeToOriginalPictureSize()](#getRelativeToOriginalPictureSize--) | 指示形状是否相对于原始图片尺寸。 |
| [getResultOfSmartArt()](#getResultOfSmartArt--) | 将 SmartArt 转换为组合形状。 |
| [getRichFormattings()](#getRichFormattings--) | 返回表示文本中字符范围的所有 Characters 对象。 |
| [getRight()](#getRight--) | 表示形状相对于其右下角列的水平偏移宽度，单位为像素。 |
| [getRotationAngle()](#getRotationAngle--) | 获取形状的旋转角度。 |
| [getShadowEffect()](#getShadowEffect--) | 表示一个 [ShadowEffect](../../com.aspose.cells/shadoweffect) 对象，用于指定图表元素或形状的阴影效果。 |
| [getSoftEdges()](#getSoftEdges--) | 获取要应用于边缘的模糊半径，单位为点。 |
| [getSpid()](#getSpid--) | 指定一个可选的字符串标识符，应用程序可使用它来标识特定形状。 |
| [getSpt()](#getSpt--) | 指定一个可选的数字，应用程序可使用它将特定形状关联到已定义的形状类型。 |
| [getText()](#getText--) | 获取此形状的文本。 |
| [getTextBody()](#getTextBody--) | 获取形状文本的设置。 |
| [getTextBoxOptions()](#getTextBoxOptions--) | 获取形状中的文本信息 |
| [getTextDirection()](#getTextDirection--) | 获取此对象的文本流向。 |
| [getTextEffect()](#getTextEffect--) | 返回一个 TextEffectFormat 对象，其中包含指定形状的文本效果格式属性。 |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--) | 获取形状的文本水平对齐类型。 |
| [getTextHorizontalOverflow()](#getTextHorizontalOverflow--) | 获取包含文本的形状的文本水平溢出类型。 |
| [getTextOptions()](#getTextOptions--) | 表示形状的文本选项。 |
| [getTextOrientationType()](#getTextOrientationType--) | 获取形状的文本方向类型。 |
| [getTextShapeType()](#getTextShapeType--) | 获取预设文本形状类型。 |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--) | 获取形状的文本垂直对齐类型。 |
| [getTextVerticalOverflow()](#getTextVerticalOverflow--) | 获取包含文本的形状的文本垂直溢出类型。 |
| [getThreeDFormat()](#getThreeDFormat--) | 获取形状的 3D 格式。 |
| [getTitle()](#getTitle--) | 指定当前形状对象的标题（说明）。 |
| [getTop()](#getTop--) | 表示形状相对于其顶部行的垂直偏移量，单位为像素。 |
| [getTopCM()](#getTopCM--) | 表示形状相对于其顶部行的垂直偏移量，单位为厘米。 |
| [getTopInShape()](#getTopInShape--) | 表示形状相对于父形状顶部边界的垂直偏移量，单位为父形状高度的 1/4000。 |
| [getTopInch()](#getTopInch--) | 表示形状相对于其顶部行的垂直偏移量，单位为英寸。 |
| [getTopToCorner()](#getTopToCorner--) | 获取形状相对于工作表顶部边界的垂直偏移量，单位为像素。 |
| [getType()](#getType--) | 获取自动形状类型。 |
| [getUpperDeltaX()](#getUpperDeltaX--) | 获取形状相对于其左上角列的水平偏移量。 |
| [getUpperDeltaY()](#getUpperDeltaY--) | 获取形状相对于其左上角行的垂直偏移量。 |
| [getUpperLeftColumn()](#getUpperLeftColumn--) | 表示左上角列索引。 |
| [getUpperLeftRow()](#getUpperLeftRow--) | 表示顶部行索引。 |
| [getWidth()](#getWidth--) | 表示形状的宽度，单位为像素。 |
| [getWidthCM()](#getWidthCM--) | 表示形状的宽度，单位为厘米。 |
| [getWidthInShape()](#getWidthInShape--) | 表示形状的宽度，单位为父形状的 1/4000。 |
| [getWidthInch()](#getWidthInch--) | 表示形状的宽度，单位为英寸。 |
| [getWidthPt()](#getWidthPt--) | 表示形状的宽度，单位为点。 |
| [getWidthScale()](#getWidthScale--) | 获取宽度比例，单位为原始图片宽度的百分比。 |
| [getWorksheet()](#getWorksheet--) | 获取包含此形状的 [Worksheet](../../com.aspose.cells/worksheet) 对象。 |
| [getX()](#getX--) | 获取形状相对于工作表左边界的水平偏移，单位为像素。 |
| [getY()](#getY--) | 获取形状相对于工作表顶部边界的垂直偏移，单位为像素。 |
| [getZOrderPosition()](#getZOrderPosition--) | 返回形状在 Z 顺序中的位置。 |
| [hasLine()](#hasLine--) | 获取形状的线边框是否可见。 |
| [hashCode()](#hashCode--) |  |
| [isAspectRatioLocked()](#isAspectRatioLocked--) | True 表示形状的宽高比被锁定。 |
| [isDecorative()](#isDecorative--) | 指示对象是否为装饰性的。 |
| [isEquation()](#isEquation--) | 指示形状是否仅包含一个公式。 |
| [isFilled()](#isFilled--) | 指示填充格式是否可见。 |
| [isFlippedHorizontally()](#isFlippedHorizontally--) | 获取形状是否水平翻转。 |
| [isFlippedVertically()](#isFlippedVertically--) | 获取形状是否垂直翻转。 |
| [isGroup()](#isGroup--) | 指示此形状是否为组合形状。 |
| [isHidden()](#isHidden--) | 指示对象是否可见。 |
| [isInGroup()](#isInGroup--) | 指示形状是否已分组。 |
| [isLockAspectRatio()](#isLockAspectRatio--) | True 表示形状的宽高比被锁定。 |
| [isLocked()](#isLocked--) | True 表示在工作表受保护时对象不能被修改。 |
| [isPrintable()](#isPrintable--) | 指示对象是否可打印。 |
| [isRichText()](#isRichText--) | 指示文本是否为富文本。 |
| [isSameSetting(Object obj)](#isSameSetting-java.lang.Object-) | 返回形状是否相同。 |
| [isSmartArt()](#isSmartArt--) | 指示形状是否为智能艺术。 |
| [isTextWrapped()](#isTextWrapped--) | 获取包含文本的形状的文本换行类型。 |
| [isWordArt()](#isWordArt--) | 指示此形状是否为文字艺术。 |
| [moveToRange(int topRow, int leftColumn, int bottomRow, int rightColumn)](#moveToRange-int-int-int-int-) | 将形状移动到指定范围。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeActiveXControl()](#removeActiveXControl--) | 移除 ActiveX 控件。 |
| [removeHyperlink()](#removeHyperlink--) | 移除形状的超链接。 |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | 返回或设置 [Shape](../../com.aspose.cells/shape) 对象的描述性（替代）文本字符串。 |
| [setAnchorType(int value)](#setAnchorType-int-) | 设置形状锚点占位符的类型。 |
| [setAspectRatioLocked(boolean value)](#setAspectRatioLocked-boolean-) | True 表示形状的宽高比被锁定。 |
| [setAutoShapeType(int value)](#setAutoShapeType-int-) | 设置自动形状类型。 |
| [setBottom(int value)](#setBottom-int-) | 表示形状从其左下角行的垂直偏移宽度，单位为像素。 |
| [setCreateId(UUID value)](#setCreateId-java.util.UUID-) | 为此形状设置创建 ID。 |
| [setDecorative(boolean value)](#setDecorative-boolean-) | 指示对象是否为装饰性的。 |
| [setFilled(boolean value)](#setFilled-boolean-) | 指示填充格式是否可见。 |
| [setFlippedHorizontally(boolean value)](#setFlippedHorizontally-boolean-) | 设置形状是否水平翻转。 |
| [setFlippedVertically(boolean value)](#setFlippedVertically-boolean-) | 设置形状是否垂直翻转。 |
| [setFont(Font value)](#setFont-com.aspose.cells.Font-) | 表示形状的字体。 |
| [setHasLine(boolean value)](#setHasLine-boolean-) | 设置形状的线条边框是否可见。 |
| [setHeight(int value)](#setHeight-int-) | 表示形状的高度，单位为像素。 |
| [setHeightCM(double value)](#setHeightCM-double-) | 表示形状的高度，单位为厘米。 |
| [setHeightInShape(int value)](#setHeightInShape-int-) | 表示形状相对于父形状顶部边界的垂直偏移，单位为父形状高度的 1/4000。 |
| [setHeightInch(double value)](#setHeightInch-double-) | 表示形状的高度，单位为英寸。 |
| [setHeightPt(double value)](#setHeightPt-double-) | 表示形状的高度，单位为点。 |
| [setHeightScale(int value)](#setHeightScale-int-) | 设置高度比例，以原始图片高度的百分比为单位。 |
| [setHidden(boolean value)](#setHidden-boolean-) | 指示对象是否可见。 |
| [setHtmlText(String value)](#setHtmlText-java.lang.String-) | 设置包含数据和某些格式的 HTML 字符串到此文本框。 |
| [setInputRange(String value)](#setInputRange-java.lang.String-) | 设置用于填充指定组合框的工作表范围。 |
| [setInputRange(String formula, boolean isR1C1, boolean isLocal)](#setInputRange-java.lang.String-boolean-boolean-) | 设置用于填充控件的范围。 |
| [setLeft(int value)](#setLeft-int-) | 表示形状相对于其左列的水平偏移，单位为像素。 |
| [setLeftCM(double value)](#setLeftCM-double-) | 表示形状相对于其左列的水平偏移，单位为厘米。 |
| [setLeftInShape(int value)](#setLeftInShape-int-) | 表示形状相对于父形状左边框的水平偏移，单位为父形状宽度的 1/4000。 |
| [setLeftInch(double value)](#setLeftInch-double-) | 表示形状相对于其左列的水平偏移，单位为英寸。 |
| [setLeftToCorner(int value)](#setLeftToCorner-int-) | 设置形状相对于工作表左边界的水平偏移。 |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | 设置与控件值关联的工作表范围。 |
| [setLinkedCell(String formula, boolean isR1C1, boolean isLocal)](#setLinkedCell-java.lang.String-boolean-boolean-) | 设置与控件值关联的范围。 |
| [setLockAspectRatio(boolean value)](#setLockAspectRatio-boolean-) | True 表示形状的宽高比被锁定。 |
| [setLocked(boolean value)](#setLocked-boolean-) | True 表示在工作表受保护时对象不能被修改。 |
| [setLockedProperty(int type, boolean value)](#setLockedProperty-int-boolean-) | 设置锁定属性。 |
| [setLowerDeltaX(int value)](#setLowerDeltaX-int-) | 设置形状相对于其右下角列的水平偏移。 |
| [setLowerDeltaY(int value)](#setLowerDeltaY-int-) | 设置形状相对于其右下角行的垂直偏移。 |
| [setLowerRightColumn(int value)](#setLowerRightColumn-int-) | 表示右下角列索引。 |
| [setLowerRightRow(int value)](#setLowerRightRow-int-) | 表示右下角行索引。 |
| [setMacroName(String value)](#setMacroName-java.lang.String-) | 设置宏的名称。 |
| [setName(String value)](#setName-java.lang.String-) | 设置形状的名称。 |
| [setPlacement(int value)](#setPlacement-int-) | 表示绘图对象附着在其下方单元格的方式。 |
| [setPrintable(boolean value)](#setPrintable-boolean-) | 指示对象是否可打印。 |
| [setRelativeToOriginalPictureSize(boolean value)](#setRelativeToOriginalPictureSize-boolean-) | 指示形状是否相对于原始图片尺寸。 |
| [setRight(int value)](#setRight-int-) | 表示形状相对于其右下角列的水平偏移宽度，单位为像素。 |
| [setRotationAngle(double value)](#setRotationAngle-double-) | 设置形状的旋转角度。 |
| [setSoftEdges(double value)](#setSoftEdges-double-) | 设置要应用于边缘的模糊半径，单位为点。 |
| [setText(String value)](#setText-java.lang.String-) | 设置此形状的文本。 |
| [setTextDirection(int value)](#setTextDirection-int-) | 设置此对象的文本流方向。 |
| [setTextHorizontalAlignment(int value)](#setTextHorizontalAlignment-int-) | 设置形状的文本水平对齐类型。 |
| [setTextHorizontalOverflow(int value)](#setTextHorizontalOverflow-int-) | 设置包含文本的形状的文本水平溢出类型。 |
| [setTextOptions(TextOptions value)](#setTextOptions-com.aspose.cells.TextOptions-) | 表示形状的文本选项。 |
| [setTextOrientationType(int value)](#setTextOrientationType-int-) | 设置形状的文本方向类型。 |
| [setTextShapeType(int value)](#setTextShapeType-int-) | 设置预设文本形状类型。 |
| [setTextVerticalAlignment(int value)](#setTextVerticalAlignment-int-) | 设置形状的文本垂直对齐类型。 |
| [setTextVerticalOverflow(int value)](#setTextVerticalOverflow-int-) | 设置包含文本的形状的文本垂直溢出类型。 |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | 设置包含文本的形状的文本换行类型。 |
| [setTitle(String value)](#setTitle-java.lang.String-) | 指定当前形状对象的标题（说明）。 |
| [setTop(int value)](#setTop-int-) | 表示形状相对于其顶部行的垂直偏移量，单位为像素。 |
| [setTopCM(double value)](#setTopCM-double-) | 表示形状相对于其顶部行的垂直偏移量，单位为厘米。 |
| [setTopInShape(int value)](#setTopInShape-int-) | 表示形状相对于父形状顶部边界的垂直偏移量，单位为父形状高度的 1/4000。 |
| [setTopInch(double value)](#setTopInch-double-) | 表示形状相对于其顶部行的垂直偏移量，单位为英寸。 |
| [setTopToCorner(int value)](#setTopToCorner-int-) | 设置形状相对于工作表顶部边界的垂直偏移，单位为像素。 |
| [setUpperDeltaX(int value)](#setUpperDeltaX-int-) | 设置形状相对于其左上角列的水平偏移。 |
| [setUpperDeltaY(int value)](#setUpperDeltaY-int-) | 设置形状相对于其左上角行的垂直偏移。 |
| [setUpperLeftColumn(int value)](#setUpperLeftColumn-int-) | 表示左上角列索引。 |
| [setUpperLeftRow(int value)](#setUpperLeftRow-int-) | 表示顶部行索引。 |
| [setWidth(int value)](#setWidth-int-) | 表示形状的宽度，单位为像素。 |
| [setWidthCM(double value)](#setWidthCM-double-) | 表示形状的宽度，单位为厘米。 |
| [setWidthInShape(int value)](#setWidthInShape-int-) | 表示形状的宽度，单位为父形状的 1/4000。 |
| [setWidthInch(double value)](#setWidthInch-double-) | 表示形状的宽度，单位为英寸。 |
| [setWidthPt(double value)](#setWidthPt-double-) | 表示形状的宽度，单位为点。 |
| [setWidthScale(int value)](#setWidthScale-int-) | 设置宽度比例，单位为原始图片宽度的百分比。 |
| [setX(int value)](#setX-int-) | 设置形状相对于工作表左边界的水平偏移，单位为像素。 |
| [setY(int value)](#setY-int-) | 设置形状相对于工作表顶部边界的垂直偏移，单位为像素。 |
| [setZOrderPosition(int value)](#setZOrderPosition-int-) | 返回形状在 Z 顺序中的位置。 |
| [toFrontOrBack(int orders)](#toFrontOrBack-int-) | 将形状置于前面或发送到后面。 |
| [toImage(OutputStream stream, ImageFormat imageFormat)](#toImage-java.io.OutputStream-com.aspose.cells.ImageFormat-) | 创建形状图像并以指定格式保存到流中。 |
| [toImage(OutputStream stream, ImageOrPrintOptions options)](#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-) | 将形状保存到流中。 |
| [toImage(String imageFile, ImageOrPrintOptions options)](#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-) | 将形状保存到文件中。 |
| [toString()](#toString--) |  |
| [updateSelectedValue()](#updateSelectedValue--) | 通过链接单元格的值更新选定的值。 |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addHyperlink(String address) {#addHyperlink-java.lang.String-}
```
public Hyperlink addHyperlink(String address)
```


向形状添加超链接。

**Example**

```
         Hyperlink hyperlink = shape.addHyperlink("https://www.aspose.com/");
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 地址 | java.lang.String | 超链接的地址。 |

**Returns:**
[Hyperlink](../../com.aspose.cells/hyperlink) - Returns the new hyperlink object.
### alignTopRightCorner(int topRow, int rightColumn) {#alignTopRightCorner-int-int-}
```
public void alignTopRightCorner(int topRow, int rightColumn)
```


将图片移动到右上角。

**Example**

```
         shape.alignTopRightCorner(2, 5);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| topRow | int | 行索引。 |
| rightColumn | int | 列索引。 |

### calculateTextSize() {#calculateTextSize--}
```
public int[] calculateTextSize()
```


重新计算文本区域

**Example**

```
         //The size of the text area is:w=size[0],h=size[1]
         int[] size = shape.calculateTextSize();
```

**Returns:**
int[] - 文本的大小以数组形式（宽度和高度）。
### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```


返回一个 Characters 对象，表示文本中的字符范围。

**Remarks**

此方法仅适用于带标题的形状。

**Example**

```
         FontSetting fontSetting = shape.characters(0, 4);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startIndex | int | 字符起始位置的索引。 |
| length | int | 字符数。 |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - Characters object.
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### fitToTextSize() {#fitToTextSize--}
```
public void fitToTextSize()
```


重新计算适合显示所有文本内容的文本区域。

**Example**

```
         if (shape.getName().startsWith("Your traget"))
         {
             shape.fitToTextSize();
         }
```

### formatCharacters(int startIndex, int length, Font font, StyleFlag flag) {#formatCharacters-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-}
```
public void formatCharacters(int startIndex, int length, Font font, StyleFlag flag)
```


使用字体设置格式化部分字符。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startIndex | int | 起始索引。 |
| length | int | 长度。 |
| font | [Font](../../com.aspose.cells/font) | 字体设置。 |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | 字体设置的标志。 |

### getActiveXControl() {#getActiveXControl--}
```
public ActiveXControl getActiveXControl()
```


获取 ActiveX 控件。

**Example**

```
         if(shape.getActiveXControl() != null)
         {
             CheckBoxActiveXControl checkBox1 = (CheckBoxActiveXControl)shape.getActiveXControl();
             //The font name of CheckBox
             String fontName = checkBox1.getFont().getName();
         }
```

**Returns:**
[ActiveXControl](../../com.aspose.cells/activexcontrol)
### getActualBox() {#getActualBox--}
```
public float[] getActualBox()
```


获取形状的实际位置和大小（在应用旋转、翻转等之后）。

**Remarks**

注意：该接口功能不完整，尤其是位置信息不正确。建议在功能完善之前不要使用此接口。

**Example**

```
         float[] box = shape.getActualBox();
         System.out.println("x = " + box[0]);
         System.out.println("y = " + box[1]);
         System.out.println("w = " + box[2]);
         System.out.println("h = " + box[3]);
```

**Returns:**
float[] - 按 x、y、w、h 顺序返回位置和大小。
### getActualLowerRightRow() {#getActualLowerRightRow--}
```
public int getActualLowerRightRow()
```


获取实际的底部行。

**Example**

```
         int rRow = shape.getActualLowerRightRow();
```

**Returns:**
int
### getAlternativeText() {#getAlternativeText--}
```
public String getAlternativeText()
```


返回或设置 [Shape](../../com.aspose.cells/shape) 对象的描述性（替代）文本字符串。

**Example**

```
         shape.setAlternativeText("a rectangle");
```

**Returns:**
java.lang.String
### getAnchorType() {#getAnchorType--}
```
public int getAnchorType()
```


获取形状锚点占位符的类型。

参见 [ShapeAnchorType](../../com.aspose.cells/shapeanchortype)。

**Example**

```
         if (shape.getAnchorType() == ShapeAnchorType.ONE_CELL_ANCHOR)
             shape.setAnchorType(ShapeAnchorType.TWO_CELL_ANCHOR);
```

**Returns:**
int
### getAutoShapeType() {#getAutoShapeType--}
```
public int getAutoShapeType()
```


获取自动形状类型。

参见 [AutoShapeType](../../com.aspose.cells/autoshapetype)。

**Example**

```
         if (shape.getAutoShapeType() == com.aspose.cells.AutoShapeType.UNKNOWN)
             shape.setAutoShapeType(com.aspose.cells.AutoShapeType.RECTANGLE);
```

**Returns:**
int
### getBottom() {#getBottom--}
```
public int getBottom()
```


表示形状从其左下角行的垂直偏移宽度，单位为像素。

**Example**

```
         if (shape.getBottom() == 3)
             shape.setBottom(1);
```

**Returns:**
int
### getCharacters() {#getCharacters--}
```
public ArrayList getCharacters()
```


返回表示文本中字符范围的所有 Characters 对象。

**Remarks**

注意：此方法已过时。请改用 Shape.GetRichFormattings() 方法。该方法将在自2023年11月起的12个月后被移除。Aspose 对给您带来的任何不便表示歉意。

**Example**

```
         FontSetting fontSetting = shape.characters(0, 4);
```

**Returns:**
java.util.ArrayList - 所有 Characters 对象
### getChart() {#getChart--}
```
public Chart getChart()
```


返回一个表示对象中包含的图表的 Chart 对象。

**Returns:**
[Chart](../../com.aspose.cells/chart)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getConnectionPoints() {#getConnectionPoints--}
```
public float[][] getConnectionPoints()
```


获取连接点

**Example**

```
         float[][] points = shape.getConnectionPoints();
```

**Returns:**
float[][] - 连接点的 [X,Y] 对。每个项都是一个 float[2] 数组，[0] 表示 x，[1] 表示 y。
### getControlData() {#getControlData--}
```
public byte[] getControlData()
```


获取控件的数据。

**Example**

```
         if(shape.getControlData() == null)
             System.out.println("No data.");
```

**Returns:**
byte[]
### getCreateId() {#getCreateId--}
```
public UUID getCreateId()
```


获取此形状的创建 ID。

**Example**

```
         System.out.println(shape.getCreateId());
         java.util.UUID g = java.util.UUID.randomUUID();
         shape.setCreateId(g);
         System.out.println(shape.getCreateId());
```

**Returns:**
java.util.UUID
### getFill() {#getFill--}
```
public FillFormat getFill()
```


返回一个 [getFillFormat()](../../com.aspose.cells/shape\\#getFillFormat--) 对象，该对象包含指定形状的填充格式属性。

**Example**

```
         FillFormat fillFmt = shape.getFill();
```

**Returns:**
[FillFormat](../../com.aspose.cells/fillformat)
### getFillFormat() {#getFillFormat--}
```
public MsoFillFormat getFillFormat()
```


返回一个 MsoFillFormat 对象，该对象包含指定形状的填充格式属性。

**Remarks**

注意：此成员已过时。请改用 Shape.Fill 属性。该属性将在自2016年7月起的12个月后被移除。Aspose 对给您带来的任何不便表示歉意。

**Returns:**
[MsoFillFormat](../../com.aspose.cells/msofillformat)
### getFont() {#getFont--}
```
public Font getFont()
```


表示形状的字体。

**Example**

```
         Font font = shape.getFont();
         font.setName("Arial");
         font.setSize(12);
         font.setColor(Color.getRed());
```

**Returns:**
[Font](../../com.aspose.cells/font)
### getFormatPicture() {#getFormatPicture--}
```
public MsoFormatPicture getFormatPicture()
```


获取图片格式的选项。

**Example**

```
         MsoFormatPicture msoFormatPicture = shape.getFormatPicture();
```

**Returns:**
[MsoFormatPicture](../../com.aspose.cells/msoformatpicture)
### getGeometry() {#getGeometry--}
```
public Geometry getGeometry()
```


获取几何形状

**Example**

```
         if (shape.getGeometry() != null &&shape.getGeometry().getShapeAdjustValues().getCount() == 0)
             System.out.println("No geometry path.");
```

**Returns:**
[Geometry](../../com.aspose.cells/geometry)
### getGlow() {#getGlow--}
```
public GlowEffect getGlow()
```


表示一个 [GlowEffect](../../com.aspose.cells/gloweffect) 对象，用于指定图表元素或形状的发光效果。

**Example**

```
         GlowEffect glowEffect = shape.getGlow();
```

**Returns:**
[GlowEffect](../../com.aspose.cells/gloweffect)
### getGroup() {#getGroup--}
```
public GroupShape getGroup()
```


获取包含此形状的组形状。

**Example**

```
         GroupShape groupShape = shape.getGroup();
```

**Returns:**
[GroupShape](../../com.aspose.cells/groupshape)
### getHeight() {#getHeight--}
```
public int getHeight()
```


表示形状的高度，单位为像素。

**Example**

```
         if (shape.getHeight() == 3)
             shape.setHeight(1);
```

**Returns:**
int
### getHeightCM() {#getHeightCM--}
```
public double getHeightCM()
```


表示形状的高度，单位为厘米。

**Example**

```
         if (shape.getHeightCM() == 3)
             shape.setHeightCM(1);
```

**Returns:**
double
### getHeightInShape() {#getHeightInShape--}
```
public int getHeightInShape()
```


表示形状相对于父形状顶部边界的垂直偏移，单位为父形状高度的 1/4000。

**Remarks**

仅在此形状位于组或图表中时适用。

**Example**

```
         if (shape.isInGroup() &&shape.getHeightInShape() == 4000)
             shape.setHeightInShape(2000);
```

**Returns:**
int
### getHeightInch() {#getHeightInch--}
```
public double getHeightInch()
```


表示形状的高度，单位为英寸。

**Example**

```
         if (shape.getHeightInch() == 3)
             shape.setHeightInch(1);
```

**Returns:**
double
### getHeightPt() {#getHeightPt--}
```
public double getHeightPt()
```


表示形状的高度，单位为点。

**Example**

```
         if (shape.getHeightPt() == 3)
             shape.setHeightPt(1);
```

**Returns:**
double
### getHeightScale() {#getHeightScale--}
```
public int getHeightScale()
```


获取高度比例，单位为原始图片高度的百分比。如果形状不是图片，HeightScale 属性仅返回 100；

**Example**

```
         if (shape.getHeightScale() == 3)
             shape.setHeightScale(1);
```

**Returns:**
int
### getHtmlText() {#getHtmlText--}
```
public String getHtmlText()
```


获取包含此文本框中数据和部分格式的 HTML 字符串。

**Example**

```
         String html = shape.getHtmlText();
         if(html == null || "".equals(html))
         {
             shape.setHtmlText("<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>");
         }
```

**Returns:**
java.lang.String
### getHyperlink() {#getHyperlink--}
```
public Hyperlink getHyperlink()
```


获取形状的超链接。

**Example**

```
         Hyperlink hyperlink = shape.getHyperlink();
```

**Returns:**
[Hyperlink](../../com.aspose.cells/hyperlink)
### getId() {#getId--}
```
public int getId()
```


获取此形状的标识符。

**Example**

```
         int id = shape.getId();
```

**Returns:**
int
### getInputRange() {#getInputRange--}
```
public String getInputRange()
```


获取用于填充指定组合框的工作表范围。

**Example**

```
         if (shape.getInputRange().equals("$B$6:$B10"))
             shape.setInputRange("$A$1:$A$5");
```

**Returns:**
java.lang.String
### getInputRange(boolean isR1C1, boolean isLocal) {#getInputRange-boolean-boolean-}
```
public String getInputRange(boolean isR1C1, boolean isLocal)
```


获取用于填充控件的范围。

**Example**

```
         String range = shape.getInputRange(false, true);
         //If successful, a value like "$A$1:$A$3" will be returned
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| isR1C1 | boolean | 公式是否需要以 R1C1 格式化。 |
| isLocal | boolean | 公式是否需要根据区域设置进行格式化。 |

**Returns:**
java.lang.String - 用于填充控件的范围。
### getLeft() {#getLeft--}
```
public int getLeft()
```


表示形状相对于其左列的水平偏移，单位为像素。

**Example**

```
         if (shape.getLeft() == 3)
             shape.setLeft(1);
```

**Returns:**
int
### getLeftCM() {#getLeftCM--}
```
public double getLeftCM()
```


表示形状相对于其左列的水平偏移，单位为厘米。

**Example**

```
         if (shape.getLeftCM() == 3)
             shape.setLeftCM(1);
```

**Returns:**
double
### getLeftInShape() {#getLeftInShape--}
```
public int getLeftInShape()
```


表示形状相对于父形状左边框的水平偏移，单位为父形状宽度的 1/4000。

**Remarks**

仅在此形状位于组或图表中时适用。

**Example**

```
         if (shape.isInGroup() &&shape.getLeftInShape() == 2000)
             shape.setLeftInShape(4000);
```

**Returns:**
int
### getLeftInch() {#getLeftInch--}
```
public double getLeftInch()
```


表示形状相对于其左列的水平偏移，单位为英寸。

**Example**

```
         if (shape.getLeftInch() == 3)
             shape.setLeftInch(1);
```

**Returns:**
double
### getLeftToCorner() {#getLeftToCorner--}
```
public int getLeftToCorner()
```


获取形状相对于工作表左边框的水平偏移。

**Example**

```
         if (shape.getLeftToCorner() == 3)
             shape.setLeftToCorner(1);
```

**Returns:**
int
### getLine() {#getLine--}
```
public LineFormat getLine()
```


获取线条样式

**Example**

```
         LineFormat lineFmt = shape.getLine();
```

**Returns:**
[LineFormat](../../com.aspose.cells/lineformat)
### getLineFormat() {#getLineFormat--}
```
public MsoLineFormat getLineFormat()
```


返回一个 MsoLineFormat 对象，其中包含指定形状的线条格式属性。

**Remarks**

注意：此成员已过时。请改用 Shape.Line 属性。此属性将在自 2016 年 7 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
[MsoLineFormat](../../com.aspose.cells/msolineformat)
### getLinkedCell() {#getLinkedCell--}
```
public String getLinkedCell()
```


获取与控件值关联的工作表范围。

**Example**

```
         if (shape.getLinkedCell().equals("$B$6"))
         {
             shape.setLinkedCell("A1");
         }
         shape.updateSelectedValue();
```

**Returns:**
java.lang.String
### getLinkedCell(boolean isR1C1, boolean isLocal) {#getLinkedCell-boolean-boolean-}
```
public String getLinkedCell(boolean isR1C1, boolean isLocal)
```


获取与控件值关联的范围。

**Example**

```
         //You may get results like '$A$1'
         String link = shape.getLinkedCell(false, false);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| isR1C1 | boolean | 公式是否需要以 R1C1 格式化。 |
| isLocal | boolean | 公式是否需要根据区域设置进行格式化。 |

**Returns:**
java.lang.String - 与控件值关联的范围。
### getLockedProperty(int type) {#getLockedProperty-int-}
```
public boolean getLockedProperty(int type)
```


获取 locked 属性的值。

**Example**

```
         int noAdjustHandles = 0;
         if (shape.getLockedProperty(ShapeLockType.ADJUST_HANDLES))
             noAdjustHandles = 1;
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [ShapeLockType](../../com.aspose.cells/shapelocktype)。形状锁定属性的类型。 |

**Returns:**
boolean - 返回锁定属性的值。
### getLowerDeltaX() {#getLowerDeltaX--}
```
public int getLowerDeltaX()
```


获取形状相对于其右下角列的水平偏移。

**Remarks**

值的范围是 0 到 1024。

**Example**

```
         if (shape.getLowerDeltaX() == 3)
             shape.setLowerDeltaX(1);
```

**Returns:**
int
### getLowerDeltaY() {#getLowerDeltaY--}
```
public int getLowerDeltaY()
```


获取形状相对于其右下角行的垂直偏移。

**Remarks**

值的范围是 0 到 256。

**Example**

```
         if (shape.getLowerDeltaY() == 3)
             shape.setLowerDeltaY(1);
```

**Returns:**
int
### getLowerRightColumn() {#getLowerRightColumn--}
```
public int getLowerRightColumn()
```


表示右下角列索引。

**Example**

```
         if (shape.getLowerRightColumn() == 3)
             shape.setLowerRightColumn(1);
```

**Returns:**
int
### getLowerRightRow() {#getLowerRightRow--}
```
public int getLowerRightRow()
```


表示右下角行索引。

**Example**

```
         if (shape.getLowerRightRow() == 3)
             shape.setLowerRightRow(1);
```

**Returns:**
int
### getMacroName() {#getMacroName--}
```
public String getMacroName()
```


获取宏的名称。

**Example**

```
         //Sets the name of macro.
         shape.setMacroName("DoWork()");
```

**Returns:**
java.lang.String
### getMsoDrawingType() {#getMsoDrawingType--}
```
public int getMsoDrawingType()
```


获取绘图类型。

参见 [MsoDrawingType](../../com.aspose.cells/msodrawingtype)。

**Example**

```
         /*Aspose.Cells.Drawing.MsoDrawingType*/int msoDrawingType = shape.getMsoDrawingType();
```

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


获取形状的名称。

**Example**

```
         shape.setName("shape1");
```

**Returns:**
java.lang.String
### getPaths() {#getPaths--}
```
public ShapePathCollection getPaths()
```


获取自定义几何形状的路径。

**Example**

```
         //Returns non-null if there is a path to the custom geometry
         if(shape.getPaths() == null)
             System.out.println("No custom geometry path.");
```

**Returns:**
[ShapePathCollection](../../com.aspose.cells/shapepathcollection)
### getPlacement() {#getPlacement--}
```
public int getPlacement()
```


表示绘图对象附着在其下方单元格的方式。该属性控制对象在工作表上的放置位置。

参见 [PlacementType](../../com.aspose.cells/placementtype)。

**Example**

```
         if (shape.getPlacement() == PlacementType.MOVE)
             shape.setPlacement(PlacementType.MOVE_AND_SIZE);
```

**Returns:**
int
### getReflection() {#getReflection--}
```
public ReflectionEffect getReflection()
```


表示一个 [ReflectionEffect](../../com.aspose.cells/reflectioneffect) 对象，用于指定图表元素或形状的反射效果。

**Example**

```
         ReflectionEffect reflectionEffect = shape.getReflection();
```

**Returns:**
[ReflectionEffect](../../com.aspose.cells/reflectioneffect)
### getRelativeToOriginalPictureSize() {#getRelativeToOriginalPictureSize--}
```
public boolean getRelativeToOriginalPictureSize()
```


指示形状是否相对于原始图片尺寸。

**Example**

```
         if(shape.getRelativeToOriginalPictureSize())
             shape.setRelativeToOriginalPictureSize(false);
```

**Returns:**
boolean
### getResultOfSmartArt() {#getResultOfSmartArt--}
```
public GroupShape getResultOfSmartArt()
```


将 SmartArt 转换为组合形状。

**Example**

```
         if(shape.isSmartArt())
         {
             GroupShape groupShape = shape.getResultOfSmartArt();
         }
```

**Returns:**
[GroupShape](../../com.aspose.cells/groupshape)
### getRichFormattings() {#getRichFormattings--}
```
public FontSetting[] getRichFormattings()
```


返回表示文本中字符范围的所有 Characters 对象。

**Example**

```
         FontSetting[] list = shape.getRichFormattings();
```

**Returns:**
com.aspose.cells.FontSetting[] - 所有字符对象
### getRight() {#getRight--}
```
public int getRight()
```


表示形状相对于其右下角列的水平偏移宽度，单位为像素。

**Example**

```
         if (shape.getRight() == 3)
             shape.setRight(1);
```

**Returns:**
int
### getRotationAngle() {#getRotationAngle--}
```
public double getRotationAngle()
```


获取形状的旋转角度。

**Example**

```
         //Gets rotation angle of the shape.
         double angle = shape.getRotationAngle() ;
 
         //Gets rotation angle of the shape.
          shape.setRotationAngle(60);
```

**Returns:**
double
### getShadowEffect() {#getShadowEffect--}
```
public ShadowEffect getShadowEffect()
```


表示一个 [ShadowEffect](../../com.aspose.cells/shadoweffect) 对象，用于指定图表元素或形状的阴影效果。

**Example**

```
         ShadowEffect shadowEffect = shape.getShadowEffect();
```

**Returns:**
[ShadowEffect](../../com.aspose.cells/shadoweffect)
### getSoftEdges() {#getSoftEdges--}
```
public double getSoftEdges()
```


获取要应用于边缘的模糊半径，单位为点。

**Example**

```
         shape.setSoftEdges(0.5d);
```

**Returns:**
double
### getSpid() {#getSpid--}
```
public String getSpid()
```


指定一个可选的字符串标识符，应用程序可使用它来标识特定形状。

**Example**

```
         String spid = shape.getSpid();
```

**Returns:**
java.lang.String
### getSpt() {#getSpt--}
```
public int getSpt()
```


指定一个可选的数字，应用程序可使用它将特定形状关联到已定义的形状类型。

**Example**

```
         int spt = shape.getSpt();
```

**Returns:**
int
### getText() {#getText--}
```
public String getText()
```


获取此形状的文本。

**Example**

```
         if(shape.getText() == null)
             shape.setText("This is a test.");
```

**Returns:**
java.lang.String
### getTextBody() {#getTextBody--}
```
public FontSettingCollection getTextBody()
```


获取形状文本的设置。

**Example**

```
         FontSettingCollection fontSettingCollection = shape.getTextBody();
         fontSettingCollection.setText("This is a test.");
```

**Returns:**
[FontSettingCollection](../../com.aspose.cells/fontsettingcollection)
### getTextBoxOptions() {#getTextBoxOptions--}
```
public TextBoxOptions getTextBoxOptions()
```


获取形状中的文本信息

**Example**

```
         TextBoxOptions textBoxOpt = shape.getTextBoxOptions();
         textBoxOpt.setShapeTextVerticalAlignment(ShapeTextVerticalAlignmentType.LEFT);
         textBoxOpt.setTopMarginPt(0.2d);
         textBoxOpt.setLeftMarginPt(0.2d);
         textBoxOpt.setRightMarginPt(0.2d);
         textBoxOpt.setBottomMarginPt(0.2d);
```

**Returns:**
[TextBoxOptions](../../com.aspose.cells/textboxoptions)
### getTextDirection() {#getTextDirection--}
```
public int getTextDirection()
```


获取此对象的文本流向。

参见 [TextDirectionType](../../com.aspose.cells/textdirectiontype)。

**Example**

```
         if (shape.getTextDirection() == com.aspose.cells.TextDirectionType.CONTEXT)
             shape.setTextDirection(com.aspose.cells.TextDirectionType.LEFT_TO_RIGHT);
```

**Returns:**
int
### getTextEffect() {#getTextEffect--}
```
public TextEffectFormat getTextEffect()
```


返回一个 TextEffectFormat 对象，其中包含指定形状的文字效果格式属性。适用于表示 WordArt 的 Shape 对象。

**Example**

```
         if(shape.isWordArt())
         {
             TextEffectFormat textEffectFormat = shape.getTextEffect();
         }
```

**Returns:**
[TextEffectFormat](../../com.aspose.cells/texteffectformat)
### getTextHorizontalAlignment() {#getTextHorizontalAlignment--}
```
public int getTextHorizontalAlignment()
```


获取形状的文本水平对齐类型。

参见 [TextAlignmentType](../../com.aspose.cells/textalignmenttype)。

**Example**

```
         if (shape.getTextHorizontalAlignment() == com.aspose.cells.TextAlignmentType.BOTTOM)
             shape.setTextHorizontalAlignment(com.aspose.cells.TextAlignmentType.CENTER);
```

**Returns:**
int
### getTextHorizontalOverflow() {#getTextHorizontalOverflow--}
```
public int getTextHorizontalOverflow()
```


获取包含文本的形状的文本水平溢出类型。

参见 [TextOverflowType](../../com.aspose.cells/textoverflowtype)。

**Example**

```
         if (shape.getTextHorizontalOverflow() == com.aspose.cells.TextOverflowType.CLIP)
             shape.setTextHorizontalOverflow(com.aspose.cells.TextOverflowType.OVERFLOW);
```

**Returns:**
int
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


表示形状的文本选项。

**Example**

```
         TextOptions opt = shape.getTextOptions();
         opt.setColor(Color.getBlue());
         opt.setSize(8);
```

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getTextOrientationType() {#getTextOrientationType--}
```
public int getTextOrientationType()
```


获取形状的文本方向类型。

参见 [TextOrientationType](../../com.aspose.cells/textorientationtype)。

**Example**

```
         if (shape.getTextOrientationType() == com.aspose.cells.TextOrientationType.NO_ROTATION)
             shape.setTextOrientationType(com.aspose.cells.TextOrientationType.TOP_TO_BOTTOM);
```

**Returns:**
int
### getTextShapeType() {#getTextShapeType--}
```
public int getTextShapeType()
```


获取预设文本形状类型。

参见 [AutoShapeType](../../com.aspose.cells/autoshapetype)。

**Example**

```
         if (shape.getTextShapeType() == com.aspose.cells.AutoShapeType.UNKNOWN)
             shape.setTextShapeType(com.aspose.cells.AutoShapeType.RECTANGLE);
```

**Returns:**
int
### getTextVerticalAlignment() {#getTextVerticalAlignment--}
```
public int getTextVerticalAlignment()
```


获取形状的文本垂直对齐类型。

参见 [TextAlignmentType](../../com.aspose.cells/textalignmenttype)。

**Example**

```
         if (shape.getTextVerticalAlignment() == com.aspose.cells.TextAlignmentType.BOTTOM)
             shape.setTextVerticalAlignment(com.aspose.cells.TextAlignmentType.CENTER);
```

**Returns:**
int
### getTextVerticalOverflow() {#getTextVerticalOverflow--}
```
public int getTextVerticalOverflow()
```


获取包含文本的形状的文本垂直溢出类型。

参见 [TextOverflowType](../../com.aspose.cells/textoverflowtype)。

**Example**

```
         if (shape.getTextVerticalOverflow() == com.aspose.cells.TextOverflowType.CLIP)
             shape.setTextVerticalOverflow(com.aspose.cells.TextOverflowType.OVERFLOW);
```

**Returns:**
int
### getThreeDFormat() {#getThreeDFormat--}
```
public ThreeDFormat getThreeDFormat()
```


获取形状的 3D 格式。

**Example**

```
         ThreeDFormat threeDFormat = shape.getThreeDFormat();
```

**Returns:**
[ThreeDFormat](../../com.aspose.cells/threedformat)
### getTitle() {#getTitle--}
```
public String getTitle()
```


指定当前形状对象的标题（说明）。

**Example**

```
         shape.setTitle("title1");
```

**Returns:**
java.lang.String
### getTop() {#getTop--}
```
public int getTop()
```


表示形状相对于其顶部行的垂直偏移量，单位为像素。

**Remarks**

如果形状位于图表中，表示形状相对于其上边框的垂直偏移量。

**Example**

```
         if (shape.getTop() == 3)
             shape.setTop(1);
```

**Returns:**
int
### getTopCM() {#getTopCM--}
```
public double getTopCM()
```


表示形状相对于其顶部行的垂直偏移量，单位为厘米。

**Example**

```
         if (shape.getTopCM() == 3)
             shape.setTopCM(1);
```

**Returns:**
double
### getTopInShape() {#getTopInShape--}
```
public int getTopInShape()
```


表示形状相对于父形状顶部边界的垂直偏移量，单位为父形状高度的 1/4000。

**Remarks**

仅在此形状位于组或图表中时适用。

**Example**

```
         if (shape.isInGroup() &&shape.getTopInShape() == 8000)
             shape.setTopInShape(4000);
```

**Returns:**
int
### getTopInch() {#getTopInch--}
```
public double getTopInch()
```


表示形状相对于其顶部行的垂直偏移量，单位为英寸。

**Example**

```
         if (shape.getTopInch() == 3)
             shape.setTopInch(1);
```

**Returns:**
double
### getTopToCorner() {#getTopToCorner--}
```
public int getTopToCorner()
```


获取形状相对于工作表顶部边界的垂直偏移量，单位为像素。

**Example**

```
         if (shape.getTopToCorner() == 3)
             shape.setTopToCorner(1);
```

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


获取自动形状类型。

参见 [AutoShapeType](../../com.aspose.cells/autoshapetype)。

**Example**

```
         /*Aspose.Cells.Drawing.AutoShapeType*/int autoShapeType = shape.getType();
```

**Returns:**
int
### getUpperDeltaX() {#getUpperDeltaX--}
```
public int getUpperDeltaX()
```


获取形状相对于其左上角列的水平偏移量。

**Remarks**

值的范围是 0 到 1024。

**Example**

```
         if (shape.getUpperDeltaX() == 3)
             shape.setUpperDeltaX(1);
```

**Returns:**
int
### getUpperDeltaY() {#getUpperDeltaY--}
```
public int getUpperDeltaY()
```


获取形状相对于其左上角行的垂直偏移量。

**Remarks**

值的范围是 0 到 256。

**Example**

```
         if (shape.getUpperDeltaY() == 3)
             shape.setUpperDeltaY(1);
```

**Returns:**
int
### getUpperLeftColumn() {#getUpperLeftColumn--}
```
public int getUpperLeftColumn()
```


表示左上角列索引。

**Example**

```
         if (shape.getUpperLeftColumn() == 3)
             shape.setUpperLeftColumn(1);
```

**Returns:**
int
### getUpperLeftRow() {#getUpperLeftRow--}
```
public int getUpperLeftRow()
```


表示顶部行索引。

**Remarks**

如果形状位于形状内部或组中，UpperLeftRow 将被忽略。

**Example**

```
         if (shape.getUpperLeftRow() == 3)
             shape.setUpperLeftRow(1);
```

**Returns:**
int
### getWidth() {#getWidth--}
```
public int getWidth()
```


表示形状的宽度，单位为像素。

**Example**

```
         if (shape.getWidth() == 3)
             shape.setWidth(1);
```

**Returns:**
int
### getWidthCM() {#getWidthCM--}
```
public double getWidthCM()
```


表示形状的宽度，单位为厘米。

**Example**

```
         if (shape.getWidthCM() == 3)
             shape.setWidthCM(1);
```

**Returns:**
double
### getWidthInShape() {#getWidthInShape--}
```
public int getWidthInShape()
```


表示形状的宽度，单位为父形状的 1/4000。

**Remarks**

仅在此形状位于组或图表中时适用。

**Example**

```
         if (shape.isInGroup() &&shape.getWidthInShape() == 2000)
             shape.setWidthInShape(4000);
```

**Returns:**
int
### getWidthInch() {#getWidthInch--}
```
public double getWidthInch()
```


表示形状的宽度，单位为英寸。

**Example**

```
         if (shape.getWidthInch() == 3)
             shape.setWidthInch(1);
```

**Returns:**
double
### getWidthPt() {#getWidthPt--}
```
public double getWidthPt()
```


表示形状的宽度，单位为点。

**Example**

```
         if (shape.getWidthPt() == 3)
             shape.setWidthPt(1);
```

**Returns:**
double
### getWidthScale() {#getWidthScale--}
```
public int getWidthScale()
```


获取宽度比例，单位为原始图片宽度的百分比。如果形状不是图片，WidthScale 属性仅返回 100；

**Example**

```
         if (shape.getWidthScale() == 3)
             shape.setWidthScale(1);
```

**Returns:**
int
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


获取包含此形状的 [Worksheet](../../com.aspose.cells/worksheet) 对象。

**Example**

```
         Worksheet worksheet = shape.getWorksheet();
```

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### getX() {#getX--}
```
public int getX()
```


获取形状相对于工作表左边界的水平偏移，单位为像素。

**Example**

```
         if (shape.getX() == 3)
             shape.setX(1);
```

**Returns:**
int
### getY() {#getY--}
```
public int getY()
```


获取形状相对于工作表顶部边界的垂直偏移，单位为像素。

**Example**

```
         if (shape.getY() == 3)
             shape.setY(1);
```

**Returns:**
int
### getZOrderPosition() {#getZOrderPosition--}
```
public int getZOrderPosition()
```


返回形状在 Z 顺序中的位置。

**Example**

```
         shape.setZOrderPosition(3);
```

**Returns:**
int
### hasLine() {#hasLine--}
```
public boolean hasLine()
```


获取形状的线边框是否可见。

**Example**

```
         if(shape.hasLine() == false)
             shape.setHasLine(true);
```

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAspectRatioLocked() {#isAspectRatioLocked--}
```
public boolean isAspectRatioLocked()
```


True 表示形状的宽高比被锁定。

**Remarks**

仅适用于图片和 Ole 对象。

**Example**

```
         shape.setAspectRatioLocked(false);
```

**Returns:**
boolean
### isDecorative() {#isDecorative--}
```
public boolean isDecorative()
```


指示对象是否为装饰性的。

**Example**

```
         if (!shape.isDecorative())
             shape.setDecorative(true);
```

**Returns:**
boolean
### isEquation() {#isEquation--}
```
public boolean isEquation()
```


指示形状是否仅包含一个公式。

**Example**

```
         //If true,the shape only contains an equation.
         if(shape.isEquation())
         {
             //The shape contains only an equation
         }
```

**Returns:**
boolean
### isFilled() {#isFilled--}
```
public boolean isFilled()
```


指示填充格式是否可见。

**Example**

```
         if(shape.isFilled() == false)
             shape.setFilled(true);
```

**Returns:**
boolean
### isFlippedHorizontally() {#isFlippedHorizontally--}
```
public boolean isFlippedHorizontally()
```


获取形状是否水平翻转。

**Example**

```
         if(shape.isFlippedHorizontally() == false)
             shape.setFlippedHorizontally(true);
```

**Returns:**
boolean
### isFlippedVertically() {#isFlippedVertically--}
```
public boolean isFlippedVertically()
```


获取形状是否垂直翻转。

**Example**

```
         if(shape.isFlippedVertically() == false)
             shape.setFlippedVertically(true);
```

**Returns:**
boolean
### isGroup() {#isGroup--}
```
public boolean isGroup()
```


指示此形状是否为组合形状。

**Example**

```
         if(shape.isGroup())
         {
             //This shape is a group.
         }
```

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


指示对象是否可见。

**Example**

```
         shape.setHidden(false);
```

**Returns:**
boolean
### isInGroup() {#isInGroup--}
```
public boolean isInGroup()
```


指示形状是否已分组。

**Returns:**
boolean
### isLockAspectRatio() {#isLockAspectRatio--}
```
public boolean isLockAspectRatio()
```


True 表示形状的宽高比被锁定。

**Remarks**

仅适用于图片和 Ole 对象。注意：此成员现已过时。请改用 Shape.IsAspectRatioLocked 属性。此属性将在自 2024 年 7 月起的 12 个月后移除。Aspose 对给您带来的任何不便表示歉意。

**Example**

```
         shape.setHidden(false);
```

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


True 表示在工作表受保护时对象不能被修改。请注意，此值仅在工作表或工作表中的对象受到保护时才有意义。

**Example**

```
         //Sets the specified shape to unlocked state
         if (shape.getWorksheet().isProtected() &&shape.isLocked())
         {
             shape.setLocked(false);
         }
 
         //Sets the specified shape to a locked state
         if (shape.getWorksheet().isProtected() &&!shape.isLocked())
         {
             shape.setLocked(true);
         }
```

**Returns:**
boolean
### isPrintable() {#isPrintable--}
```
public boolean isPrintable()
```


指示对象是否可打印。如果为 False，则此形状在打印时不会被打印。

**Example**

```
         if(shape.isPrintable())
             shape.setPrintable(false);
```

**Returns:**
boolean
### isRichText() {#isRichText--}
```
public boolean isRichText()
```


指示文本是否为富文本。

**Example**

```
         if(shape.isRichText())
             System.out.println("The text is rich text.");
```

**Returns:**
boolean
### isSameSetting(Object obj) {#isSameSetting-java.lang.Object-}
```
public boolean isSameSetting(Object obj)
```


返回形状是否相同。

**Example**

```
         if (shape.isSameSetting(shape))
             System.out.println("Two objects the same.");
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
boolean -
### isSmartArt() {#isSmartArt--}
```
public boolean isSmartArt()
```


指示形状是否为智能艺术。

**Remarks**

仅适用于 ooxml 文件。

**Example**

```
         //if true,the shape is a smart art.
         if(shape.isSmartArt())
         {
             //The shape is SmartArt object.
         }
```

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


获取包含文本的形状的文本换行类型。

**Example**

```
         if (shape.isTextWrapped())
             shape.setTextWrapped(!shape.isTextWrapped());
```

**Returns:**
boolean
### isWordArt() {#isWordArt--}
```
public boolean isWordArt()
```


指示此形状是否为文字艺术。

**Remarks**

仅适用于 xls 文件的传统形状。

**Example**

```
         if(shape.isWordArt())
         {
             //This shape is a WordArt object.
         }
```

**Returns:**
boolean
### moveToRange(int topRow, int leftColumn, int bottomRow, int rightColumn) {#moveToRange-int-int-int-int-}
```
public void moveToRange(int topRow, int leftColumn, int bottomRow, int rightColumn)
```


将形状移动到指定范围。

**Example**

```
         shape.moveToRange(12, 3, 13, 5);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| topRow | int | 左上行索引。 |
| leftColumn | int | 左上列索引。 |
| bottomRow | int | 右下行索引 |
| rightColumn | int | 右下列索引 |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeActiveXControl() {#removeActiveXControl--}
```
public void removeActiveXControl()
```


移除 ActiveX 控件。

**Example**

```
         if(shape.getActiveXControl() != null)
         {
             shape.removeActiveXControl();
         }
```

### removeHyperlink() {#removeHyperlink--}
```
public void removeHyperlink()
```


移除形状的超链接。

**Example**

```
         shape.removeHyperlink();
```

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


返回或设置 [Shape](../../com.aspose.cells/shape) 对象的描述性（替代）文本字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setAnchorType(int value) {#setAnchorType-int-}
```
public void setAnchorType(int value)
```


设置形状锚点占位符的类型。

参见 [ShapeAnchorType](../../com.aspose.cells/shapeanchortype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setAspectRatioLocked(boolean value) {#setAspectRatioLocked-boolean-}
```
public void setAspectRatioLocked(boolean value)
```


True 表示形状的宽高比被锁定。

**Remarks**

仅适用于图片和 Ole 对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAutoShapeType(int value) {#setAutoShapeType-int-}
```
public void setAutoShapeType(int value)
```


设置自动形状类型。

参见 [AutoShapeType](../../com.aspose.cells/autoshapetype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setBottom(int value) {#setBottom-int-}
```
public void setBottom(int value)
```


表示形状从其左下角行的垂直偏移宽度，单位为像素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setCreateId(UUID value) {#setCreateId-java.util.UUID-}
```
public void setCreateId(UUID value)
```


为此形状设置创建 ID。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.UUID |  |

### setDecorative(boolean value) {#setDecorative-boolean-}
```
public void setDecorative(boolean value)
```


指示对象是否为装饰性的。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setFilled(boolean value) {#setFilled-boolean-}
```
public void setFilled(boolean value)
```


指示填充格式是否可见。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setFlippedHorizontally(boolean value) {#setFlippedHorizontally-boolean-}
```
public void setFlippedHorizontally(boolean value)
```


设置形状是否水平翻转。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setFlippedVertically(boolean value) {#setFlippedVertically-boolean-}
```
public void setFlippedVertically(boolean value)
```


设置形状是否垂直翻转。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setFont(Font value) {#setFont-com.aspose.cells.Font-}
```
public void setFont(Font value)
```


表示形状的字体。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Font](../../com.aspose.cells/font) |  |

### setHasLine(boolean value) {#setHasLine-boolean-}
```
public void setHasLine(boolean value)
```


设置形状的线条边框是否可见。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


表示形状的高度，单位为像素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setHeightCM(double value) {#setHeightCM-double-}
```
public void setHeightCM(double value)
```


表示形状的高度，单位为厘米。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setHeightInShape(int value) {#setHeightInShape-int-}
```
public void setHeightInShape(int value)
```


表示形状相对于父形状顶部边界的垂直偏移，单位为父形状高度的 1/4000。

**Remarks**

仅在此形状位于组或图表中时适用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setHeightInch(double value) {#setHeightInch-double-}
```
public void setHeightInch(double value)
```


表示形状的高度，单位为英寸。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setHeightPt(double value) {#setHeightPt-double-}
```
public void setHeightPt(double value)
```


表示形状的高度，单位为点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setHeightScale(int value) {#setHeightScale-int-}
```
public void setHeightScale(int value)
```


设置高度比例，单位为原始图片高度的百分比。如果形状不是图片，HeightScale 属性仅返回 100；

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


指示对象是否可见。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setHtmlText(String value) {#setHtmlText-java.lang.String-}
```
public void setHtmlText(String value)
```


设置包含数据和某些格式的 HTML 字符串到此文本框。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setInputRange(String value) {#setInputRange-java.lang.String-}
```
public void setInputRange(String value)
```


设置用于填充指定组合框的工作表范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setInputRange(String formula, boolean isR1C1, boolean isLocal) {#setInputRange-java.lang.String-boolean-boolean-}
```
public void setInputRange(String formula, boolean isR1C1, boolean isLocal)
```


设置用于填充控件的范围。

**Example**

```
         //After executing the code below, a ListBox object is created in the generated file. When the selected option is clicked, the selected value is displayed in cell A12.
 
         for (int i = 0; i? ++i)
         {
             Cell cell = book.getWorksheets().get(0).getCells().get(i, 0);
             cell.setValue(i + 1);
         }
 
         //Create a ListBox object
 
         //ActiveX Controls
         //Aspose.Cells.Drawing.Shape listBox = book.Worksheets[0].Shapes.AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox,2, 0, 2, 0, 130, 130);
 
         //Form Controls
         Shape listBox = book.getWorksheets().get(0).getShapes().addListBox(2, 0, 2, 0, 130, 130);
 
         //Sets the range used to fill the control.
         listBox.setInputRange("$A$1:$A$6", false, false);
 
         //Sets the range linked to the control's value.
         listBox.setLinkedCell("$A$12", false, true);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| formula | java.lang.String | 用于填充控件的范围。 |
| isR1C1 | boolean | 公式是否需要以 R1C1 格式化。 |
| isLocal | boolean | 公式是否需要根据区域设置进行格式化。 |

### setLeft(int value) {#setLeft-int-}
```
public void setLeft(int value)
```


表示形状相对于其左列的水平偏移，单位为像素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setLeftCM(double value) {#setLeftCM-double-}
```
public void setLeftCM(double value)
```


表示形状相对于其左列的水平偏移，单位为厘米。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setLeftInShape(int value) {#setLeftInShape-int-}
```
public void setLeftInShape(int value)
```


表示形状相对于父形状左边框的水平偏移，单位为父形状宽度的 1/4000。

**Remarks**

仅在此形状位于组或图表中时适用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setLeftInch(double value) {#setLeftInch-double-}
```
public void setLeftInch(double value)
```


表示形状相对于其左列的水平偏移，单位为英寸。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setLeftToCorner(int value) {#setLeftToCorner-int-}
```
public void setLeftToCorner(int value)
```


设置形状相对于工作表左边界的水平偏移。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setLinkedCell(String value) {#setLinkedCell-java.lang.String-}
```
public void setLinkedCell(String value)
```


设置与控件值关联的工作表范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setLinkedCell(String formula, boolean isR1C1, boolean isLocal) {#setLinkedCell-java.lang.String-boolean-boolean-}
```
public void setLinkedCell(String formula, boolean isR1C1, boolean isLocal)
```


设置与控件值关联的范围。

**Example**

```
         //After executing the code below, a ScrollBar object is created in the generated file. As you drag the slider, the value is displayed in cell A12.
 
         //ActiveX Controls
         //Aspose.Cells.Drawing.Shape scrollBar = book.Worksheets[0].Shapes.AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType.ScrollBar,2, 0, 2, 0, 30, 130);
 
         //Form Controls
         Shape scrollBar = book.getWorksheets().get(0).getShapes().addScrollBar(2, 0, 2, 0, 130, 30);
 
         //Sets the range linked to the control's value.
         scrollBar.setLinkedCell("$A$12", false, true);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| formula | java.lang.String | 与控件值关联的范围。 |
| isR1C1 | boolean | 公式是否需要以 R1C1 格式化。 |
| isLocal | boolean | 公式是否需要根据区域设置进行格式化。 |

### setLockAspectRatio(boolean value) {#setLockAspectRatio-boolean-}
```
public void setLockAspectRatio(boolean value)
```


True 表示形状的宽高比被锁定。

**Remarks**

仅适用于图片和 Ole 对象。注意：此成员现已过时。请改用 Shape.IsAspectRatioLocked 属性。此属性将在自 2024 年 7 月起的 12 个月后移除。Aspose 对给您带来的任何不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


True 表示在工作表受保护时对象不能被修改。请注意，此值仅在工作表或工作表中的对象受到保护时才有意义。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setLockedProperty(int type, boolean value) {#setLockedProperty-int-boolean-}
```
public void setLockedProperty(int type, boolean value)
```


设置锁定属性。

**Example**

```
         shape.setLockedProperty(ShapeLockType.ADJUST_HANDLES, true);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [ShapeLockType](../../com.aspose.cells/shapelocktype)。锁定类型。 |
| 值 | boolean | 属性的值。 |

### setLowerDeltaX(int value) {#setLowerDeltaX-int-}
```
public void setLowerDeltaX(int value)
```


设置形状相对于其右下角列的水平偏移。

**Remarks**

值的范围是 0 到 1024。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setLowerDeltaY(int value) {#setLowerDeltaY-int-}
```
public void setLowerDeltaY(int value)
```


设置形状相对于其右下角行的垂直偏移。

**Remarks**

值的范围是 0 到 256。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setLowerRightColumn(int value) {#setLowerRightColumn-int-}
```
public void setLowerRightColumn(int value)
```


表示右下角列索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setLowerRightRow(int value) {#setLowerRightRow-int-}
```
public void setLowerRightRow(int value)
```


表示右下角行索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setMacroName(String value) {#setMacroName-java.lang.String-}
```
public void setMacroName(String value)
```


设置宏的名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


设置形状的名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setPlacement(int value) {#setPlacement-int-}
```
public void setPlacement(int value)
```


表示绘图对象附着在其下方单元格的方式。该属性控制对象在工作表上的放置位置。

参见 [PlacementType](../../com.aspose.cells/placementtype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPrintable(boolean value) {#setPrintable-boolean-}
```
public void setPrintable(boolean value)
```


指示对象是否可打印。如果为 False，则此形状在打印时不会被打印。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setRelativeToOriginalPictureSize(boolean value) {#setRelativeToOriginalPictureSize-boolean-}
```
public void setRelativeToOriginalPictureSize(boolean value)
```


指示形状是否相对于原始图片尺寸。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setRight(int value) {#setRight-int-}
```
public void setRight(int value)
```


表示形状相对于其右下角列的水平偏移宽度，单位为像素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setRotationAngle(double value) {#setRotationAngle-double-}
```
public void setRotationAngle(double value)
```


设置形状的旋转角度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setSoftEdges(double value) {#setSoftEdges-double-}
```
public void setSoftEdges(double value)
```


设置要应用于边缘的模糊半径，单位为点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


设置此形状的文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setTextDirection(int value) {#setTextDirection-int-}
```
public void setTextDirection(int value)
```


设置此对象的文本流方向。

参见 [TextDirectionType](../../com.aspose.cells/textdirectiontype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTextHorizontalAlignment(int value) {#setTextHorizontalAlignment-int-}
```
public void setTextHorizontalAlignment(int value)
```


设置形状的文本水平对齐类型。

参见 [TextAlignmentType](../../com.aspose.cells/textalignmenttype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTextHorizontalOverflow(int value) {#setTextHorizontalOverflow-int-}
```
public void setTextHorizontalOverflow(int value)
```


设置包含文本的形状的文本水平溢出类型。

参见 [TextOverflowType](../../com.aspose.cells/textoverflowtype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTextOptions(TextOptions value) {#setTextOptions-com.aspose.cells.TextOptions-}
```
public void setTextOptions(TextOptions value)
```


表示形状的文本选项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [TextOptions](../../com.aspose.cells/textoptions) |  |

### setTextOrientationType(int value) {#setTextOrientationType-int-}
```
public void setTextOrientationType(int value)
```


设置形状的文本方向类型。

参见 [TextOrientationType](../../com.aspose.cells/textorientationtype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTextShapeType(int value) {#setTextShapeType-int-}
```
public void setTextShapeType(int value)
```


设置预设文本形状类型。

参见 [AutoShapeType](../../com.aspose.cells/autoshapetype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTextVerticalAlignment(int value) {#setTextVerticalAlignment-int-}
```
public void setTextVerticalAlignment(int value)
```


设置形状的文本垂直对齐类型。

参见 [TextAlignmentType](../../com.aspose.cells/textalignmenttype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTextVerticalOverflow(int value) {#setTextVerticalOverflow-int-}
```
public void setTextVerticalOverflow(int value)
```


设置包含文本的形状的文本垂直溢出类型。

参见 [TextOverflowType](../../com.aspose.cells/textoverflowtype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


设置包含文本的形状的文本换行类型。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


指定当前形状对象的标题（说明）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setTop(int value) {#setTop-int-}
```
public void setTop(int value)
```


表示形状相对于其顶部行的垂直偏移量，单位为像素。

**Remarks**

如果形状位于图表中，表示形状相对于其上边框的垂直偏移量。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTopCM(double value) {#setTopCM-double-}
```
public void setTopCM(double value)
```


表示形状相对于其顶部行的垂直偏移量，单位为厘米。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setTopInShape(int value) {#setTopInShape-int-}
```
public void setTopInShape(int value)
```


表示形状相对于父形状顶部边界的垂直偏移量，单位为父形状高度的 1/4000。

**Remarks**

仅在此形状位于组或图表中时适用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTopInch(double value) {#setTopInch-double-}
```
public void setTopInch(double value)
```


表示形状相对于其顶部行的垂直偏移量，单位为英寸。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setTopToCorner(int value) {#setTopToCorner-int-}
```
public void setTopToCorner(int value)
```


设置形状相对于工作表顶部边界的垂直偏移，单位为像素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setUpperDeltaX(int value) {#setUpperDeltaX-int-}
```
public void setUpperDeltaX(int value)
```


设置形状相对于其左上角列的水平偏移。

**Remarks**

值的范围是 0 到 1024。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setUpperDeltaY(int value) {#setUpperDeltaY-int-}
```
public void setUpperDeltaY(int value)
```


设置形状相对于其左上角行的垂直偏移。

**Remarks**

值的范围是 0 到 256。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setUpperLeftColumn(int value) {#setUpperLeftColumn-int-}
```
public void setUpperLeftColumn(int value)
```


表示左上角列索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setUpperLeftRow(int value) {#setUpperLeftRow-int-}
```
public void setUpperLeftRow(int value)
```


表示顶部行索引。

**Remarks**

如果形状位于形状内部或组中，UpperLeftRow 将被忽略。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


表示形状的宽度，单位为像素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setWidthCM(double value) {#setWidthCM-double-}
```
public void setWidthCM(double value)
```


表示形状的宽度，单位为厘米。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setWidthInShape(int value) {#setWidthInShape-int-}
```
public void setWidthInShape(int value)
```


表示形状的宽度，单位为父形状的 1/4000。

**Remarks**

仅在此形状位于组或图表中时适用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setWidthInch(double value) {#setWidthInch-double-}
```
public void setWidthInch(double value)
```


表示形状的宽度，单位为英寸。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setWidthPt(double value) {#setWidthPt-double-}
```
public void setWidthPt(double value)
```


表示形状的宽度，单位为点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setWidthScale(int value) {#setWidthScale-int-}
```
public void setWidthScale(int value)
```


设置宽度比例，单位为原始图片宽度的百分比。如果形状不是图片，WidthScale 属性仅返回 100；

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setX(int value) {#setX-int-}
```
public void setX(int value)
```


设置形状相对于工作表左边界的水平偏移，单位为像素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


设置形状相对于工作表顶部边界的垂直偏移，单位为像素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setZOrderPosition(int value) {#setZOrderPosition-int-}
```
public void setZOrderPosition(int value)
```


返回形状在 Z 顺序中的位置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### toFrontOrBack(int orders) {#toFrontOrBack-int-}
```
public void toFrontOrBack(int orders)
```


将形状置于前面或发送到后面。

**Example**

```
         shape.toFrontOrBack(2);
         //or shape.ToFrontOrBack(-1);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| orders | int | 如果小于零，则将形状置于后面。如果大于零，则将形状置于前面。 |

### toImage(OutputStream stream, ImageFormat imageFormat) {#toImage-java.io.OutputStream-com.aspose.cells.ImageFormat-}
```
public void toImage(OutputStream stream, ImageFormat imageFormat)
```


创建形状图像并以指定格式保存到流中。

**Remarks**

支持以下格式：.bmp、.gif、.jpg、.jpeg、.tiff、.emf。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.OutputStream | 输出流。 |
| imageFormat | [ImageFormat](../../com.aspose.cells/imageformat) | 保存图像的格式。 |

### toImage(OutputStream stream, ImageOrPrintOptions options) {#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(OutputStream stream, ImageOrPrintOptions options)
```


将形状保存到流中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.OutputStream |  |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) |  |

### toImage(String imageFile, ImageOrPrintOptions options) {#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(String imageFile, ImageOrPrintOptions options)
```


将形状保存到文件中。

**Example**

```
         ImageOrPrintOptions op = new ImageOrPrintOptions();
         shape.toImage("exmaple.png", op);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| imageFile | java.lang.String |  |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### updateSelectedValue() {#updateSelectedValue--}
```
public void updateSelectedValue()
```


通过链接单元格的值更新选定的值。

**Example**

```
         Cell cell = null;
         for (int i = 0; i? ++i)
         {
             cell = book.getWorksheets().get(0).getCells().get(i, 0);
             cell.setValue(i + 1);
         }
 
         //Create a ListBox object
 
         //ActiveX Controls
         //Aspose.Cells.Drawing.Shape listBox = book.Worksheets[0].Shapes.AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox,2, 0, 2, 0, 130, 130);
 
         //Form Controls
         Shape listBox = book.getWorksheets().get(0).getShapes().addListBox(2, 0, 2, 0, 130, 130);
 
         //Sets the range used to fill the control.
         listBox.setInputRange("$A$1:$A$6", false, false);
 
         //Sets the range linked to the control's value.
         listBox.setLinkedCell("$A$12", false, true);
 
         ListBox listbx = (ListBox)listBox;
 
         //Set the value of cell A12
         cell = book.getWorksheets().get(0).getCells().get(11, 0);
         cell.setValue(3);
 
         //Update the selected value by the value of the linked cell.
         listBox.updateSelectedValue();
 
         //-1 default, no option selected
         if(listbx.isSelected(2))
         {
             //Option 3 of the ListBox is selected
         }
 
         //Change the value of a linked cell
         cell.setValue(4);
 
         //Update the selected value by the value of the linked cell.
         listBox.updateSelectedValue();
         if(listbx.isSelected(3))
         {
             //Option 4 of the ListBox is selected
         }
```

### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

