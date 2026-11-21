---
title: "DefaultStyleSettings"
second_title: "Aspose.Cells för Java API-referens"
description: "Inställningar för standardvärdena för arbetsbokens stilegenskaper."
type: docs
url: /sv/java/com.aspose.cells/defaultstylesettings/
---

**Inheritance:**
java.lang.Object
```
public class DefaultStyleSettings
```

Inställningar för standardvärdena för arbetsbokens stilegenskaper.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBuiltInPreference()](#getBuiltInPreference--) | Indikerar om egenskapen för talformat är att föredra när stilen definierar både inbyggt tal och anpassat mönster. |
| [getClass()](#getClass--) |  |
| [getFontName()](#getFontName--) | Hämtar standardteckensnittets namn för arbetsboken |
| [getFontSize()](#getFontSize--) | Hämtar standardstorleken för standardteckensnittet för arbetsboken. |
| [getHorizontalAlignment()](#getHorizontalAlignment--) | Hämtar standardvärdet för horisontell justering |
| [getVerticalAlignment()](#getVerticalAlignment--) | Hämtar standardvärdet för vertikal justering |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBuiltInPreference(boolean value)](#setBuiltInPreference-boolean-) | Indikerar om egenskapen för talformat är att föredra när stilen definierar både inbyggt tal och anpassat mönster. |
| [setFontName(String value)](#setFontName-java.lang.String-) | Ställer in standardteckensnittets namn för arbetsboken |
| [setFontSize(double value)](#setFontSize-double-) | Ställer in standardstorleken för standardteckensnittet för arbetsboken. |
| [setHorizontalAlignment(int value)](#setHorizontalAlignment-int-) | Ställer in standardvärdet för horisontell justering |
| [setVerticalAlignment(int value)](#setVerticalAlignment-int-) | Ställer in standardvärdet för vertikal justering |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getBuiltInPreference() {#getBuiltInPreference--}
```
public boolean getBuiltInPreference()
```


Indikerar om egenskapen för talformat föredras när stilen definierar både inbyggt tal och anpassat mönster. Standardvärdet är falskt, vilket betyder att standardmässigt kommer det anpassade mönstret att användas för att formatera värden så länge det inte är tomt för en stil.

**Remarks**

När arbetsboken laddas från en befintlig mallfil kan både inbyggt tal och anpassat mönster vara definierade för en stil. Denna egenskap bestämmer om vi ska använda det inbyggda talet eller det anpassade mönstret när värden formateras med stilen.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFontName() {#getFontName--}
```
public String getFontName()
```


Hämtar standardteckensnittets namn för arbetsboken

**Returns:**
java.lang.String
### getFontSize() {#getFontSize--}
```
public double getFontSize()
```


Hämtar standardstorleken för standardteckensnittet för arbetsboken.

**Returns:**
double
### getHorizontalAlignment() {#getHorizontalAlignment--}
```
public int getHorizontalAlignment()
```


Hämtar standardvärdet för horisontell justering

Se [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getVerticalAlignment() {#getVerticalAlignment--}
```
public int getVerticalAlignment()
```


Hämtar standardvärdet för vertikal justering

Se [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

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




### setBuiltInPreference(boolean value) {#setBuiltInPreference-boolean-}
```
public void setBuiltInPreference(boolean value)
```


Indikerar om egenskapen för talformat föredras när stilen definierar både inbyggt tal och anpassat mönster. Standardvärdet är falskt, vilket betyder att standardmässigt kommer det anpassade mönstret att användas för att formatera värden så länge det inte är tomt för en stil.

**Remarks**

När arbetsboken laddas från en befintlig mallfil kan både inbyggt tal och anpassat mönster vara definierade för en stil. Denna egenskap bestämmer om vi ska använda det inbyggda talet eller det anpassade mönstret när värden formateras med stilen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setFontName(String value) {#setFontName-java.lang.String-}
```
public void setFontName(String value)
```


Ställer in standardteckensnittets namn för arbetsboken

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setFontSize(double value) {#setFontSize-double-}
```
public void setFontSize(double value)
```


Ställer in standardstorleken för standardteckensnittet för arbetsboken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setHorizontalAlignment(int value) {#setHorizontalAlignment-int-}
```
public void setHorizontalAlignment(int value)
```


Ställer in standardvärdet för horisontell justering

Se [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setVerticalAlignment(int value) {#setVerticalAlignment-int-}
```
public void setVerticalAlignment(int value)
```


Ställer in standardvärdet för vertikal justering

Se [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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

