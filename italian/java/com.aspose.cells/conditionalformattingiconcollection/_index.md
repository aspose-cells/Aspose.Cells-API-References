---
title: "ConditionalFormattingIconCollection"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta una collezione di oggetti."
type: docs
url: /it/java/com.aspose.cells/conditionalformattingiconcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ConditionalFormattingIconCollection extends CollectionBase
```

Rappresenta una collezione di oggetti [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon).

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
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add(ConditionalFormattingIcon cficon)](#add-com.aspose.cells.ConditionalFormattingIcon-) | Aggiunge l'oggetto [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon). |
| [add(int type, int index)](#add-int-int-) | Aggiunge l'oggetto [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon). |
| [add(Object o)](#add-java.lang.Object-) | Aggiunge un elemento all'istanza di CollectionBase. |
| [clear()](#clear--) | Rimuove tutti gli oggetti dall'istanza di CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | Restituisce se l'istanza contiene questo oggetto |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Recupera l'elemento ConditionalFormattingIcon all'indice specificato. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ottiene il numero di elementi contenuti nell'istanza di CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determina l'indice di un elemento specifico nell'istanza di CollectionBase. |
| [iterator()](#iterator--) | Restituisce un enumeratore che itera attraverso l'istanza di CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Rimuove l'elemento all'indice specificato. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(ConditionalFormattingIcon cficon) {#add-com.aspose.cells.ConditionalFormattingIcon-}
```
public int add(ConditionalFormattingIcon cficon)
```


Aggiunge l'oggetto [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon).

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo Add(IconSetType, int). Questo metodo sarà rimosso 6 mesi dopo, a partire da dicembre 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cficon | [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) | Restituisce l'indice del nuovo oggetto nella lista. |

**Returns:**
int
### add(int type, int index) {#add-int-int-}
```
public int add(int type, int index)
```


Aggiunge l'oggetto [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | int | [IconSetType](../../com.aspose.cells/iconsettype). Il tipo di valore. |
| indice | int | L'indice. |

**Returns:**
int - Restituisce l'indice del nuovo oggetto nella lista.
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Aggiunge un elemento all'istanza di CollectionBase.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| o | java.lang.Object | L'Object da aggiungere all'istanza di CollectionBase. |

**Returns:**
int - La posizione in cui è stato inserito il nuovo elemento.
### clear() {#clear--}
```
public void clear()
```


Rimuove tutti gli oggetti dall'istanza di CollectionBase.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Restituisce se l'istanza contiene questo oggetto

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| o | java.lang.Object | oggetto di test |

**Returns:**
boolean - Se l'istanza contiene questo oggetto
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
### get(int index) {#get-int-}
```
public ConditionalFormattingIcon get(int index)
```


Recupera l'elemento ConditionalFormattingIcon all'indice specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice basato su zero dell'elemento. |

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


Ottiene il numero di elementi contenuti nell'istanza di CollectionBase.

**Returns:**
int - Il numero di elementi contenuti nell'istanza di CollectionBase.
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


Determina l'indice di un elemento specifico nell'istanza di CollectionBase.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| o | java.lang.Object | Determina l'indice di un elemento specifico nell'istanza di CollectionBase. |

**Returns:**
int - L'indice del valore se trovato nella lista; altrimenti, -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Restituisce un enumeratore che itera attraverso l'istanza di CollectionBase.

**Returns:**
java.util.Iterator - Un iteratore per l'istanza di CollectionBase.
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


Rimuove l'elemento all'indice specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice basato su zero dell'elemento da rimuovere. |

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

