---
title: "Комментарий"
second_title: "Справочник API Aspose.Cells for Java"
description: "Инкапсулирует объект, представляющий комментарий ячейки."
type: docs
url: /ru/java/com.aspose.cells/comment/
---

**Inheritance:**
java.lang.Object
```
public class Comment
```

Инкапсулирует объект, представляющий комментарий ячейки.

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
## Методы

| Метод | Описание |
| --- | --- |
| [characters(int startIndex, int length)](#characters-int-int-) | Возвращает объект Characters, представляющий диапазон символов в тексте комментария. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [formatCharacters(int startIndex, int length, Font font, StyleFlag flag)](#formatCharacters-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-) | Форматировать некоторые символы с помощью настройки шрифта. |
| [getAuthor()](#getAuthor--) | Получает имя оригинального автора комментария. |
| [getAutoSize()](#getAutoSize--) | Указывает, автоматически ли размер комментария регулируется в соответствии с его содержимым. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Получает индекс столбца комментария. |
| [getCommentShape()](#getCommentShape--) | Получить объект Shape, представляющий форму, прикреплённую к указанному комментарию. |
| [getFont()](#getFont--) | Получает шрифт комментария. |
| [getHeight()](#getHeight--) | Представляет высоту комментария в пикселях. |
| [getHeightCM()](#getHeightCM--) | Представляет высоту комментария в сантиметрах. |
| [getHeightInch()](#getHeightInch--) | Представляет высоту комментария в дюймах. |
| [getHtmlNote()](#getHtmlNote--) | Получает HTML‑строку, содержащую данные и некоторые форматы в этом комментарии. |
| [getNote()](#getNote--) | Представляет содержимое комментария. |
| [getRichFormattings()](#getRichFormattings--) | Возвращает все объекты Characters, представляющие диапазон символов в тексте комментария. |
| [getRow()](#getRow--) | Получает индекс строки комментария. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--) | Получает тип горизонтального выравнивания текста комментария. |
| [getTextOrientationType()](#getTextOrientationType--) | Получает тип ориентации текста комментария. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--) | Получает тип вертикального выравнивания текста комментария. |
| [getThreadedComments()](#getThreadedComments--) | Получает список вложенных комментариев; |
| [getWidth()](#getWidth--) | Представляет ширину комментария в пикселях. |
| [getWidthCM()](#getWidthCM--) | Представляет ширину комментария в сантиметрах. |
| [getWidthInch()](#getWidthInch--) | Представляет ширину комментария в дюймах. |
| [hashCode()](#hashCode--) |  |
| [isThreadedComment()](#isThreadedComment--) | Указывает, является ли данный комментарий вложенным. |
| [isVisible()](#isVisible--) | Отображает, видим ли комментарий. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Устанавливает имя оригинального автора комментария |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Указывает, автоматически ли размер комментария регулируется в соответствии с его содержимым. |
| [setHeight(int value)](#setHeight-int-) | Представляет высоту комментария в пикселях. |
| [setHeightCM(double value)](#setHeightCM-double-) | Представляет высоту комментария в сантиметрах. |
| [setHeightInch(double value)](#setHeightInch-double-) | Представляет высоту комментария в дюймах. |
| [setHtmlNote(String value)](#setHtmlNote-java.lang.String-) | Устанавливает HTML-строку, содержащую данные и некоторые форматы в этом комментарии. |
| [setNote(String value)](#setNote-java.lang.String-) | Представляет содержимое комментария. |
| [setTextHorizontalAlignment(int value)](#setTextHorizontalAlignment-int-) | Устанавливает тип горизонтального выравнивания текста комментария. |
| [setTextOrientationType(int value)](#setTextOrientationType-int-) | Устанавливает тип ориентации текста комментария. |
| [setTextVerticalAlignment(int value)](#setTextVerticalAlignment-int-) | Устанавливает тип вертикального выравнивания текста комментария. |
| [setVisible(boolean value)](#setVisible-boolean-) | Отображает, видим ли комментарий. |
| [setWidth(int value)](#setWidth-int-) | Представляет ширину комментария в пикселях. |
| [setWidthCM(double value)](#setWidthCM-double-) | Представляет ширину комментария в сантиметрах. |
| [setWidthInch(double value)](#setWidthInch-double-) | Представляет ширину комментария в дюймах. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```


Возвращает объект Characters, представляющий диапазон символов в тексте комментария.

**Example**

```
         FontSetting fontSetting = comment1.characters(0, 4);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startIndex | int | Индекс начала символа. |
| length | int | Количество символов. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - Characters object.
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### formatCharacters(int startIndex, int length, Font font, StyleFlag flag) {#formatCharacters-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-}
```
public void formatCharacters(int startIndex, int length, Font font, StyleFlag flag)
```


Форматировать некоторые символы с помощью настройки шрифта.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startIndex | int | Начальный индекс. |
| length | int | Длина. |
| font | [Font](../../com.aspose.cells/font) | Настройка шрифта. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Флаг настройки шрифта. |

### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Получает имя оригинального автора комментария.

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


Указывает, автоматически ли размер комментария подстраивается под его содержимое. Примечание: в некоторых особых случаях (например, в среде Mac) эта настройка может не сработать. Если настройка не сработает, пожалуйста, замените её на FitToTextSize().

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


Получает индекс столбца комментария.

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


Получить объект Shape, представляющий форму, прикреплённую к указанному комментарию.

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


Получает шрифт комментария.

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


Представляет высоту комментария в пикселях.

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


Представляет высоту комментария в сантиметрах.

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


Представляет высоту комментария в дюймах.

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


Получает HTML‑строку, содержащую данные и некоторые форматы в этом комментарии.

**Remarks**

Если это вложенный комментарий, заметка не может быть изменена, иначе MS Excel не сможет обработать её как вложенный комментарий.

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


Представляет содержимое комментария.

**Remarks**

Если это вложенный комментарий, заметка не может быть изменена, иначе MS Excel не сможет обработать её как вложенный комментарий.

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


Возвращает все объекты Characters, представляющие диапазон символов в тексте комментария.

**Example**

```
         FontSetting[] list = comment1.getRichFormattings();
```

**Returns:**
com.aspose.cells.FontSetting[] - Все объекты Characters
### getRow() {#getRow--}
```
public int getRow()
```


Получает индекс строки комментария.

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


Получает тип горизонтального выравнивания текста комментария.

См. [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

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


Получает тип ориентации текста комментария.

См. [TextOrientationType](../../com.aspose.cells/textorientationtype).

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


Получает тип вертикального выравнивания текста комментария.

См. [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

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


Получает список вложенных комментариев;

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


Представляет ширину комментария в пикселях.

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


Представляет ширину комментария в сантиметрах.

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


Представляет ширину комментария в дюймах.

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


Указывает, является ли данный комментарий вложенным.

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


Отображает, видим ли комментарий.

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


Устанавливает имя оригинального автора комментария

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setAutoSize(boolean value) {#setAutoSize-boolean-}
```
public void setAutoSize(boolean value)
```


Указывает, автоматически ли размер комментария подстраивается под его содержимое. Примечание: в некоторых особых случаях (например, в среде Mac) эта настройка может не сработать. Если настройка не сработает, пожалуйста, замените её на FitToTextSize().

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


Представляет высоту комментария в пикселях.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setHeightCM(double value) {#setHeightCM-double-}
```
public void setHeightCM(double value)
```


Представляет высоту комментария в сантиметрах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setHeightInch(double value) {#setHeightInch-double-}
```
public void setHeightInch(double value)
```


Представляет высоту комментария в дюймах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setHtmlNote(String value) {#setHtmlNote-java.lang.String-}
```
public void setHtmlNote(String value)
```


Устанавливает HTML-строку, содержащую данные и некоторые форматы в этом комментарии.

**Remarks**

Если это вложенный комментарий, заметка не может быть изменена, иначе MS Excel не сможет обработать её как вложенный комментарий.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setNote(String value) {#setNote-java.lang.String-}
```
public void setNote(String value)
```


Представляет содержимое комментария.

**Remarks**

Если это вложенный комментарий, заметка не может быть изменена, иначе MS Excel не сможет обработать её как вложенный комментарий.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setTextHorizontalAlignment(int value) {#setTextHorizontalAlignment-int-}
```
public void setTextHorizontalAlignment(int value)
```


Устанавливает тип горизонтального выравнивания текста комментария.

См. [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setTextOrientationType(int value) {#setTextOrientationType-int-}
```
public void setTextOrientationType(int value)
```


Устанавливает тип ориентации текста комментария.

См. [TextOrientationType](../../com.aspose.cells/textorientationtype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setTextVerticalAlignment(int value) {#setTextVerticalAlignment-int-}
```
public void setTextVerticalAlignment(int value)
```


Устанавливает тип вертикального выравнивания текста комментария.

См. [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Отображает, видим ли комментарий.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


Представляет ширину комментария в пикселях.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setWidthCM(double value) {#setWidthCM-double-}
```
public void setWidthCM(double value)
```


Представляет ширину комментария в сантиметрах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setWidthInch(double value) {#setWidthInch-double-}
```
public void setWidthInch(double value)
```


Представляет ширину комментария в дюймах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

