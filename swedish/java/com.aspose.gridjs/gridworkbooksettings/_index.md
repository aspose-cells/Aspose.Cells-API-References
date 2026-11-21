---
title: "GridWorkbookSettings"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar inställningarna för arbetsboken."
type: docs
url: /sv/java/com.aspose.gridjs/gridworkbooksettings/
---

**Inheritance:**
java.lang.Object
```
public class GridWorkbookSettings
```

Representerar inställningarna för arbetsboken.

**Example**

```
         GridJsWorkbook g = new GridJsWorkbook();
 
         GridWorkbookSettings gsettings = new GridWorkbookSettings();
         g.setSettings(gsettings);
 
         //do your business
```
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [GridWorkbookSettings()](#GridWorkbookSettings--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAuthor()](#getAuthor--) | Hämtar filens författare. |
| [getCheckCustomNumberFormat()](#getCheckCustomNumberFormat--) | Anger om anpassat talformat ska kontrolleras när Style.Custom sätts, standardvärdet är false. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Om restriktioner för Excel-filen ska kontrolleras när användaren modifierar cellrelaterade objekt. |
| [getClass()](#getClass--) |  |
| [getCreateCalcChain()](#getCreateCalcChain--) | Indikerar om en kedja av beräknade formler ska skapas. |
| [getDate1904()](#getDate1904--) | Hämtar ett värde som visar om arbetsboken använder 1904-datersystemet. |
| [getEnableMacros()](#getEnableMacros--) | Aktivera makron; Nu fungerar det endast när ett kalkylblad kopieras till ett annat kalkylblad i en arbetsbok. |
| [getForceFullCalculate()](#getForceFullCalculate--) | Indikerar om den beräknar helt varje gång en beräkning utlöses. |
| [getIteration()](#getIteration--) | Indikerar om iteration ska användas för att lösa cirkulära referenser. |
| [getMaxIteration()](#getMaxIteration--) | Returnerar eller anger det maximala antalet iterationer för att lösa en cirkulär referens, standardvärdet är 100. |
| [getPrecisionAsDisplayed()](#getPrecisionAsDisplayed--) | Sant om beräkningarna i den här arbetsboken endast utförs med den precision som siffrorna visas med |
| [getReCalculateOnOpen()](#getReCalculateOnOpen--) | Indikerar om alla formler ska beräknas om vid öppning av filen. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Ställer in filens författare. |
| [setCheckCustomNumberFormat(boolean value)](#setCheckCustomNumberFormat-boolean-) | Anger om anpassat talformat ska kontrolleras när Style.Custom sätts, standardvärdet är false. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Om restriktioner för Excel-filen ska kontrolleras när användaren modifierar cellrelaterade objekt. |
| [setCreateCalcChain(boolean value)](#setCreateCalcChain-boolean-) | Indikerar om en kedja av beräknade formler ska skapas. |
| [setDate1904(boolean value)](#setDate1904-boolean-) | Ställer in ett värde som representerar om arbetsboken använder 1904-datumsystemet. |
| [setEnableMacros(boolean value)](#setEnableMacros-boolean-) | Aktivera makron; Nu fungerar det endast när ett kalkylblad kopieras till ett annat kalkylblad i en arbetsbok. |
| [setForceFullCalculate(boolean value)](#setForceFullCalculate-boolean-) | Indikerar om den beräknar helt varje gång en beräkning utlöses. |
| [setIteration(boolean value)](#setIteration-boolean-) | Indikerar om iteration ska användas för att lösa cirkulära referenser. |
| [setMaxIteration(int value)](#setMaxIteration-int-) | Returnerar eller anger det maximala antalet iterationer för att lösa en cirkulär referens, standardvärdet är 100. |
| [setPrecisionAsDisplayed(boolean value)](#setPrecisionAsDisplayed-boolean-) | Sant om beräkningarna i den här arbetsboken endast utförs med den precision som siffrorna visas med |
| [setReCalculateOnOpen(boolean value)](#setReCalculateOnOpen-boolean-) | Indikerar om alla formler ska beräknas om vid öppning av filen. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridWorkbookSettings() {#GridWorkbookSettings--}
```
public GridWorkbookSettings()
```


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


Anger om anpassat talformat ska kontrolleras när Style.Custom sätts, standardvärdet är false.

**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Om restriktioner för Excel-filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att ange ett strängvärde längre än 32 K. När du anger ett värde längre än 32 K, exempelvis via Cell.PutValue(string), får du ett Exception om den här egenskapen är sann. Om egenskapen är falsk accepterar vi ditt inmatade strängvärde som cellens värde så att du senare kan exportera hela strängvärdet till andra filformat som CSV. Däremot, om du har angett ett värde som är ogiltigt för Excel-filformatet bör du inte spara arbetsboken som Excel-filformat senare. Annars kan det uppstå oväntade fel i den genererade Excel-filen. standard är falskt.

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


Indikerar om en kedja av beräknade formler ska skapas. Standard är falskt.

**Returns:**
boolean
### getDate1904() {#getDate1904--}
```
public boolean getDate1904()
```


Hämtar ett värde som visar om arbetsboken använder 1904-datersystemet.

**Returns:**
boolean
### getEnableMacros() {#getEnableMacros--}
```
public boolean getEnableMacros()
```


Aktivera makron; Nu fungerar det endast när ett kalkylblad kopieras till ett annat kalkylblad i en arbetsbok.

**Returns:**
boolean
### getForceFullCalculate() {#getForceFullCalculate--}
```
public boolean getForceFullCalculate()
```


Indikerar om den beräknar helt varje gång en beräkning utlöses.

**Returns:**
boolean
### getIteration() {#getIteration--}
```
public boolean getIteration()
```


Indikerar om iteration ska användas för att lösa cirkulära referenser.

**Returns:**
boolean
### getMaxIteration() {#getMaxIteration--}
```
public int getMaxIteration()
```


Returnerar eller anger det maximala antalet iterationer för att lösa en cirkulär referens, standardvärdet är 100.

**Returns:**
int
### getPrecisionAsDisplayed() {#getPrecisionAsDisplayed--}
```
public boolean getPrecisionAsDisplayed()
```


Sant om beräkningarna i den här arbetsboken endast utförs med den precision som siffrorna visas med

**Returns:**
boolean
### getReCalculateOnOpen() {#getReCalculateOnOpen--}
```
public boolean getReCalculateOnOpen()
```


Indikerar om alla formler ska beräknas om vid öppning av filen. Standard är sant.

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


Anger om anpassat talformat ska kontrolleras när Style.Custom sätts, standardvärdet är false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Om restriktioner för Excel-filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att ange ett strängvärde längre än 32 K. När du anger ett värde längre än 32 K, exempelvis via Cell.PutValue(string), får du ett Exception om den här egenskapen är sann. Om egenskapen är falsk accepterar vi ditt inmatade strängvärde som cellens värde så att du senare kan exportera hela strängvärdet till andra filformat som CSV. Däremot, om du har angett ett värde som är ogiltigt för Excel-filformatet bör du inte spara arbetsboken som Excel-filformat senare. Annars kan det uppstå oväntade fel i den genererade Excel-filen. standard är falskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setCreateCalcChain(boolean value) {#setCreateCalcChain-boolean-}
```
public void setCreateCalcChain(boolean value)
```


Indikerar om en kedja av beräknade formler ska skapas. Standard är falskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setDate1904(boolean value) {#setDate1904-boolean-}
```
public void setDate1904(boolean value)
```


Ställer in ett värde som representerar om arbetsboken använder 1904-datumsystemet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEnableMacros(boolean value) {#setEnableMacros-boolean-}
```
public void setEnableMacros(boolean value)
```


Aktivera makron; Nu fungerar det endast när ett kalkylblad kopieras till ett annat kalkylblad i en arbetsbok.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setForceFullCalculate(boolean value) {#setForceFullCalculate-boolean-}
```
public void setForceFullCalculate(boolean value)
```


Indikerar om den beräknar helt varje gång en beräkning utlöses.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setIteration(boolean value) {#setIteration-boolean-}
```
public void setIteration(boolean value)
```


Indikerar om iteration ska användas för att lösa cirkulära referenser.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setMaxIteration(int value) {#setMaxIteration-int-}
```
public void setMaxIteration(int value)
```


Returnerar eller anger det maximala antalet iterationer för att lösa en cirkulär referens, standardvärdet är 100.

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

### setReCalculateOnOpen(boolean value) {#setReCalculateOnOpen-boolean-}
```
public void setReCalculateOnOpen(boolean value)
```


Indikerar om alla formler ska beräknas om vid öppning av filen. Standard är sant.

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

