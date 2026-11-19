---
title: "GridTableItemStyle"
second_title: "Aspose.Cells for Java API 参考"
description: "继承自 System.Web.UI.WebControls.TableItemStyle。"
type: docs
url: /zh/java/com.aspose.gridweb/gridtableitemstyle/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.WebStyle](../../com.aspose.gridweb/webstyle), [com.aspose.gridweb.WebTableItemStyle](../../com.aspose.gridweb/webtableitemstyle)
```
public class GridTableItemStyle extends WebTableItemStyle
```

继承自 System.Web.UI.WebControls.TableItemStyle。封装 WebCell 的样式。

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridWorksheetCollection sheets = GridWeb1.getWorkSheets();
 
         GridWorksheet sheet = sheets.add("demo1");
 
         sheet.getCells().get(0,0).putValue("Demo Text");
         GridTableItemStyle style = sheet.getCells().get(0, 0).getStyle();
 
         style.getFont().setSize(FontUnit.Point(72));
         style.setWrap(false);
 
         style.setBackColor(Color.getGray());
         	style.setBorderStyle(com.aspose.gridweb.BorderStyle.Solid);
         style.setBorderWidth(Unit.Pixel(1));
         style.setBorderColor(Color.getSilver());
         style.getRightBorderStyle().setBorderColor(Color.getBlack());
         	style.getRightBorderStyle().setBorderStyle(com.aspose.gridweb.BorderStyle.Solid);
         	style.getRightBorderStyle().setBorderWidth(Unit.Pixel(1));
         style.getBottomBorderStyle().setBorderColor(Color.getBlack());
         style.getBottomBorderStyle().setBorderStyle(com.aspose.gridweb.BorderStyle.Solid);
         style.getBottomBorderStyle().setBorderWidth(Unit.Pixel(1));
         sheet.getCells().get(0, 0).setStyle(style);
```
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [GridTableItemStyle()](#GridTableItemStyle--) | 默认构造函数。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [copyFrom(WebStyle s)](#copyFrom-com.aspose.gridweb.WebStyle-) | 从另一个样式对象复制。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackColor()](#getBackColor--) | 获取样式中的 BackColor |
| [getBackImageAttributes()](#getBackImageAttributes--) | 背景图像属性。 |
| [getBackImageUrl()](#getBackImageUrl--) | 背景图像 URL。 |
| [getBorderColor()](#getBorderColor--) | 获取样式中的 BorderColor |
| [getBorderStyle()](#getBorderStyle--) | 获取样式中的 BorderStyle |
| [getBorderWidth()](#getBorderWidth--) | 获取样式中的 BorderWidth |
| [getBottomBorderStyle()](#getBottomBorderStyle--) | 指定单元格底部边框的样式。 |
| [getClass()](#getClass--) |  |
| [getCssClass()](#getCssClass--) | 获取样式中的 CssClass |
| [getCustom()](#getCustom--) | 获取自定义格式，null 或空字符串表示没有自定义格式。 |
| [getFont()](#getFont--) | 获取样式中的 Font |
| [getForeColor()](#getForeColor--) | 获取样式中的 ForeColor |
| [getHeight()](#getHeight--) | 获取样式中的 Height |
| [getHorizontalAlign()](#getHorizontalAlign--) | 获取样式中的 HorizontalAlign |
| [getIndentLevel()](#getIndentLevel--) | 获取缩进级别。 |
| [getLeftBorderStyle()](#getLeftBorderStyle--) | 指定单元格左边框的样式。 |
| [getNumberType()](#getNumberType--) | 获取数字和日期的显示格式。 |
| [getQuotePrefix()](#getQuotePrefix--) | 指示单元格的值是否以单引号开头。 |
| [getRightBorderStyle()](#getRightBorderStyle--) | 指定单元格右边框的样式。 |
| [getRotationAngle()](#getRotationAngle--) | 获取 Rotation 属性。 |
| [getTopBorderStyle()](#getTopBorderStyle--) | 指定单元格上边框的样式。 |
| [getVerticalAlign()](#getVerticalAlign--) | 获取样式中的 VerticalAlign。 |
| [getWidth()](#getWidth--) | 获取样式中的 Width |
| [getWrap()](#getWrap--) | 获取样式中的 Wrap。 |
| [hashCode()](#hashCode--) | 作为特定类型的哈希函数，适用于哈希算法和诸如哈希表之类的数据结构。 |
| [isLocked()](#isLocked--) | 获取一个值，指示在工作表受保护时单元格是否可以被修改。 |
| [mergeWith(WebStyle s)](#mergeWith-com.aspose.gridweb.WebStyle-) | 与另一个样式对象合并。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackColor(Color value)](#setBackColor-com.aspose.gridweb.Color-) | 设置样式中的 BackColor |
| [setBackImageAttributes(String value)](#setBackImageAttributes-java.lang.String-) | 背景图像属性。 |
| [setBackImageUrl(String value)](#setBackImageUrl-java.lang.String-) | 背景图像 URL。 |
| [setBorderColor(Color value)](#setBorderColor-com.aspose.gridweb.Color-) | 设置样式中的 BorderColor |
| [setBorderStyle(int value)](#setBorderStyle-int-) | 设置样式中的 BorderStyle |
| [setBorderWidth(Unit value)](#setBorderWidth-com.aspose.gridweb.Unit-) | 设置样式中的 BorderWidth |
| [setBottomBorderStyle(WebBorderStyle value)](#setBottomBorderStyle-com.aspose.gridweb.WebBorderStyle-) | 指定单元格底部边框的样式。 |
| [setCssClass(String value)](#setCssClass-java.lang.String-) | 在样式中设置 CssClass |
| [setCustom(String value)](#setCustom-java.lang.String-) | 设置自定义格式，null 或空字符串表示没有自定义格式。 |
| [setForeColor(Color value)](#setForeColor-com.aspose.gridweb.Color-) | 在样式中设置 ForeColor |
| [setHeight(Unit value)](#setHeight-com.aspose.gridweb.Unit-) | 在样式中设置 Height |
| [setHorizontalAlign(int value)](#setHorizontalAlign-int-) | 在样式中设置 HorizontalAlign |
| [setIndentLevel(int value)](#setIndentLevel-int-) | 设置缩进级别。 |
| [setLeftBorderStyle(WebBorderStyle value)](#setLeftBorderStyle-com.aspose.gridweb.WebBorderStyle-) | 指定单元格左边框的样式。 |
| [setLocked(boolean value)](#setLocked-boolean-) | 设置一个值，指示在工作表受保护时单元格是否可以被修改。 |
| [setNumberType(int value)](#setNumberType-int-) | 设置数字和日期的显示格式。 |
| [setQuotePrefix(boolean value)](#setQuotePrefix-boolean-) | 指示单元格的值是否以单引号开头。 |
| [setRightBorderStyle(WebBorderStyle value)](#setRightBorderStyle-com.aspose.gridweb.WebBorderStyle-) | 指定单元格右边框的样式。 |
| [setRotationAngle(short value)](#setRotationAngle-short-) | 设置 Rotation 属性。 |
| [setTopBorderStyle(WebBorderStyle value)](#setTopBorderStyle-com.aspose.gridweb.WebBorderStyle-) | 指定单元格上边框的样式。 |
| [setVerticalAlign(int value)](#setVerticalAlign-int-) | 设置样式中的 VerticalAlign。 |
| [setWidth(Unit value)](#setWidth-com.aspose.gridweb.Unit-) | 在样式中设置 Width |
| [setWrap(boolean value)](#setWrap-boolean-) | 设置样式中的 Wrap。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridTableItemStyle() {#GridTableItemStyle--}
```
public GridTableItemStyle()
```


默认构造函数。

### copyFrom(WebStyle s) {#copyFrom-com.aspose.gridweb.WebStyle-}
```
public void copyFrom(WebStyle s)
```


从另一个样式对象复制。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| s | [WebStyle](../../com.aspose.gridweb/webstyle) | 另一个样式对象 |

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
### getBackColor() {#getBackColor--}
```
public Color getBackColor()
```


获取样式中的 BackColor

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBackImageAttributes() {#getBackImageAttributes--}
```
public String getBackImageAttributes()
```


背景图像属性。

**Returns:**
java.lang.String
### getBackImageUrl() {#getBackImageUrl--}
```
public String getBackImageUrl()
```


背景图像 URL。

**Returns:**
java.lang.String
### getBorderColor() {#getBorderColor--}
```
public Color getBorderColor()
```


获取样式中的 BorderColor

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```


获取样式中的 BorderStyle

