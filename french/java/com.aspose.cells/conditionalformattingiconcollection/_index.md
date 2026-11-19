---
title: "ConditionalFormattingIconCollection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente une collection d'objets."
type: docs
url: /fr/java/com.aspose.cells/conditionalformattingiconcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ConditionalFormattingIconCollection extends CollectionBase
```

Représente une collection d'objets [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon).

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Worksheet sheet = workbook.getWorksheets().get(0);
         //Get Conditional Formatting
         ConditionalFormattingCollection cformattings = sheet.getConditionalFormattings();
         //Adds an empty conditional formatting
         int index = cformattings.add();
         //Get newly added Conditional formatting
         FormatConditionCollection fcs = cformattings.get(index);
         //Sets the conditional format range.
         CellArea ca = new CellArea();
         ca.StartRow = 0;
         ca.EndRow = 0;
         ca.StartColumn = 0;
         ca.EndColumn = 0;
         fcs.addArea(ca);
         ca = new CellArea();
         ca.StartRow = 1;
         ca.EndRow = 1;
         ca.StartColumn = 1;
         ca.EndColumn = 1;
         fcs.addArea(ca);
         //Sets condition
         int idx = fcs.addCondition(FormatConditionType.ICON_SET);
         FormatCondition cond = fcs.get(idx);
         //Sets condition's type
         cond.getIconSet().setType(IconSetType.ARROWS_GRAY_3);
         //Add custom iconset condition.
         ConditionalFormattingIcon cfIcon = cond.getIconSet().getCfIcons().get(0);
         cfIcon.setType(IconSetType.ARROWS_3);
         cfIcon.setIndex(0);
         ConditionalFormattingIcon cfIcon1 = cond.getIconSet().getCfIcons().get(1);
         cfIcon1.setType(IconSetType.ARROWS_GRAY_3);
         cfIcon1.setIndex(1);
         ConditionalFormattingIcon cfIcon2 = cond.getIconSet().getCfIcons().get(2);
         cfIcon2.setType(IconSetType.BOXES_5);
         cfIcon2.setIndex(2);
         //Saving the Excel file
         workbook.save("output.xls");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [add(ConditionalFormattingIcon cficon)](#add-com.aspose.cells.ConditionalFormattingIcon-) | Ajoute l'objet [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon). |
| [add(int type, int index)](#add-int-int-) | Ajoute l'objet [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon). |
| [add(Object o)](#add-java.lang.Object-) | Ajoute un élément à l'instance CollectionBase. |
| [clear()](#clear--) | Supprime tous les objets de l'instance CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | Renvoie si l'instance contient cet objet |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtient l'élément ConditionalFormattingIcon à l'index spécifié. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtient le nombre d'éléments contenus dans l'instance CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Détermine l'index d'un élément spécifique dans l'instance CollectionBase. |
| [iterator()](#iterator--) | Renvoie un énumérateur qui parcourt l'instance CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Supprime l'élément à l'index spécifié. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(ConditionalFormattingIcon cficon) {#add-com.aspose.cells.ConditionalFormattingIcon-}
```
public int add(ConditionalFormattingIcon cficon)
```


Ajoute l'objet [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon).

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode Add(IconSetType, int). Cette méthode sera supprimée 6 mois plus tard à compter de décembre 2025. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cficon | [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) | Renvoie l'index du nouvel objet dans la liste. |

**Returns:**
int
### add(int type, int index) {#add-int-int-}
```
public int add(int type, int index)
```


Ajoute l'objet [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | [IconSetType](../../com.aspose.cells/iconsettype). Le type de valeur. |
| index | int | L'index. |

**Returns:**
int - Renvoie l'index du nouvel objet dans la liste.
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Ajoute un élément à l'instance CollectionBase.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | L'objet à ajouter à l'instance CollectionBase. |

**Returns:**
int - La position dans laquelle le nouvel élément a été inséré.
### clear() {#clear--}
```
public void clear()
```


Supprime tous les objets de l'instance CollectionBase.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Renvoie si l'instance contient cet objet

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | objet de test |

**Returns:**
boolean - Si l'instance contient cet objet
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
### get(int index) {#get-int-}
```
public ConditionalFormattingIcon get(int index)
```


Obtient l'élément ConditionalFormattingIcon à l'index spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index de base zéro de l'élément. |

**Returns:**
[ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) - The element at the specified index.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


Obtient le nombre d'éléments contenus dans l'instance CollectionBase.

**Returns:**
int - Le nombre d'éléments contenus dans l'instance CollectionBase.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


Détermine l'index d'un élément spécifique dans l'instance CollectionBase.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | Détermine l'index d'un élément spécifique dans l'instance CollectionBase. |

**Returns:**
int - L'index de la valeur si elle est trouvée dans la liste ; sinon, -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Renvoie un énumérateur qui parcourt l'instance CollectionBase.

**Returns:**
java.util.Iterator - Un itérateur pour l'instance CollectionBase.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Supprime l'élément à l'index spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index basé sur zéro de l'élément à supprimer. |

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

