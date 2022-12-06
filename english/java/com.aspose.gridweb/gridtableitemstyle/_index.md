---
title: GridTableItemStyle
second_title: Aspose.Cells for Java API Reference
description: Inherited from System.Web.UI.WebControls.TableItemStyle.
type: docs
url: /java/com.aspose.gridweb/gridtableitemstyle/
---

**Inheritance:**
java.lang.Object
```
public class GridTableItemStyle
```

Inherited from System.Web.UI.WebControls.TableItemStyle. Encapsulates the styles of a WebCell.

```
...
          System.Web.UI.WebControls;
         try //JAVA: was using
         {;
         }
         finally { if (/*JAVA: using statement with anonimous resource does not supported yet*/ != null) /*JAVA: using statement with anonimous resource does not supported yet*/.close(); }
         ...
         ...
         WebWorksheets sheets = GridWeb1.WebWorksheets;
         	sheets.Clear();
         	WebWorksheet sheet = sheets[sheets.Add("demo1")];
 
         	WebCell cell = sheet.Cells[0][0];
         	cell.StringValue = "Demo Text";
 
         Aspose.Cells.GridWeb.TableItemStyle style = cell.GetStyle();
         	style.Font.Size = new FontUnit("72pt");
         	style.Wrap = false;
 
         	style.BackColor = Color.getGray();
         	style.BorderStyle = BorderStyle.Solid;
         	style.BorderWidth = new Unit(1, UnitType.Pixel);
         	style.BorderColor = Color.getSilver();
 
         	style.RightBorderStyle.BorderColor = Color.getBlack();
         	style.RightBorderStyle.BorderStyle = BorderStyle.Solid;
         	style.RightBorderStyle.BorderWidth = new Unit(1, UnitType.Pixel);
         	style.BottomBorderStyle.BorderColor = Color.getBlack();
         	style.BottomBorderStyle.BorderStyle = BorderStyle.Solid;
         	style.BottomBorderStyle.BorderWidth = new Unit(1, UnitType.Pixel);
         cell.SetStyle(style);
```
## Constructors