参见 [BorderStyle](../../com.aspose.gridweb/borderstyle)。

**Returns:**
int
### getBorderWidth() {#getBorderWidth--}
```
public Unit getBorderWidth()
```


获取样式中的 BorderWidth

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getBottomBorderStyle() {#getBottomBorderStyle--}
```
public WebBorderStyle getBottomBorderStyle()
```


指定单元格底部边框的样式。

**Returns:**
[WebBorderStyle](../../com.aspose.gridweb/webborderstyle)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCssClass() {#getCssClass--}
```
public String getCssClass()
```


获取样式中的 CssClass

**Returns:**
java.lang.String
### getCustom() {#getCustom--}
```
public String getCustom()
```


获取自定义格式，null 或空字符串表示没有自定义格式。

**Returns:**
java.lang.String
### getFont() {#getFont--}
```
public FontInfo getFont()
```


获取样式中的 Font

**Returns:**
[FontInfo](../../com.aspose.gridweb/fontinfo)
### getForeColor() {#getForeColor--}
```
public Color getForeColor()
```


获取样式中的 ForeColor

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getHeight() {#getHeight--}
```
public Unit getHeight()
```


获取样式中的 Height

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getHorizontalAlign() {#getHorizontalAlign--}
```
public int getHorizontalAlign()
```


获取样式中的 HorizontalAlign

参见 [HorizontalAlign](../../com.aspose.gridweb/horizontalalign)。

**Returns:**
int
### getIndentLevel() {#getIndentLevel--}
```
public int getIndentLevel()
```


获取缩进级别。

**Remarks**

**Returns:**
int
### getLeftBorderStyle() {#getLeftBorderStyle--}
```
public WebBorderStyle getLeftBorderStyle()
```


指定单元格左边框的样式。

**Returns:**
[WebBorderStyle](../../com.aspose.gridweb/webborderstyle)
### getNumberType() {#getNumberType--}
```
public int getNumberType()
```


获取数字和日期的显示格式。不同地区的格式模式各不相同。

**Remarks**

例如，针对 en\_US 区域的数字所表示的格式模式如下：

| 值 | 类型 | 格式字符串 |
| ----- | ---------- | ---------------------------------------------------- |
| 0 | General | `General` |
| 1 | Decimal | `0` |
| 2 | Decimal | `0.00` |
| 3 | Decimal | `#,##0` |
| 4 | Decimal | `#,##0.00` |
| 5 | Currency | `$#,##0_);($#,##0)` |
| 6 | Currency | `$#,##0_);[Red](../$#,##0)` |
| 7 | Currency | `$#,##0.00_);($#,##0.00)` |
| 8 | Currency | `$#,##0.00_);[Red](../$#,##0.00)` |
| 9 | Percentage | `0%` |
| 10 | Percentage | `0.00%` |
| 11 | Scientific | `0.00E+00` |
| 12 | Fraction | `# ?/?` |
| 13 | Fraction | `# ??/??` |
| 14 | Date | `m/d/yyyy` |
| 15 | Date | `d-mmm-yy` |
| 16 | Date | `d-mmm` |
| 17 | Date | `mmm-yy` |
| 18 | Time | `h:mm AM/PM` |
| 19 | Time | `h:mm:ss AM/PM` |
| 20 | Time | `h:mm` |
| 21 | Time | `h:mm:ss` |
| 22 | Time | `m/d/yyyy h:mm` |
| 37 | Accounting | `#,##0_);(#,##0)` |
| 38 | Accounting | `#,##0_);[Red](../#,##0)` |
| 39 | Accounting | `#,##0.00_);(#,##0.00)` |
| 40 | Accounting | `#,##0.00_);[Red](../#,##0.00)` |
| 41 | Accounting | `_(* #,##0_);_(* (#,##0);_(* "-"_);_(@_)` |
| 42 | Currency | `_($* #,##0_);_($* (#,##0);_($* "-"_);_(@_)` |
| 43 | Accounting | `_(* #,##0.00_);_(* (#,##0.00);_(* "-"??_);_(@_)` |
| 44 | Currency | `_($* #,##0.00_);_($* (#,##0.00);_($* "-"??_);_(@_)` |
| 45 | Time | `mm:ss` |
| 46 | Time | `[h]:mm:ss` |
| 47 | Time | `mm:ss.0` |
| 48 | Scientific | `##0.0E+0` |
| 49 | Text | `@` |

**Returns:**
int
### getQuotePrefix() {#getQuotePrefix--}
```
public boolean getQuotePrefix()
```


指示单元格的值是否以单引号开头。

**Returns:**
boolean
### getRightBorderStyle() {#getRightBorderStyle--}
```
public WebBorderStyle getRightBorderStyle()
```


指定单元格右边框的样式。

**Returns:**
[WebBorderStyle](../../com.aspose.gridweb/webborderstyle)
### getRotationAngle() {#getRotationAngle--}
```
public short getRotationAngle()
```


获取 Rotation 属性。

**Remarks**

0：未旋转。

255：从上到下。

\-90：向下。

90：向上。

您可以设置 255 或范围在 -90 到 90 之间的值。

**Returns:**
短
### getTopBorderStyle() {#getTopBorderStyle--}
```
public WebBorderStyle getTopBorderStyle()
```


指定单元格上边框的样式。

**Returns:**
[WebBorderStyle](../../com.aspose.gridweb/webborderstyle)
### getVerticalAlign() {#getVerticalAlign--}
```
public int getVerticalAlign()
```


获取样式中的 VerticalAlign。

参见 [VerticalAlign](../../com.aspose.gridweb/verticalalign)。

**Returns:**
int
### getWidth() {#getWidth--}
```
public Unit getWidth()
```


获取样式中的 Width

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getWrap() {#getWrap--}
```
public boolean getWrap()
```


获取样式中的 Wrap。

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```


作为特定类型的哈希函数，适用于哈希算法和诸如哈希表之类的数据结构。

**Returns:**
int - 当前 Style 的哈希码。
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


获取一个值，指示在工作表受保护时单元格是否可以被修改。当工作表受保护且 IsLocked 为 true 时，单元格不可编辑。当工作表受保护且 IsLocked 为 false 时，单元格可以编辑。

**Returns:**
boolean
### mergeWith(WebStyle s) {#mergeWith-com.aspose.gridweb.WebStyle-}
```
public void mergeWith(WebStyle s)
```


与另一个样式对象合并。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| s | [WebStyle](../../com.aspose.gridweb/webstyle) | 另一个样式对象 |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setBackColor(Color value) {#setBackColor-com.aspose.gridweb.Color-}
```
public void setBackColor(Color value)
```


设置样式中的 BackColor

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBackImageAttributes(String value) {#setBackImageAttributes-java.lang.String-}
```
public void setBackImageAttributes(String value)
```


背景图像属性。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setBackImageUrl(String value) {#setBackImageUrl-java.lang.String-}
```
public void setBackImageUrl(String value)
```


背景图像 URL。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setBorderColor(Color value) {#setBorderColor-com.aspose.gridweb.Color-}
```
public void setBorderColor(Color value)
```


设置样式中的 BorderColor

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBorderStyle(int value) {#setBorderStyle-int-}
```
public void setBorderStyle(int value)
```


设置样式中的 BorderStyle

参见 [BorderStyle](../../com.aspose.gridweb/borderstyle)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setBorderWidth(Unit value) {#setBorderWidth-com.aspose.gridweb.Unit-}
```
public void setBorderWidth(Unit value)
```


设置样式中的 BorderWidth

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setBottomBorderStyle(WebBorderStyle value) {#setBottomBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setBottomBorderStyle(WebBorderStyle value)
```


指定单元格底部边框的样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

### setCssClass(String value) {#setCssClass-java.lang.String-}
```
public void setCssClass(String value)
```


在样式中设置 CssClass

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setCustom(String value) {#setCustom-java.lang.String-}
```
public void setCustom(String value)
```


设置自定义格式，null 或空字符串表示没有自定义格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setForeColor(Color value) {#setForeColor-com.aspose.gridweb.Color-}
```
public void setForeColor(Color value)
```


在样式中设置 ForeColor

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setHeight(Unit value) {#setHeight-com.aspose.gridweb.Unit-}
```
public void setHeight(Unit value)
```


在样式中设置 Height

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setHorizontalAlign(int value) {#setHorizontalAlign-int-}
```
public void setHorizontalAlign(int value)
```


在样式中设置 HorizontalAlign

参见 [HorizontalAlign](../../com.aspose.gridweb/horizontalalign)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setIndentLevel(int value) {#setIndentLevel-int-}
```
public void setIndentLevel(int value)
```


设置缩进级别。

**Remarks**

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setLeftBorderStyle(WebBorderStyle value) {#setLeftBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setLeftBorderStyle(WebBorderStyle value)
```


指定单元格左边框的样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


设置一个值，指示在工作表受保护时单元格是否可以被修改。当工作表受保护且 IsLocked 为 true 时，单元格不可编辑。当工作表受保护且 IsLocked 为 false 时，单元格可以编辑。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setNumberType(int value) {#setNumberType-int-}
```
public void setNumberType(int value)
```


设置数字和日期的显示格式。不同地区的格式模式不同。

**Remarks**

例如，针对 en\_US 区域的数字所表示的格式模式如下：

| 值 | 类型 | 格式字符串 |
| ----- | ---------- | ---------------------------------------------------- |
| 0 | General | `General` |
| 1 | Decimal | `0` |
| 2 | Decimal | `0.00` |
| 3 | Decimal | `#,##0` |
| 4 | Decimal | `#,##0.00` |
| 5 | Currency | `$#,##0_);($#,##0)` |
| 6 | Currency | `$#,##0_);[Red](../$#,##0)` |
| 7 | Currency | `$#,##0.00_);($#,##0.00)` |
| 8 | Currency | `$#,##0.00_);[Red](../$#,##0.00)` |
| 9 | Percentage | `0%` |
| 10 | Percentage | `0.00%` |
| 11 | Scientific | `0.00E+00` |
| 12 | Fraction | `# ?/?` |
| 13 | Fraction | `# ??/??` |
| 14 | Date | `m/d/yyyy` |
| 15 | Date | `d-mmm-yy` |
| 16 | Date | `d-mmm` |
| 17 | Date | `mmm-yy` |
| 18 | Time | `h:mm AM/PM` |
| 19 | Time | `h:mm:ss AM/PM` |
| 20 | Time | `h:mm` |
| 21 | Time | `h:mm:ss` |
| 22 | Time | `m/d/yyyy h:mm` |
| 37 | Accounting | `#,##0_);(#,##0)` |
| 38 | Accounting | `#,##0_);[Red](../#,##0)` |
| 39 | Accounting | `#,##0.00_);(#,##0.00)` |
| 40 | Accounting | `#,##0.00_);[Red](../#,##0.00)` |
| 41 | Accounting | `_(* #,##0_);_(* (#,##0);_(* "-"_);_(@_)` |
| 42 | Currency | `_($* #,##0_);_($* (#,##0);_($* "-"_);_(@_)` |
| 43 | Accounting | `_(* #,##0.00_);_(* (#,##0.00);_(* "-"??_);_(@_)` |
| 44 | Currency | `_($* #,##0.00_);_($* (#,##0.00);_($* "-"??_);_(@_)` |
| 45 | Time | `mm:ss` |
| 46 | Time | `[h]:mm:ss` |
| 47 | Time | `mm:ss.0` |
| 48 | Scientific | `##0.0E+0` |
| 49 | Text | `@` |

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setQuotePrefix(boolean value) {#setQuotePrefix-boolean-}
```
public void setQuotePrefix(boolean value)
```


指示单元格的值是否以单引号开头。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setRightBorderStyle(WebBorderStyle value) {#setRightBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setRightBorderStyle(WebBorderStyle value)
```


指定单元格右边框的样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

### setRotationAngle(short value) {#setRotationAngle-short-}
```
public void setRotationAngle(short value)
```


设置 Rotation 属性。

**Remarks**

0：未旋转。

255：从上到下。

\-90：向下。

90：向上。

您可以设置 255 或范围在 -90 到 90 之间的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | 短 |  |

### setTopBorderStyle(WebBorderStyle value) {#setTopBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setTopBorderStyle(WebBorderStyle value)
```


指定单元格上边框的样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

### setVerticalAlign(int value) {#setVerticalAlign-int-}
```
public void setVerticalAlign(int value)
```


设置样式中的 VerticalAlign。

参见 [VerticalAlign](../../com.aspose.gridweb/verticalalign)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setWidth(Unit value) {#setWidth-com.aspose.gridweb.Unit-}
```
public void setWidth(Unit value)
```


在样式中设置 Width

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setWrap(boolean value) {#setWrap-boolean-}
```
public void setWrap(boolean value)
```


设置样式中的 Wrap。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

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

