---
title: "ConditionalFormattingIconCollection"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa una colección de objetos."
type: docs
url: /es/java/com.aspose.cells/conditionalformattingiconcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ConditionalFormattingIconCollection extends CollectionBase
```

Representa una colección de objetos [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon).

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
## Métodos

| Método | Descripción |
| --- | --- |
| [add(ConditionalFormattingIcon cficon)](#add-com.aspose.cells.ConditionalFormattingIcon-) | Agrega un objeto [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon). |
| [add(int type, int index)](#add-int-int-) | Agrega un objeto [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon). |
| [add(Object o)](#add-java.lang.Object-) | Agrega un elemento a la instancia de CollectionBase. |
| [clear()](#clear--) | Elimina todos los objetos de la instancia de CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | Devuelve si la instancia contiene este objeto |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtiene el elemento ConditionalFormattingIcon en el índice especificado. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtiene el número de elementos contenidos en la instancia de CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determina el índice de un elemento específico en la instancia de CollectionBase. |
| [iterator()](#iterator--) | Devuelve un enumerador que recorre la instancia de CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Elimina el elemento en el índice especificado. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(ConditionalFormattingIcon cficon) {#add-com.aspose.cells.ConditionalFormattingIcon-}
```
public int add(ConditionalFormattingIcon cficon)
```


Agrega un objeto [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon).

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use el método Add(IconSetType, int). Este método será eliminado 6 meses después, a partir de diciembre de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cficon | [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) | Devuelve el índice del nuevo objeto en la lista. |

**Returns:**
int
### add(int type, int index) {#add-int-int-}
```
public int add(int type, int index)
```


Agrega un objeto [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [IconSetType](../../com.aspose.cells/iconsettype). El tipo de valor. |
| índice | int | El índice. |

**Returns:**
int - Devuelve el índice del nuevo objeto en la lista.
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Agrega un elemento a la instancia de CollectionBase.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| o | java.lang.Object | El objeto a agregar a la instancia de CollectionBase. |

**Returns:**
int - La posición en la que se insertó el nuevo elemento.
### clear() {#clear--}
```
public void clear()
```


Elimina todos los objetos de la instancia de CollectionBase.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Devuelve si la instancia contiene este objeto

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| o | java.lang.Object | objeto de prueba |

**Returns:**
boolean - Si la instancia contiene este objeto
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
### get(int index) {#get-int-}
```
public ConditionalFormattingIcon get(int index)
```


Obtiene el elemento ConditionalFormattingIcon en el índice especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice basado en cero del elemento. |

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


Obtiene el número de elementos contenidos en la instancia de CollectionBase.

**Returns:**
int - El número de elementos contenidos en la instancia de CollectionBase.
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


Determina el índice de un elemento específico en la instancia de CollectionBase.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| o | java.lang.Object | Determina el índice de un elemento específico en la instancia de CollectionBase. |

**Returns:**
int - El índice del valor si se encuentra en la lista; de lo contrario, -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Devuelve un enumerador que recorre la instancia de CollectionBase.

**Returns:**
java.util.Iterator - Un iterador para la instancia de CollectionBase.
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


Elimina el elemento en el índice especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice basado en cero del elemento a eliminar. |

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

