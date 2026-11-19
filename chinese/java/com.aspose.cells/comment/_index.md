---
title: "批注"
second_title: "Aspose.Cells for Java API 参考"
description: "封装表示单元格批注的对象。"
type: docs
url: /zh/java/com.aspose.cells/comment/
---

**Inheritance:**
java.lang.Object
```
public class Comment
```

封装表示单元格批注的对象。

**Example**

```
         Workbook workbook = new Workbook();
         CommentCollection comments = workbook.getWorksheets().get(0).getComments();
 
         //Add comment to cell A1
         int commentIndex1 = comments.add(0, 0);
         Comment comment1 = comments.get(commentIndex1);
         comment1.setNote("First note.");
         comment1.getFont().setName("Times New Roman");
 
         //Add comment to cell B2
         comments.add("B2");
         Comment comment2 = comments.get("B2");
         comment2.setNote("Second note.");
 
         //do your business
 
         //Save the excel file.
         workbook.save("exmaple.xlsx");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [characters(int startIndex, int length)](#characters-int-int-) | 返回一个 Characters 对象，表示注释文本中一段字符范围。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [formatCharacters(int startIndex, int length, Font font, StyleFlag flag)](#formatCharacters-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-) | 使用字体设置格式化部分字符。 |
| [getAuthor()](#getAuthor--) | 获取原始注释作者的姓名。 |
| [getAutoSize()](#getAutoSize--) | 指示是否根据内容自动调整注释的大小。 |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | 获取评论的列索引。 |
| [getCommentShape()](#getCommentShape--) | 获取一个 Shape 对象，表示附加到指定注释的形状。 |
| [getFont()](#getFont--) | 获取注释的字体。 |
| [getHeight()](#getHeight--) | 表示注释的高度，单位为像素。 |
| [getHeightCM()](#getHeightCM--) | 表示注释的高度，单位为厘米。 |
| [getHeightInch()](#getHeightInch--) | 表示注释的高度，单位为英寸。 |
| [getHtmlNote()](#getHtmlNote--) | 获取包含此注释中数据和部分格式的 HTML 字符串。 |
| [getNote()](#getNote--) | 表示注释的内容。 |
| [getRichFormattings()](#getRichFormattings--) | 返回所有 Characters 对象，表示注释文本中一段字符范围。 |
| [getRow()](#getRow--) | 获取注释的行索引。 |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--) | 获取评论的文本水平对齐类型。 |
| [getTextOrientationType()](#getTextOrientationType--) | 获取评论的文本方向类型。 |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--) | 获取评论的文本垂直对齐类型。 |
| [getThreadedComments()](#getThreadedComments--) | 获取线程评论的列表； |
| [getWidth()](#getWidth--) | 表示评论的宽度，单位为像素。 |
| [getWidthCM()](#getWidthCM--) | 表示评论的宽度，单位为厘米。 |
| [getWidthInch()](#getWidthInch--) | 表示评论的宽度，单位为英寸。 |
| [hashCode()](#hashCode--) |  |
| [isThreadedComment()](#isThreadedComment--) | 指示此评论是否为线程评论。 |
| [isVisible()](#isVisible--) | 表示评论是否可见。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | 设置原始评论作者的名称 |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | 指示是否根据内容自动调整注释的大小。 |
| [setHeight(int value)](#setHeight-int-) | 表示注释的高度，单位为像素。 |
| [setHeightCM(double value)](#setHeightCM-double-) | 表示注释的高度，单位为厘米。 |
| [setHeightInch(double value)](#setHeightInch-double-) | 表示注释的高度，单位为英寸。 |
| [setHtmlNote(String value)](#setHtmlNote-java.lang.String-) | 设置包含数据和某些格式的 HTML 字符串于此评论中。 |
| [setNote(String value)](#setNote-java.lang.String-) | 表示注释的内容。 |
| [setTextHorizontalAlignment(int value)](#setTextHorizontalAlignment-int-) | 设置评论的文本水平对齐类型。 |
| [setTextOrientationType(int value)](#setTextOrientationType-int-) | 设置评论的文本方向类型。 |
| [setTextVerticalAlignment(int value)](#setTextVerticalAlignment-int-) | 设置评论的文本垂直对齐类型。 |
| [setVisible(boolean value)](#setVisible-boolean-) | 表示评论是否可见。 |
| [setWidth(int value)](#setWidth-int-) | 表示评论的宽度，单位为像素。 |
| [setWidthCM(double value)](#setWidthCM-double-) | 表示评论的宽度，单位为厘米。 |
| [setWidthInch(double value)](#setWidthInch-double-) | 表示评论的宽度，单位为英寸。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```


