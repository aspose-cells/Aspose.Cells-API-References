---
title: "Yorum"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir hücre yorumunu temsil eden nesneyi kapsüller."
type: docs
url: /tr/java/com.aspose.cells/comment/
---

**Inheritance:**
java.lang.Object
```
public class Comment
```

Bir hücre yorumunu temsil eden nesneyi kapsüller.

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
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [characters(int startIndex, int length)](#characters-int-int-) | Yorum metni içinde bir karakter aralığını temsil eden bir Characters nesnesi döndürür. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [formatCharacters(int startIndex, int length, Font font, StyleFlag flag)](#formatCharacters-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-) | Bazı karakterleri yazı tipi ayarıyla biçimlendir. |
| [getAuthor()](#getAuthor--) | Orijinal yorum yazarının adını alır. |
| [getAutoSize()](#getAutoSize--) | Yorumun boyutunun içeriğine göre otomatik olarak ayarlanıp ayarlanmadığını gösterir. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Yorumun sütun indeksini alır. |
| [getCommentShape()](#getCommentShape--) | Belirtilen yoruma ekli şekli temsil eden bir Shape nesnesi alır. |
| [getFont()](#getFont--) | Yorumun yazı tipini alır. |
| [getHeight()](#getHeight--) | Yorumun yüksekliğini piksel biriminde temsil eder. |
| [getHeightCM()](#getHeightCM--) | Yorumun yüksekliğini santimetre biriminde temsil eder. |
| [getHeightInch()](#getHeightInch--) | Yorumun yüksekliğini inç biriminde temsil eder. |
| [getHtmlNote()](#getHtmlNote--) | Bu yorumda veri ve bazı biçimlendirmeleri içeren html dizesini alır. |
| [getNote()](#getNote--) | Yorumun içeriğini temsil eder. |
| [getRichFormattings()](#getRichFormattings--) | Yorum metni içinde bir karakter aralığını temsil eden tüm Characters nesnelerini döndürür. |
| [getRow()](#getRow--) | Yorumun satır indeksini alır. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--) | Yorumun metin yatay hizalama türünü alır. |
| [getTextOrientationType()](#getTextOrientationType--) | Yorumun metin yönlendirme türünü alır. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--) | Yorumun metin dikey hizalama türünü alır. |
| [getThreadedComments()](#getThreadedComments--) | İş parçacıklı yorumların listesini alır; |
| [getWidth()](#getWidth--) | Yorumun genişliğini piksel biriminde temsil eder. |
| [getWidthCM()](#getWidthCM--) | Yorumun genişliğini santimetre biriminde temsil eder. |
| [getWidthInch()](#getWidthInch--) | Yorumun genişliğini inç biriminde temsil eder. |
| [hashCode()](#hashCode--) |  |
| [isThreadedComment()](#isThreadedComment--) | Bu yorumun iş parçacıklı bir yorum olup olmadığını gösterir. |
| [isVisible()](#isVisible--) | Yorumun görünür olup olmadığını temsil eder. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Orijinal yorum yazarının adını ayarlar |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Yorumun boyutunun içeriğine göre otomatik olarak ayarlanıp ayarlanmadığını gösterir. |
| [setHeight(int value)](#setHeight-int-) | Yorumun yüksekliğini piksel biriminde temsil eder. |
| [setHeightCM(double value)](#setHeightCM-double-) | Yorumun yüksekliğini santimetre biriminde temsil eder. |
| [setHeightInch(double value)](#setHeightInch-double-) | Yorumun yüksekliğini inç biriminde temsil eder. |
| [setHtmlNote(String value)](#setHtmlNote-java.lang.String-) | Bu yorumda veri ve bazı biçimleri içeren html dizesini ayarlar. |
| [setNote(String value)](#setNote-java.lang.String-) | Yorumun içeriğini temsil eder. |
| [setTextHorizontalAlignment(int value)](#setTextHorizontalAlignment-int-) | Yorumun metin yatay hizalama türünü ayarlar. |
| [setTextOrientationType(int value)](#setTextOrientationType-int-) | Yorumun metin yönlendirme türünü ayarlar. |
| [setTextVerticalAlignment(int value)](#setTextVerticalAlignment-int-) | Yorumun metin dikey hizalama türünü ayarlar. |
| [setVisible(boolean value)](#setVisible-boolean-) | Yorumun görünür olup olmadığını temsil eder. |
| [setWidth(int value)](#setWidth-int-) | Yorumun genişliğini piksel biriminde temsil eder. |
| [setWidthCM(double value)](#setWidthCM-double-) | Yorumun genişliğini santimetre biriminde temsil eder. |
| [setWidthInch(double value)](#setWidthInch-double-) | Yorumun genişliğini inç biriminde temsil eder. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```


Yorum metni içinde bir karakter aralığını temsil eden bir Characters nesnesi döndürür.

**Example**

```
         FontSetting fontSetting = comment1.characters(0, 4);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startIndex | int | Karakterin başlangıç indeksi. |
| length | int | Karakter sayısı. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - Characters object.
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### formatCharacters(int startIndex, int length, Font font, StyleFlag flag) {#formatCharacters-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-}
```
public void formatCharacters(int startIndex, int length, Font font, StyleFlag flag)
```


Bazı karakterleri yazı tipi ayarıyla biçimlendir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startIndex | int | Başlangıç indeksi. |
| length | int | Uzunluk. |
| font | [Font](../../com.aspose.cells/font) | Yazı tipi ayarı. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Yazı tipi ayarının bayrağı. |

### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Orijinal yorum yazarının adını alır.

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


Yorumun boyutunun içeriğine göre otomatik olarak ayarlanıp ayarlanmadığını gösterir. Not: Bazı özel durumlarda (örneğin Mac ortamı), bu ayar etkili olmayabilir. Bu ayar etkili olmazsa, lütfen FitToTextSize() ile değiştirin.

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


Yorumun sütun indeksini alır.

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


Belirtilen yoruma ekli şekli temsil eden bir Shape nesnesi alır.

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


Yorumun yazı tipini alır.

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


Yorumun yüksekliğini piksel biriminde temsil eder.

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


Yorumun yüksekliğini santimetre biriminde temsil eder.

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


Yorumun yüksekliğini inç biriminde temsil eder.

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


Bu yorumda veri ve bazı biçimlendirmeleri içeren html dizesini alır.

**Remarks**

Bu bir iş parçacıklı yorum ise, not değiştirilemez, aksi takdirde MS Excel bunu iş parçacıklı yorum olarak işleyemez.

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


Yorumun içeriğini temsil eder.

**Remarks**

Bu bir iş parçacıklı yorum ise, not değiştirilemez, aksi takdirde MS Excel bunu iş parçacıklı yorum olarak işleyemez.

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


Yorum metni içinde bir karakter aralığını temsil eden tüm Characters nesnelerini döndürür.

**Example**

```
         FontSetting[] list = comment1.getRichFormattings();
```

**Returns:**
com.aspose.cells.FontSetting[] - Tüm Karakter nesneleri
### getRow() {#getRow--}
```
public int getRow()
```


Yorumun satır indeksini alır.

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


Yorumun metin yatay hizalama türünü alır.

Bakınız [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

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


Yorumun metin yönlendirme türünü alır.

Bakınız [TextOrientationType](../../com.aspose.cells/textorientationtype).

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


Yorumun metin dikey hizalama türünü alır.

Bakınız [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

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


İş parçacıklı yorumların listesini alır;

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


Yorumun genişliğini piksel biriminde temsil eder.

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


Yorumun genişliğini santimetre biriminde temsil eder.

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


Yorumun genişliğini inç biriminde temsil eder.

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


Bu yorumun iş parçacıklı bir yorum olup olmadığını gösterir.

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


Yorumun görünür olup olmadığını temsil eder.

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


Orijinal yorum yazarının adını ayarlar

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setAutoSize(boolean value) {#setAutoSize-boolean-}
```
public void setAutoSize(boolean value)
```


Yorumun boyutunun içeriğine göre otomatik olarak ayarlanıp ayarlanmadığını gösterir. Not: Bazı özel durumlarda (örneğin Mac ortamı), bu ayar etkili olmayabilir. Bu ayar etkili olmazsa, lütfen FitToTextSize() ile değiştirin.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


Yorumun yüksekliğini piksel biriminde temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setHeightCM(double value) {#setHeightCM-double-}
```
public void setHeightCM(double value)
```


Yorumun yüksekliğini santimetre biriminde temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setHeightInch(double value) {#setHeightInch-double-}
```
public void setHeightInch(double value)
```


Yorumun yüksekliğini inç biriminde temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setHtmlNote(String value) {#setHtmlNote-java.lang.String-}
```
public void setHtmlNote(String value)
```


Bu yorumda veri ve bazı biçimleri içeren html dizesini ayarlar.

**Remarks**

Bu bir iş parçacıklı yorum ise, not değiştirilemez, aksi takdirde MS Excel bunu iş parçacıklı yorum olarak işleyemez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setNote(String value) {#setNote-java.lang.String-}
```
public void setNote(String value)
```


Yorumun içeriğini temsil eder.

**Remarks**

Bu bir iş parçacıklı yorum ise, not değiştirilemez, aksi takdirde MS Excel bunu iş parçacıklı yorum olarak işleyemez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setTextHorizontalAlignment(int value) {#setTextHorizontalAlignment-int-}
```
public void setTextHorizontalAlignment(int value)
```


Yorumun metin yatay hizalama türünü ayarlar.

Bakınız [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setTextOrientationType(int value) {#setTextOrientationType-int-}
```
public void setTextOrientationType(int value)
```


Yorumun metin yönlendirme türünü ayarlar.

Bakınız [TextOrientationType](../../com.aspose.cells/textorientationtype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setTextVerticalAlignment(int value) {#setTextVerticalAlignment-int-}
```
public void setTextVerticalAlignment(int value)
```


Yorumun metin dikey hizalama türünü ayarlar.

Bakınız [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Yorumun görünür olup olmadığını temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


Yorumun genişliğini piksel biriminde temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setWidthCM(double value) {#setWidthCM-double-}
```
public void setWidthCM(double value)
```


Yorumun genişliğini santimetre biriminde temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setWidthInch(double value) {#setWidthInch-double-}
```
public void setWidthInch(double value)
```


Yorumun genişliğini inç biriminde temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

