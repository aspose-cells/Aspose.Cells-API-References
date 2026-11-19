---
title: "GridTableItemStyle"
second_title: "Aspose.Cells for Java API Reference"
description: "موروث من System.Web.UI.WebControls.TableItemStyle."
type: docs
url: /ar/java/com.aspose.gridweb/gridtableitemstyle/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.WebStyle](../../com.aspose.gridweb/webstyle), [com.aspose.gridweb.WebTableItemStyle](../../com.aspose.gridweb/webtableitemstyle)
```
public class GridTableItemStyle extends WebTableItemStyle
```

موروث من System.Web.UI.WebControls.TableItemStyle. يضم أنماط WebCell.

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
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [GridTableItemStyle()](#GridTableItemStyle--) | المنشئ الافتراضي. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [copyFrom(WebStyle s)](#copyFrom-com.aspose.gridweb.WebStyle-) | ينسخ من كائن نمط آخر. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackColor()](#getBackColor--) | يحصل على BackColor في النمط |
| [getBackImageAttributes()](#getBackImageAttributes--) | سمات صورة الخلفية. |
| [getBackImageUrl()](#getBackImageUrl--) | عنوان URL لصورة الخلفية. |
| [getBorderColor()](#getBorderColor--) | يحصل على BorderColor في النمط |
| [getBorderStyle()](#getBorderStyle--) | يحصل على BorderStyle في النمط |
| [getBorderWidth()](#getBorderWidth--) | يحصل على BorderWidth في النمط |
| [getBottomBorderStyle()](#getBottomBorderStyle--) | يحدد نمط الحد السفلي للخلية. |
| [getClass()](#getClass--) |  |
| [getCssClass()](#getCssClass--) | يحصل على CssClass في النمط |
| [getCustom()](#getCustom--) | يحصل على التنسيق المخصص، القيمة null أو السلسلة الفارغة تعني عدم وجود تنسيق مخصص. |
| [getFont()](#getFont--) | يحصل على Font في النمط |
| [getForeColor()](#getForeColor--) | يحصل على ForeColor في النمط |
| [getHeight()](#getHeight--) | يحصل على Height في النمط |
| [getHorizontalAlign()](#getHorizontalAlign--) | يحصل على HorizontalAlign في النمط |
| [getIndentLevel()](#getIndentLevel--) | يحصل على مستوى المسافة البادئة. |
| [getLeftBorderStyle()](#getLeftBorderStyle--) | يحدد نمط الحد الأيسر للخلية. |
| [getNumberType()](#getNumberType--) | يحصل على تنسيق العرض للأرقام والتواريخ. |
| [getQuotePrefix()](#getQuotePrefix--) | يشير إلى ما إذا كانت قيمة الخلية تبدأ بعلامة اقتباس مفردة. |
| [getRightBorderStyle()](#getRightBorderStyle--) | يحدد نمط الحد الأيمن للخلية. |
| [getRotationAngle()](#getRotationAngle--) | يحصل على سمة الدوران. |
| [getTopBorderStyle()](#getTopBorderStyle--) | يحدد نمط الحد العلوي للخلية. |
| [getVerticalAlign()](#getVerticalAlign--) | يحصل على محاذاة عمودية في النمط |
| [getWidth()](#getWidth--) | يحصل على Width في النمط |
| [getWrap()](#getWrap--) | يحصل على التفاف في النمط |
| [hashCode()](#hashCode--) | يعمل كدالة تجزئة لنوع معين، مناسبة للاستخدام في خوارزميات التجزئة والهياكل البيانية مثل جدول التجزئة. |
| [isLocked()](#isLocked--) | يحصل على قيمة تشير إلى ما إذا كان يمكن تعديل الخلية أم لا عندما تكون ورقة العمل محمية. |
| [mergeWith(WebStyle s)](#mergeWith-com.aspose.gridweb.WebStyle-) | يدمج مع كائن نمط آخر. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackColor(Color value)](#setBackColor-com.aspose.gridweb.Color-) | يضبط BackColor في النمط |
| [setBackImageAttributes(String value)](#setBackImageAttributes-java.lang.String-) | سمات صورة الخلفية. |
| [setBackImageUrl(String value)](#setBackImageUrl-java.lang.String-) | عنوان URL لصورة الخلفية. |
| [setBorderColor(Color value)](#setBorderColor-com.aspose.gridweb.Color-) | يضبط BorderColor في النمط |
| [setBorderStyle(int value)](#setBorderStyle-int-) | يضبط BorderStyle في النمط |
| [setBorderWidth(Unit value)](#setBorderWidth-com.aspose.gridweb.Unit-) | يضبط BorderWidth في النمط |
| [setBottomBorderStyle(WebBorderStyle value)](#setBottomBorderStyle-com.aspose.gridweb.WebBorderStyle-) | يحدد نمط الحد السفلي للخلية. |
| [setCssClass(String value)](#setCssClass-java.lang.String-) | يضبط CssClass في النمط |
| [setCustom(String value)](#setCustom-java.lang.String-) | يضبط التنسيق المخصص، القيمة null أو السلسلة الفارغة تعني عدم وجود تنسيق مخصص. |
| [setForeColor(Color value)](#setForeColor-com.aspose.gridweb.Color-) | يضبط ForeColor في النمط |
| [setHeight(Unit value)](#setHeight-com.aspose.gridweb.Unit-) | يضبط Height في النمط |
| [setHorizontalAlign(int value)](#setHorizontalAlign-int-) | يضبط HorizontalAlign في النمط |
| [setIndentLevel(int value)](#setIndentLevel-int-) | يضبط مستوى المسافة البادئة. |
| [setLeftBorderStyle(WebBorderStyle value)](#setLeftBorderStyle-com.aspose.gridweb.WebBorderStyle-) | يحدد نمط الحد الأيسر للخلية. |
| [setLocked(boolean value)](#setLocked-boolean-) | يضبط قيمة تشير إلى ما إذا كان يمكن تعديل الخلية أم لا عندما تكون ورقة العمل محمية. |
| [setNumberType(int value)](#setNumberType-int-) | يضبط تنسيق العرض للأرقام والتواريخ. |
| [setQuotePrefix(boolean value)](#setQuotePrefix-boolean-) | يشير إلى ما إذا كانت قيمة الخلية تبدأ بعلامة اقتباس مفردة. |
| [setRightBorderStyle(WebBorderStyle value)](#setRightBorderStyle-com.aspose.gridweb.WebBorderStyle-) | يحدد نمط الحد الأيمن للخلية. |
| [setRotationAngle(short value)](#setRotationAngle-short-) | يضبط سمة الدوران. |
| [setTopBorderStyle(WebBorderStyle value)](#setTopBorderStyle-com.aspose.gridweb.WebBorderStyle-) | يحدد نمط الحد العلوي للخلية. |
| [setVerticalAlign(int value)](#setVerticalAlign-int-) | يضبط محاذاة عمودية في النمط |
| [setWidth(Unit value)](#setWidth-com.aspose.gridweb.Unit-) | يضبط Width في النمط |
| [setWrap(boolean value)](#setWrap-boolean-) | يضبط التفاف في النمط |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridTableItemStyle() {#GridTableItemStyle--}
```
public GridTableItemStyle()
```


المنشئ الافتراضي.

### copyFrom(WebStyle s) {#copyFrom-com.aspose.gridweb.WebStyle-}
```
public void copyFrom(WebStyle s)
```


ينسخ من كائن نمط آخر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| s | [WebStyle](../../com.aspose.gridweb/webstyle) | كائن نمط آخر |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getBackColor() {#getBackColor--}
```
public Color getBackColor()
```


يحصل على BackColor في النمط

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBackImageAttributes() {#getBackImageAttributes--}
```
public String getBackImageAttributes()
```


سمات صورة الخلفية.

**Returns:**
java.lang.String
### getBackImageUrl() {#getBackImageUrl--}
```
public String getBackImageUrl()
```


عنوان URL لصورة الخلفية.

**Returns:**
java.lang.String
### getBorderColor() {#getBorderColor--}
```
public Color getBorderColor()
```


يحصل على BorderColor في النمط

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```


يحصل على BorderStyle في النمط

انظر [BorderStyle](../../com.aspose.gridweb/borderstyle).

**Returns:**
int
### getBorderWidth() {#getBorderWidth--}
```
public Unit getBorderWidth()
```


يحصل على BorderWidth في النمط

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getBottomBorderStyle() {#getBottomBorderStyle--}
```
public WebBorderStyle getBottomBorderStyle()
```


يحدد نمط الحد السفلي للخلية.

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


يحصل على CssClass في النمط

**Returns:**
java.lang.String
### getCustom() {#getCustom--}
```
public String getCustom()
```


يحصل على التنسيق المخصص، القيمة null أو السلسلة الفارغة تعني عدم وجود تنسيق مخصص.

**Returns:**
java.lang.String
### getFont() {#getFont--}
```
public FontInfo getFont()
```


يحصل على Font في النمط

**Returns:**
[FontInfo](../../com.aspose.gridweb/fontinfo)
### getForeColor() {#getForeColor--}
```
public Color getForeColor()
```


يحصل على ForeColor في النمط

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getHeight() {#getHeight--}
```
public Unit getHeight()
```


يحصل على Height في النمط

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getHorizontalAlign() {#getHorizontalAlign--}
```
public int getHorizontalAlign()
```


يحصل على HorizontalAlign في النمط

انظر [HorizontalAlign](../../com.aspose.gridweb/horizontalalign).

**Returns:**
int
### getIndentLevel() {#getIndentLevel--}
```
public int getIndentLevel()
```


يحصل على مستوى المسافة البادئة.

**Remarks**

**Returns:**
int
### getLeftBorderStyle() {#getLeftBorderStyle--}
```
public WebBorderStyle getLeftBorderStyle()
```


يحدد نمط الحد الأيسر للخلية.

**Returns:**
[WebBorderStyle](../../com.aspose.gridweb/webborderstyle)
### getNumberType() {#getNumberType--}
```
public int getNumberType()
```


يحصل على تنسيق العرض للأرقام والتواريخ. أنماط التنسيق تختلف بين المناطق.

**Remarks**

على سبيل المثال، أنماط التنسيق الممثلة بأرقام لمنطقة en\\_US:

| Value | نوع | سلسلة التنسيق |
| ----- | ---------- | ---------------------------------------------------- |
| 0 | General | `General` |
| 1 | Decimal | `0` |
| 2 | Decimal | `0.00` |
| 3 | Decimal | `#,##0` |
| 4 | Decimal | `#,##0.00` |
| 5 | Currency | `$#,##0_);($#,##0)` |
| 6 | Currency | `$#,##0_);[أحمر](../$#,##0)` |
| 7 | Currency | `$#,##0.00_);($#,##0.00)` |
| 8 | Currency | `$#,##0.00_);[أحمر](../$#,##0.00)` |
| 9 | Percentage | `0%` |
| 10 | Percentage | `0.00%` |
| 11 | Scientific | `0.00E+00` |
| 12 | Fraction | `# ?/?` |
| 13 | Fraction | `# ??/??` |
| 14 | Date | `m/d/yyyy` |
| 15 | Date | `d-mmm-yy` |
| 16 | Date | `d-mmm` |
| 17 | Date | `mmm-yy` |
| 18 | Time | `h:mm ص/م` |
| 19 | Time | `h:mm:ss ص/م` |
| 20 | Time | `h:mm` |
| 21 | Time | `h:mm:ss` |
| 22 | Time | `m/d/yyyy h:mm` |
| 37 | Accounting | `#,##0_);(#,##0)` |
| 38 | Accounting | `#,##0_);[أحمر](../#,##0)` |
| 39 | Accounting | `#,##0.00_);(#,##0.00)` |
| 40 | Accounting | `#,##0.00_);[أحمر](../#,##0.00)` |
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


يشير إلى ما إذا كانت قيمة الخلية تبدأ بعلامة اقتباس مفردة.

**Returns:**
boolean
### getRightBorderStyle() {#getRightBorderStyle--}
```
public WebBorderStyle getRightBorderStyle()
```


يحدد نمط الحد الأيمن للخلية.

**Returns:**
[WebBorderStyle](../../com.aspose.gridweb/webborderstyle)
### getRotationAngle() {#getRotationAngle--}
```
public short getRotationAngle()
```


يحصل على سمة الدوران.

**Remarks**

0: غير مدور.

255: من الأعلى إلى الأسفل.

\-90: إلى الأسفل.

90: إلى الأعلى.

يمكنك تعيين 255 أو قيمة تتراوح من -90 إلى 90.

**Returns:**
short
### getTopBorderStyle() {#getTopBorderStyle--}
```
public WebBorderStyle getTopBorderStyle()
```


يحدد نمط الحد العلوي للخلية.

**Returns:**
[WebBorderStyle](../../com.aspose.gridweb/webborderstyle)
### getVerticalAlign() {#getVerticalAlign--}
```
public int getVerticalAlign()
```


يحصل على محاذاة عمودية في النمط

انظر [VerticalAlign](../../com.aspose.gridweb/verticalalign).

**Returns:**
int
### getWidth() {#getWidth--}
```
public Unit getWidth()
```


يحصل على Width في النمط

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getWrap() {#getWrap--}
```
public boolean getWrap()
```


يحصل على التفاف في النمط

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```


يعمل كدالة تجزئة لنوع معين، مناسبة للاستخدام في خوارزميات التجزئة والهياكل البيانية مثل جدول التجزئة.

**Returns:**
int - رمز تجزئة للنمط الحالي.
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


يحصل على قيمة تشير إلى ما إذا كان يمكن تعديل الخلية أم لا عندما تكون ورقة العمل محمية. عندما تكون ورقة العمل محمية وتكون IsLocked صحيحة، لا يمكن تحرير الخلية. عندما تكون ورقة العمل محمية وتكون IsLocked خاطئة، يمكن تحرير الخلية.

**Returns:**
boolean
### mergeWith(WebStyle s) {#mergeWith-com.aspose.gridweb.WebStyle-}
```
public void mergeWith(WebStyle s)
```


يدمج مع كائن نمط آخر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| s | [WebStyle](../../com.aspose.gridweb/webstyle) | كائن نمط آخر |

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


يضبط BackColor في النمط

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBackImageAttributes(String value) {#setBackImageAttributes-java.lang.String-}
```
public void setBackImageAttributes(String value)
```


سمات صورة الخلفية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setBackImageUrl(String value) {#setBackImageUrl-java.lang.String-}
```
public void setBackImageUrl(String value)
```


عنوان URL لصورة الخلفية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setBorderColor(Color value) {#setBorderColor-com.aspose.gridweb.Color-}
```
public void setBorderColor(Color value)
```


يضبط BorderColor في النمط

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBorderStyle(int value) {#setBorderStyle-int-}
```
public void setBorderStyle(int value)
```


يضبط BorderStyle في النمط

انظر [BorderStyle](../../com.aspose.gridweb/borderstyle).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setBorderWidth(Unit value) {#setBorderWidth-com.aspose.gridweb.Unit-}
```
public void setBorderWidth(Unit value)
```


يضبط BorderWidth في النمط

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setBottomBorderStyle(WebBorderStyle value) {#setBottomBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setBottomBorderStyle(WebBorderStyle value)
```


يحدد نمط الحد السفلي للخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

### setCssClass(String value) {#setCssClass-java.lang.String-}
```
public void setCssClass(String value)
```


يضبط CssClass في النمط

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setCustom(String value) {#setCustom-java.lang.String-}
```
public void setCustom(String value)
```


يضبط التنسيق المخصص، القيمة null أو السلسلة الفارغة تعني عدم وجود تنسيق مخصص.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setForeColor(Color value) {#setForeColor-com.aspose.gridweb.Color-}
```
public void setForeColor(Color value)
```


يضبط ForeColor في النمط

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setHeight(Unit value) {#setHeight-com.aspose.gridweb.Unit-}
```
public void setHeight(Unit value)
```


يضبط Height في النمط

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setHorizontalAlign(int value) {#setHorizontalAlign-int-}
```
public void setHorizontalAlign(int value)
```


يضبط HorizontalAlign في النمط

انظر [HorizontalAlign](../../com.aspose.gridweb/horizontalalign).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setIndentLevel(int value) {#setIndentLevel-int-}
```
public void setIndentLevel(int value)
```


يضبط مستوى المسافة البادئة.

**Remarks**

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setLeftBorderStyle(WebBorderStyle value) {#setLeftBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setLeftBorderStyle(WebBorderStyle value)
```


يحدد نمط الحد الأيسر للخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يمكن تعديل الخلية أم لا عندما تكون ورقة العمل محمية. عندما تكون ورقة العمل محمية وتكون IsLocked صحيحة، لا يمكن تحرير الخلية. عندما تكون ورقة العمل محمية وتكون IsLocked خاطئة، يمكن تحرير الخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setNumberType(int value) {#setNumberType-int-}
```
public void setNumberType(int value)
```


يضبط تنسيق عرض الأرقام والتواريخ. أنماط التنسيق تختلف بين المناطق.

**Remarks**

على سبيل المثال، أنماط التنسيق الممثلة بأرقام لمنطقة en\\_US:

| Value | نوع | سلسلة التنسيق |
| ----- | ---------- | ---------------------------------------------------- |
| 0 | General | `General` |
| 1 | Decimal | `0` |
| 2 | Decimal | `0.00` |
| 3 | Decimal | `#,##0` |
| 4 | Decimal | `#,##0.00` |
| 5 | Currency | `$#,##0_);($#,##0)` |
| 6 | Currency | `$#,##0_);[أحمر](../$#,##0)` |
| 7 | Currency | `$#,##0.00_);($#,##0.00)` |
| 8 | Currency | `$#,##0.00_);[أحمر](../$#,##0.00)` |
| 9 | Percentage | `0%` |
| 10 | Percentage | `0.00%` |
| 11 | Scientific | `0.00E+00` |
| 12 | Fraction | `# ?/?` |
| 13 | Fraction | `# ??/??` |
| 14 | Date | `m/d/yyyy` |
| 15 | Date | `d-mmm-yy` |
| 16 | Date | `d-mmm` |
| 17 | Date | `mmm-yy` |
| 18 | Time | `h:mm ص/م` |
| 19 | Time | `h:mm:ss ص/م` |
| 20 | Time | `h:mm` |
| 21 | Time | `h:mm:ss` |
| 22 | Time | `m/d/yyyy h:mm` |
| 37 | Accounting | `#,##0_);(#,##0)` |
| 38 | Accounting | `#,##0_);[أحمر](../#,##0)` |
| 39 | Accounting | `#,##0.00_);(#,##0.00)` |
| 40 | Accounting | `#,##0.00_);[أحمر](../#,##0.00)` |
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
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setQuotePrefix(boolean value) {#setQuotePrefix-boolean-}
```
public void setQuotePrefix(boolean value)
```


يشير إلى ما إذا كانت قيمة الخلية تبدأ بعلامة اقتباس مفردة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setRightBorderStyle(WebBorderStyle value) {#setRightBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setRightBorderStyle(WebBorderStyle value)
```


يحدد نمط الحد الأيمن للخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

### setRotationAngle(short value) {#setRotationAngle-short-}
```
public void setRotationAngle(short value)
```


يضبط سمة الدوران.

**Remarks**

0: غير مدور.

255: من الأعلى إلى الأسفل.

\-90: إلى الأسفل.

90: إلى الأعلى.

يمكنك تعيين 255 أو قيمة تتراوح من -90 إلى 90.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | short |  |

### setTopBorderStyle(WebBorderStyle value) {#setTopBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setTopBorderStyle(WebBorderStyle value)
```


يحدد نمط الحد العلوي للخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

### setVerticalAlign(int value) {#setVerticalAlign-int-}
```
public void setVerticalAlign(int value)
```


يضبط محاذاة عمودية في النمط

انظر [VerticalAlign](../../com.aspose.gridweb/verticalalign).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setWidth(Unit value) {#setWidth-com.aspose.gridweb.Unit-}
```
public void setWidth(Unit value)
```


يضبط Width في النمط

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setWrap(boolean value) {#setWrap-boolean-}
```
public void setWrap(boolean value)
```


يضبط التفاف في النمط

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

