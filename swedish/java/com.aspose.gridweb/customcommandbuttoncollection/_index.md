---
title: "CustomCommandButtonCollection"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar samlingen av CustomCommandButton."
type: docs
url: /sv/java/com.aspose.gridweb/customcommandbuttoncollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.CollectionBase](../../com.aspose.gridweb/collectionbase)
```
public class CustomCommandButtonCollection extends CollectionBase
```

Representerar samlingen av CustomCommandButton.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         CustomCommandButton button = new CustomCommandButton();
         button.setCommand("MyCommand");
         button.setImageUrl("images/button1.gif");
         GridWeb1.getCustomCommandButtons().add(button);
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(Object value)](#add-java.lang.Object-) | Lägg till ett anpassat kommandoknappobjekt i samlingen. |
| [clear()](#clear--) | Rensar samlingen. |
| [contains(Object value)](#contains-java.lang.Object-) | Anger om det anpassade kommandoknappobjektet finns i samlingen. |
| [copyTo(Object[] array, int index)](#copyTo-java.lang.Object---int-) | Kopierar samlingen till en array. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Hämtar ett anpassat kommandoknappobjekt på indexet. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Hämtar antalet i samlingen. |
| [getSyncRoot()](#getSyncRoot--) | Endast för internt bruk. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object value)](#indexOf-java.lang.Object-) | Hämtar knappens index. |
| [insert(int index, Object value)](#insert-int-java.lang.Object-) | Infogar en knapp på indexet. |
| [isFixedSize()](#isFixedSize--) | Endast för internt bruk. |
| [isReadOnly()](#isReadOnly--) | Endast för internt bruk. |
| [isSynchronized()](#isSynchronized--) | Endast för internt bruk. |
| [iterator()](#iterator--) | Hämtar ett IEnumerator-objekt från samlingen. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Object value)](#remove-java.lang.Object-) | Tar bort det anpassade kommandoknappobjektet. |
| [removeAt(int index)](#removeAt-int-) | Tar bort på indexet. |
| [set(int index, CustomCommandButton value)](#set-int-com.aspose.gridweb.CustomCommandButton-) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Object value) {#add-java.lang.Object-}
```
public int add(Object value)
```


Lägg till ett anpassat kommandoknappobjekt i samlingen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.Object | Det anpassade kommandoknappobjektet. |

**Returns:**
int - Indexet.
### clear() {#clear--}
```
public void clear()
```


Rensar samlingen.

### contains(Object value) {#contains-java.lang.Object-}
```
public boolean contains(Object value)
```


Anger om det anpassade kommandoknappobjektet finns i samlingen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.Object | Anger om det anpassade kommandoknappobjektet finns i samlingen. |

**Returns:**
boolean - Sant eller falskt.
### copyTo(Object[] array, int index) {#copyTo-java.lang.Object---int-}
```
public void copyTo(Object[] array, int index)
```


Kopierar samlingen till en array.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| array | java.lang.Object[] | Arrayen. |
| index | int | Startindexet för arrayen. |

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
public CustomCommandButton get(int index)
```


Hämtar ett anpassat kommandoknappobjekt på indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int |  |

**Returns:**
[CustomCommandButton](../../com.aspose.gridweb/customcommandbutton)
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


Hämtar antalet i samlingen.

**Returns:**
int
### getSyncRoot() {#getSyncRoot--}
```
public Object getSyncRoot()
```


Endast för internt bruk.

**Returns:**
java.lang.Object
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object value) {#indexOf-java.lang.Object-}
```
public int indexOf(Object value)
```


Hämtar knappens index.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.Object | Knappobjektet. |

**Returns:**
int - Indexet.
### insert(int index, Object value) {#insert-int-java.lang.Object-}
```
public void insert(int index, Object value)
```


Infogar en knapp på indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Index. |
| värde | java.lang.Object | CustomCommandButton-objektet. |

### isFixedSize() {#isFixedSize--}
```
public boolean isFixedSize()
```


Endast för internt bruk.

**Returns:**
boolean
### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


Endast för internt bruk.

**Returns:**
boolean
### isSynchronized() {#isSynchronized--}
```
public boolean isSynchronized()
```


Endast för internt bruk.

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


Hämtar ett IEnumerator-objekt från samlingen.

**Returns:**
java.util.Iterator - IEnumerator-objektet.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### remove(Object value) {#remove-java.lang.Object-}
```
public void remove(Object value)
```


Tar bort det anpassade kommandoknappobjektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.Object | Det anpassade kommandoknappobjektet. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Tar bort på indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Index. |

### set(int index, CustomCommandButton value) {#set-int-com.aspose.gridweb.CustomCommandButton-}
```
public void set(int index, CustomCommandButton value)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int |  |
| value | [CustomCommandButton](../../com.aspose.gridweb/customcommandbutton) |  |

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