返回一个 Characters 对象，表示注释文本中一段字符范围。

**Example**

```
         FontSetting fontSetting = comment1.characters(0, 4);
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

### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


获取原始注释作者的姓名。

**Example**

```
         comment1.setAuthor("Carl.Yang");
```

**Returns:**
java.lang.String
### getAutoSize() {#getAutoSize--}
```
public boolean getAutoSize()
```


指示评论的大小是否根据其内容自动调整。注意：在某些特殊情况下（例如 Mac 环境），此设置可能不起作用。如果此设置未生效，请改用 FitToTextSize()。

**Example**

```
         if(!comment1.getAutoSize())
         {
             //The size of the comment varies with the content
             comment1.setAutoSize(true);
         }
```

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumn() {#getColumn--}
```
public int getColumn()
```


获取评论的列索引。

**Example**

```
         int column = comment1.getColumn();
```

**Returns:**
int
### getCommentShape() {#getCommentShape--}
```
public CommentShape getCommentShape()
```


获取一个 Shape 对象，表示附加到指定注释的形状。

**Example**

```
         CommentShape shape = comment1.getCommentShape();
         int w = shape.getWidth();
         int h = shape.getHeight();
```

**Returns:**
[CommentShape](../../com.aspose.cells/commentshape)
### getFont() {#getFont--}
```
public Font getFont()
```


获取注释的字体。

**Example**

```
         Font font = comment1.getFont();
         font.setSize(12);
```

**Returns:**
[Font](../../com.aspose.cells/font)
### getHeight() {#getHeight--}
```
public int getHeight()
```


表示注释的高度，单位为像素。

**Example**

```
         comment1.setHeight(10);
```

**Returns:**
int
### getHeightCM() {#getHeightCM--}
```
public double getHeightCM()
```


表示注释的高度，单位为厘米。

**Example**

```
         comment1.setHeightCM(1.0);
```

**Returns:**
double
### getHeightInch() {#getHeightInch--}
```
public double getHeightInch()
```


表示注释的高度，单位为英寸。

**Example**

```
         comment1.setHeightInch(1.0);
```

**Returns:**
double
### getHtmlNote() {#getHtmlNote--}
```
public String getHtmlNote()
```


获取包含此注释中数据和部分格式的 HTML 字符串。

**Remarks**

如果这是线程评论，则无法更改该备注，否则 MS Excel 将无法将其处理为线程评论。

**Example**

```
         comment1.setHtmlNote("<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>");
```

**Returns:**
java.lang.String
### getNote() {#getNote--}
```
public String getNote()
```


表示注释的内容。

**Remarks**

如果这是线程评论，则无法更改该备注，否则 MS Excel 将无法将其处理为线程评论。

**Example**

```
         comment1.setNote("First note.");
```

**Returns:**
java.lang.String
### getRichFormattings() {#getRichFormattings--}
```
public FontSetting[] getRichFormattings()
```


返回所有 Characters 对象，表示注释文本中一段字符范围。

**Example**

```
         FontSetting[] list = comment1.getRichFormattings();
```

**Returns:**
com.aspose.cells.FontSetting[] - 所有字符对象
### getRow() {#getRow--}
```
public int getRow()
```


获取注释的行索引。

**Example**

```
         int row = comment1.getRow();
```

**Returns:**
int
### getTextHorizontalAlignment() {#getTextHorizontalAlignment--}
```
public int getTextHorizontalAlignment()
```


获取评论的文本水平对齐类型。

参见 [TextAlignmentType](../../com.aspose.cells/textalignmenttype)。

**Example**

```
         if (comment1.getTextHorizontalAlignment() ==  TextAlignmentType.FILL)
         {
             comment1.setTextHorizontalAlignment(TextAlignmentType.CENTER);
         }
```

**Returns:**
int
### getTextOrientationType() {#getTextOrientationType--}
```
public int getTextOrientationType()
```


获取评论的文本方向类型。

参见 [TextOrientationType](../../com.aspose.cells/textorientationtype)。

**Example**

```
         if(comment1.getTextOrientationType() == TextOrientationType.NO_ROTATION)
         {
             comment1.setTextOrientationType(TextOrientationType.TOP_TO_BOTTOM);
         }
