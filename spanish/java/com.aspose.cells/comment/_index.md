---
title: "Comment"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Encapsula el objeto que representa un comentario de celda."
type: docs
url: /es/java/com.aspose.cells/comment/
---

**Inheritance:**
java.lang.Object
```
public class Comment
```

Encapsula el objeto que representa un comentario de celda.

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
## Métodos

| Método | Descripción |
| --- | --- |
| [characters(int startIndex, int length)](#characters-int-int-) | Devuelve un objeto Characters que representa un rango de caracteres dentro del texto del comentario. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [formatCharacters(int startIndex, int length, Font font, StyleFlag flag)](#formatCharacters-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-) | Formatea algunos caracteres con la configuración de fuente. |
| [getAuthor()](#getAuthor--) | Obtiene el nombre del autor original del comentario. |
| [getAutoSize()](#getAutoSize--) | Indica si el tamaño del comentario se ajusta automáticamente según su contenido. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Obtiene el índice de columna del comentario. |
| [getCommentShape()](#getCommentShape--) | Obtiene un objeto Shape que representa la forma adjunta al comentario especificado. |
| [getFont()](#getFont--) | Obtiene la fuente del comentario. |
| [getHeight()](#getHeight--) | Representa la altura del comentario, en unidades de píxeles. |
| [getHeightCM()](#getHeightCM--) | Representa la altura del comentario, en unidades de centímetros. |
| [getHeightInch()](#getHeightInch--) | Representa la altura del comentario, en unidades de pulgadas. |
| [getHtmlNote()](#getHtmlNote--) | Obtiene la cadena html que contiene datos y algunos formatos en este comentario. |
| [getNote()](#getNote--) | Representa el contenido del comentario. |
| [getRichFormattings()](#getRichFormattings--) | Devuelve todos los objetos Characters que representan un rango de caracteres dentro del texto del comentario. |
| [getRow()](#getRow--) | Obtiene el índice de fila del comentario. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--) | Obtiene el tipo de alineación horizontal del texto del comentario. |
| [getTextOrientationType()](#getTextOrientationType--) | Obtiene el tipo de orientación del texto del comentario. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--) | Obtiene el tipo de alineación vertical del texto del comentario. |
| [getThreadedComments()](#getThreadedComments--) | Obtiene la lista de comentarios en hilo; |
| [getWidth()](#getWidth--) | Representa el ancho del comentario, en unidades de píxeles. |
| [getWidthCM()](#getWidthCM--) | Representa el ancho del comentario, en unidades de centímetros. |
| [getWidthInch()](#getWidthInch--) | Representa el ancho del comentario, en unidades de pulgadas. |
| [hashCode()](#hashCode--) |  |
| [isThreadedComment()](#isThreadedComment--) | Indica si este comentario es un comentario en hilo. |
| [isVisible()](#isVisible--) | Representa si el comentario es visible o no. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Establece el nombre del autor original del comentario |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Indica si el tamaño del comentario se ajusta automáticamente según su contenido. |
| [setHeight(int value)](#setHeight-int-) | Representa la altura del comentario, en unidades de píxeles. |
| [setHeightCM(double value)](#setHeightCM-double-) | Representa la altura del comentario, en unidades de centímetros. |
| [setHeightInch(double value)](#setHeightInch-double-) | Representa la altura del comentario, en unidades de pulgadas. |
| [setHtmlNote(String value)](#setHtmlNote-java.lang.String-) | Establece la cadena html que contiene datos y algunos formatos en este comentario. |
| [setNote(String value)](#setNote-java.lang.String-) | Representa el contenido del comentario. |
| [setTextHorizontalAlignment(int value)](#setTextHorizontalAlignment-int-) | Establece el tipo de alineación horizontal del texto del comentario. |
| [setTextOrientationType(int value)](#setTextOrientationType-int-) | Establece el tipo de orientación del texto del comentario. |
| [setTextVerticalAlignment(int value)](#setTextVerticalAlignment-int-) | Establece el tipo de alineación vertical del texto del comentario. |
| [setVisible(boolean value)](#setVisible-boolean-) | Representa si el comentario es visible o no. |
| [setWidth(int value)](#setWidth-int-) | Representa el ancho del comentario, en unidades de píxeles. |
| [setWidthCM(double value)](#setWidthCM-double-) | Representa el ancho del comentario, en unidades de centímetros. |
| [setWidthInch(double value)](#setWidthInch-double-) | Representa el ancho del comentario, en unidades de pulgadas. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```


Devuelve un objeto Characters que representa un rango de caracteres dentro del texto del comentario.

**Example**

```
         FontSetting fontSetting = comment1.characters(0, 4);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startIndex | int | El índice del inicio del carácter. |
| length | int | El número de caracteres. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - Characters object.
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### formatCharacters(int startIndex, int length, Font font, StyleFlag flag) {#formatCharacters-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-}
```
public void formatCharacters(int startIndex, int length, Font font, StyleFlag flag)
```


Formatea algunos caracteres con la configuración de fuente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startIndex | int | El índice de inicio. |
| length | int | La longitud. |
| font | [Font](../../com.aspose.cells/font) | La configuración de la fuente. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | La bandera de la configuración de la fuente. |

### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Obtiene el nombre del autor original del comentario.

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


Indica si el tamaño del comentario se ajusta automáticamente según su contenido. Nota: En algunos casos especiales (como el entorno Mac), esta configuración puede no tener efecto. Si esta configuración no tiene efecto, por favor reemplácela con FitToTextSize().

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


Obtiene el índice de columna del comentario.

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


Obtiene un objeto Shape que representa la forma adjunta al comentario especificado.

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


Obtiene la fuente del comentario.

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


Representa la altura del comentario, en unidades de píxeles.

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


Representa la altura del comentario, en unidades de centímetros.

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


Representa la altura del comentario, en unidades de pulgadas.

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


Obtiene la cadena html que contiene datos y algunos formatos en este comentario.

**Remarks**

Si este es un comentario en hilo, la nota no podría cambiarse, de lo contrario MS Excel no podría procesarlo como un comentario en hilo.

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


Representa el contenido del comentario.

**Remarks**

Si este es un comentario en hilo, la nota no podría cambiarse, de lo contrario MS Excel no podría procesarlo como un comentario en hilo.

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


Devuelve todos los objetos Characters que representan un rango de caracteres dentro del texto del comentario.

**Example**

```
         FontSetting[] list = comment1.getRichFormattings();
```

**Returns:**
com.aspose.cells.FontSetting[] - Todos los objetos Characters
### getRow() {#getRow--}
```
public int getRow()
```


Obtiene el índice de fila del comentario.

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


Obtiene el tipo de alineación horizontal del texto del comentario.

Ver [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

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


Obtiene el tipo de orientación del texto del comentario.

Ver [TextOrientationType](../../com.aspose.cells/textorientationtype).

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


Obtiene el tipo de alineación vertical del texto del comentario.

Ver [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

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


Obtiene la lista de comentarios en hilo;

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


Representa el ancho del comentario, en unidades de píxeles.

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


Representa el ancho del comentario, en unidades de centímetros.

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


Representa el ancho del comentario, en unidades de pulgadas.

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


Indica si este comentario es un comentario en hilo.

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


Representa si el comentario es visible o no.

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


Establece el nombre del autor original del comentario

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setAutoSize(boolean value) {#setAutoSize-boolean-}
```
public void setAutoSize(boolean value)
```


Indica si el tamaño del comentario se ajusta automáticamente según su contenido. Nota: En algunos casos especiales (como el entorno Mac), esta configuración puede no tener efecto. Si esta configuración no tiene efecto, por favor reemplácela con FitToTextSize().

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


Representa la altura del comentario, en unidades de píxeles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setHeightCM(double value) {#setHeightCM-double-}
```
public void setHeightCM(double value)
```


Representa la altura del comentario, en unidades de centímetros.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setHeightInch(double value) {#setHeightInch-double-}
```
public void setHeightInch(double value)
```


Representa la altura del comentario, en unidades de pulgadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setHtmlNote(String value) {#setHtmlNote-java.lang.String-}
```
public void setHtmlNote(String value)
```


Establece la cadena html que contiene datos y algunos formatos en este comentario.

**Remarks**

Si este es un comentario en hilo, la nota no podría cambiarse, de lo contrario MS Excel no podría procesarlo como un comentario en hilo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setNote(String value) {#setNote-java.lang.String-}
```
public void setNote(String value)
```


Representa el contenido del comentario.

**Remarks**

Si este es un comentario en hilo, la nota no podría cambiarse, de lo contrario MS Excel no podría procesarlo como un comentario en hilo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setTextHorizontalAlignment(int value) {#setTextHorizontalAlignment-int-}
```
public void setTextHorizontalAlignment(int value)
```


Establece el tipo de alineación horizontal del texto del comentario.

Ver [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setTextOrientationType(int value) {#setTextOrientationType-int-}
```
public void setTextOrientationType(int value)
```


Establece el tipo de orientación del texto del comentario.

Ver [TextOrientationType](../../com.aspose.cells/textorientationtype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setTextVerticalAlignment(int value) {#setTextVerticalAlignment-int-}
```
public void setTextVerticalAlignment(int value)
```


Establece el tipo de alineación vertical del texto del comentario.

Ver [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Representa si el comentario es visible o no.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


Representa el ancho del comentario, en unidades de píxeles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setWidthCM(double value) {#setWidthCM-double-}
```
public void setWidthCM(double value)
```


Representa el ancho del comentario, en unidades de centímetros.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

### setWidthInch(double value) {#setWidthInch-double-}
```
public void setWidthInch(double value)
```


Representa el ancho del comentario, en unidades de pulgadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double |  |

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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

