##GridTableItemStyle
Inherited from System.Web.UI.WebControls.TableItemStyle.
**Inheritance:**
java.lang.Object, [com.aspose.gridweb.WebStyle](../../com.aspose.gridweb/webstyle), [com.aspose.gridweb.WebTableItemStyle](../../com.aspose.gridweb/webtableitemstyle)
```
public class GridTableItemStyle extends WebTableItemStyle
```
Inherited from System.Web.UI.WebControls.TableItemStyle. Encapsulates the styles of a WebCell.
**Example**
```
GridWeb GridWeb1 = new GridWeb();
GridWorksheetCollection sheets = GridWeb1.getWorkSheets();
GridWorksheet sheet = sheets.add("demo1");
sheet.getCells().get(0,0).putValue("Demo Text");
GridTableItemStyle style = sheet.getCells().get(0, 0).getStyle();
style.getFont().setSize(FontUnit.point(72));
style.setWrap(false);
style.setBackColor(Color.getGray());
style.setBorderStyle(BorderStyle.SOLID);
style.setBorderWidth(Unit.pixel(1));
style.setBorderColor(Color.getSilver());
style.getRightBorderStyle().setBorderColor(Color.getBlack());
style.getRightBorderStyle().setBorderStyle(BorderStyle.SOLID);
style.getRightBorderStyle().setBorderWidth(Unit.pixel(1));
style.getBottomBorderStyle().setBorderColor(Color.getBlack());
style.getBottomBorderStyle().setBorderStyle(BorderStyle.SOLID);
style.getBottomBorderStyle().setBorderWidth(Unit.pixel(1));
sheet.getCells().get(0, 0).setStyle(style);
```
## Constructors
| Constructor | Description |
| --- | --- |
| [GridTableItemStyle()](#GridTableItemStyle--) | Default constructor. |
## Methods
| Method | Description |
| --- | --- |
| [copyFrom(WebStyle s)](#copyFrom-com.aspose.gridweb.WebStyle-) | Copies from another style object. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackColor()](#getBackColor--) | Gets the BackColor in the style |
| [getBackImageAttributes()](#getBackImageAttributes--) | Background image attributes. |
| [getBackImageUrl()](#getBackImageUrl--) | Background image url. |
| [getBorderColor()](#getBorderColor--) | Gets the BorderColor in the style |
| [getBorderStyle()](#getBorderStyle--) | Gets the BorderStyle in the style |
| [getBorderWidth()](#getBorderWidth--) | Gets the BorderWidth in the style |
| [getBottomBorderStyle()](#getBottomBorderStyle--) | Specifies the style of the cell's bottom border. |
| [getClass()](#getClass--) |  |
| [getCssClass()](#getCssClass--) | Gets the CssClass in the style |
| [getCustom()](#getCustom--) | Gets the custom format, null or empty string means no custom format. |
| [getFont()](#getFont--) | Gets the Font in the style |
| [getForeColor()](#getForeColor--) | Gets the ForeColor in the style |
| [getHeight()](#getHeight--) | Gets the Height in the style |
| [getHorizontalAlign()](#getHorizontalAlign--) | Gets the HorizontalAlign in the style |
| [getIndentLevel()](#getIndentLevel--) | Gets indent level. |
| [getLeftBorderStyle()](#getLeftBorderStyle--) | Specifies the style of the cell's left border. |
| [getNumberType()](#getNumberType--) | Gets the display format of numbers and dates. |
| [getQuotePrefix()](#getQuotePrefix--) | Indicates whether the cell's value starts with single quote mark. |
| [getRightBorderStyle()](#getRightBorderStyle--) | Specifies the style of the cell's right border. |
| [getRotationAngle()](#getRotationAngle--) | Gets Rotation attribute. |
| [getTopBorderStyle()](#getTopBorderStyle--) | Specifies the style of the cell's top border. |
| [getVerticalAlign()](#getVerticalAlign--) | Gets the VerticalAlign in the style |
| [getWidth()](#getWidth--) | Gets the Width in the style |
| [getWrap()](#getWrap--) | Gets the Wrap in the style |
| [hashCode()](#hashCode--) | Serves as a hash function for a particular type, suitable for use in hashing algorithms and data structures like a hash table. |
| [isLocked()](#isLocked--) | Gets a value indicating whether a cell can be modified or not when its worksheet is protected. |
| [mergeWith(WebStyle s)](#mergeWith-com.aspose.gridweb.WebStyle-) | Merges with another style object. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackColor(Color value)](#setBackColor-com.aspose.gridweb.Color-) | Sets the BackColor in the style |
| [setBackImageAttributes(String value)](#setBackImageAttributes-java.lang.String-) | Background image attributes. |
| [setBackImageUrl(String value)](#setBackImageUrl-java.lang.String-) | Background image url. |
| [setBorderColor(Color value)](#setBorderColor-com.aspose.gridweb.Color-) | Sets the BorderColor in the style |
| [setBorderStyle(int value)](#setBorderStyle-int-) | Sets the BorderStyle in the style |
| [setBorderWidth(Unit value)](#setBorderWidth-com.aspose.gridweb.Unit-) | Sets the BorderWidth in the style |
| [setBottomBorderStyle(WebBorderStyle value)](#setBottomBorderStyle-com.aspose.gridweb.WebBorderStyle-) | Specifies the style of the cell's bottom border. |
| [setCssClass(String value)](#setCssClass-java.lang.String-) | Sets the CssClass in the style |
| [setCustom(String value)](#setCustom-java.lang.String-) | Sets the custom format, null or empty string means no custom format. |
| [setForeColor(Color value)](#setForeColor-com.aspose.gridweb.Color-) | Sets the ForeColor in the style |
| [setHeight(Unit value)](#setHeight-com.aspose.gridweb.Unit-) | Sets the Height in the style |
| [setHorizontalAlign(int value)](#setHorizontalAlign-int-) | Sets the HorizontalAlign in the style |
| [setIndentLevel(int value)](#setIndentLevel-int-) | Sets indent level. |
| [setLeftBorderStyle(WebBorderStyle value)](#setLeftBorderStyle-com.aspose.gridweb.WebBorderStyle-) | Specifies the style of the cell's left border. |
| [setLocked(boolean value)](#setLocked-boolean-) | Sets a value indicating whether a cell can be modified or not when its worksheet is protected. |
| [setNumberType(int value)](#setNumberType-int-) | Sets the display format of numbers and dates. |
| [setQuotePrefix(boolean value)](#setQuotePrefix-boolean-) | Indicates whether the cell's value starts with single quote mark. |
| [setRightBorderStyle(WebBorderStyle value)](#setRightBorderStyle-com.aspose.gridweb.WebBorderStyle-) | Specifies the style of the cell's right border. |
| [setRotationAngle(short value)](#setRotationAngle-short-) | Sets Rotation attribute. |
| [setTopBorderStyle(WebBorderStyle value)](#setTopBorderStyle-com.aspose.gridweb.WebBorderStyle-) | Specifies the style of the cell's top border. |
| [setVerticalAlign(int value)](#setVerticalAlign-int-) | Sets the VerticalAlign in the style |
| [setWidth(Unit value)](#setWidth-com.aspose.gridweb.Unit-) | Sets the Width in the style |
| [setWrap(boolean value)](#setWrap-boolean-) | Sets the Wrap in the style |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridTableItemStyle() {#GridTableItemStyle--}
```
public GridTableItemStyle()
```
Default constructor.
### copyFrom(WebStyle s) {#copyFrom-com.aspose.gridweb.WebStyle-}
```
public void copyFrom(WebStyle s)
```
Copies from another style object.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| s | [WebStyle](../../com.aspose.gridweb/webstyle) | another style object |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |
**Returns:**
boolean
### getBackColor() {#getBackColor--}
```
public Color getBackColor()
```
Gets the BackColor in the style
**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBackImageAttributes() {#getBackImageAttributes--}
```
public String getBackImageAttributes()
```
Background image attributes.
**Returns:**
java.lang.String
### getBackImageUrl() {#getBackImageUrl--}
```
public String getBackImageUrl()
```
Background image url.
**Returns:**
java.lang.String
### getBorderColor() {#getBorderColor--}
```
public Color getBorderColor()
```
Gets the BorderColor in the style
**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```
Gets the BorderStyle in the style
See [BorderStyle](../../com.aspose.gridweb/borderstyle).
**Returns:**
int
### getBorderWidth() {#getBorderWidth--}
```
public Unit getBorderWidth()
```
Gets the BorderWidth in the style
**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getBottomBorderStyle() {#getBottomBorderStyle--}
```
public WebBorderStyle getBottomBorderStyle()
```
Specifies the style of the cell's bottom border.
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
Gets the CssClass in the style
**Returns:**
java.lang.String
### getCustom() {#getCustom--}
```
public String getCustom()
```
Gets the custom format, null or empty string means no custom format.
**Returns:**
java.lang.String
### getFont() {#getFont--}
```
public FontInfo getFont()
```
Gets the Font in the style
**Returns:**
[FontInfo](../../com.aspose.gridweb/fontinfo)
### getForeColor() {#getForeColor--}
```
public Color getForeColor()
```
Gets the ForeColor in the style
**Returns:**
[Color](../../com.aspose.gridweb/color)
### getHeight() {#getHeight--}
```
public Unit getHeight()
```
Gets the Height in the style
**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getHorizontalAlign() {#getHorizontalAlign--}
```
public int getHorizontalAlign()
```
Gets the HorizontalAlign in the style
See [HorizontalAlign](../../com.aspose.gridweb/horizontalalign).
**Returns:**
int
### getIndentLevel() {#getIndentLevel--}
```
public int getIndentLevel()
```
Gets indent level.
**Remarks**
**Returns:**
int
### getLeftBorderStyle() {#getLeftBorderStyle--}
```
public WebBorderStyle getLeftBorderStyle()
```
Specifies the style of the cell's left border.
**Returns:**
[WebBorderStyle](../../com.aspose.gridweb/webborderstyle)
### getNumberType() {#getNumberType--}
```
public int getNumberType()
```
Gets the display format of numbers and dates. The formatting patterns are different for different regions.
**Remarks**
For example, the formatting patterns represented by numbers for en\_US region:
| Value | Type       | Format String                                        |
| ----- | ---------- | ---------------------------------------------------- |
| 0     | General    | `General`                                            |
| 1     | Decimal    | `0`                                                  |
| 2     | Decimal    | `0.00`                                               |
| 3     | Decimal    | `#,##0`                                              |
| 4     | Decimal    | `#,##0.00`                                           |
| 5     | Currency   | `$#,##0_);($#,##0)`                                  |
| 6     | Currency   | `$#,##0_);[Red](../$#,##0)`                             |
| 7     | Currency   | `$#,##0.00_);($#,##0.00)`                            |
| 8     | Currency   | `$#,##0.00_);[Red](../$#,##0.00)`                       |
| 9     | Percentage | `0%`                                                 |
| 10    | Percentage | `0.00%`                                              |
| 11    | Scientific | `0.00E+00`                                           |
| 12    | Fraction   | `# ?/?`                                              |
| 13    | Fraction   | `# ??/??`                                            |
| 14    | Date       | `m/d/yyyy`                                           |
| 15    | Date       | `d-mmm-yy`                                           |
| 16    | Date       | `d-mmm`                                              |
| 17    | Date       | `mmm-yy`                                             |
| 18    | Time       | `h:mm AM/PM`                                         |
| 19    | Time       | `h:mm:ss AM/PM`                                      |
| 20    | Time       | `h:mm`                                               |
| 21    | Time       | `h:mm:ss`                                            |
| 22    | Time       | `m/d/yyyy h:mm`                                      |
| 37    | Accounting | `#,##0_);(#,##0)`                                    |
| 38    | Accounting | `#,##0_);[Red](../#,##0)`                               |
| 39    | Accounting | `#,##0.00_);(#,##0.00)`                              |
| 40    | Accounting | `#,##0.00_);[Red](../#,##0.00)`                         |
| 41    | Accounting | `_(* #,##0_);_(* (#,##0);_(* "-"_);_(@_)`            |
| 42    | Currency   | `_($* #,##0_);_($* (#,##0);_($* "-"_);_(@_)`         |
| 43    | Accounting | `_(* #,##0.00_);_(* (#,##0.00);_(* "-"??_);_(@_)`    |
| 44    | Currency   | `_($* #,##0.00_);_($* (#,##0.00);_($* "-"??_);_(@_)` |
| 45    | Time       | `mm:ss`                                              |
| 46    | Time       | `[h]:mm:ss`                                          |
| 47    | Time       | `mm:ss.0`                                            |
| 48    | Scientific | `##0.0E+0`                                           |
| 49    | Text       | `@`                                                  |
**Returns:**
int
### getQuotePrefix() {#getQuotePrefix--}
```
public boolean getQuotePrefix()
```
Indicates whether the cell's value starts with single quote mark.
**Returns:**
boolean
### getRightBorderStyle() {#getRightBorderStyle--}
```
public WebBorderStyle getRightBorderStyle()
```
Specifies the style of the cell's right border.
**Returns:**
[WebBorderStyle](../../com.aspose.gridweb/webborderstyle)
### getRotationAngle() {#getRotationAngle--}
```
public short getRotationAngle()
```
Gets Rotation attribute.
**Remarks**
0: Not rotated.
255: Top to Bottom.
\-90: Downward.
90: Upward.
You can set 255 or value ranged from -90 to 90.
**Returns:**
short
### getTopBorderStyle() {#getTopBorderStyle--}
```
public WebBorderStyle getTopBorderStyle()
```
Specifies the style of the cell's top border.
**Returns:**
[WebBorderStyle](../../com.aspose.gridweb/webborderstyle)
### getVerticalAlign() {#getVerticalAlign--}
```
public int getVerticalAlign()
```
Gets the VerticalAlign in the style
See [VerticalAlign](../../com.aspose.gridweb/verticalalign).
**Returns:**
int
### getWidth() {#getWidth--}
```
public Unit getWidth()
```
Gets the Width in the style
**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getWrap() {#getWrap--}
```
public boolean getWrap()
```
Gets the Wrap in the style
**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```
Serves as a hash function for a particular type, suitable for use in hashing algorithms and data structures like a hash table.
**Returns:**
int - A hash code for the current Style.
### isLocked() {#isLocked--}
```
public boolean isLocked()
```
Gets a value indicating whether a cell can be modified or not when its worksheet is protected. When its worksheet is protected and IsLocked is true, the cell can not be edit. When its worksheet is protected and IsLocked is false, the cell can be edit.
**Returns:**
boolean
### mergeWith(WebStyle s) {#mergeWith-com.aspose.gridweb.WebStyle-}
```
public void mergeWith(WebStyle s)
```
Merges with another style object.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| s | [WebStyle](../../com.aspose.gridweb/webstyle) | another style object |
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
Sets the BackColor in the style
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |
### setBackImageAttributes(String value) {#setBackImageAttributes-java.lang.String-}
```
public void setBackImageAttributes(String value)
```
Background image attributes.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setBackImageUrl(String value) {#setBackImageUrl-java.lang.String-}
```
public void setBackImageUrl(String value)
```
Background image url.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setBorderColor(Color value) {#setBorderColor-com.aspose.gridweb.Color-}
```
public void setBorderColor(Color value)
```
Sets the BorderColor in the style
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |
### setBorderStyle(int value) {#setBorderStyle-int-}
```
public void setBorderStyle(int value)
```
Sets the BorderStyle in the style
See [BorderStyle](../../com.aspose.gridweb/borderstyle).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setBorderWidth(Unit value) {#setBorderWidth-com.aspose.gridweb.Unit-}
```
public void setBorderWidth(Unit value)
```
Sets the BorderWidth in the style
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |
### setBottomBorderStyle(WebBorderStyle value) {#setBottomBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setBottomBorderStyle(WebBorderStyle value)
```
Specifies the style of the cell's bottom border.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |
### setCssClass(String value) {#setCssClass-java.lang.String-}
```
public void setCssClass(String value)
```
Sets the CssClass in the style
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setCustom(String value) {#setCustom-java.lang.String-}
```
public void setCustom(String value)
```
Sets the custom format, null or empty string means no custom format.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setForeColor(Color value) {#setForeColor-com.aspose.gridweb.Color-}
```
public void setForeColor(Color value)
```
Sets the ForeColor in the style
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |
### setHeight(Unit value) {#setHeight-com.aspose.gridweb.Unit-}
```
public void setHeight(Unit value)
```
Sets the Height in the style
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |
### setHorizontalAlign(int value) {#setHorizontalAlign-int-}
```
public void setHorizontalAlign(int value)
```
Sets the HorizontalAlign in the style
See [HorizontalAlign](../../com.aspose.gridweb/horizontalalign).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setIndentLevel(int value) {#setIndentLevel-int-}
```
public void setIndentLevel(int value)
```
Sets indent level.
**Remarks**
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setLeftBorderStyle(WebBorderStyle value) {#setLeftBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setLeftBorderStyle(WebBorderStyle value)
```
Specifies the style of the cell's left border.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |
### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```
Sets a value indicating whether a cell can be modified or not when its worksheet is protected. When its worksheet is protected and IsLocked is true, the cell can not be edit. When its worksheet is protected and IsLocked is false, the cell can be edit.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setNumberType(int value) {#setNumberType-int-}
```
public void setNumberType(int value)
```
Sets the display format of numbers and dates. The formatting patterns are different for different regions.
**Remarks**
For example, the formatting patterns represented by numbers for en\_US region:
| Value | Type       | Format String                                        |
| ----- | ---------- | ---------------------------------------------------- |
| 0     | General    | `General`                                            |
| 1     | Decimal    | `0`                                                  |
| 2     | Decimal    | `0.00`                                               |
| 3     | Decimal    | `#,##0`                                              |
| 4     | Decimal    | `#,##0.00`                                           |
| 5     | Currency   | `$#,##0_);($#,##0)`                                  |
| 6     | Currency   | `$#,##0_);[Red](../$#,##0)`                             |
| 7     | Currency   | `$#,##0.00_);($#,##0.00)`                            |
| 8     | Currency   | `$#,##0.00_);[Red](../$#,##0.00)`                       |
| 9     | Percentage | `0%`                                                 |
| 10    | Percentage | `0.00%`                                              |
| 11    | Scientific | `0.00E+00`                                           |
| 12    | Fraction   | `# ?/?`                                              |
| 13    | Fraction   | `# ??/??`                                            |
| 14    | Date       | `m/d/yyyy`                                           |
| 15    | Date       | `d-mmm-yy`                                           |
| 16    | Date       | `d-mmm`                                              |
| 17    | Date       | `mmm-yy`                                             |
| 18    | Time       | `h:mm AM/PM`                                         |
| 19    | Time       | `h:mm:ss AM/PM`                                      |
| 20    | Time       | `h:mm`                                               |
| 21    | Time       | `h:mm:ss`                                            |
| 22    | Time       | `m/d/yyyy h:mm`                                      |
| 37    | Accounting | `#,##0_);(#,##0)`                                    |
| 38    | Accounting | `#,##0_);[Red](../#,##0)`                               |
| 39    | Accounting | `#,##0.00_);(#,##0.00)`                              |
| 40    | Accounting | `#,##0.00_);[Red](../#,##0.00)`                         |
| 41    | Accounting | `_(* #,##0_);_(* (#,##0);_(* "-"_);_(@_)`            |
| 42    | Currency   | `_($* #,##0_);_($* (#,##0);_($* "-"_);_(@_)`         |
| 43    | Accounting | `_(* #,##0.00_);_(* (#,##0.00);_(* "-"??_);_(@_)`    |
| 44    | Currency   | `_($* #,##0.00_);_($* (#,##0.00);_($* "-"??_);_(@_)` |
| 45    | Time       | `mm:ss`                                              |
| 46    | Time       | `[h]:mm:ss`                                          |
| 47    | Time       | `mm:ss.0`                                            |
| 48    | Scientific | `##0.0E+0`                                           |
| 49    | Text       | `@`                                                  |
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setQuotePrefix(boolean value) {#setQuotePrefix-boolean-}
```
public void setQuotePrefix(boolean value)
```
Indicates whether the cell's value starts with single quote mark.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setRightBorderStyle(WebBorderStyle value) {#setRightBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setRightBorderStyle(WebBorderStyle value)
```
Specifies the style of the cell's right border.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |
### setRotationAngle(short value) {#setRotationAngle-short-}
```
public void setRotationAngle(short value)
```
Sets Rotation attribute.
**Remarks**
0: Not rotated.
255: Top to Bottom.
\-90: Downward.
90: Upward.
You can set 255 or value ranged from -90 to 90.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | short |  |
### setTopBorderStyle(WebBorderStyle value) {#setTopBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setTopBorderStyle(WebBorderStyle value)
```
Specifies the style of the cell's top border.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |
### setVerticalAlign(int value) {#setVerticalAlign-int-}
```
public void setVerticalAlign(int value)
```
Sets the VerticalAlign in the style
See [VerticalAlign](../../com.aspose.gridweb/verticalalign).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setWidth(Unit value) {#setWidth-com.aspose.gridweb.Unit-}
```
public void setWidth(Unit value)
```
Sets the Width in the style
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |
### setWrap(boolean value) {#setWrap-boolean-}
```
public void setWrap(boolean value)
```
Sets the Wrap in the style
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
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
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |
