---
title: "Column"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente une seule colonne dans une feuille de calcul."
type: docs
url: /fr/java/com.aspose.cells/column/
---

**Inheritance:**
java.lang.Object
```
public class Column
```

Représente une seule colonne dans une feuille de calcul.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
         Style style = workbook.createStyle();
 
         //Setting the background color to Blue
         style.setBackgroundColor(Color.getBlue());
 
         //Setting the foreground color to Red
         style.setForegroundColor(Color.getRed());
 
         //setting Background Pattern
         style.setPattern(BackgroundType.DIAGONAL_STRIPE);
 
         //New Style Flag
         StyleFlag styleFlag = new StyleFlag();
 
         //Set All Styles
         styleFlag.setAll(true);
 
         //Get first Column
         Column column = worksheet.getCells().getColumns().get(0);
 
         //Apply Style to first Column
         column.applyStyle(style, styleFlag);
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Applique des formats à une colonne entière. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getGroupLevel()](#getGroupLevel--) | Obtient le niveau de groupe de la colonne. |
| [getIndex()](#getIndex--) | Obtient l'index de cette colonne. |
| [getStyle()](#getStyle--) | Obtient le style de cette colonne. |
| [getWidth()](#getWidth--) | Obtient la largeur de la colonne en unités de caractères. |
| [hasCustomStyle()](#hasCustomStyle--) | Indique si cette colonne possède des paramètres de style personnalisés (différents du style par défaut hérité du classeur). |
| [hashCode()](#hashCode--) |  |
| [isCollapsed()](#isCollapsed--) | si la colonne est réduite |
| [isHidden()](#isHidden--) | Indique si la colonne est masquée. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCollapsed(boolean value)](#setCollapsed-boolean-) | si la colonne est réduite |
| [setGroupLevel(byte value)](#setGroupLevel-byte-) | Obtient le niveau de groupe de la colonne. |
| [setHidden(boolean value)](#setHidden-boolean-) | Indique si la colonne est masquée. |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Définit le style de cette colonne. |
| [setWidth(double value)](#setWidth-double-) | Définit la largeur de la colonne en unités de caractères. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


Applique des formats à une colonne entière.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | L'objet de style qui sera appliqué. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Drapeaux qui indiquent les propriétés de formatage appliquées. |

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
### getGroupLevel() {#getGroupLevel--}
```
public byte getGroupLevel()
```


Obtient le niveau de groupe de la colonne.

**Returns:**
byte
### getIndex() {#getIndex--}
```
public int getIndex()
```


Obtient l'index de cette colonne.

**Returns:**
int
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Obtient le style de cette colonne.

**Remarks**

Modifier directement l'objet style retourné n'a aucun effet sur cette colonne ou sur les cellules de cette colonne. Vous devez appeler la méthode [applyStyle(Style,StyleFlag)](../../com.aspose.cells/column\#applyStyle-Style-StyleFlag-) ou [setStyle(Style)](../../com.aspose.cells/column\#setStyle-Style-) pour appliquer la modification à cette colonne.

Le style de la colonne est le style qui sera hérité par les cellules de cette colonne (ces cellules qui n'ont pas de paramètres de style personnalisés, comme les cellules existantes qui n'ont pas reçu de style explicitement, ou celles qui n'ont pas été instanciées).

**Returns:**
[Style](../../com.aspose.cells/style)
### getWidth() {#getWidth--}
```
public double getWidth()
```


Obtient la largeur de la colonne en unités de caractères.

**Remarks**

Pour les feuilles de calcul, la largeur de colonne est mesurée en nombre de caractères correspondant à la largeur maximale d'un chiffre des nombres 0~9 tels qu'ils sont rendus avec la police du style normal.

**Returns:**
double
### hasCustomStyle() {#hasCustomStyle--}
```
public boolean hasCustomStyle()
```


Indique si cette colonne possède des paramètres de style personnalisés (différents du style par défaut hérité du classeur).

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCollapsed() {#isCollapsed--}
```
public boolean isCollapsed()
```


si la colonne est réduite

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Indique si la colonne est masquée.

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




### setCollapsed(boolean value) {#setCollapsed-boolean-}
```
public void setCollapsed(boolean value)
```


si la colonne est réduite

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setGroupLevel(byte value) {#setGroupLevel-byte-}
```
public void setGroupLevel(byte value)
```


Obtient le niveau de groupe de la colonne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | byte |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Indique si la colonne est masquée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


Définit le style de cette colonne.

**Remarks**

Cette méthode définit uniquement le style donné comme style par défaut pour cette colonne, sans modifier les paramètres de style des cellules existantes dans cette colonne. Pour mettre à jour les paramètres de style des cellules existantes avec le style spécifié en même temps, veuillez utiliser [applyStyle(Style,StyleFlag)](../../com.aspose.cells/column\#applyStyle-Style-StyleFlag-)

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | le style à utiliser comme style par défaut pour les cellules de cette colonne. |

### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```


Définit la largeur de la colonne en unités de caractères.

**Remarks**

Pour les feuilles de calcul, la largeur de colonne est mesurée en nombre de caractères correspondant à la largeur maximale d'un chiffre des nombres 0~9 tels qu'ils sont rendus avec la police du style normal.

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