| Constructor | Description |
| --- | --- |
| [GridTableItemStyle()](#GridTableItemStyle--) | Default constructor. |
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackImageAttributes()](#getBackImageAttributes--) | Background image attributes. |
| [getBackImageUrl()](#getBackImageUrl--) | Background image url. |
| [getBottomBorderStyle()](#getBottomBorderStyle--) | Specifies the style of the cell's bottom border. |
| [getClass()](#getClass--) |  |
| [getCustom()](#getCustom--) | the custom format, null or empty string means no custom format. |
| [getIndentLevel()](#getIndentLevel--) | indent level. |
| [getLeftBorderStyle()](#getLeftBorderStyle--) | Specifies the style of the cell's left border. |
| [getNumberType()](#getNumberType--) | the display format of numbers and dates |
| [getRightBorderStyle()](#getRightBorderStyle--) | Specifies the style of the cell's right border. |
| [getRotationAngle()](#getRotationAngle--) | Rotation attribute. |
| [getTopBorderStyle()](#getTopBorderStyle--) | Specifies the style of the cell's top border. |
| [hashCode()](#hashCode--) | Serves as a hash function for a particular type, suitable for use in hashing algorithms and data structures like a hash table. |
| [isLocked()](#isLocked--) | a value indicating whether a cell can be modified or not when its worksheet is protected. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackImageAttributes(String value)](#setBackImageAttributes-java.lang.String-) | For the description of this property, please see [getBackImageAttributes()](../../com.aspose.gridweb/gridtableitemstyle\#getBackImageAttributes--) |
| [setBackImageUrl(String value)](#setBackImageUrl-java.lang.String-) | For the description of this property, please see [getBackImageUrl()](../../com.aspose.gridweb/gridtableitemstyle\#getBackImageUrl--) |
| [setBottomBorderStyle(WebBorderStyle value)](#setBottomBorderStyle-com.aspose.gridweb.WebBorderStyle-) | For the description of this property, please see [getBottomBorderStyle()](../../com.aspose.gridweb/gridtableitemstyle\#getBottomBorderStyle--) |
| [setCustom(String value)](#setCustom-java.lang.String-) | For the description of this property, please see [getCustom()](../../com.aspose.gridweb/gridtableitemstyle\#getCustom--) |
| [setIndentLevel(int value)](#setIndentLevel-int-) | For the description of this property, please see [getIndentLevel()](../../com.aspose.gridweb/gridtableitemstyle\#getIndentLevel--) |
| [setLeftBorderStyle(WebBorderStyle value)](#setLeftBorderStyle-com.aspose.gridweb.WebBorderStyle-) | For the description of this property, please see [getLeftBorderStyle()](../../com.aspose.gridweb/gridtableitemstyle\#getLeftBorderStyle--) |
| [setLocked(boolean value)](#setLocked-boolean-) | For the description of this property, please see [isLocked()](../../com.aspose.gridweb/gridtableitemstyle\#isLocked--) |
| [setNumberType(int value)](#setNumberType-int-) | For the description of this property, please see [getNumberType()](../../com.aspose.gridweb/gridtableitemstyle\#getNumberType--) |
| [setRightBorderStyle(WebBorderStyle value)](#setRightBorderStyle-com.aspose.gridweb.WebBorderStyle-) | For the description of this property, please see [getRightBorderStyle()](../../com.aspose.gridweb/gridtableitemstyle\#getRightBorderStyle--) |
| [setRotationAngle(short value)](#setRotationAngle-short-) | For the description of this property, please see [getRotationAngle()](../../com.aspose.gridweb/gridtableitemstyle\#getRotationAngle--) |
| [setTopBorderStyle(WebBorderStyle value)](#setTopBorderStyle-com.aspose.gridweb.WebBorderStyle-) | For the description of this property, please see [getTopBorderStyle()](../../com.aspose.gridweb/gridtableitemstyle\#getTopBorderStyle--) |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridTableItemStyle() {#GridTableItemStyle--}
```
public GridTableItemStyle()
```


Default constructor.

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
### getCustom() {#getCustom--}
```
public String getCustom()
```


the custom format, null or empty string means no custom format.

**Returns:**
java.lang.String
### getIndentLevel() {#getIndentLevel--}
```
public int getIndentLevel()
```


indent level.

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


the display format of numbers and dates. ///

    | --------- | ---------- | -------------------------------------------------------------------- |
    | **Value** | **Type**   | **Format String**                                                    |
    | 0         | General    | General                                                              |
    | 1         | Decimal    | 0                                                                    |
    | 2         | Decimal    | 0.00                                                                 |
    | 3         | Decimal    | \#,\#\#0                                                             |
    | 4         | Decimal    | \#,\#\#0.00                                                          |
    | 5         | Currency   | $\#,\#\#0;($\#,\#\#0)                                                |
    | 6         | Currency   | $\#,\#\#0;[Red](../$\#,\#\#0)                                         |
    | 7         | Currency   | $\#,\#\#0.00;($\#,\#\#0.00)                                          |
    | 8         | Currency   | $\#,\#\#0.00;[Red](../$\#,\#\#0.00)                                   |
    | 9         | Percentage | 0%                                                                   |
    | 10        | Percentage | 0.00%                                                                |
    | 11        | Scientific | 0.00E+00                                                             |
    | 12        | Fraction   | \# ?/?                                                               |
    | 13        | Fraction   | \# ??/??                                                             |
    | 14        | Date       | m/d/yyyy                                                             |
    | 15        | Date       | d-mmm-yy                                                             |
    | 16        | Date       | d-mmm                                                                |
    | 17        | Date       | mmm-yy                                                               |
    | 18        | Time       | h:mm AM/PM                                                           |
    | 19        | Time       | h:mm:ss AM/PM                                                        |
    | 20        | Time       | h:mm                                                                 |
    | 21        | Time       | h:mm:ss                                                              |
    | 22        | Time       | m/d/yyyy h:mm                                                        |
    | 37        | Accounting | \#,\#\#0;(\#,\#\#0)                                                  |
    | 38        | Accounting | \#,\#\#0;[Red](../\#,\#\#0)                                           |
    | 39        | Accounting | \#,\#\#0.00;(\#,\#\#0.00)                                            |
    | 40        | Accounting | \#,\#\#0.00;[Red](../\#,\#\#0.00)                                     |
    | 41        | Accounting | \_ \* \#,\#\#0\_ ;\_ \* (\#,\#\#0)\_ ;\_ \* "-"\_ ;\_ @\_            |
    | 42        | Currency   | \_ $\* \#,\#\#0\_ ;\_ $\* (\#,\#\#0)\_ ;\_ $\* "-"\_ ;\_ @\_         |
    | 43        | Accounting | \_ \* \#,\#\#0.00\_ ;\_ \* (\#,\#\#0.00)\_ ;\_ \* "-"??\_ ;\_ @\_    |
    | 44        | Currency   | \_ $\* \#,\#\#0.00\_ ;\_ $\* (\#,\#\#0.00)\_ ;\_ $\* "-"??\_ ;\_ @\_ |
    | 45        | Time       | mm:ss                                                                |
    | 46        | Time       | [h]:mm:ss                                                          |
    | 47        | Time       | mm:ss.0                                                              |
    | 48        | Scientific | \#\#0.0E+00                                                          |
    | 49        | Text       | @                                                                    |

**Returns:**
int
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


Rotation attribute.

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


a value indicating whether a cell can be modified or not when its worksheet is protected. When its worksheet is protected and IsLocked is true, the cell can not be edit. When its worksheet is protected and IsLocked is false, the cell can be edit.

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




### setBackImageAttributes(String value) {#setBackImageAttributes-java.lang.String-}
```
public void setBackImageAttributes(String value)
```


For the description of this property, please see [getBackImageAttributes()](../../com.aspose.gridweb/gridtableitemstyle\#getBackImageAttributes--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setBackImageUrl(String value) {#setBackImageUrl-java.lang.String-}
```
public void setBackImageUrl(String value)
```


For the description of this property, please see [getBackImageUrl()](../../com.aspose.gridweb/gridtableitemstyle\#getBackImageUrl--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setBottomBorderStyle(WebBorderStyle value) {#setBottomBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setBottomBorderStyle(WebBorderStyle value)
```


For the description of this property, please see [getBottomBorderStyle()](../../com.aspose.gridweb/gridtableitemstyle\#getBottomBorderStyle--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

### setCustom(String value) {#setCustom-java.lang.String-}
```
public void setCustom(String value)
```


For the description of this property, please see [getCustom()](../../com.aspose.gridweb/gridtableitemstyle\#getCustom--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setIndentLevel(int value) {#setIndentLevel-int-}
```
public void setIndentLevel(int value)
```


For the description of this property, please see [getIndentLevel()](../../com.aspose.gridweb/gridtableitemstyle\#getIndentLevel--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setLeftBorderStyle(WebBorderStyle value) {#setLeftBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setLeftBorderStyle(WebBorderStyle value)
```


For the description of this property, please see [getLeftBorderStyle()](../../com.aspose.gridweb/gridtableitemstyle\#getLeftBorderStyle--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


For the description of this property, please see [isLocked()](../../com.aspose.gridweb/gridtableitemstyle\#isLocked--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setNumberType(int value) {#setNumberType-int-}
```
public void setNumberType(int value)
```


For the description of this property, please see [getNumberType()](../../com.aspose.gridweb/gridtableitemstyle\#getNumberType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setRightBorderStyle(WebBorderStyle value) {#setRightBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setRightBorderStyle(WebBorderStyle value)
```


For the description of this property, please see [getRightBorderStyle()](../../com.aspose.gridweb/gridtableitemstyle\#getRightBorderStyle--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

### setRotationAngle(short value) {#setRotationAngle-short-}
```
public void setRotationAngle(short value)
```


For the description of this property, please see [getRotationAngle()](../../com.aspose.gridweb/gridtableitemstyle\#getRotationAngle--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | short |  |

### setTopBorderStyle(WebBorderStyle value) {#setTopBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setTopBorderStyle(WebBorderStyle value)
```


For the description of this property, please see [getTopBorderStyle()](../../com.aspose.gridweb/gridtableitemstyle\#getTopBorderStyle--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

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

