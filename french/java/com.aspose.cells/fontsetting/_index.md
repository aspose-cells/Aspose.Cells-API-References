---
title: "FontSetting"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente une plage de caractères dans le texte de la cellule."
type: docs
url: /fr/java/com.aspose.cells/fontsetting/
---

**Inheritance:**
java.lang.Object
```
public class FontSetting
```

Représente une plage de caractères dans le texte de la cellule.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Adding a new worksheet to the Excel object
         workbook.getWorksheets().add();
 
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         //Accessing the "A1" cell from the worksheet
         Cell cell = worksheet.getCells().get("A1");
 
         //Adding some value to the "A1" cell
         cell.putValue("Visit Aspose!");
 
         //getting characters
         FontSetting character = cell.characters(6, 7);
 
         //Setting the font of selected characters to bold
         character.getFont().setBold(true);
 
         //Setting the font color of selected characters to blue
         character.getFont().setColor(Color.getBlue());
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [FontSetting(int startIndex, int length, WorksheetCollection sheets)](#FontSetting-int-int-com.aspose.cells.WorksheetCollection-) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFont()](#getFont--) | Renvoie la police de cet objet. |
| [getLength()](#getLength--) | Obtient la longueur des caractères. |
| [getStartIndex()](#getStartIndex--) | Obtient l'index de départ des caractères. |
| [getTextOptions()](#getTextOptions--) | Renvoie les options de texte. |
| [getType()](#getType--) | Obtient le type de nœud de texte. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setWordArtStyle(int style)](#setWordArtStyle-int-) | Définit le style WordArt prédéfini. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### FontSetting(int startIndex, int length, WorksheetCollection sheets) {#FontSetting-int-int-com.aspose.cells.WorksheetCollection-}
```
public FontSetting(int startIndex, int length, WorksheetCollection sheets)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startIndex | int |  |
| length | int |  |
| sheets | [WorksheetCollection](../../com.aspose.cells/worksheetcollection) |  |

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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFont() {#getFont--}
```
public Font getFont()
```


Renvoie la police de cet objet.

**Returns:**
[Font](../../com.aspose.cells/font)
### getLength() {#getLength--}
```
public int getLength()
```


Obtient la longueur des caractères.

**Returns:**
int
### getStartIndex() {#getStartIndex--}
```
public int getStartIndex()
```


Obtient l'index de départ des caractères.

**Returns:**
int
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


Renvoie les options de texte.

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getType() {#getType--}
```
public int getType()
```


Obtient le type de nœud de texte.

Voir [TextNodeType](../../com.aspose.cells/textnodetype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setWordArtStyle(int style) {#setWordArtStyle-int-}
```
public void setWordArtStyle(int style)
```


Définit le style WordArt prédéfini.

**Remarks**

Uniquement pour le texte de la forme/graphique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| style | int | [PresetWordArtStyle](../../com.aspose.cells/presetwordartstyle). Le style WordArt prédéfini. |

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

