---
title: "LoadFilter"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar filtret som tillhandahåller alternativ för att ladda data när arbetsboken laddas från en mall."
type: docs
url: /sv/java/com.aspose.cells/loadfilter/
---

**Inheritance:**
java.lang.Object
```
public class LoadFilter
```

Representerar filtret som tillhandahåller alternativ för att ladda data när arbetsboken laddas från en mall.

**Remarks**

Användaren kan ange filteralternativen eller implementera sin egen LoadFilter för att ange hur data ska laddas.

**Example**

Följande exempel visar hur man bestämmer filteralternativen enligt kalkylbladets egenskaper.

```
         class LoadFilterSheet extends LoadFilter
         {
             public /*override*/ void startSheet(Worksheet sheet) 
             {
                 if ("Sheet1".equals(sheet.getName()))
                 {
                     setLoadDataFilterOptions(LoadDataFilterOptions.ALL);
                 }
                 else
                 {
                     setLoadDataFilterOptions(LoadDataFilterOptions.STRUCTURE);
                 }
             }
         }
         LoadOptions opts = new LoadOptions();
         opts.setLoadFilter(new LoadFilterSheet());
         Workbook wb = new Workbook("template.xlsx", opts);
         //Custom LoadFilter implementation
```
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [LoadFilter()](#LoadFilter--) | Skapar en LoadFilter med standardfilteralternativen LoadDataFilterOptions.All. |
| [LoadFilter(int opts)](#LoadFilter-int-) | Skapar en LoadFilter med angivna filteralternativ. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getLoadDataFilterOptions()](#getLoadDataFilterOptions--) | Filteralternativen för att ange vilken data som ska laddas. |
| [getSheetsInLoadingOrder()](#getSheetsInLoadingOrder--) | Anger bladen (index) och ordning som ska laddas. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setLoadDataFilterOptions(int value)](#setLoadDataFilterOptions-int-) | Filteralternativen för att ange vilken data som ska laddas. |
| [startSheet(Worksheet sheet)](#startSheet-com.aspose.cells.Worksheet-) | Förbereder filteralternativen innan angivet kalkylblad laddas. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LoadFilter() {#LoadFilter--}
```
public LoadFilter()
```


Skapar en LoadFilter med standardfilteralternativen LoadDataFilterOptions.All.

### LoadFilter(int opts) {#LoadFilter-int-}
```
public LoadFilter(int opts)
```


Skapar en LoadFilter med angivna filteralternativ.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| opts | int | [LoadDataFilterOptions](../../com.aspose.cells/loaddatafilteroptions). standardfilteralternativen |

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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getLoadDataFilterOptions() {#getLoadDataFilterOptions--}
```
public int getLoadDataFilterOptions()
```


Filteralternativen för att ange vilken data som ska laddas.

Se [LoadDataFilterOptions](../../com.aspose.cells/loaddatafilteroptions).

**Returns:**
int
### getSheetsInLoadingOrder() {#getSheetsInLoadingOrder--}
```
public int[] getSheetsInLoadingOrder()
```


Anger bladen (index) och ordning som ska laddas. Standard är null, vilket betyder att alla blad ska laddas i standardordning i mallfilen. Om inte null och ett bladindex inte finns i den returnerade arrayen, laddas bladet inte.

**Returns:**
int[]
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




### setLoadDataFilterOptions(int value) {#setLoadDataFilterOptions-int-}
```
public void setLoadDataFilterOptions(int value)
```


Filteralternativen för att ange vilken data som ska laddas.

Se [LoadDataFilterOptions](../../com.aspose.cells/loaddatafilteroptions).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### startSheet(Worksheet sheet) {#startSheet-com.aspose.cells.Worksheet-}
```
public void startSheet(Worksheet sheet)
```


Förbereder filteralternativen innan angivet kalkylblad laddas. Användarens implementation av LoadFilter kan ändra LoadDataFilterOptions här för att ange hur data ska laddas för detta kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheet | [Worksheet](../../com.aspose.cells/worksheet) | Kalkylbladet som ska laddas. Det finns bara några få egenskaper som kan användas för det angivna kalkylbladsobjektet här eftersom de flesta data och egenskaper inte har laddats. Tillgängliga egenskaper är: Name, Index, VisibilityType |

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

