---
title: "GridPicture"
second_title: "Aspose.Cells for Java API 参考"
description: "封装表示电子表格中单个图片的对象。"
type: docs
url: /zh/java/com.aspose.gridweb/gridpicture/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.gridweb.IGridSave
```
public class GridPicture implements IGridSave
```

封装表示电子表格中单个图片的对象。
## 方法

| 方法 | 描述 |
| --- | --- |
| [addHyperlink(String address)](#addHyperlink-java.lang.String-) | 向形状添加超链接。 |
| [alignTopRightCorner(int topRow, int rightColumn)](#alignTopRightCorner-int-int-) | 将图片移动到右上角。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlternativeText()](#getAlternativeText--) | 返回或设置 [GridShape](../../com.aspose.gridweb/gridshape) 对象的描述性（替代）文本字符串。 |
| [getBorderLineColor()](#getBorderLineColor--) | 表示图片边框线的 [Color](../../com.aspose.cells/color)。 |
| [getBorderWeight()](#getBorderWeight--) | 获取图片边框线的粗细，单位为 pt。 |
| [getBottom()](#getBottom--) | 表示形状从其左下角行的垂直偏移宽度，单位为像素。 |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | 获取图片的数据。 |
| [getHeight()](#getHeight--) | 表示形状的高度，单位为像素。 |
| [getHeightCM()](#getHeightCM--) | 表示形状的高度，单位为英寸。 |
| [getHeightInch()](#getHeightInch--) | 表示形状的高度，单位为英寸。 |
| [getHeightPt()](#getHeightPt--) | 表示形状的高度，单位为点。 |
| [getHeightScale()](#getHeightScale--) | 获取高度比例，单位为原始图片高度的百分比。 |
| [getHtmlText()](#getHtmlText--) | 获取包含数据和一些格式的 html 字符串，该字符串位于此文本框中。 |
| [getHyperlink()](#getHyperlink--) | 获取形状的超链接。 |
| [getID()](#getID--) | 获取/设置图片的 ID。 |
| [getImageFormat()](#getImageFormat--) | 获取图片的图像格式。 |
| [getLeft()](#getLeft--) | 表示形状相对于其左列的水平偏移，单位为像素。 |
| [getLeftCM()](#getLeftCM--) | 表示形状相对于其左列的水平偏移，单位为厘米。 |
| [getLeftInch()](#getLeftInch--) | 表示形状相对于其左列的水平偏移，单位为英寸。 |
| [getLeftToCorner()](#getLeftToCorner--) | 表示形状相对于工作表左边界的水平偏移量，单位为像素。 |
| [getLinkedCell()](#getLinkedCell--) | 获取与控件值关联的工作表范围。 |
| [getLowerDeltaX()](#getLowerDeltaX--) | 获取形状相对于其右下角列的水平偏移。 |
| [getLowerDeltaY()](#getLowerDeltaY--) | 获取形状相对于其右下角行的垂直偏移。 |
| [getLowerRightColumn()](#getLowerRightColumn--) | 表示右下角列索引。 |
| [getLowerRightRow()](#getLowerRightRow--) | 表示右下角行索引。 |
| [getName()](#getName--) | 获取形状的名称。 |
| [getOriginalHeight()](#getOriginalHeight--) | 获取图片的原始高度。 |
| [getOriginalHeightCM()](#getOriginalHeightCM--) | 获取图片的原始高度，单位为厘米。 |
| [getOriginalHeightInch()](#getOriginalHeightInch--) | 获取图片的原始高度，单位为英寸。 |
| [getOriginalWidth()](#getOriginalWidth--) | 获取图片的原始宽度。 |
| [getOriginalWidthCM()](#getOriginalWidthCM--) | 获取图片的原始宽度，单位为厘米。 |
| [getOriginalWidthInch()](#getOriginalWidthInch--) | 获取图片的原始宽度，单位为英寸。 |
| [getRelativeToOriginalPictureSize()](#getRelativeToOriginalPictureSize--) | 指示形状是否相对于原始图片尺寸。 |
| [getRight()](#getRight--) | 表示形状相对于其右下角列的水平偏移宽度，单位为像素。 |
| [getRotationAngle()](#getRotationAngle--) | 获取形状的旋转角度。 |
| [getSourceFullName()](#getSourceFullName--) | 获取链接图像的源文件路径和名称。 |
| [getText()](#getText--) | 表示此 TextBox 对象中的字符串。 |
| [getTitle()](#getTitle--) | 指定当前形状对象的标题（说明）。 |
| [getTop()](#getTop--) | 表示形状相对于其顶部行的垂直偏移量，单位为像素。 |
| [getTopCM()](#getTopCM--) | 表示形状相对于其顶部行的垂直偏移量，单位为厘米。 |
| [getTopInch()](#getTopInch--) | 表示形状相对于其顶部行的垂直偏移量，单位为英寸。 |
| [getTopToCorner()](#getTopToCorner--) | 表示形状相对于工作表顶部边界的垂直偏移量，单位为像素。 |
| [getUpperDeltaX()](#getUpperDeltaX--) | 获取形状相对于其左上角列的水平偏移量。 |
| [getUpperDeltaY()](#getUpperDeltaY--) | 获取形状相对于其左上角行的垂直偏移量。 |
| [getUpperLeftColumn()](#getUpperLeftColumn--) | 表示左上角列索引。 |
| [getUpperLeftRow()](#getUpperLeftRow--) | 表示左上角行索引。 |
| [getWidth()](#getWidth--) | 表示形状的宽度，单位为像素。 |
| [getWidthCM()](#getWidthCM--) | 表示形状的宽度，单位为厘米。 |
| [getWidthInch()](#getWidthInch--) | 表示形状的宽度，单位为英寸。 |
| [getWidthPt()](#getWidthPt--) | 表示形状的宽度，单位为点。 |
| [getWidthScale()](#getWidthScale--) | 获取宽度比例，单位为原始图片宽度的百分比。 |
| [getX()](#getX--) | 获取形状相对于工作表左边框的水平偏移量，单位为像素。 |
| [getY()](#getY--) | 获取形状相对于工作表顶部边界的垂直偏移，单位为像素。 |
| [getZOrderPosition()](#getZOrderPosition--) | 返回形状在 Z 顺序中的位置。 |
| [hasLine()](#hasLine--) | 获取形状的线边框是否可见。 |
| [hashCode()](#hashCode--) |  |
| [isFlippedVertically()](#isFlippedVertically--) | 获取形状是否垂直翻转。 |
| [isGroup()](#isGroup--) | 指示形状是否为组。 |
| [isHidden()](#isHidden--) | 指示对象是否可见。 |
| [isLockAspectRatio()](#isLockAspectRatio--) | True 表示不允许更改宽高比。 |
| [isLocked()](#isLocked--) | 如果对象被锁定则为 True；如果在工作表受保护时对象可以被修改则为 False。 |
| [isTextWrapped()](#isTextWrapped--) | 获取包含文本的形状的文本换行类型。 |
| [move(int upperLeftRow, int upperLeftColumn)](#move-int-int-) | 将图片移动到指定位置。 |
| [moveToRange(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn)](#moveToRange-int-int-int-int-) | 将形状移动到指定范围。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeHyperlink()](#removeHyperlink--) | 移除形状的超链接。 |
| [saveToImage(InputStream s)](#saveToImage-java.io.InputStream-) | 创建图像并将其保存到流中。 |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | 返回或设置 [GridShape](../../com.aspose.gridweb/gridshape) 对象的描述性（替代）文本字符串。 |
| [setBorderLineColor(Color value)](#setBorderLineColor-com.aspose.gridweb.Color-) | 表示图片边框线的 [Color](../../com.aspose.cells/color)。 |
| [setBorderWeight(double value)](#setBorderWeight-double-) | 设置图片边框线的粗细，单位为 pt。 |
| [setBottom(int value)](#setBottom-int-) | 表示形状从其左下角行的垂直偏移宽度，单位为像素。 |
| [setData(byte[] value)](#setData-byte---) | 获取图片的数据。 |
| [setFlippedVertically(boolean value)](#setFlippedVertically-boolean-) | 设置形状是否垂直翻转。 |
| [setHasLine(boolean value)](#setHasLine-boolean-) | 设置形状的线条边框是否可见。 |
| [setHeight(int value)](#setHeight-int-) | 表示形状的高度，单位为像素。 |
| [setHeightCM(double value)](#setHeightCM-double-) | 表示形状的高度，单位为英寸。 |
| [setHeightInch(double value)](#setHeightInch-double-) | 表示形状的高度，单位为英寸。 |
| [setHeightPt(double value)](#setHeightPt-double-) | 表示形状的高度，单位为点。 |
| [setHeightScale(int value)](#setHeightScale-int-) | 设置高度比例，以原始图片高度的百分比为单位。 |
| [setHidden(boolean value)](#setHidden-boolean-) | 指示对象是否可见。 |
| [setHtmlText(String value)](#setHtmlText-java.lang.String-) | 设置包含数据和一些格式的 html 字符串，该字符串位于此文本框中。 |
| [setID(String value)](#setID-java.lang.String-) | 获取/设置图片的 ID。 |
| [setLeft(int value)](#setLeft-int-) | 表示形状相对于其左列的水平偏移，单位为像素。 |
| [setLeftCM(double value)](#setLeftCM-double-) | 表示形状相对于其左列的水平偏移，单位为厘米。 |
| [setLeftInch(double value)](#setLeftInch-double-) | 表示形状相对于其左列的水平偏移，单位为英寸。 |
| [setLeftToCorner(int value)](#setLeftToCorner-int-) | 表示形状相对于工作表左边界的水平偏移量，单位为像素。 |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | 设置与控件值关联的工作表范围。 |
| [setLockAspectRatio(boolean value)](#setLockAspectRatio-boolean-) | True 表示不允许更改宽高比。 |
| [setLocked(boolean value)](#setLocked-boolean-) | 如果对象被锁定则为 True；如果在工作表受保护时对象可以被修改则为 False。 |
| [setLowerDeltaX(int value)](#setLowerDeltaX-int-) | 设置形状相对于其右下角列的水平偏移。 |
| [setLowerDeltaY(int value)](#setLowerDeltaY-int-) | 设置形状相对于其右下角行的垂直偏移。 |
| [setLowerRightColumn(int value)](#setLowerRightColumn-int-) | 表示右下角列索引。 |
| [setLowerRightRow(int value)](#setLowerRightRow-int-) | 表示右下角行索引。 |
| [setName(String value)](#setName-java.lang.String-) | 设置形状的名称。 |
| [setRelativeToOriginalPictureSize(boolean value)](#setRelativeToOriginalPictureSize-boolean-) | 指示形状是否相对于原始图片尺寸。 |
| [setRight(int value)](#setRight-int-) | 表示形状相对于其右下角列的水平偏移宽度，单位为像素。 |
| [setRotationAngle(double value)](#setRotationAngle-double-) | 设置形状的旋转角度。 |
| [setSourceFullName(String value)](#setSourceFullName-java.lang.String-) | 设置链接图像的源文件路径和名称。 |
| [setText(String value)](#setText-java.lang.String-) | 表示此 TextBox 对象中的字符串。 |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | 设置包含文本的形状的文本换行类型。 |
| [setTitle(String value)](#setTitle-java.lang.String-) | 指定当前形状对象的标题（说明）。 |
| [setTop(int value)](#setTop-int-) | 表示形状相对于其顶部行的垂直偏移量，单位为像素。 |
| [setTopCM(double value)](#setTopCM-double-) | 表示形状相对于其顶部行的垂直偏移量，单位为厘米。 |
| [setTopInch(double value)](#setTopInch-double-) | 表示形状相对于其顶部行的垂直偏移量，单位为英寸。 |
| [setTopToCorner(int value)](#setTopToCorner-int-) | 表示形状相对于工作表顶部边界的垂直偏移量，单位为像素。 |
| [setUpperDeltaX(int value)](#setUpperDeltaX-int-) | 设置形状相对于其左上角列的水平偏移。 |
| [setUpperDeltaY(int value)](#setUpperDeltaY-int-) | 设置形状相对于其左上角行的垂直偏移。 |
| [setUpperLeftColumn(int value)](#setUpperLeftColumn-int-) | 表示左上角列索引。 |
| [setUpperLeftRow(int value)](#setUpperLeftRow-int-) | 表示左上角行索引。 |
| [setWidth(int value)](#setWidth-int-) | 表示形状的宽度，单位为像素。 |
| [setWidthCM(double value)](#setWidthCM-double-) | 表示形状的宽度，单位为厘米。 |
| [setWidthInch(double value)](#setWidthInch-double-) | 表示形状的宽度，单位为英寸。 |
| [setWidthPt(double value)](#setWidthPt-double-) | 表示形状的宽度，单位为点。 |
| [setWidthScale(int value)](#setWidthScale-int-) | 设置宽度比例，单位为原始图片宽度的百分比。 |
| [setX(int value)](#setX-int-) | 设置形状相对于工作表左边框的水平偏移量，单位为像素。 |
| [setY(int value)](#setY-int-) | 设置形状相对于工作表顶部边界的垂直偏移，单位为像素。 |
| [setZOrderPosition(int value)](#setZOrderPosition-int-) | 返回形状在 Z 顺序中的位置。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addHyperlink(String address) {#addHyperlink-java.lang.String-}
```
public GridHyperlink addHyperlink(String address)
```


向形状添加超链接。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 地址 | java.lang.String | 超链接的地址。 |

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink) - Return the new hyperlink object.
### alignTopRightCorner(int topRow, int rightColumn) {#alignTopRightCorner-int-int-}
```
public void alignTopRightCorner(int topRow, int rightColumn)
```


将图片移动到右上角。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| topRow | int | 行索引。 |
| rightColumn | int | 列索引。 |

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
### getAlternativeText() {#getAlternativeText--}
```
public String getAlternativeText()
```


返回或设置 [GridShape](../../com.aspose.gridweb/gridshape) 对象的描述性（替代）文本字符串。

**Returns:**
java.lang.String
### getBorderLineColor() {#getBorderLineColor--}
```
public Color getBorderLineColor()
```


表示图片边框线的 [Color](../../com.aspose.cells/color)。

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBorderWeight() {#getBorderWeight--}
```
public double getBorderWeight()
```


获取图片边框线的粗细，单位为 pt。

**Returns:**
double
### getBottom() {#getBottom--}
```
public int getBottom()
```


表示形状从其左下角行的垂直偏移宽度，单位为像素。

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getData() {#getData--}
```
public byte[] getData()
```


获取图片的数据。

**Returns:**
byte[]
### getHeight() {#getHeight--}
```
public int getHeight()
```


表示形状的高度，单位为像素。

**Returns:**
int
### getHeightCM() {#getHeightCM--}
```
public double getHeightCM()
```


表示形状的高度，单位为英寸。

**Returns:**
double
### getHeightInch() {#getHeightInch--}
```
public double getHeightInch()
```


表示形状的高度，单位为英寸。

**Returns:**
double
### getHeightPt() {#getHeightPt--}
```
public double getHeightPt()
```


表示形状的高度，单位为点。

**Returns:**
double
### getHeightScale() {#getHeightScale--}
```
public int getHeightScale()
```


获取高度比例，单位为原始图片高度的百分比。如果形状不是图片，HeightScale 属性仅返回 100；

**Returns:**
int
### getHtmlText() {#getHtmlText--}
```
public String getHtmlText()
```


获取包含数据和一些格式的 html 字符串，该字符串位于此文本框中。

**Returns:**
java.lang.String
### getHyperlink() {#getHyperlink--}
```
public GridHyperlink getHyperlink()
```


获取形状的超链接。

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink)
### getID() {#getID--}
```
public String getID()
```


获取/设置图片的 ID。

**Returns:**
java.lang.String
### getImageFormat() {#getImageFormat--}
```
public int getImageFormat()
```


获取图片的图像格式。

参见 [GridImageType](../../com.aspose.gridweb/gridimagetype)。

**Returns:**
int
### getLeft() {#getLeft--}
```
public int getLeft()
```


表示形状相对于其左列的水平偏移，单位为像素。

**Returns:**
int
### getLeftCM() {#getLeftCM--}
```
public double getLeftCM()
```


表示形状相对于其左列的水平偏移，单位为厘米。

**Returns:**
double
### getLeftInch() {#getLeftInch--}
```
public double getLeftInch()
```


表示形状相对于其左列的水平偏移，单位为英寸。

**Returns:**
double
### getLeftToCorner() {#getLeftToCorner--}
```
public int getLeftToCorner()
```


表示形状相对于工作表左边界的水平偏移量，单位为像素。

**Returns:**
int
### getLinkedCell() {#getLinkedCell--}
```
public String getLinkedCell()
```


获取与控件值关联的工作表范围。

**Returns:**
java.lang.String
### getLowerDeltaX() {#getLowerDeltaX--}
```
public int getLowerDeltaX()
```


获取形状相对于其右下角列的水平偏移量。取值范围为 0 到 1024。

**Returns:**
int
### getLowerDeltaY() {#getLowerDeltaY--}
```
public int getLowerDeltaY()
```


获取形状相对于其右下角行的垂直偏移量。取值范围为 0 到 256。

**Returns:**
int
### getLowerRightColumn() {#getLowerRightColumn--}
```
public int getLowerRightColumn()
```


表示右下角列索引。

**Returns:**
int
### getLowerRightRow() {#getLowerRightRow--}
```
public int getLowerRightRow()
```


表示右下角行索引。

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


获取形状的名称。

**Returns:**
java.lang.String
### getOriginalHeight() {#getOriginalHeight--}
```
public int getOriginalHeight()
```


获取图片的原始高度。

**Returns:**
int
### getOriginalHeightCM() {#getOriginalHeightCM--}
```
public double getOriginalHeightCM()
```


获取图片的原始高度，单位为厘米。

**Returns:**
double
### getOriginalHeightInch() {#getOriginalHeightInch--}
```
public double getOriginalHeightInch()
```


获取图片的原始高度，单位为英寸。

**Returns:**
double
### getOriginalWidth() {#getOriginalWidth--}
```
public int getOriginalWidth()
```


获取图片的原始宽度。

**Returns:**
int
### getOriginalWidthCM() {#getOriginalWidthCM--}
```
public double getOriginalWidthCM()
```


获取图片的原始宽度，单位为厘米。

**Returns:**
double
### getOriginalWidthInch() {#getOriginalWidthInch--}
```
public double getOriginalWidthInch()
```


获取图片的原始宽度，单位为英寸。

**Returns:**
double
### getRelativeToOriginalPictureSize() {#getRelativeToOriginalPictureSize--}
```
public boolean getRelativeToOriginalPictureSize()
```


指示形状是否相对于原始图片尺寸。

**Returns:**
boolean
### getRight() {#getRight--}
```
public int getRight()
```


表示形状相对于其右下角列的水平偏移宽度，单位为像素。

**Returns:**
int
### getRotationAngle() {#getRotationAngle--}
```
public double getRotationAngle()
```


获取形状的旋转角度。

**Returns:**
double
### getSourceFullName() {#getSourceFullName--}
```
public String getSourceFullName()
```


获取链接图像的源文件路径和名称。

**Remarks**

默认值为空字符串。如果 SourceFullName 不是空字符串，则图片为链接。如果 SourceFullName 不是空字符串，但 Data 为 null，则图片为链接且不存储在文件中。

**Returns:**
java.lang.String
### getText() {#getText--}
```
public String getText()
```


表示此 TextBox 对象中的字符串。

**Returns:**
java.lang.String
### getTitle() {#getTitle--}
```
public String getTitle()
```


指定当前形状对象的标题（说明）。

**Returns:**
java.lang.String
### getTop() {#getTop--}
```
public int getTop()
```


表示形状相对于其顶部行的垂直偏移量，单位为像素。

**Remarks**

如果形状位于图表中，表示形状相对于其上边框的垂直偏移量。

**Returns:**
int
### getTopCM() {#getTopCM--}
```
public double getTopCM()
```


表示形状相对于其顶部行的垂直偏移量，单位为厘米。

**Returns:**
double
### getTopInch() {#getTopInch--}
```
public double getTopInch()
```


表示形状相对于其顶部行的垂直偏移量，单位为英寸。

**Returns:**
double
### getTopToCorner() {#getTopToCorner--}
```
public int getTopToCorner()
```


表示形状相对于工作表顶部边界的垂直偏移量，单位为像素。

**Returns:**
int
### getUpperDeltaX() {#getUpperDeltaX--}
```
public int getUpperDeltaX()
```


获取形状相对于左上角列的水平偏移量。取值范围为 0 到 1024。

**Returns:**
int
### getUpperDeltaY() {#getUpperDeltaY--}
```
public int getUpperDeltaY()
```


获取形状相对于左上角行的垂直偏移量。取值范围为 0 到 256。

**Returns:**
int
### getUpperLeftColumn() {#getUpperLeftColumn--}
```
public int getUpperLeftColumn()
```


表示左上角列索引。

**Returns:**
int
### getUpperLeftRow() {#getUpperLeftRow--}
```
public int getUpperLeftRow()
```


表示左上角行索引。

**Remarks**

如果形状位于形状内部或组中，UpperLeftRow 将被忽略。

**Returns:**
int
### getWidth() {#getWidth--}
```
public int getWidth()
```


表示形状的宽度，单位为像素。

**Returns:**
int
### getWidthCM() {#getWidthCM--}
```
public double getWidthCM()
```


表示形状的宽度，单位为厘米。

**Returns:**
double
### getWidthInch() {#getWidthInch--}
```
public double getWidthInch()
```


表示形状的宽度，单位为英寸。

**Returns:**
double
### getWidthPt() {#getWidthPt--}
```
public double getWidthPt()
```


表示形状的宽度，单位为点。

**Returns:**
double
### getWidthScale() {#getWidthScale--}
```
public int getWidthScale()
```


获取宽度比例，单位为原始图片宽度的百分比。如果形状不是图片，WidthScale 属性仅返回 100；

**Returns:**
int
### getX() {#getX--}
```
public int getX()
```


获取形状相对于工作表左边框的水平偏移量，单位为像素。

**Returns:**
int
### getY() {#getY--}
```
public int getY()
```


获取形状相对于工作表顶部边界的垂直偏移，单位为像素。

**Returns:**
int
### getZOrderPosition() {#getZOrderPosition--}
```
public int getZOrderPosition()
```


返回形状在 Z 顺序中的位置。

**Returns:**
int
### hasLine() {#hasLine--}
```
public boolean hasLine()
```


获取形状的线边框是否可见。

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isFlippedVertically() {#isFlippedVertically--}
```
public boolean isFlippedVertically()
```


获取形状是否垂直翻转。

**Returns:**
boolean
### isGroup() {#isGroup--}
```
public boolean isGroup()
```


指示形状是否为组。

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


指示对象是否可见。

**Returns:**
boolean
### isLockAspectRatio() {#isLockAspectRatio--}
```
public boolean isLockAspectRatio()
```


True 表示不允许更改宽高比。

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


如果对象被锁定则为 True；如果在工作表受保护时对象可以被修改则为 False。

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


获取包含文本的形状的文本换行类型。

**Returns:**
boolean
### move(int upperLeftRow, int upperLeftColumn) {#move-int-int-}
```
public void move(int upperLeftRow, int upperLeftColumn)
```


将图片移动到指定位置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| upperLeftRow | int | 左上行索引。 |
| upperLeftColumn | int | 左上列索引。 |

### moveToRange(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn) {#moveToRange-int-int-int-int-}
```
public void moveToRange(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn)
```


将形状移动到指定范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| upperLeftRow | int | 左上行索引。 |
| upperLeftColumn | int | 左上列索引。 |
| lowerRightRow | int | 右下行索引 |
| lowerRightColumn | int | 右下列索引 |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeHyperlink() {#removeHyperlink--}
```
public void removeHyperlink()
```


移除形状的超链接。

### saveToImage(InputStream s) {#saveToImage-java.io.InputStream-}
```
public void saveToImage(InputStream s)
```


创建图像并将其保存到流中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| s | java.io.InputStream |  |

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


返回或设置 [GridShape](../../com.aspose.gridweb/gridshape) 对象的描述性（替代）文本字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setBorderLineColor(Color value) {#setBorderLineColor-com.aspose.gridweb.Color-}
```
public void setBorderLineColor(Color value)
```


表示图片边框线的 [Color](../../com.aspose.cells/color)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBorderWeight(double value) {#setBorderWeight-double-}
```
public void setBorderWeight(double value)
```


设置图片边框线的粗细，单位为 pt。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setBottom(int value) {#setBottom-int-}
```
public void setBottom(int value)
```


表示形状从其左下角行的垂直偏移宽度，单位为像素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setData(byte[] value) {#setData-byte---}
```
public void setData(byte[] value)
```


获取图片的数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | byte[] |  |

### setFlippedVertically(boolean value) {#setFlippedVertically-boolean-}
```
public void setFlippedVertically(boolean value)
```


设置形状是否垂直翻转。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

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


表示形状的高度，单位为英寸。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

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


设置包含数据和一些格式的 html 字符串，该字符串位于此文本框中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setID(String value) {#setID-java.lang.String-}
```
public void setID(String value)
```


获取/设置图片的 ID。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

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


表示形状相对于工作表左边界的水平偏移量，单位为像素。

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

### setLockAspectRatio(boolean value) {#setLockAspectRatio-boolean-}
```
public void setLockAspectRatio(boolean value)
```


True 表示不允许更改宽高比。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


如果对象被锁定则为 True；如果在工作表受保护时对象可以被修改则为 False。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setLowerDeltaX(int value) {#setLowerDeltaX-int-}
```
public void setLowerDeltaX(int value)
```


设置形状相对于右下角列的水平偏移量。取值范围为 0 到 1024。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setLowerDeltaY(int value) {#setLowerDeltaY-int-}
```
public void setLowerDeltaY(int value)
```


设置形状相对于右下角行的垂直偏移量。取值范围为 0 到 256。

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

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


设置形状的名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

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

### setSourceFullName(String value) {#setSourceFullName-java.lang.String-}
```
public void setSourceFullName(String value)
```


设置链接图像的源文件路径和名称。

**Remarks**

默认值为空字符串。如果 SourceFullName 不是空字符串，则图片为链接。如果 SourceFullName 不是空字符串，但 Data 为 null，则图片为链接且不存储在文件中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


表示此 TextBox 对象中的字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

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


表示形状相对于工作表顶部边界的垂直偏移量，单位为像素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setUpperDeltaX(int value) {#setUpperDeltaX-int-}
```
public void setUpperDeltaX(int value)
```


设置形状相对于左上角列的水平偏移量。取值范围为 0 到 1024。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setUpperDeltaY(int value) {#setUpperDeltaY-int-}
```
public void setUpperDeltaY(int value)
```


设置形状相对于左上角行的垂直偏移量。取值范围为 0 到 256。

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


表示左上角行索引。

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


设置形状相对于工作表左边框的水平偏移量，单位为像素。

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

