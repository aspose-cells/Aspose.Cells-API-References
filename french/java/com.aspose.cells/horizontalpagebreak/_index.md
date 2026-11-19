---
title: "HorizontalPageBreak"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Encapsule l'objet qui représente un saut de page horizontal."
type: docs
url: /fr/java/com.aspose.cells/horizontalpagebreak/
---

**Inheritance:**
java.lang.Object
```
public class HorizontalPageBreak
```

Encapsule l'objet qui représente un saut de page horizontal.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         //Add a page break at cell Y30
         int Index = worksheet.getHorizontalPageBreaks().add("Y30");
 
         //get the newly added horizontal page break
         HorizontalPageBreak hPageBreak = worksheet.getHorizontalPageBreaks().get(Index);
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getEndColumn()](#getEndColumn--) | Obtient l'index de la colonne de fin de cette rupture de page horizontale. |
| [getRow()](#getRow--) | Obtient l'index de ligne basé sur zéro. |
| [getStartColumn()](#getStartColumn--) | Obtient l'index de la colonne de début de cette rupture de page horizontale. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getEndColumn() {#getEndColumn--}
```
public int getEndColumn()
```


Obtient l'index de la colonne de fin de cette rupture de page horizontale.

**Returns:**
int
### getRow() {#getRow--}
```
public int getRow()
```


Obtient l'index de ligne basé sur zéro.

**Returns:**
int
### getStartColumn() {#getStartColumn--}
```
public int getStartColumn()
```


Obtient l'index de la colonne de début de cette rupture de page horizontale.

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

