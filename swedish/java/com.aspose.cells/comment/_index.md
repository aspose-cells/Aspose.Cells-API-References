---
title: "Comment"
second_title: "Aspose.Cells för Java API-referens"
description: "Inkapslar objektet som representerar en cellkommentar."
type: docs
url: /sv/java/com.aspose.cells/comment/
---

**Inheritance:**
java.lang.Object
```
public class Comment
```

Inkapslar objektet som representerar en cellkommentar.

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
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [characters(int startIndex, int length)](#characters-int-int-) | Returnerar ett Characters-objekt som representerar ett intervall av tecken inom kommentartexten. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [formatCharacters(int startIndex, int length, Font font, StyleFlag flag)](#formatCharacters-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-) | Formatera vissa tecken med teckensnittsinställningen. |
| [getAuthor()](#getAuthor--) | Hämtar namnet på den ursprungliga kommentarsförfattaren |
| [getAutoSize()](#getAutoSize--) | Indikerar om kommentarsstorleken justeras automatiskt enligt dess innehåll. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Hämtar kolumnindexet för kommentaren. |
| [getCommentShape()](#getCommentShape--) | Hämta ett Shape-objekt som representerar formen som är bifogad till den angivna kommentaren. |
| [getFont()](#getFont--) | Hämtar kommentarsfonten. |
| [getHeight()](#getHeight--) | Representerar kommentarsens höjd, i enheten pixlar. |
| [getHeightCM()](#getHeightCM--) | Representerar kommentarsens höjd, i enheten centimeter. |
| [getHeightInch()](#getHeightInch--) | Representerar kommentarsens höjd, i enheten tum. |
| [getHtmlNote()](#getHtmlNote--) | Hämtar HTML-strängen som innehåller data och vissa format i denna kommentar. |
| [getNote()](#getNote--) | Representerar kommentarens innehåll. |
| [getRichFormattings()](#getRichFormattings--) | Returnerar alla Characters-objekt som representerar ett intervall av tecken inom kommentartexten. |
| [getRow()](#getRow--) | Hämtar radindexet för kommentaren. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--) | Hämtar den horisontella justeringstypen för kommentarens text. |
| [getTextOrientationType()](#getTextOrientationType--) | Hämtar textorienteringstypen för kommentaren. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--) | Hämtar den vertikala justeringstypen för kommentarens text. |
| [getThreadedComments()](#getThreadedComments--) | Hämtar listan med trådade kommentarer; |
| [getWidth()](#getWidth--) | Representerar kommentarsens bredd, i enheten pixlar. |
| [getWidthCM()](#getWidthCM--) | Representerar kommentarsens bredd, i enheten centimeter. |
| [getWidthInch()](#getWidthInch--) | Representerar kommentarsens bredd, i enheten tum. |
| [hashCode()](#hashCode--) |  |
| [isThreadedComment()](#isThreadedComment--) | Indikerar om denna kommentar är en trådad kommentar. |
| [isVisible()](#isVisible--) | Representerar om kommentaren är synlig eller inte. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Ställer in namn på den ursprungliga kommentarsförfattaren |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Indikerar om kommentarsstorleken justeras automatiskt enligt dess innehåll. |
| [setHeight(int value)](#setHeight-int-) | Representerar kommentarsens höjd, i enheten pixlar. |
| [setHeightCM(double value)](#setHeightCM-double-) | Representerar kommentarsens höjd, i enheten centimeter. |
| [setHeightInch(double value)](#setHeightInch-double-) | Representerar kommentarsens höjd, i enheten tum. |
| [setHtmlNote(String value)](#setHtmlNote-java.lang.String-) | Ställer in HTML-strängen som innehåller data och vissa format i den här kommentaren. |
| [setNote(String value)](#setNote-java.lang.String-) | Representerar kommentarens innehåll. |
| [setTextHorizontalAlignment(int value)](#setTextHorizontalAlignment-int-) | Ställer in den horisontella justeringstypen för texten i kommentaren. |
| [setTextOrientationType(int value)](#setTextOrientationType-int-) | Ställer in textorienteringstypen för kommentaren. |
| [setTextVerticalAlignment(int value)](#setTextVerticalAlignment-int-) | Ställer in den vertikala justeringstypen för texten i kommentaren. |
| [setVisible(boolean value)](#setVisible-boolean-) | Representerar om kommentaren är synlig eller inte. |
| [setWidth(int value)](#setWidth-int-) | Representerar kommentarsens bredd, i enheten pixlar. |
| [setWidthCM(double value)](#setWidthCM-double-) | Representerar kommentarsens bredd, i enheten centimeter. |
| [setWidthInch(double value)](#setWidthInch-double-) | Representerar kommentarsens bredd, i enheten tum. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```


Returnerar ett Characters-objekt som representerar ett intervall av tecken inom kommentartexten.

**Example**

```
         FontSetting fontSetting = comment1.characters(0, 4);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startIndex | int | Indexet för tecknets början. |
| length | int | Antalet tecken. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - Characters object.
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### formatCharacters(int startIndex, int length, Font font, StyleFlag flag) {#formatCharacters-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-}
```
public void formatCharacters(int startIndex, int length, Font font, StyleFlag flag)
```


Formatera vissa tecken med teckensnittsinställningen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startIndex | int | Startindexet. |
| length | int | Längden. |
| font | [Font](../../com.aspose.cells/font) | Typsnittsinställningen. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Flaggan för typsnittsinställningen. |

### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Hämtar namnet på den ursprungliga kommentarsförfattaren

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


Indikerar om storleken på kommentaren justeras automatiskt enligt dess innehåll. Obs: I vissa speciella fall (t.ex. Mac-miljö) kan den här inställningen inte träda i kraft. Om den här inställningen inte fungerar, ersätt den med FitToTextSize().

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


Hämtar kolumnindexet för kommentaren.

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


Hämta ett Shape-objekt som representerar formen som är bifogad till den angivna kommentaren.

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


Hämtar kommentarsfonten.

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


Representerar kommentarsens höjd, i enheten pixlar.

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


Representerar kommentarsens höjd, i enheten centimeter.

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


Representerar kommentarsens höjd, i enheten tum.

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


Hämtar HTML-strängen som innehåller data och vissa format i denna kommentar.

**Remarks**

Om detta är en trådad kommentar kan noteringen inte ändras, annars kan MS Excel inte behandla den som en trådad kommentar.

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


Representerar kommentarens innehåll.

**Remarks**

Om detta är en trådad kommentar kan noteringen inte ändras, annars kan MS Excel inte behandla den som en trådad kommentar.

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


Returnerar alla Characters-objekt som representerar ett intervall av tecken inom kommentartexten.

**Example**

```
         FontSetting[] list = comment1.getRichFormattings();
```

**Returns:**
com.aspose.cells.FontSetting[] - Alla tecken‑objekt
### getRow() {#getRow--}
```
public int getRow()
```


Hämtar radindexet för kommentaren.

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


Hämtar den horisontella justeringstypen för kommentarens text.

Se [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

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


Hämtar textorienteringstypen för kommentaren.

Se [TextOrientationType](../../com.aspose.cells/textorientationtype).

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


Hämtar den vertikala justeringstypen för kommentarens text.

Se [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

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


Hämtar listan med trådade kommentarer;

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


Representerar kommentarsens bredd, i enheten pixlar.

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


Representerar kommentarsens bredd, i enheten centimeter.

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


Representerar kommentarsens bredd, i enheten tum.

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


Indikerar om denna kommentar är en trådad kommentar.

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


Representerar om kommentaren är synlig eller inte.

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


Ställer in namn på den ursprungliga kommentarsförfattaren

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setAutoSize(boolean value) {#setAutoSize-boolean-}
```
public void setAutoSize(boolean value)
```


Indikerar om storleken på kommentaren justeras automatiskt enligt dess innehåll. Obs: I vissa speciella fall (t.ex. Mac-miljö) kan den här inställningen inte träda i kraft. Om den här inställningen inte fungerar, ersätt den med FitToTextSize().

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


Representerar kommentarsens höjd, i enheten pixlar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setHeightCM(double value) {#setHeightCM-double-}
```
public void setHeightCM(double value)
```


Representerar kommentarsens höjd, i enheten centimeter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setHeightInch(double value) {#setHeightInch-double-}
```
public void setHeightInch(double value)
```


Representerar kommentarsens höjd, i enheten tum.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setHtmlNote(String value) {#setHtmlNote-java.lang.String-}
```
public void setHtmlNote(String value)
```


Ställer in HTML-strängen som innehåller data och vissa format i den här kommentaren.

**Remarks**

Om detta är en trådad kommentar kan noteringen inte ändras, annars kan MS Excel inte behandla den som en trådad kommentar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setNote(String value) {#setNote-java.lang.String-}
```
public void setNote(String value)
```


Representerar kommentarens innehåll.

**Remarks**

Om detta är en trådad kommentar kan noteringen inte ändras, annars kan MS Excel inte behandla den som en trådad kommentar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setTextHorizontalAlignment(int value) {#setTextHorizontalAlignment-int-}
```
public void setTextHorizontalAlignment(int value)
```


Ställer in den horisontella justeringstypen för texten i kommentaren.

Se [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setTextOrientationType(int value) {#setTextOrientationType-int-}
```
public void setTextOrientationType(int value)
```


Ställer in textorienteringstypen för kommentaren.

Se [TextOrientationType](../../com.aspose.cells/textorientationtype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setTextVerticalAlignment(int value) {#setTextVerticalAlignment-int-}
```
public void setTextVerticalAlignment(int value)
```


Ställer in den vertikala justeringstypen för texten i kommentaren.

Se [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Representerar om kommentaren är synlig eller inte.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


Representerar kommentarsens bredd, i enheten pixlar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setWidthCM(double value) {#setWidthCM-double-}
```
public void setWidthCM(double value)
```


Representerar kommentarsens bredd, i enheten centimeter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setWidthInch(double value) {#setWidthInch-double-}
```
public void setWidthInch(double value)
```


Representerar kommentarsens bredd, i enheten tum.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

