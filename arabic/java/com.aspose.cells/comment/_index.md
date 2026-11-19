---
title: "Comment"
second_title: "Aspose.Cells for Java API Reference"
description: "يغلف الكائن الذي يمثل تعليق خلية."
type: docs
url: /ar/java/com.aspose.cells/comment/
---

**Inheritance:**
java.lang.Object
```
public class Comment
```

يغلف الكائن الذي يمثل تعليق خلية.

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
## الطرق

| طريقة | الوصف |
| --- | --- |
| [characters(int startIndex, int length)](#characters-int-int-) | يرجع كائن Characters يمثل نطاقًا من الأحرف داخل نص التعليق. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [formatCharacters(int startIndex, int length, Font font, StyleFlag flag)](#formatCharacters-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-) | قم بتنسيق بعض الأحرف باستخدام إعداد الخط. |
| [getAuthor()](#getAuthor--) | يحصل على اسم مؤلف التعليق الأصلي |
| [getAutoSize()](#getAutoSize--) | يشير إلى ما إذا كان حجم التعليق يتم ضبطه تلقائيًا وفقًا لمحتواه. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | يحصل على فهرس العمود للتعليق. |
| [getCommentShape()](#getCommentShape--) | احصل على كائن Shape يمثل الشكل المرفق بالتعليق المحدد. |
| [getFont()](#getFont--) | يحصل على خط التعليق. |
| [getHeight()](#getHeight--) | يمثل ارتفاع التعليق، بوحدة البكسل. |
| [getHeightCM()](#getHeightCM--) | يمثل ارتفاع التعليق، بوحدة السنتيمتر. |
| [getHeightInch()](#getHeightInch--) | يمثل ارتفاع التعليق، بوحدة البوصة. |
| [getHtmlNote()](#getHtmlNote--) | يحصل على سلسلة HTML التي تحتوي على البيانات وبعض التنسيقات في هذا التعليق. |
| [getNote()](#getNote--) | يمثل محتوى التعليق. |
| [getRichFormattings()](#getRichFormattings--) | يرجع جميع كائنات Characters التي تمثل نطاقًا من الأحرف داخل نص التعليق. |
| [getRow()](#getRow--) | يحصل على فهرس الصف للتعليق. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--) | يحصل على نوع محاذاة النص الأفقية للتعليق. |
| [getTextOrientationType()](#getTextOrientationType--) | يحصل على نوع اتجاه النص للتعليق. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--) | يحصل على نوع محاذاة النص العمودية للتعليق. |
| [getThreadedComments()](#getThreadedComments--) | يحصل على قائمة التعليقات المتسلسلة؛ |
| [getWidth()](#getWidth--) | يمثل عرض التعليق بوحدة البكسل. |
| [getWidthCM()](#getWidthCM--) | يمثل عرض التعليق بوحدة السنتيمتر. |
| [getWidthInch()](#getWidthInch--) | يمثل عرض التعليق بوحدة البوصة. |
| [hashCode()](#hashCode--) |  |
| [isThreadedComment()](#isThreadedComment--) | يشير إلى ما إذا كان هذا التعليق تعليقًا متسلسلًا. |
| [isVisible()](#isVisible--) | يمثل ما إذا كان التعليق مرئيًا أم لا. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | يضبط اسم مؤلف التعليق الأصلي |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | يشير إلى ما إذا كان حجم التعليق يتم ضبطه تلقائيًا وفقًا لمحتواه. |
| [setHeight(int value)](#setHeight-int-) | يمثل ارتفاع التعليق، بوحدة البكسل. |
| [setHeightCM(double value)](#setHeightCM-double-) | يمثل ارتفاع التعليق، بوحدة السنتيمتر. |
| [setHeightInch(double value)](#setHeightInch-double-) | يمثل ارتفاع التعليق، بوحدة البوصة. |
| [setHtmlNote(String value)](#setHtmlNote-java.lang.String-) | يضبط سلسلة HTML التي تحتوي على البيانات وبعض الصيغ في هذا التعليق. |
| [setNote(String value)](#setNote-java.lang.String-) | يمثل محتوى التعليق. |
| [setTextHorizontalAlignment(int value)](#setTextHorizontalAlignment-int-) | يضبط نوع محاذاة النص الأفقية للتعليق. |
| [setTextOrientationType(int value)](#setTextOrientationType-int-) | يضبط نوع اتجاه النص للتعليق. |
| [setTextVerticalAlignment(int value)](#setTextVerticalAlignment-int-) | يضبط نوع محاذاة النص العمودية للتعليق. |
| [setVisible(boolean value)](#setVisible-boolean-) | يمثل ما إذا كان التعليق مرئيًا أم لا. |
| [setWidth(int value)](#setWidth-int-) | يمثل عرض التعليق بوحدة البكسل. |
| [setWidthCM(double value)](#setWidthCM-double-) | يمثل عرض التعليق بوحدة السنتيمتر. |
| [setWidthInch(double value)](#setWidthInch-double-) | يمثل عرض التعليق بوحدة البوصة. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```


يرجع كائن Characters يمثل نطاقًا من الأحرف داخل نص التعليق.

**Example**

```
         FontSetting fontSetting = comment1.characters(0, 4);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startIndex | int | فهرس بداية الحرف. |
| length | int | عدد الأحرف. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - Characters object.
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
### formatCharacters(int startIndex, int length, Font font, StyleFlag flag) {#formatCharacters-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-}
```
public void formatCharacters(int startIndex, int length, Font font, StyleFlag flag)
```


قم بتنسيق بعض الأحرف باستخدام إعداد الخط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startIndex | int | فهرس البداية. |
| length | int | الطول. |
| font | [Font](../../com.aspose.cells/font) | إعداد الخط. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | علامة إعداد الخط. |

### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


يحصل على اسم مؤلف التعليق الأصلي

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


يشير إلى ما إذا تم تعديل حجم التعليق تلقائيًا وفقًا لمحتواه. ملاحظة: في بعض الحالات الخاصة (مثل بيئة ماك)، قد لا يكون لهذا الإعداد تأثير. إذا لم يحدث تأثير لهذا الإعداد، يرجى استبداله بـ FitToTextSize().

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


يحصل على فهرس العمود للتعليق.

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


احصل على كائن Shape يمثل الشكل المرفق بالتعليق المحدد.

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


يحصل على خط التعليق.

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


يمثل ارتفاع التعليق، بوحدة البكسل.

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


يمثل ارتفاع التعليق، بوحدة السنتيمتر.

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


يمثل ارتفاع التعليق، بوحدة البوصة.

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


يحصل على سلسلة HTML التي تحتوي على البيانات وبعض التنسيقات في هذا التعليق.

**Remarks**

إذا كان هذا تعليقًا متسلسلًا، لا يمكن تغيير الملاحظة، وإلا لن يتمكن MS Excel من معالجته كتعليق متسلسل.

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


يمثل محتوى التعليق.

**Remarks**

إذا كان هذا تعليقًا متسلسلًا، لا يمكن تغيير الملاحظة، وإلا لن يتمكن MS Excel من معالجته كتعليق متسلسل.

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


يرجع جميع كائنات Characters التي تمثل نطاقًا من الأحرف داخل نص التعليق.

**Example**

```
         FontSetting[] list = comment1.getRichFormattings();
```

**Returns:**
com.aspose.cells.FontSetting[] - جميع كائنات الأحرف
### getRow() {#getRow--}
```
public int getRow()
```


يحصل على فهرس الصف للتعليق.

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


يحصل على نوع محاذاة النص الأفقية للتعليق.

انظر [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

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


يحصل على نوع اتجاه النص للتعليق.

انظر [TextOrientationType](../../com.aspose.cells/textorientationtype).

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


يحصل على نوع محاذاة النص العمودية للتعليق.

انظر [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

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


يحصل على قائمة التعليقات المتسلسلة؛

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


يمثل عرض التعليق بوحدة البكسل.

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


يمثل عرض التعليق بوحدة السنتيمتر.

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


يمثل عرض التعليق بوحدة البوصة.

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


يشير إلى ما إذا كان هذا التعليق تعليقًا متسلسلًا.

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


يمثل ما إذا كان التعليق مرئيًا أم لا.

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


يضبط اسم مؤلف التعليق الأصلي

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setAutoSize(boolean value) {#setAutoSize-boolean-}
```
public void setAutoSize(boolean value)
```


يشير إلى ما إذا تم تعديل حجم التعليق تلقائيًا وفقًا لمحتواه. ملاحظة: في بعض الحالات الخاصة (مثل بيئة ماك)، قد لا يكون لهذا الإعداد تأثير. إذا لم يحدث تأثير لهذا الإعداد، يرجى استبداله بـ FitToTextSize().

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


يمثل ارتفاع التعليق، بوحدة البكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setHeightCM(double value) {#setHeightCM-double-}
```
public void setHeightCM(double value)
```


يمثل ارتفاع التعليق، بوحدة السنتيمتر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setHeightInch(double value) {#setHeightInch-double-}
```
public void setHeightInch(double value)
```


يمثل ارتفاع التعليق، بوحدة البوصة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setHtmlNote(String value) {#setHtmlNote-java.lang.String-}
```
public void setHtmlNote(String value)
```


يضبط سلسلة HTML التي تحتوي على البيانات وبعض الصيغ في هذا التعليق.

**Remarks**

إذا كان هذا تعليقًا متسلسلًا، لا يمكن تغيير الملاحظة، وإلا لن يتمكن MS Excel من معالجته كتعليق متسلسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setNote(String value) {#setNote-java.lang.String-}
```
public void setNote(String value)
```


يمثل محتوى التعليق.

**Remarks**

إذا كان هذا تعليقًا متسلسلًا، لا يمكن تغيير الملاحظة، وإلا لن يتمكن MS Excel من معالجته كتعليق متسلسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setTextHorizontalAlignment(int value) {#setTextHorizontalAlignment-int-}
```
public void setTextHorizontalAlignment(int value)
```


يضبط نوع محاذاة النص الأفقية للتعليق.

انظر [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTextOrientationType(int value) {#setTextOrientationType-int-}
```
public void setTextOrientationType(int value)
```


يضبط نوع اتجاه النص للتعليق.

انظر [TextOrientationType](../../com.aspose.cells/textorientationtype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTextVerticalAlignment(int value) {#setTextVerticalAlignment-int-}
```
public void setTextVerticalAlignment(int value)
```


يضبط نوع محاذاة النص العمودية للتعليق.

انظر [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


يمثل ما إذا كان التعليق مرئيًا أم لا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


يمثل عرض التعليق بوحدة البكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setWidthCM(double value) {#setWidthCM-double-}
```
public void setWidthCM(double value)
```


يمثل عرض التعليق بوحدة السنتيمتر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setWidthInch(double value) {#setWidthInch-double-}
```
public void setWidthInch(double value)
```


يمثل عرض التعليق بوحدة البوصة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

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

