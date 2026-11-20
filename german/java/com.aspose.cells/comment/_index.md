---
title: "Comment"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Kapselt das Objekt, das einen Zellkommentar darstellt."
type: docs
url: /de/java/com.aspose.cells/comment/
---

**Inheritance:**
java.lang.Object
```
public class Comment
```

Kapselt das Objekt, das einen Zellkommentar darstellt.

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
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [characters(int startIndex, int length)](#characters-int-int-) | Gibt ein Characters-Objekt zurück, das einen Zeichenbereich im Kommentartext darstellt. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [formatCharacters(int startIndex, int length, Font font, StyleFlag flag)](#formatCharacters-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-) | Formatiere einige Zeichen mit den Schriftarteinstellungen. |
| [getAuthor()](#getAuthor--) | Ermittelt den Namen des ursprünglichen Kommentarautors. |
| [getAutoSize()](#getAutoSize--) | Gibt an, ob die Größe des Kommentars automatisch an dessen Inhalt angepasst wird. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Liefert den Spaltenindex des Kommentars. |
| [getCommentShape()](#getCommentShape--) | Erhalte ein Shape-Objekt, das die dem angegebenen Kommentar zugefügte Form darstellt. |
| [getFont()](#getFont--) | Ermittelt die Schriftart des Kommentars. |
| [getHeight()](#getHeight--) | Stellt die Höhe des Kommentars in Pixeln dar. |
| [getHeightCM()](#getHeightCM--) | Stellt die Höhe des Kommentars in Zentimetern dar. |
| [getHeightInch()](#getHeightInch--) | Stellt die Höhe des Kommentars in Zoll dar. |
| [getHtmlNote()](#getHtmlNote--) | Liefert die html-Zeichenkette, die Daten und einige Formate in diesem Kommentar enthält. |
| [getNote()](#getNote--) | Stellt den Inhalt des Kommentars dar. |
| [getRichFormattings()](#getRichFormattings--) | Gibt alle Characters-Objekte zurück, die einen Zeichenbereich im Kommentartext darstellen. |
| [getRow()](#getRow--) | Liefert den Zeilenindex des Kommentars. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--) | Liefert den horizontalen Ausrichtungstyp des Textes im Kommentar. |
| [getTextOrientationType()](#getTextOrientationType--) | Liefert den Orientierungstyp des Textes im Kommentar. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--) | Liefert den vertikalen Ausrichtungstyp des Textes im Kommentar. |
| [getThreadedComments()](#getThreadedComments--) | Liefert die Liste der Threaded-Kommentare; |
| [getWidth()](#getWidth--) | Stellt die Breite des Kommentars in Pixeln dar. |
| [getWidthCM()](#getWidthCM--) | Stellt die Breite des Kommentars in Zentimetern dar. |
| [getWidthInch()](#getWidthInch--) | Stellt die Breite des Kommentars in Zoll dar. |
| [hashCode()](#hashCode--) |  |
| [isThreadedComment()](#isThreadedComment--) | Gibt an, ob dieser Kommentar ein Threaded-Kommentar ist. |
| [isVisible()](#isVisible--) | Stellt dar, ob der Kommentar sichtbar ist oder nicht. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Setzt den Namen des ursprünglichen Kommentarautors |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Gibt an, ob die Größe des Kommentars automatisch an dessen Inhalt angepasst wird. |
| [setHeight(int value)](#setHeight-int-) | Stellt die Höhe des Kommentars in Pixeln dar. |
| [setHeightCM(double value)](#setHeightCM-double-) | Stellt die Höhe des Kommentars in Zentimetern dar. |
| [setHeightInch(double value)](#setHeightInch-double-) | Stellt die Höhe des Kommentars in Zoll dar. |
| [setHtmlNote(String value)](#setHtmlNote-java.lang.String-) | Setzt die html-Zeichenkette, die Daten und einige Formate in diesem Kommentar enthält. |
| [setNote(String value)](#setNote-java.lang.String-) | Stellt den Inhalt des Kommentars dar. |
| [setTextHorizontalAlignment(int value)](#setTextHorizontalAlignment-int-) | Setzt den horizontalen Ausrichtungstyp des Textes im Kommentar. |
| [setTextOrientationType(int value)](#setTextOrientationType-int-) | Setzt den Orientierungstyp des Textes im Kommentar. |
| [setTextVerticalAlignment(int value)](#setTextVerticalAlignment-int-) | Setzt den vertikalen Ausrichtungstyp des Textes im Kommentar. |
| [setVisible(boolean value)](#setVisible-boolean-) | Stellt dar, ob der Kommentar sichtbar ist oder nicht. |
| [setWidth(int value)](#setWidth-int-) | Stellt die Breite des Kommentars in Pixeln dar. |
| [setWidthCM(double value)](#setWidthCM-double-) | Stellt die Breite des Kommentars in Zentimetern dar. |
| [setWidthInch(double value)](#setWidthInch-double-) | Stellt die Breite des Kommentars in Zoll dar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```


Gibt ein Characters-Objekt zurück, das einen Zeichenbereich im Kommentartext darstellt.

**Example**

```
         FontSetting fontSetting = comment1.characters(0, 4);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startIndex | int | Der Index des Beginns des Zeichens. |
| length | int | Die Anzahl der Zeichen. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - Characters object.
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### formatCharacters(int startIndex, int length, Font font, StyleFlag flag) {#formatCharacters-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-}
```
public void formatCharacters(int startIndex, int length, Font font, StyleFlag flag)
```


Formatiere einige Zeichen mit den Schriftarteinstellungen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startIndex | int | Der Startindex. |
| length | int | Die Länge. |
| font | [Font](../../com.aspose.cells/font) | Die Schriftarteinstellung. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Das Flag der Schriftarteinstellung. |

### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Ermittelt den Namen des ursprünglichen Kommentarautors.

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


Gibt an, ob die Größe des Kommentars automatisch an seinen Inhalt angepasst wird. Hinweis: In einigen Sonderfällen (wie z. B. einer Mac-Umgebung) kann diese Einstellung keine Wirkung zeigen. Wenn diese Einstellung keine Wirkung zeigt, ersetzen Sie sie bitte durch FitToTextSize().

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


Liefert den Spaltenindex des Kommentars.

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


Erhalte ein Shape-Objekt, das die dem angegebenen Kommentar zugefügte Form darstellt.

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


Ermittelt die Schriftart des Kommentars.

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


Stellt die Höhe des Kommentars in Pixeln dar.

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


Stellt die Höhe des Kommentars in Zentimetern dar.

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


Stellt die Höhe des Kommentars in Zoll dar.

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


Liefert die html-Zeichenkette, die Daten und einige Formate in diesem Kommentar enthält.

**Remarks**

Wenn dies ein Threaded-Kommentar ist, kann die Notiz nicht geändert werden, da sonst MS Excel ihn nicht als Threaded-Kommentar verarbeiten kann.

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


Stellt den Inhalt des Kommentars dar.

**Remarks**

Wenn dies ein Threaded-Kommentar ist, kann die Notiz nicht geändert werden, da sonst MS Excel ihn nicht als Threaded-Kommentar verarbeiten kann.

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


Gibt alle Characters-Objekte zurück, die einen Zeichenbereich im Kommentartext darstellen.

**Example**

```
         FontSetting[] list = comment1.getRichFormattings();
```

**Returns:**
com.aspose.cells.FontSetting[] - Alle Characters objects
### getRow() {#getRow--}
```
public int getRow()
```


Liefert den Zeilenindex des Kommentars.

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


Liefert den horizontalen Ausrichtungstyp des Textes im Kommentar.

Siehe [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

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


Liefert den Orientierungstyp des Textes im Kommentar.

Siehe [TextOrientationType](../../com.aspose.cells/textorientationtype).

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


Liefert den vertikalen Ausrichtungstyp des Textes im Kommentar.

Siehe [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

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


Liefert die Liste der Threaded-Kommentare;

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


Stellt die Breite des Kommentars in Pixeln dar.

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


Stellt die Breite des Kommentars in Zentimetern dar.

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


Stellt die Breite des Kommentars in Zoll dar.

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


Gibt an, ob dieser Kommentar ein Threaded-Kommentar ist.

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


Stellt dar, ob der Kommentar sichtbar ist oder nicht.

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


Setzt den Namen des ursprünglichen Kommentarautors

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setAutoSize(boolean value) {#setAutoSize-boolean-}
```
public void setAutoSize(boolean value)
```


Gibt an, ob die Größe des Kommentars automatisch an seinen Inhalt angepasst wird. Hinweis: In einigen Sonderfällen (wie z. B. einer Mac-Umgebung) kann diese Einstellung keine Wirkung zeigen. Wenn diese Einstellung keine Wirkung zeigt, ersetzen Sie sie bitte durch FitToTextSize().

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


Stellt die Höhe des Kommentars in Pixeln dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setHeightCM(double value) {#setHeightCM-double-}
```
public void setHeightCM(double value)
```


Stellt die Höhe des Kommentars in Zentimetern dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setHeightInch(double value) {#setHeightInch-double-}
```
public void setHeightInch(double value)
```


Stellt die Höhe des Kommentars in Zoll dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setHtmlNote(String value) {#setHtmlNote-java.lang.String-}
```
public void setHtmlNote(String value)
```


Setzt die html-Zeichenkette, die Daten und einige Formate in diesem Kommentar enthält.

**Remarks**

Wenn dies ein Threaded-Kommentar ist, kann die Notiz nicht geändert werden, da sonst MS Excel ihn nicht als Threaded-Kommentar verarbeiten kann.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setNote(String value) {#setNote-java.lang.String-}
```
public void setNote(String value)
```


Stellt den Inhalt des Kommentars dar.

**Remarks**

Wenn dies ein Threaded-Kommentar ist, kann die Notiz nicht geändert werden, da sonst MS Excel ihn nicht als Threaded-Kommentar verarbeiten kann.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setTextHorizontalAlignment(int value) {#setTextHorizontalAlignment-int-}
```
public void setTextHorizontalAlignment(int value)
```


Setzt den horizontalen Ausrichtungstyp des Textes im Kommentar.

Siehe [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setTextOrientationType(int value) {#setTextOrientationType-int-}
```
public void setTextOrientationType(int value)
```


Setzt den Orientierungstyp des Textes im Kommentar.

Siehe [TextOrientationType](../../com.aspose.cells/textorientationtype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setTextVerticalAlignment(int value) {#setTextVerticalAlignment-int-}
```
public void setTextVerticalAlignment(int value)
```


Setzt den vertikalen Ausrichtungstyp des Textes im Kommentar.

Siehe [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Stellt dar, ob der Kommentar sichtbar ist oder nicht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


Stellt die Breite des Kommentars in Pixeln dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setWidthCM(double value) {#setWidthCM-double-}
```
public void setWidthCM(double value)
```


Stellt die Breite des Kommentars in Zentimetern dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setWidthInch(double value) {#setWidthInch-double-}
```
public void setWidthInch(double value)
```


Stellt die Breite des Kommentars in Zoll dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

