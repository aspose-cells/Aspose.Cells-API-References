---
title: "GridWorksheetCollection"
second_title: "Aspose.Cells för Java API-referens"
description: "Inkapslar en samling av objekt."
type: docs
url: /sv/java/com.aspose.gridweb/gridworksheetcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.CollectionBase](../../com.aspose.gridweb/collectionbase)
```
public class GridWorksheetCollection extends CollectionBase
```

Innesluter en samling av [GridWorksheet](../../com.aspose.gridweb/gridworksheet)-objekt.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add()](#add--) | Lägger till ett kalkylblad i samlingen. |
| [add(Object o)](#add-java.lang.Object-) | Lägger till ett objekt i CollectionBase-instansen. |
| [add(String sheetName)](#add-java.lang.String-) | Lägger till ett kalkylblad i samlingen. |
| [addCopy(int sheetIndex)](#addCopy-int-) | Lägger till ett kalkylblad i samlingen och kopierar data från ett befintligt kalkylblad. |
| [addCopy(String sheetName)](#addCopy-java.lang.String-) | Lägger till ett kalkylblad i samlingen och kopierar data från ett befintligt kalkylblad. |
| [calculateFormula()](#calculateFormula--) | Beräknar resultatet av formler. |
| [clear()](#clear--) | Rensa alla kalkylblad. |
| [contains(Object o)](#contains-java.lang.Object-) | Returnerar om instansen innehåller detta objekt |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Hämtar [GridWorksheet](../../com.aspose.gridweb/gridworksheet)-elementet på det angivna indexet. |
| [get(String sheetName)](#get-java.lang.String-) | Hämtar [GridWorksheet](../../com.aspose.gridweb/gridworksheet)-elementet med det angivna namnet. |
| [getActiveSheetIndex()](#getActiveSheetIndex--) | Representerar indexet för det aktiva kalkylbladet när kalkylbladet öppnas. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Hämtar storleken på enumeratorn |
| [getDefaultFontName()](#getDefaultFontName--) | Hämtar kontrollens standardteckensnittsnamn. |
| [getDefaultFontSize()](#getDefaultFontSize--) | ????????? |
| [getNames()](#getNames--) | Hämtar samlingen av alla Name-objekt i kalkylbladet. |
| [getNumberDecimalSeparator()](#getNumberDecimalSeparator--) | Hämtar decimalavgränsaren för formatering/parsning av numeriska värden. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen. |
| [insert(int index, String sheetName)](#insert-int-java.lang.String-) | Infoga ett kalkylblad. |
| [iterator()](#iterator--) | Hämtar enumerator för rader |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Tar bort elementet på ett angivet index. |
| [removeAt(String name)](#removeAt-java.lang.String-) | Tar bort elementet med ett angivet namn. |
| [setActiveSheetIndex(int value)](#setActiveSheetIndex-int-) | Representerar indexet för det aktiva kalkylbladet när kalkylbladet öppnas. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Ställer in kontrollens standardteckensnittsnamn. |
| [setDefaultFontSize(FontUnit value)](#setDefaultFontSize-com.aspose.gridweb.FontUnit-) | ????????? |
| [setNumberDecimalSeparator(char value)](#setNumberDecimalSeparator-char-) | Ställer in decimalavgränsaren för formatering/avläsning av numeriska värden. |
| [setVisible(String sheetName, boolean isVisible)](#setVisible-java.lang.String-boolean-) | Ställer in synligheten för bladet. |
| [swapSheet(int sheetIndex1, int sheetIndex2)](#swapSheet-int-int-) | Byter plats på de två bladen. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add() {#add--}
```
public int add()
```


Lägger till ett kalkylblad i samlingen.

**Returns:**
int - [GridWorksheet](../../com.aspose.gridweb/gridworksheet)-objektets index.
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
### add(String sheetName) {#add-java.lang.String-}
```
public GridWorksheet add(String sheetName)
```


Lägger till ett kalkylblad i samlingen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetName | java.lang.String | Kalkylbladsnamn |

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet) - [GridWorksheet](../../com.aspose.gridweb/gridworksheet) object.
### addCopy(int sheetIndex) {#addCopy-int-}
```
public int addCopy(int sheetIndex)
```


Lägger till ett kalkylblad i samlingen och kopierar data från ett befintligt kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetIndex | int | Index för källkalkylblad. |

**Returns:**
int - [GridWorksheet](../../com.aspose.gridweb/gridworksheet)-objektets index.
### addCopy(String sheetName) {#addCopy-java.lang.String-}
```
public int addCopy(String sheetName)
```


Lägger till ett kalkylblad i samlingen och kopierar data från ett befintligt kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetName | java.lang.String | Namn på källkalkylblad. |

**Returns:**
int - [GridWorksheet](../../com.aspose.gridweb/gridworksheet)-objektets index.
### calculateFormula() {#calculateFormula--}
```
public void calculateFormula()
```


Beräknar resultatet av formler.

### clear() {#clear--}
```
public void clear()
```


Rensa alla kalkylblad.

**Remarks**

En arbetsbok måste innehålla ett kalkylblad.

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
public GridWorksheet get(int index)
```


Hämtar [GridWorksheet](../../com.aspose.gridweb/gridworksheet)-elementet på det angivna indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Det nollbaserade indexet för elementet. |

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet) - The element at the specified index.
### get(String sheetName) {#get-java.lang.String-}
```
public GridWorksheet get(String sheetName)
```


Hämtar [GridWorksheet](../../com.aspose.gridweb/gridworksheet)-elementet med det angivna namnet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetName | java.lang.String | Namnet på arbetsbladet. |

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet) - The GridWorksheet with the name.
### getActiveSheetIndex() {#getActiveSheetIndex--}
```
public int getActiveSheetIndex()
```


Representerar indexet för det aktiva kalkylbladet när kalkylbladet öppnas.

**Remarks**

Bladindex är nollbaserat.

**Returns:**
int
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


Hämtar storleken på enumeratorn

**Returns:**
int
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```


Hämtar kontrollens standardteckensnittsnamn.

**Example**

```
             GridWeb GridWeb1=new GridWeb();
         		GridWeb1.setDefaultFontName("Arial");
```

**Returns:**
java.lang.String
### getDefaultFontSize() {#getDefaultFontSize--}
```
public FontUnit getDefaultFontSize()
```


?????????

**Returns:**
[FontUnit](../../com.aspose.gridweb/fontunit)
### getNames() {#getNames--}
```
public GridNameCollection getNames()
```


Hämtar samlingen av alla Name-objekt i kalkylbladet.

**Returns:**
[GridNameCollection](../../com.aspose.gridweb/gridnamecollection)
### getNumberDecimalSeparator() {#getNumberDecimalSeparator--}
```
public char getNumberDecimalSeparator()
```


Hämtar decimalavgränsaren för formatering/parsning av numeriska värden. Standard är decimalavgränsaren för den aktuella regionen.

**Returns:**
char
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
### insert(int index, String sheetName) {#insert-int-java.lang.String-}
```
public GridWorksheet insert(int index, String sheetName)
```


Infoga ett kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Bladindexet |
| sheetName | java.lang.String |  |

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet)
### iterator() {#iterator--}
```
public Iterator iterator()
```


Hämtar enumerator för rader

**Returns:**
java.util.Iterator - Enumeratör för rader
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


Tar bort elementet på ett angivet index.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Indexvärdet för elementet som ska tas bort. |

### removeAt(String name) {#removeAt-java.lang.String-}
```
public void removeAt(String name)
```


Tar bort elementet med ett angivet namn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Namnet på elementet som ska tas bort. |

### setActiveSheetIndex(int value) {#setActiveSheetIndex-int-}
```
public void setActiveSheetIndex(int value)
```


Representerar indexet för det aktiva kalkylbladet när kalkylbladet öppnas.

**Remarks**

Bladindex är nollbaserat.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


Ställer in kontrollens standardteckensnittsnamn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setDefaultFontSize(FontUnit value) {#setDefaultFontSize-com.aspose.gridweb.FontUnit-}
```
public void setDefaultFontSize(FontUnit value)
```


?????????

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [FontUnit](../../com.aspose.gridweb/fontunit) |  |

### setNumberDecimalSeparator(char value) {#setNumberDecimalSeparator-char-}
```
public void setNumberDecimalSeparator(char value)
```


Ställer in decimalavgränsaren för formatering/parsing av numeriska värden. Standard är decimalavgränsaren för den aktuella regionen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | char |  |

### setVisible(String sheetName, boolean isVisible) {#setVisible-java.lang.String-boolean-}
```
public void setVisible(String sheetName, boolean isVisible)
```


Ställer in synligheten för bladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetName | java.lang.String | Namn på källkalkylblad. |
| isVisible | boolean | Om kalkylbladet är synligt |

### swapSheet(int sheetIndex1, int sheetIndex2) {#swapSheet-int-int-}
```
public void swapSheet(int sheetIndex1, int sheetIndex2)
```


Byter plats på de två bladen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetIndex1 | int | Det första kalkylbladet. |
| sheetIndex2 | int | Det andra kalkylbladet. |

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

