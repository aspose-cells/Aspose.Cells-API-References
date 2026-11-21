---
title: "GridWorkbookSettings"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar inställningarna för arbetsboken."
type: docs
url: /sv/java/com.aspose.gridweb/gridworkbooksettings/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Serializable
```
public class GridWorkbookSettings implements Serializable
```

Representerar inställningarna för arbetsboken.

**Example**

```
         GridWeb gridweb = new GridWeb();
         GridWorkbookSettings gsettings = new GridWorkbookSettings();
         gridweb.setSettings(gsettings);
 
         //do your business
```
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [GridWorkbookSettings()](#GridWorkbookSettings--) | standardkonstruktor |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAuthor()](#getAuthor--) | Hämtar filens författare. |
| [getCheckCustomNumberFormat()](#getCheckCustomNumberFormat--) | Hämtar om anpassat talformat kontrolleras när Style.Custom sätts. |
| [getClass()](#getClass--) |  |
| [getCreateCalcChain()](#getCreateCalcChain--) | Hämtar om en kedja av beräknade formler skapas. |
| [getDate1904()](#getDate1904--) | Hämtar värdet som representerar om arbetsboken använder 1904-datumsystemet. |
| [getEnableMacros()](#getEnableMacros--) | Hämtar om makron är aktiverade; Nu fungerar det endast när ett arbetsblad kopieras till ett annat arbetsblad i en arbetsbok. |
| [getForceFullCalculate()](#getForceFullCalculate--) | Hämtar om hela beräkningen utförs varje gång en beräkning triggas. |
| [getIteration()](#getIteration--) | Hämtar om iteration används för att lösa cirkulära referenser. |
| [getMaxIteration()](#getMaxIteration--) | Hämtar det maximala antalet iterationer för att lösa en cirkulär referens, standardvärdet är 100. |
| [getPrecisionAsDisplayed()](#getPrecisionAsDisplayed--) | Sant om beräkningarna i den här arbetsboken endast utförs med den precision som siffrorna visas med |
| [getPreservePaddingSpaces()](#getPreservePaddingSpaces--) | Anger om mellanslag och radbrytningar som finns mellan formeltoken ska bevaras när formler hämtas och sätts. |
| [getReCalculateOnOpen()](#getReCalculateOnOpen--) | Hämtar om alla formler ska omberäknas vid öppning av filen. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Ställer in filens författare. |
| [setCheckCustomNumberFormat(boolean value)](#setCheckCustomNumberFormat-boolean-) | Ställer in om anpassade talformat ska kontrolleras när Style.Custom sätts. |
| [setCreateCalcChain(boolean value)](#setCreateCalcChain-boolean-) | Ställer in om en kedja av beräknade formler ska skapas. |
| [setDate1904(boolean value)](#setDate1904-boolean-) | Ställer in värdet som representerar om arbetsboken använder 1904-datumsystemet. |
| [setEnableMacros(boolean value)](#setEnableMacros-boolean-) | Ställer in om makron är aktiverade; Nu fungerar det endast när ett arbetsblad kopieras till ett annat arbetsblad i en arbetsbok. |
| [setForceFullCalculate(boolean value)](#setForceFullCalculate-boolean-) | Ställer in om hela beräkningen ska utföras varje gång en beräkning triggas. |
| [setIteration(boolean value)](#setIteration-boolean-) | Ställer in om iteration ska användas för att lösa cirkulära referenser. |
| [setMaxIteration(int value)](#setMaxIteration-int-) | Ställer in det maximala antalet iterationer för att lösa en cirkulär referens, standardvärdet är 100. |
| [setPrecisionAsDisplayed(boolean value)](#setPrecisionAsDisplayed-boolean-) | Sant om beräkningarna i den här arbetsboken endast utförs med den precision som siffrorna visas med |
| [setPreservePaddingSpaces(boolean value)](#setPreservePaddingSpaces-boolean-) | Anger om mellanslag och radbrytningar som finns mellan formeltoken ska bevaras när formler hämtas och sätts. |
| [setReCalculateOnOpen(boolean value)](#setReCalculateOnOpen-boolean-) | Ställer in om alla formler ska omberäknas vid öppning av filen. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridWorkbookSettings() {#GridWorkbookSettings--}
```
public GridWorkbookSettings()
```


standardkonstruktor

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
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Hämtar filens författare.

**Returns:**
java.lang.String
### getCheckCustomNumberFormat() {#getCheckCustomNumberFormat--}
```
public boolean getCheckCustomNumberFormat()
```


Hämtar om anpassat talformat kontrolleras när Style.Custom sätts.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCreateCalcChain() {#getCreateCalcChain--}
```
public boolean getCreateCalcChain()
```


Hämtar om en kedja av beräknade formler ska skapas. Standard är falskt.

**Returns:**
boolean
### getDate1904() {#getDate1904--}
```
public boolean getDate1904()
```


Hämtar värdet som representerar om arbetsboken använder 1904-datumsystemet.

**Returns:**
boolean
### getEnableMacros() {#getEnableMacros--}
```
public boolean getEnableMacros()
```


Hämtar om makron är aktiverade; Nu fungerar det endast när ett arbetsblad kopieras till ett annat arbetsblad i en arbetsbok.

**Returns:**
boolean
### getForceFullCalculate() {#getForceFullCalculate--}
```
public boolean getForceFullCalculate()
```


Hämtar om hela beräkningen utförs varje gång en beräkning triggas.

**Returns:**
boolean
### getIteration() {#getIteration--}
```
public boolean getIteration()
```


Hämtar om iteration används för att lösa cirkulära referenser.

**Returns:**
boolean
### getMaxIteration() {#getMaxIteration--}
```
public int getMaxIteration()
```


Hämtar det maximala antalet iterationer för att lösa en cirkulär referens, standardvärdet är 100.

**Returns:**
int
### getPrecisionAsDisplayed() {#getPrecisionAsDisplayed--}
```
public boolean getPrecisionAsDisplayed()
```


Sant om beräkningarna i den här arbetsboken endast utförs med den precision som siffrorna visas med

**Returns:**
boolean
### getPreservePaddingSpaces() {#getPreservePaddingSpaces--}
```
public boolean getPreservePaddingSpaces()
```


Anger om de mellanslag och radbrytningar som är utfyllda mellan formeltoken ska bevaras vid hämtning och inställning av formler. Standardvärdet är falskt.

**Remarks**

Generellt är dessa mellanslag och radbrytningar bara för visuell presentation, att bevara dem eller inte påverkar inte det beräknade resultatet. Av prestandaskäl, om det inte finns något särskilt krav, är det bättre att inte bevara dem vid bearbetning av formler.

**Returns:**
boolean
### getReCalculateOnOpen() {#getReCalculateOnOpen--}
```
public boolean getReCalculateOnOpen()
```


Hämtar om alla formler ska omberäknas vid öppning av filen.

**Returns:**
boolean
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




### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


Ställer in filens författare.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setCheckCustomNumberFormat(boolean value) {#setCheckCustomNumberFormat-boolean-}
```
public void setCheckCustomNumberFormat(boolean value)
```


Ställer in om anpassade talformat ska kontrolleras när Style.Custom sätts.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setCreateCalcChain(boolean value) {#setCreateCalcChain-boolean-}
```
public void setCreateCalcChain(boolean value)
```


Ställer in om en kedja av beräknade formler ska skapas. Standard är falskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setDate1904(boolean value) {#setDate1904-boolean-}
```
public void setDate1904(boolean value)
```


Ställer in värdet som representerar om arbetsboken använder 1904-datumsystemet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEnableMacros(boolean value) {#setEnableMacros-boolean-}
```
public void setEnableMacros(boolean value)
```


Ställer in om makron är aktiverade; Nu fungerar det endast när ett arbetsblad kopieras till ett annat arbetsblad i en arbetsbok.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setForceFullCalculate(boolean value) {#setForceFullCalculate-boolean-}
```
public void setForceFullCalculate(boolean value)
```


Ställer in om hela beräkningen ska utföras varje gång en beräkning triggas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setIteration(boolean value) {#setIteration-boolean-}
```
public void setIteration(boolean value)
```


Ställer in om iteration ska användas för att lösa cirkulära referenser.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setMaxIteration(int value) {#setMaxIteration-int-}
```
public void setMaxIteration(int value)
```


Ställer in det maximala antalet iterationer för att lösa en cirkulär referens, standardvärdet är 100.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setPrecisionAsDisplayed(boolean value) {#setPrecisionAsDisplayed-boolean-}
```
public void setPrecisionAsDisplayed(boolean value)
```


Sant om beräkningarna i den här arbetsboken endast utförs med den precision som siffrorna visas med

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setPreservePaddingSpaces(boolean value) {#setPreservePaddingSpaces-boolean-}
```
public void setPreservePaddingSpaces(boolean value)
```


Anger om de mellanslag och radbrytningar som är utfyllda mellan formeltoken ska bevaras vid hämtning och inställning av formler. Standardvärdet är falskt.

**Remarks**

Generellt är dessa mellanslag och radbrytningar bara för visuell presentation, att bevara dem eller inte påverkar inte det beräknade resultatet. Av prestandaskäl, om det inte finns något särskilt krav, är det bättre att inte bevara dem vid bearbetning av formler.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setReCalculateOnOpen(boolean value) {#setReCalculateOnOpen-boolean-}
```
public void setReCalculateOnOpen(boolean value)
```


Ställer in om alla formler ska omberäknas vid öppning av filen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

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

