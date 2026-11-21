---
title: "GridLoadOptions"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar alternativen för att ladda filen."
type: docs
url: /sv/java/com.aspose.gridweb/gridloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class GridLoadOptions
```

Representerar alternativen för att ladda filen. [Obsolete("This class will be obsoleted after stand alone dll usage of cells public api,instead you can use Aspose.Cells.LodOptions ")]
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [GridLoadOptions()](#GridLoadOptions--) | Skapar ett alternativ för att läsa in filen. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | Anger om data automatiskt filtreras när filerna laddas. |
| [getCheckDataValid()](#getCheckDataValid--) | Kontrollera om data är giltiga i mallfilen. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Om restriktioner för Excel-filen ska kontrolleras när användaren modifierar cellrelaterade objekt. |
| [getClass()](#getClass--) |  |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | Ignorera data som inte skrivs ut om filen skrivs ut direkt |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | Om oparsade data ska behållas i minnet för arbetsboken när den laddas från mallfilen. |
| [getOnlyAuto()](#getOnlyAuto--) | Anger om endast rader vars höjd inte är anpassad ska anpassas. |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | Anger om formeln ska parsas när filen läses. |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | Anger om pivottabellens cachade poster ska parsas när filen laddas. |
| [getPassword()](#getPassword--) | Hämtar arbetsbokens lösenord. |
| [getPreservePaddingSpacesInFormula()](#getPreservePaddingSpacesInFormula--) | Anger om mellanslag och radbrytningar som finns mellan formeltoken ska bevaras när formler hämtas och sätts. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | Anger om data automatiskt filtreras när filerna laddas. |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | Kontrollera om data är giltiga i mallfilen. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Om restriktioner för Excel-filen ska kontrolleras när användaren modifierar cellrelaterade objekt. |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | Ignorera data som inte skrivs ut om filen skrivs ut direkt |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | Om oparsade data ska behållas i minnet för arbetsboken när den laddas från mallfilen. |
| [setOnlyAuto(boolean value)](#setOnlyAuto-boolean-) | Anger om endast rader vars höjd inte är anpassad ska anpassas. |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | Anger om formeln ska parsas när filen läses. |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | Anger om pivottabellens cachade poster ska parsas när filen laddas. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Ställer in lösenordet för arbetsboken. |
| [setPreservePaddingSpacesInFormula(boolean value)](#setPreservePaddingSpacesInFormula-boolean-) | Anger om mellanslag och radbrytningar som finns mellan formeltoken ska bevaras när formler hämtas och sätts. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridLoadOptions() {#GridLoadOptions--}
```
public GridLoadOptions()
```


Skapar ett alternativ för att läsa in filen.

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
### getAutoFilter() {#getAutoFilter--}
```
public boolean getAutoFilter()
```


Anger om data automatiskt filtreras när filerna laddas.

**Remarks**

Ibland, även om autofilter är inställt, döljs inte motsvarande rader i filen. Fungerar nu endast för SpreadSheetML-filen.

**Returns:**
boolean
### getCheckDataValid() {#getCheckDataValid--}
```
public boolean getCheckDataValid()
```


Kontrollera om data är giltiga i mallfilen.

**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Om restriktioner för Excel-filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att ange ett strängvärde som är längre än 32 K. När du anger ett värde längre än 32 K, t.ex. med Cell.PutValue(string), får du ett Exception om den här egenskapen är sann. Om egenskapen är falsk accepterar vi ditt inmatade strängvärde som cellens värde så att du senare kan skriva ut hela strängvärdet för andra filformat som CSV. Däremot, om du har angett ett värde som är ogiltigt för Excel-filformatet bör du inte spara arbetsboken som Excel-filformat senare. Annars kan det uppstå oväntade fel i den genererade Excel-filen.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getIgnoreNotPrinted() {#getIgnoreNotPrinted--}
```
public boolean getIgnoreNotPrinted()
```


Ignorera data som inte skrivs ut om filen skrivs ut direkt

**Remarks**

Endast för xlsx-fil.

**Returns:**
boolean
### getKeepUnparsedData() {#getKeepUnparsedData--}
```
public boolean getKeepUnparsedData()
```


Om oparsade data ska behållas i minnet för Workbook när den laddas från en mallfil. Standard är true.

**Remarks**

För scenarier där användaren bara behöver läsa vissa innehåll från mallfilen och inte behöver spara arbetsboken igen, kan du sätta denna egenskap till false för att förbättra prestanda, särskilt när den används tillsammans med någon typ av LoadFilter,

**Returns:**
boolean
### getOnlyAuto() {#getOnlyAuto--}
```
public boolean getOnlyAuto()
```


Anger om endast rader vars höjd inte är anpassad ska anpassas.

**Returns:**
boolean
### getParsingFormulaOnOpen() {#getParsingFormulaOnOpen--}
```
public boolean getParsingFormulaOnOpen()
```


Anger om formeln ska parsas när filen läses.

**Remarks**

Gäller endast för Excel Xlsx, Xltx, Xltm och Xlsm-filer eftersom formlerna i filerna lagras som en strängformel.

**Returns:**
boolean
### getParsingPivotCachedRecords() {#getParsingPivotCachedRecords--}
```
public boolean getParsingPivotCachedRecords()
```


Anger om pivot-cachade poster ska parsas vid inläsning av filen. Standardvärdet är false.

**Remarks**

Gäller endast för Excel Xlsx, Xltx, Xltm, Xlsm och xlsb-filer

**Returns:**
boolean
### getPassword() {#getPassword--}
```
public String getPassword()
```


Hämtar arbetsbokens lösenord.

**Returns:**
java.lang.String
### getPreservePaddingSpacesInFormula() {#getPreservePaddingSpacesInFormula--}
```
public boolean getPreservePaddingSpacesInFormula()
```


Anger om de mellanslag och radbrytningar som är utfyllda mellan formeltoken ska bevaras vid hämtning och inställning av formler. Standardvärdet är falskt.

**Remarks**

Efter att ha laddat arbetsboken från mallfil med detta alternativ, [GridWorkbookSettings.getPreservePaddingSpaces()](../../com.aspose.gridweb/gridworkbooksettings\#getPreservePaddingSpaces--) kommer att sättas till samma värde som denna egenskap.

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




### setAutoFilter(boolean value) {#setAutoFilter-boolean-}
```
public void setAutoFilter(boolean value)
```


Anger om data automatiskt filtreras när filerna laddas.

**Remarks**

Ibland, även om autofilter är inställt, döljs inte motsvarande rader i filen. Fungerar nu endast för SpreadSheetML-filen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setCheckDataValid(boolean value) {#setCheckDataValid-boolean-}
```
public void setCheckDataValid(boolean value)
```


Kontrollera om data är giltiga i mallfilen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Om restriktioner för Excel-filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att ange ett strängvärde som är längre än 32 K. När du anger ett värde längre än 32 K, t.ex. med Cell.PutValue(string), får du ett Exception om den här egenskapen är sann. Om egenskapen är falsk accepterar vi ditt inmatade strängvärde som cellens värde så att du senare kan skriva ut hela strängvärdet för andra filformat som CSV. Däremot, om du har angett ett värde som är ogiltigt för Excel-filformatet bör du inte spara arbetsboken som Excel-filformat senare. Annars kan det uppstå oväntade fel i den genererade Excel-filen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setIgnoreNotPrinted(boolean value) {#setIgnoreNotPrinted-boolean-}
```
public void setIgnoreNotPrinted(boolean value)
```


Ignorera data som inte skrivs ut om filen skrivs ut direkt

**Remarks**

Endast för xlsx-fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setKeepUnparsedData(boolean value) {#setKeepUnparsedData-boolean-}
```
public void setKeepUnparsedData(boolean value)
```


Om oparsade data ska behållas i minnet för Workbook när den laddas från en mallfil. Standard är true.

**Remarks**

För scenarier där användaren bara behöver läsa vissa innehåll från mallfilen och inte behöver spara arbetsboken igen, kan du sätta denna egenskap till false för att förbättra prestanda, särskilt när den används tillsammans med någon typ av LoadFilter,

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setOnlyAuto(boolean value) {#setOnlyAuto-boolean-}
```
public void setOnlyAuto(boolean value)
```


Anger om endast rader vars höjd inte är anpassad ska anpassas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setParsingFormulaOnOpen(boolean value) {#setParsingFormulaOnOpen-boolean-}
```
public void setParsingFormulaOnOpen(boolean value)
```


Anger om formeln ska parsas när filen läses.

**Remarks**

Gäller endast för Excel Xlsx, Xltx, Xltm och Xlsm-filer eftersom formlerna i filerna lagras som en strängformel.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setParsingPivotCachedRecords(boolean value) {#setParsingPivotCachedRecords-boolean-}
```
public void setParsingPivotCachedRecords(boolean value)
```


Anger om pivot-cachade poster ska parsas vid inläsning av filen. Standardvärdet är false.

**Remarks**

Gäller endast för Excel Xlsx, Xltx, Xltm, Xlsm och xlsb-filer

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


Ställer in lösenordet för arbetsboken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setPreservePaddingSpacesInFormula(boolean value) {#setPreservePaddingSpacesInFormula-boolean-}
```
public void setPreservePaddingSpacesInFormula(boolean value)
```


Anger om de mellanslag och radbrytningar som är utfyllda mellan formeltoken ska bevaras vid hämtning och inställning av formler. Standardvärdet är falskt.

**Remarks**

Efter att ha laddat arbetsboken från mallfil med detta alternativ, [GridWorkbookSettings.getPreservePaddingSpaces()](../../com.aspose.gridweb/gridworkbooksettings\#getPreservePaddingSpaces--) kommer att sättas till samma värde som denna egenskap.

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

