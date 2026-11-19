---
title: "Commentaire"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Encapsule l'objet qui représente un commentaire de cellule."
type: docs
url: /fr/java/com.aspose.cells/comment/
---

**Inheritance:**
java.lang.Object
```
public class Comment
```

Encapsule l'objet qui représente un commentaire de cellule.

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
## Méthodes

| Méthode | Description |
| --- | --- |
| [characters(int startIndex, int length)](#characters-int-int-) | Renvoie un objet Characters qui représente une plage de caractères dans le texte du commentaire. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [formatCharacters(int startIndex, int length, Font font, StyleFlag flag)](#formatCharacters-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-) | Formate certains caractères avec le réglage de police. |
| [getAuthor()](#getAuthor--) | Obtient le nom de l'auteur original du commentaire. |
| [getAutoSize()](#getAutoSize--) | Indique si la taille du commentaire est ajustée automatiquement en fonction de son contenu. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Obtient l'index de colonne du commentaire. |
| [getCommentShape()](#getCommentShape--) | Obtenez un objet Shape qui représente la forme attachée au commentaire spécifié. |
| [getFont()](#getFont--) | Obtient la police du commentaire. |
| [getHeight()](#getHeight--) | Représente la hauteur du commentaire, en pixels. |
| [getHeightCM()](#getHeightCM--) | Représente la hauteur du commentaire, en centimètres. |
| [getHeightInch()](#getHeightInch--) | Représente la hauteur du commentaire, en pouces. |
| [getHtmlNote()](#getHtmlNote--) | Obtient la chaîne html qui contient des données et certains formats dans ce commentaire. |
| [getNote()](#getNote--) | Représente le contenu du commentaire. |
| [getRichFormattings()](#getRichFormattings--) | Renvoie tous les objets Characters qui représentent une plage de caractères dans le texte du commentaire. |
| [getRow()](#getRow--) | Obtient l'index de ligne du commentaire. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--) | Obtient le type d'alignement horizontal du texte du commentaire. |
| [getTextOrientationType()](#getTextOrientationType--) | Obtient le type d'orientation du texte du commentaire. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--) | Obtient le type d'alignement vertical du texte du commentaire. |
| [getThreadedComments()](#getThreadedComments--) | Obtient la liste des commentaires en fil de discussion ; |
| [getWidth()](#getWidth--) | Représente la largeur du commentaire, en unités de pixels. |
| [getWidthCM()](#getWidthCM--) | Représente la largeur du commentaire, en unités de centimètres. |
| [getWidthInch()](#getWidthInch--) | Représente la largeur du commentaire, en unités de pouces. |
| [hashCode()](#hashCode--) |  |
| [isThreadedComment()](#isThreadedComment--) | Indique si ce commentaire est un commentaire en fil de discussion. |
| [isVisible()](#isVisible--) | Indique si le commentaire est visible ou non. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Définit le nom de l'auteur original du commentaire |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Indique si la taille du commentaire est ajustée automatiquement en fonction de son contenu. |
| [setHeight(int value)](#setHeight-int-) | Représente la hauteur du commentaire, en pixels. |
| [setHeightCM(double value)](#setHeightCM-double-) | Représente la hauteur du commentaire, en centimètres. |
| [setHeightInch(double value)](#setHeightInch-double-) | Représente la hauteur du commentaire, en pouces. |
| [setHtmlNote(String value)](#setHtmlNote-java.lang.String-) | Définit la chaîne HTML qui contient des données et certains formats dans ce commentaire. |
| [setNote(String value)](#setNote-java.lang.String-) | Représente le contenu du commentaire. |
| [setTextHorizontalAlignment(int value)](#setTextHorizontalAlignment-int-) | Définit le type d'alignement horizontal du texte du commentaire. |
| [setTextOrientationType(int value)](#setTextOrientationType-int-) | Définit le type d'orientation du texte du commentaire. |
| [setTextVerticalAlignment(int value)](#setTextVerticalAlignment-int-) | Définit le type d'alignement vertical du texte du commentaire. |
| [setVisible(boolean value)](#setVisible-boolean-) | Indique si le commentaire est visible ou non. |
| [setWidth(int value)](#setWidth-int-) | Représente la largeur du commentaire, en unités de pixels. |
| [setWidthCM(double value)](#setWidthCM-double-) | Représente la largeur du commentaire, en unités de centimètres. |
| [setWidthInch(double value)](#setWidthInch-double-) | Représente la largeur du commentaire, en unités de pouces. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```


Renvoie un objet Characters qui représente une plage de caractères dans le texte du commentaire.

**Example**

```
         FontSetting fontSetting = comment1.characters(0, 4);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startIndex | int | L'index du début du caractère. |
| length | int | Le nombre de caractères. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - Characters object.
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### formatCharacters(int startIndex, int length, Font font, StyleFlag flag) {#formatCharacters-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-}
```
public void formatCharacters(int startIndex, int length, Font font, StyleFlag flag)
```


Formate certains caractères avec le réglage de police.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startIndex | int | L'index de départ. |
| length | int | La longueur. |
| font | [Font](../../com.aspose.cells/font) | Le paramètre de police. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Le drapeau du paramètre de police. |

### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Obtient le nom de l'auteur original du commentaire.

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


Indique si la taille du commentaire est ajustée automatiquement en fonction de son contenu. Remarque : dans certains cas particuliers (comme l'environnement Mac), ce paramètre peut ne pas prendre effet. Si ce paramètre ne prend pas effet, veuillez le remplacer par FitToTextSize().

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


Obtient l'index de colonne du commentaire.

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


Obtenez un objet Shape qui représente la forme attachée au commentaire spécifié.

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


Obtient la police du commentaire.

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


Représente la hauteur du commentaire, en pixels.

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


Représente la hauteur du commentaire, en centimètres.

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


Représente la hauteur du commentaire, en pouces.

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


Obtient la chaîne html qui contient des données et certains formats dans ce commentaire.

**Remarks**

Si c'est un commentaire en fil de discussion, la note ne peut pas être modifiée, sinon MS Excel ne pourrait pas le traiter comme un commentaire en fil de discussion.

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


Représente le contenu du commentaire.

**Remarks**

Si c'est un commentaire en fil de discussion, la note ne peut pas être modifiée, sinon MS Excel ne pourrait pas le traiter comme un commentaire en fil de discussion.

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


Renvoie tous les objets Characters qui représentent une plage de caractères dans le texte du commentaire.

**Example**

```
         FontSetting[] list = comment1.getRichFormattings();
```

**Returns:**
com.aspose.cells.FontSetting[] - Tous les objets Characters
### getRow() {#getRow--}
```
public int getRow()
```


Obtient l'index de ligne du commentaire.

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


Obtient le type d'alignement horizontal du texte du commentaire.

Voir [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

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


Obtient le type d'orientation du texte du commentaire.

Voir [TextOrientationType](../../com.aspose.cells/textorientationtype).

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


Obtient le type d'alignement vertical du texte du commentaire.

Voir [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

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


Obtient la liste des commentaires en fil de discussion ;

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


Représente la largeur du commentaire, en unités de pixels.

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


Représente la largeur du commentaire, en unités de centimètres.

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


Représente la largeur du commentaire, en unités de pouces.

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


Indique si ce commentaire est un commentaire en fil de discussion.

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


Indique si le commentaire est visible ou non.

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


Définit le nom de l'auteur original du commentaire

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setAutoSize(boolean value) {#setAutoSize-boolean-}
```
public void setAutoSize(boolean value)
```


Indique si la taille du commentaire est ajustée automatiquement en fonction de son contenu. Remarque : dans certains cas particuliers (comme l'environnement Mac), ce paramètre peut ne pas prendre effet. Si ce paramètre ne prend pas effet, veuillez le remplacer par FitToTextSize().

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


Représente la hauteur du commentaire, en pixels.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setHeightCM(double value) {#setHeightCM-double-}
```
public void setHeightCM(double value)
```


Représente la hauteur du commentaire, en centimètres.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setHeightInch(double value) {#setHeightInch-double-}
```
public void setHeightInch(double value)
```


Représente la hauteur du commentaire, en pouces.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setHtmlNote(String value) {#setHtmlNote-java.lang.String-}
```
public void setHtmlNote(String value)
```


Définit la chaîne HTML qui contient des données et certains formats dans ce commentaire.

**Remarks**

Si c'est un commentaire en fil de discussion, la note ne peut pas être modifiée, sinon MS Excel ne pourrait pas le traiter comme un commentaire en fil de discussion.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setNote(String value) {#setNote-java.lang.String-}
```
public void setNote(String value)
```


Représente le contenu du commentaire.

**Remarks**

Si c'est un commentaire en fil de discussion, la note ne peut pas être modifiée, sinon MS Excel ne pourrait pas le traiter comme un commentaire en fil de discussion.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setTextHorizontalAlignment(int value) {#setTextHorizontalAlignment-int-}
```
public void setTextHorizontalAlignment(int value)
```


Définit le type d'alignement horizontal du texte du commentaire.

Voir [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setTextOrientationType(int value) {#setTextOrientationType-int-}
```
public void setTextOrientationType(int value)
```


Définit le type d'orientation du texte du commentaire.

Voir [TextOrientationType](../../com.aspose.cells/textorientationtype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setTextVerticalAlignment(int value) {#setTextVerticalAlignment-int-}
```
public void setTextVerticalAlignment(int value)
```


Définit le type d'alignement vertical du texte du commentaire.

Voir [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Indique si le commentaire est visible ou non.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


Représente la largeur du commentaire, en unités de pixels.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setWidthCM(double value) {#setWidthCM-double-}
```
public void setWidthCM(double value)
```


Représente la largeur du commentaire, en unités de centimètres.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setWidthInch(double value) {#setWidthInch-double-}
```
public void setWidthInch(double value)
```


Représente la largeur du commentaire, en unités de pouces.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

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
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

