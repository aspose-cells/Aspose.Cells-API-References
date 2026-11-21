---
title: "ConditionalFormattingIconCollection"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar en samling av objekt."
type: docs
url: /sv/java/com.aspose.cells/conditionalformattingiconcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ConditionalFormattingIconCollection extends CollectionBase
```

Representerar en samling av [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) objekt.

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
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(ConditionalFormattingIcon cficon)](#add-com.aspose.cells.ConditionalFormattingIcon-) | Lägger till [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) objekt. |
| [add(int type, int index)](#add-int-int-) | Lägger till [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) objekt. |
| [add(Object o)](#add-java.lang.Object-) | Lägger till ett objekt i CollectionBase-instansen. |
| [clear()](#clear--) | Tar bort alla objekt från CollectionBase-instansen. |
| [contains(Object o)](#contains-java.lang.Object-) | Returnerar om instansen innehåller detta objekt |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Hämtar ConditionalFormattingIcon-elementet på det angivna indexet. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Hämtar antalet element som finns i CollectionBase-instansen. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen. |
| [iterator()](#iterator--) | Returnerar en enumerator som itererar genom CollectionBase-instansen. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Tar bort objektet på det angivna indexet. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(ConditionalFormattingIcon cficon) {#add-com.aspose.cells.ConditionalFormattingIcon-}
```
public int add(ConditionalFormattingIcon cficon)
```


Lägger till [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) objekt.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället Add(IconSetType, int)-metoden. Denna metod kommer att tas bort 6 månader senare från december 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cficon | [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) | Returnerar indexet för det nya objektet i listan. |

**Returns:**
int
### add(int type, int index) {#add-int-int-}
```
public int add(int type, int index)
```


Lägger till [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| type | int | [IconSetType](../../com.aspose.cells/iconsettype). Värdetypen. |
| index | int | Indexet. |

**Returns:**
int – Returnerar indexet för det nya objektet i listan.
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Lägger till ett objekt i CollectionBase-instansen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | java.lang.Object | Objektet som ska läggas till i CollectionBase-instansen. |

**Returns:**
int - Positionen där det nya elementet infördes.
### clear() {#clear--}
```
public void clear()
```


Tar bort alla objekt från CollectionBase-instansen.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Returnerar om instansen innehåller detta objekt

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | java.lang.Object | testobjekt |

**Returns:**
boolean - Om instansen innehåller detta objekt
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### get(int index) {#get-int-}
```
public ConditionalFormattingIcon get(int index)
```


Hämtar ConditionalFormattingIcon-elementet på det angivna indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Det nollbaserade indexet för elementet. |

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


Hämtar antalet element som finns i CollectionBase-instansen.

**Returns:**
int - Antalet element som finns i CollectionBase-instansen.
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


Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | java.lang.Object | Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen. |

**Returns:**
int - Indexet för värdet om det hittas i listan; annars -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Returnerar en enumerator som itererar genom CollectionBase-instansen.

**Returns:**
java.util.Iterator - En iterator för CollectionBase-instansen.
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


Tar bort objektet på det angivna indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Det nollbaserade indexet för objektet som ska tas bort. |

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

