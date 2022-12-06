---
title: Comment
second_title: Aspose.Cells for Java API Reference
description: Encapsulates the object that represents a cell comment.
type: docs
url: /java/com.aspose.cells/comment/
---

**Inheritance:**
java.lang.Object
```
public class Comment
```

Encapsulates the object that represents a cell comment.

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
## Methods

| Method | Description |
| --- | --- |
| [characters(int startIndex, int length)](#characters-int-int-) | Returns a Characters object that represents a range of characters within the comment text. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [formatCharacters(int startIndex, int length, Font font, StyleFlag flag)](#formatCharacters-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-) | Format some characters with the font setting. |
| [getAuthor()](#getAuthor--) | Name of the original comment author |
| [getAutoSize()](#getAutoSize--) | Indicates if size of comment is adjusted automatically according to its content. |
| [getCharacters()](#getCharacters--) | Returns all Characters objects that represents a range of characters within the comment text. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Gets the column index of the comment. |
| [getCommentShape()](#getCommentShape--) | Get a Shape object that represents the shape attached to the specified comment. |
| [getFont()](#getFont--) | Gets the font of comment. |
| [getHeight()](#getHeight--) | Represents the Height of the comment, in unit of pixels. |
| [getHeightCM()](#getHeightCM--) | Represents the height of the comment, in unit of centimeters. |
| [getHeightInch()](#getHeightInch--) | Represents the height of the comment, in unit of inches. |
| [getHtmlNote()](#getHtmlNote--) | the html string which contains data and some formats in this comment. |
| [getNote()](#getNote--) | Represents the content of comment. |
| [getRow()](#getRow--) | Gets the row index of the comment. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--) | the text horizontal alignment type of the comment. |
| [getTextOrientationType()](#getTextOrientationType--) | the text orientation type of the comment. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--) | the text vertical alignment type of the comment. |
| [getThreadedComments()](#getThreadedComments--) | Gets the list of threaded comments; |
| [getWidth()](#getWidth--) | Represents the width of the comment, in unit of pixels. |
| [getWidthCM()](#getWidthCM--) | Represents the width of the comment, in unit of centimeters. |
| [getWidthInch()](#getWidthInch--) | Represents the width of the comment, in unit of inches. |
| [hashCode()](#hashCode--) |  |
| [isThreadedComment()](#isThreadedComment--) | Indicates whether this comment is a threaded comment. |
| [isVisible()](#isVisible--) | Represents if the comment is visible or not. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | For the description of this property, please see [getAuthor()](../../com.aspose.cells/comment\#getAuthor--) |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | For the description of this property, please see [getAutoSize()](../../com.aspose.cells/comment\#getAutoSize--) |
| [setHeight(int value)](#setHeight-int-) | For the description of this property, please see [getHeight()](../../com.aspose.cells/comment\#getHeight--) |
| [setHeightCM(double value)](#setHeightCM-double-) | For the description of this property, please see [getHeightCM()](../../com.aspose.cells/comment\#getHeightCM--) |
| [setHeightInch(double value)](#setHeightInch-double-) | For the description of this property, please see [getHeightInch()](../../com.aspose.cells/comment\#getHeightInch--) |
| [setHtmlNote(String value)](#setHtmlNote-java.lang.String-) | For the description of this property, please see [getHtmlNote()](../../com.aspose.cells/comment\#getHtmlNote--) |
| [setNote(String value)](#setNote-java.lang.String-) | For the description of this property, please see [getNote()](../../com.aspose.cells/comment\#getNote--) |
| [setTextHorizontalAlignment(int value)](#setTextHorizontalAlignment-int-) | For the description of this property, please see [getTextHorizontalAlignment()](../../com.aspose.cells/comment\#getTextHorizontalAlignment--) |
| [setTextOrientationType(int value)](#setTextOrientationType-int-) | For the description of this property, please see [getTextOrientationType()](../../com.aspose.cells/comment\#getTextOrientationType--) |
| [setTextVerticalAlignment(int value)](#setTextVerticalAlignment-int-) | For the description of this property, please see [getTextVerticalAlignment()](../../com.aspose.cells/comment\#getTextVerticalAlignment--) |
| [setVisible(boolean value)](#setVisible-boolean-) | For the description of this property, please see [isVisible()](../../com.aspose.cells/comment\#isVisible--) |
| [setWidth(int value)](#setWidth-int-) | For the description of this property, please see [getWidth()](../../com.aspose.cells/comment\#getWidth--) |
| [setWidthCM(double value)](#setWidthCM-double-) | For the description of this property, please see [getWidthCM()](../../com.aspose.cells/comment\#getWidthCM--) |
| [setWidthInch(double value)](#setWidthInch-double-) | For the description of this property, please see [getWidthInch()](../../com.aspose.cells/comment\#getWidthInch--) |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```


Returns a Characters object that represents a range of characters within the comment text.

```
FontSetting fontSetting = comment1.characters(0, 4);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | int | The index of the start of the character. |
| length | int | The number of characters. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - Characters object.
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
### formatCharacters(int startIndex, int length, Font font, StyleFlag flag) {#formatCharacters-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-}
```
public void formatCharacters(int startIndex, int length, Font font, StyleFlag flag)
```


Format some characters with the font setting.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | int | The start index. |
| length | int | The length. |
| font | [Font](../../com.aspose.cells/font) | The font setting. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | The flag of the font setting. |

### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Name of the original comment author

```
comment1.setAuthor("Carl.Yang");
```

**Returns:**
java.lang.String
### getAutoSize() {#getAutoSize--}
```
public boolean getAutoSize()
```


Indicates if size of comment is adjusted automatically according to its content.

```
if(!comment1.getAutoSize())
         {
             //The size of the comment varies with the content
             comment1.setAutoSize(true);
         }
```

**Returns:**
boolean
### getCharacters() {#getCharacters--}
```
public ArrayList getCharacters()
```


Returns all Characters objects that represents a range of characters within the comment text.

```
ArrayList list = comment1.getCharacters();
```

**Returns:**
java.util.ArrayList - All Characters objects
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


Gets the column index of the comment.

```
int column = comment1.getColumn();
```

**Returns:**
int
### getCommentShape() {#getCommentShape--}
```
public CommentShape getCommentShape()
```


Get a Shape object that represents the shape attached to the specified comment.

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


Gets the font of comment.

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


Represents the Height of the comment, in unit of pixels.

```
comment1.setHeight(10);
```

**Returns:**
int
### getHeightCM() {#getHeightCM--}
```
public double getHeightCM()
```


Represents the height of the comment, in unit of centimeters.

```
comment1.setHeightCM(1.0);
```

**Returns:**
double
### getHeightInch() {#getHeightInch--}
```
public double getHeightInch()
```


Represents the height of the comment, in unit of inches.

```
comment1.setHeightInch(1.0);
```

**Returns:**
double
### getHtmlNote() {#getHtmlNote--}
```
public String getHtmlNote()
```


the html string which contains data and some formats in this comment. If this is a threaded comment, the note could not be changed, otherwise MS Excel could not process it as a threaded comment.

```
comment1.setHtmlNote("<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>");
```

**Returns:**
java.lang.String
### getNote() {#getNote--}
```
public String getNote()
```


Represents the content of comment. If this is a threaded comment, the note could not be changed, otherwise MS Excel could not process it as a threaded comment.

```
comment1.setNote("First note.");
```

**Returns:**
java.lang.String
### getRow() {#getRow--}
```
public int getRow()
```


Gets the row index of the comment.

```
int row = comment1.getRow();
```

**Returns:**
int
### getTextHorizontalAlignment() {#getTextHorizontalAlignment--}
```
public int getTextHorizontalAlignment()
```


the text horizontal alignment type of the comment.

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


the text orientation type of the comment.

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


the text vertical alignment type of the comment.

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


Gets the list of threaded comments;

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


Represents the width of the comment, in unit of pixels.

```
comment1.setWidth(10);
```

**Returns:**
int
### getWidthCM() {#getWidthCM--}
```
public double getWidthCM()
```


Represents the width of the comment, in unit of centimeters.

```
comment1.setWidthCM(1.0);
```

**Returns:**
double
### getWidthInch() {#getWidthInch--}
```
public double getWidthInch()
```


Represents the width of the comment, in unit of inches.

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


Indicates whether this comment is a threaded comment.

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


Represents if the comment is visible or not.

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


For the description of this property, please see [getAuthor()](../../com.aspose.cells/comment\#getAuthor--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setAutoSize(boolean value) {#setAutoSize-boolean-}
```
public void setAutoSize(boolean value)
```


For the description of this property, please see [getAutoSize()](../../com.aspose.cells/comment\#getAutoSize--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


For the description of this property, please see [getHeight()](../../com.aspose.cells/comment\#getHeight--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setHeightCM(double value) {#setHeightCM-double-}
```
public void setHeightCM(double value)
```


For the description of this property, please see [getHeightCM()](../../com.aspose.cells/comment\#getHeightCM--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setHeightInch(double value) {#setHeightInch-double-}
```
public void setHeightInch(double value)
```


For the description of this property, please see [getHeightInch()](../../com.aspose.cells/comment\#getHeightInch--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setHtmlNote(String value) {#setHtmlNote-java.lang.String-}
```
public void setHtmlNote(String value)
```


For the description of this property, please see [getHtmlNote()](../../com.aspose.cells/comment\#getHtmlNote--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setNote(String value) {#setNote-java.lang.String-}
```
public void setNote(String value)
```


For the description of this property, please see [getNote()](../../com.aspose.cells/comment\#getNote--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setTextHorizontalAlignment(int value) {#setTextHorizontalAlignment-int-}
```
public void setTextHorizontalAlignment(int value)
```


For the description of this property, please see [getTextHorizontalAlignment()](../../com.aspose.cells/comment\#getTextHorizontalAlignment--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTextOrientationType(int value) {#setTextOrientationType-int-}
```
public void setTextOrientationType(int value)
```


For the description of this property, please see [getTextOrientationType()](../../com.aspose.cells/comment\#getTextOrientationType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTextVerticalAlignment(int value) {#setTextVerticalAlignment-int-}
```
public void setTextVerticalAlignment(int value)
```


For the description of this property, please see [getTextVerticalAlignment()](../../com.aspose.cells/comment\#getTextVerticalAlignment--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


For the description of this property, please see [isVisible()](../../com.aspose.cells/comment\#isVisible--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


For the description of this property, please see [getWidth()](../../com.aspose.cells/comment\#getWidth--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setWidthCM(double value) {#setWidthCM-double-}
```
public void setWidthCM(double value)
```


For the description of this property, please see [getWidthCM()](../../com.aspose.cells/comment\#getWidthCM--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setWidthInch(double value) {#setWidthInch-double-}
```
public void setWidthInch(double value)
```


For the description of this property, please see [getWidthInch()](../../com.aspose.cells/comment\#getWidthInch--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

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

