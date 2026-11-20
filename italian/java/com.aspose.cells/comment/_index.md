---
title: "Comment"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Incapsula l'oggetto che rappresenta un commento di cella."
type: docs
url: /it/java/com.aspose.cells/comment/
---

**Inheritance:**
java.lang.Object
```
public class Comment
```

Incapsula l'oggetto che rappresenta un commento di cella.

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
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [characters(int startIndex, int length)](#characters-int-int-) | Restituisce un oggetto Characters che rappresenta un intervallo di caratteri nel testo del commento. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [formatCharacters(int startIndex, int length, Font font, StyleFlag flag)](#formatCharacters-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-) | Formatta alcuni caratteri con l'impostazione del font. |
| [getAuthor()](#getAuthor--) | Ottiene il Nome dell'autore originale del commento |
| [getAutoSize()](#getAutoSize--) | Indica se la dimensione del commento è regolata automaticamente in base al suo contenuto. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Restituisce l'indice della colonna del commento. |
| [getCommentShape()](#getCommentShape--) | Ottieni un oggetto Shape che rappresenta la forma allegata al commento specificato. |
| [getFont()](#getFont--) | Ottiene il font del commento. |
| [getHeight()](#getHeight--) | Rappresenta l'Altezza del commento, in unità di pixel. |
| [getHeightCM()](#getHeightCM--) | Rappresenta l'altezza del commento, in unità di centimetri. |
| [getHeightInch()](#getHeightInch--) | Rappresenta l'altezza del commento, in unità di pollici. |
| [getHtmlNote()](#getHtmlNote--) | Ottiene la stringa html che contiene dati e alcuni formati in questo commento. |
| [getNote()](#getNote--) | Rappresenta il contenuto del commento. |
| [getRichFormattings()](#getRichFormattings--) | Restituisce tutti gli oggetti Characters che rappresentano un intervallo di caratteri nel testo del commento. |
| [getRow()](#getRow--) | Restituisce l'indice della riga del commento. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--) | Ottiene il tipo di allineamento orizzontale del testo del commento. |
| [getTextOrientationType()](#getTextOrientationType--) | Ottiene il tipo di orientamento del testo del commento. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--) | Ottiene il tipo di allineamento verticale del testo del commento. |
| [getThreadedComments()](#getThreadedComments--) | Ottiene l'elenco dei commenti in thread; |
| [getWidth()](#getWidth--) | Rappresenta la larghezza del commento, in unità di pixel. |
| [getWidthCM()](#getWidthCM--) | Rappresenta la larghezza del commento, in unità di centimetri. |
| [getWidthInch()](#getWidthInch--) | Rappresenta la larghezza del commento, in unità di pollici. |
| [hashCode()](#hashCode--) |  |
| [isThreadedComment()](#isThreadedComment--) | Indica se questo commento è un commento in thread. |
| [isVisible()](#isVisible--) | Rappresenta se il commento è visibile o meno. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Imposta il nome dell'autore originale del commento |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Indica se la dimensione del commento è regolata automaticamente in base al suo contenuto. |
| [setHeight(int value)](#setHeight-int-) | Rappresenta l'Altezza del commento, in unità di pixel. |
| [setHeightCM(double value)](#setHeightCM-double-) | Rappresenta l'altezza del commento, in unità di centimetri. |
| [setHeightInch(double value)](#setHeightInch-double-) | Rappresenta l'altezza del commento, in unità di pollici. |
| [setHtmlNote(String value)](#setHtmlNote-java.lang.String-) | Imposta la stringa HTML che contiene dati e alcuni formati in questo commento. |
| [setNote(String value)](#setNote-java.lang.String-) | Rappresenta il contenuto del commento. |
| [setTextHorizontalAlignment(int value)](#setTextHorizontalAlignment-int-) | Imposta il tipo di allineamento orizzontale del testo del commento. |
| [setTextOrientationType(int value)](#setTextOrientationType-int-) | Imposta il tipo di orientamento del testo del commento. |
| [setTextVerticalAlignment(int value)](#setTextVerticalAlignment-int-) | Imposta il tipo di allineamento verticale del testo del commento. |
| [setVisible(boolean value)](#setVisible-boolean-) | Rappresenta se il commento è visibile o meno. |
| [setWidth(int value)](#setWidth-int-) | Rappresenta la larghezza del commento, in unità di pixel. |
| [setWidthCM(double value)](#setWidthCM-double-) | Rappresenta la larghezza del commento, in unità di centimetri. |
| [setWidthInch(double value)](#setWidthInch-double-) | Rappresenta la larghezza del commento, in unità di pollici. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```


Restituisce un oggetto Characters che rappresenta un intervallo di caratteri nel testo del commento.

**Example**

```
         FontSetting fontSetting = comment1.characters(0, 4);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startIndex | int | L'indice dell'inizio del carattere. |
| length | int | Il numero di caratteri. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - Characters object.
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### formatCharacters(int startIndex, int length, Font font, StyleFlag flag) {#formatCharacters-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-}
```
public void formatCharacters(int startIndex, int length, Font font, StyleFlag flag)
```


Formatta alcuni caratteri con l'impostazione del font.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startIndex | int | L'indice di inizio. |
| length | int | La lunghezza. |
| font | [Font](../../com.aspose.cells/font) | L'impostazione del carattere. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Il flag dell'impostazione del carattere. |

### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Ottiene il Nome dell'autore originale del commento

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


Indica se la dimensione del commento viene regolata automaticamente in base al suo contenuto. Nota: in alcuni casi speciali (come l'ambiente Mac), questa impostazione potrebbe non avere effetto. Se questa impostazione non ha effetto, si prega di sostituirla con FitToTextSize().

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


Restituisce l'indice della colonna del commento.

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


Ottieni un oggetto Shape che rappresenta la forma allegata al commento specificato.

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


Ottiene il font del commento.

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


Rappresenta l'Altezza del commento, in unità di pixel.

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


Rappresenta l'altezza del commento, in unità di centimetri.

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


Rappresenta l'altezza del commento, in unità di pollici.

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


Ottiene la stringa html che contiene dati e alcuni formati in questo commento.

**Remarks**

Se questo è un commento in thread, la nota non può essere modificata, altrimenti MS Excel non potrebbe elaborarla come commento in thread.

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


Rappresenta il contenuto del commento.

**Remarks**

Se questo è un commento in thread, la nota non può essere modificata, altrimenti MS Excel non potrebbe elaborarla come commento in thread.

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


Restituisce tutti gli oggetti Characters che rappresentano un intervallo di caratteri nel testo del commento.

**Example**

```
         FontSetting[] list = comment1.getRichFormattings();
```

**Returns:**
com.aspose.cells.FontSetting[] - Tutti gli oggetti Characters
### getRow() {#getRow--}
```
public int getRow()
```


Restituisce l'indice della riga del commento.

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


Ottiene il tipo di allineamento orizzontale del testo del commento.

Vedi [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

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


Ottiene il tipo di orientamento del testo del commento.

Vedi [TextOrientationType](../../com.aspose.cells/textorientationtype).

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


Ottiene il tipo di allineamento verticale del testo del commento.

Vedi [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

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


Ottiene l'elenco dei commenti in thread;

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


Rappresenta la larghezza del commento, in unità di pixel.

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


Rappresenta la larghezza del commento, in unità di centimetri.

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


Rappresenta la larghezza del commento, in unità di pollici.

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


Indica se questo commento è un commento in thread.

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


Rappresenta se il commento è visibile o meno.

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


Imposta il nome dell'autore originale del commento

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setAutoSize(boolean value) {#setAutoSize-boolean-}
```
public void setAutoSize(boolean value)
```


Indica se la dimensione del commento viene regolata automaticamente in base al suo contenuto. Nota: in alcuni casi speciali (come l'ambiente Mac), questa impostazione potrebbe non avere effetto. Se questa impostazione non ha effetto, si prega di sostituirla con FitToTextSize().

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


Rappresenta l'Altezza del commento, in unità di pixel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setHeightCM(double value) {#setHeightCM-double-}
```
public void setHeightCM(double value)
```


Rappresenta l'altezza del commento, in unità di centimetri.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setHeightInch(double value) {#setHeightInch-double-}
```
public void setHeightInch(double value)
```


Rappresenta l'altezza del commento, in unità di pollici.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setHtmlNote(String value) {#setHtmlNote-java.lang.String-}
```
public void setHtmlNote(String value)
```


Imposta la stringa HTML che contiene dati e alcuni formati in questo commento.

**Remarks**

Se questo è un commento in thread, la nota non può essere modificata, altrimenti MS Excel non potrebbe elaborarla come commento in thread.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setNote(String value) {#setNote-java.lang.String-}
```
public void setNote(String value)
```


Rappresenta il contenuto del commento.

**Remarks**

Se questo è un commento in thread, la nota non può essere modificata, altrimenti MS Excel non potrebbe elaborarla come commento in thread.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setTextHorizontalAlignment(int value) {#setTextHorizontalAlignment-int-}
```
public void setTextHorizontalAlignment(int value)
```


Imposta il tipo di allineamento orizzontale del testo del commento.

Vedi [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setTextOrientationType(int value) {#setTextOrientationType-int-}
```
public void setTextOrientationType(int value)
```


Imposta il tipo di orientamento del testo del commento.

Vedi [TextOrientationType](../../com.aspose.cells/textorientationtype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setTextVerticalAlignment(int value) {#setTextVerticalAlignment-int-}
```
public void setTextVerticalAlignment(int value)
```


Imposta il tipo di allineamento verticale del testo del commento.

Vedi [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Rappresenta se il commento è visibile o meno.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


Rappresenta la larghezza del commento, in unità di pixel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setWidthCM(double value) {#setWidthCM-double-}
```
public void setWidthCM(double value)
```


Rappresenta la larghezza del commento, in unità di centimetri.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setWidthInch(double value) {#setWidthInch-double-}
```
public void setWidthInch(double value)
```


Rappresenta la larghezza del commento, in unità di pollici.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

