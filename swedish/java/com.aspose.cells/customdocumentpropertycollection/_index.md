---
title: "CustomDocumentPropertyCollection"
second_title: "Aspose.Cells för Java API-referens"
description: "En samling av anpassade dokumentegenskaper."
type: docs
url: /sv/java/com.aspose.cells/customdocumentpropertycollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase), [com.aspose.cells.DocumentPropertyCollection](../../com.aspose.cells/documentpropertycollection)
```
public class CustomDocumentPropertyCollection extends DocumentPropertyCollection
```

En samling av anpassade dokumentegenskaper.

**Remarks**

Varje objekt representerar en anpassad egenskap i ett behållardokument.

**Example**

```
         //Instantiate a Workbook object
         Workbook workbook = new Workbook("book1.xls");
 
         //Retrieve a list of all custom document properties of the Excel file
         CustomDocumentPropertyCollection customProperties = workbook.getWorksheets().getCustomDocumentProperties();
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Lägger till ett objekt i CollectionBase-instansen. |
| [add(String name, boolean value)](#add-java.lang.String-boolean-) | Skapar en ny anpassad dokumentegenskap av datatypen **PropertyType.Boolean**. |
| [add(String name, DateTime value)](#add-java.lang.String-com.aspose.cells.DateTime-) | Skapar en ny anpassad dokumentegenskap av datatypen **PropertyType.DateTime**. |
| [add(String name, double value)](#add-java.lang.String-double-) | Skapar en ny anpassad dokumentegenskap av datatypen **PropertyType.Float**. |
| [add(String name, int value)](#add-java.lang.String-int-) | Skapar en ny anpassad dokumentegenskap av datatypen **PropertyType.Number**. |
| [add(String name, String value)](#add-java.lang.String-java.lang.String-) | Skapar en ny anpassad dokumentegenskap av datatypen **PropertyType.String**. |
| [addLinkToContent(String name, String source)](#addLinkToContent-java.lang.String-java.lang.String-) | Skapar en ny anpassad dokumentegenskap som länkar till innehåll. |
| [clear()](#clear--) | Tar bort alla objekt från CollectionBase-instansen. |
| [contains(Object o)](#contains-java.lang.Object-) | Returnerar om instansen innehåller detta objekt |
| [contains(String name)](#contains-java.lang.String-) | Returnerar true om en egenskap med det angivna namnet finns i samlingen. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Returnerar ett [DocumentProperty](../../com.aspose.cells/documentproperty)-objekt efter index. |
| [get(String name)](#get-java.lang.String-) | Returnerar ett [DocumentProperty](../../com.aspose.cells/documentproperty)-objekt efter egenskapens namn. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Hämtar antalet element som finns i CollectionBase-instansen. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen. |
| [indexOf(String name)](#indexOf-java.lang.String-) | Hämtar index för en egenskap efter namn. |
| [iterator()](#iterator--) | Returnerar en enumerator som itererar genom CollectionBase-instansen. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String name)](#remove-java.lang.String-) | Tar bort en egenskap med det angivna namnet från samlingen. |
| [removeAt(int index)](#removeAt-int-) | Tar bort en egenskap på det angivna indexet. |
| [toString()](#toString--) |  |
| [updateLinkedPropertyValue()](#updateLinkedPropertyValue--) | Uppdaterar värden för alla anpassade egenskaper som är länkade till innehåll (använd cellvärdet i det länkade området för att uppdatera värdet på den anpassade egenskapen). |
| [updateLinkedRange()](#updateLinkedRange--) | Uppdaterar alla områden som är länkade till anpassade egenskaper (använd värdet av den anpassade dokumentegenskapen för att uppdatera cellvärdet i det länkade området). |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### add(String name, boolean value) {#add-java.lang.String-boolean-}
```
public DocumentProperty add(String name, boolean value)
```


Skapar en ny anpassad dokumentegenskap av datatypen **PropertyType.Boolean**.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Namnet på egenskapen. |
| värde | boolean | Värdet på egenskapen. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### add(String name, DateTime value) {#add-java.lang.String-com.aspose.cells.DateTime-}
```
public DocumentProperty add(String name, DateTime value)
```


Skapar en ny anpassad dokumentegenskap av datatypen **PropertyType.DateTime**.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Namnet på egenskapen. |
| value | [DateTime](../../com.aspose.cells/datetime) | Värdet på egenskapen. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### add(String name, double value) {#add-java.lang.String-double-}
```
public DocumentProperty add(String name, double value)
```


Skapar en ny anpassad dokumentegenskap av datatypen **PropertyType.Float**.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Namnet på egenskapen. |
| värde | double | Värdet på egenskapen. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### add(String name, int value) {#add-java.lang.String-int-}
```
public DocumentProperty add(String name, int value)
```


Skapar en ny anpassad dokumentegenskap av datatypen **PropertyType.Number**.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Namnet på egenskapen. |
| värde | int | Värdet på egenskapen. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### add(String name, String value) {#add-java.lang.String-java.lang.String-}
```
public DocumentProperty add(String name, String value)
```


Skapar en ny anpassad dokumentegenskap av datatypen **PropertyType.String**.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Namnet på egenskapen. |
| värde | java.lang.String | Värdet på egenskapen. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### addLinkToContent(String name, String source) {#addLinkToContent-java.lang.String-java.lang.String-}
```
public DocumentProperty addLinkToContent(String name, String source)
```


Skapar en ny anpassad dokumentegenskap som länkar till innehåll.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Namnet på egenskapen. |
| källa | java.lang.String | Källan för egenskapen. Det bör vara namnet på det namngivna området. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
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
### contains(String name) {#contains-java.lang.String-}
```
public boolean contains(String name)
```


Returnerar true om en egenskap med det angivna namnet finns i samlingen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Det skiftlägesokänsliga namnet på egenskapen. |

**Returns:**
boolean - True om egenskapen finns i samlingen; false annars.
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
public DocumentProperty get(int index)
```