```

**Returns:**
int
### getTextVerticalAlignment() {#getTextVerticalAlignment--}
```
public int getTextVerticalAlignment()
```


获取评论的文本垂直对齐类型。

参见 [TextAlignmentType](../../com.aspose.cells/textalignmenttype)。

**Example**

```
         if (comment1.getTextVerticalAlignment() ==  TextAlignmentType.FILL)
         {
             comment1.setTextVerticalAlignment(TextAlignmentType.CENTER);
         }
```

**Returns:**
int
### getThreadedComments() {#getThreadedComments--}
```
public ThreadedCommentCollection getThreadedComments()
```


获取线程评论的列表；

**Example**

```
         ThreadedCommentCollection threadedComments = comment1.getThreadedComments();
         for (int i = 0; i <threadedComments.getCount(); ++i)
         {
             ThreadedComment tc = threadedComments.get(i);
             String note = tc.getNotes();
         }
```

**Returns:**
[ThreadedCommentCollection](../../com.aspose.cells/threadedcommentcollection)
### getWidth() {#getWidth--}
```
public int getWidth()
```


表示评论的宽度，单位为像素。

**Example**

```
         comment1.setWidth(10);
```

**Returns:**
int
### getWidthCM() {#getWidthCM--}
```
public double getWidthCM()
```


表示评论的宽度，单位为厘米。

**Example**

```
         comment1.setWidthCM(1.0);
```

**Returns:**
double
### getWidthInch() {#getWidthInch--}
```
public double getWidthInch()
```


表示评论的宽度，单位为英寸。

**Example**

```
         comment1.setWidthInch(1.0);
```

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isThreadedComment() {#isThreadedComment--}
```
public boolean isThreadedComment()
```


指示此评论是否为线程评论。

**Example**

```
         if(comment1.isThreadedComment())
         {
             //This comment is a threaded comment.
         }
```

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


表示评论是否可见。

**Example**

```
         if(comment1.isVisible())
         {
             //The comment is visible
         }
```

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




### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


设置原始评论作者的名称

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setAutoSize(boolean value) {#setAutoSize-boolean-}
```
public void setAutoSize(boolean value)
```


指示评论的大小是否根据其内容自动调整。注意：在某些特殊情况下（例如 Mac 环境），此设置可能不起作用。如果此设置未生效，请改用 FitToTextSize()。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


表示注释的高度，单位为像素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setHeightCM(double value) {#setHeightCM-double-}
```
public void setHeightCM(double value)
```


表示注释的高度，单位为厘米。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setHeightInch(double value) {#setHeightInch-double-}
```
public void setHeightInch(double value)
```


表示注释的高度，单位为英寸。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setHtmlNote(String value) {#setHtmlNote-java.lang.String-}
```
public void setHtmlNote(String value)
```


设置包含数据和某些格式的 HTML 字符串于此评论中。

**Remarks**

如果这是线程评论，则无法更改该备注，否则 MS Excel 将无法将其处理为线程评论。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setNote(String value) {#setNote-java.lang.String-}
```
public void setNote(String value)
```


表示注释的内容。

**Remarks**

如果这是线程评论，则无法更改该备注，否则 MS Excel 将无法将其处理为线程评论。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setTextHorizontalAlignment(int value) {#setTextHorizontalAlignment-int-}
```
public void setTextHorizontalAlignment(int value)
```


设置评论的文本水平对齐类型。

参见 [TextAlignmentType](../../com.aspose.cells/textalignmenttype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTextOrientationType(int value) {#setTextOrientationType-int-}
```
public void setTextOrientationType(int value)
```


设置评论的文本方向类型。

参见 [TextOrientationType](../../com.aspose.cells/textorientationtype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTextVerticalAlignment(int value) {#setTextVerticalAlignment-int-}
```
public void setTextVerticalAlignment(int value)
```


设置评论的文本垂直对齐类型。

参见 [TextAlignmentType](../../com.aspose.cells/textalignmenttype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


表示评论是否可见。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


表示评论的宽度，单位为像素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setWidthCM(double value) {#setWidthCM-double-}
```
public void setWidthCM(double value)
```


表示评论的宽度，单位为厘米。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setWidthInch(double value) {#setWidthInch-double-}
```
public void setWidthInch(double value)
```


表示评论的宽度，单位为英寸。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

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