Returnerar ett [DocumentProperty](../../com.aspose.cells/documentproperty)-objekt efter index.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Nollbaserat index för den [DocumentProperty](../../com.aspose.cells/documentproperty) som ska hämtas. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty)
### get(String name) {#get-java.lang.String-}
```
public DocumentProperty get(String name)
```


Returnerar ett [DocumentProperty](../../com.aspose.cells/documentproperty)-objekt efter egenskapens namn.

**Remarks**

Returnerar null om en egenskap med det angivna namnet inte hittas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Det skiftlägesokänsliga namnet på egenskapen som ska hämtas. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty)
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
### indexOf(String name) {#indexOf-java.lang.String-}
```
public int indexOf(String name)
```


Hämtar index för en egenskap efter namn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Det skiftlägesokänsliga namnet på egenskapen. |

**Returns:**
int - Det nollbaserade indexet. Negativt värde om inte hittat.
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




### remove(String name) {#remove-java.lang.String-}
```
public void remove(String name)
```


Tar bort en egenskap med det angivna namnet från samlingen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Det skiftlägesokänsliga namnet på egenskapen. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Tar bort en egenskap på det angivna indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Det nollbaserade indexet. |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### updateLinkedPropertyValue() {#updateLinkedPropertyValue--}
```
public void updateLinkedPropertyValue()
```


Uppdaterar värden för alla anpassade egenskaper som är länkade till innehåll (använd cellvärdet i det länkade området för att uppdatera värdet på den anpassade egenskapen).

### updateLinkedRange() {#updateLinkedRange--}
```
public void updateLinkedRange()
```


Uppdaterar alla områden som är länkade till anpassade egenskaper (använd värdet av den anpassade dokumentegenskapen för att uppdatera cellvärdet i det länkade området).

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

