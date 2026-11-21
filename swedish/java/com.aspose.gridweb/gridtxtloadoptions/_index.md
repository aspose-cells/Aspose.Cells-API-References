---
title: "GridTxtLoadOptions"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar alternativen för att läsa in en textfil."
type: docs
url: /sv/java/com.aspose.gridweb/gridtxtloadoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.GridLoadOptions](../../com.aspose.gridweb/gridloadoptions)
```
public class GridTxtLoadOptions extends GridLoadOptions
```

Representerar alternativen för att läsa in en textfil.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [GridTxtLoadOptions()](#GridTxtLoadOptions--) | Skapar alternativ för att läsa in textfil. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | Anger om data automatiskt filtreras när filerna laddas. |
| [getCheckDataValid()](#getCheckDataValid--) | Kontrollera om data är giltiga i mallfilen. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Om restriktioner för Excel-filen ska kontrolleras när användaren modifierar cellrelaterade objekt. |
| [getClass()](#getClass--) |  |
| [getConvertDateTimeData()](#getConvertDateTimeData--) | Hämtar ett värde som anger om strängen i textfilen konverteras till datumdata. |
| [getConvertNumericData()](#getConvertNumericData--) | Hämtar ett värde som anger om strängen i textfilen konverteras till numerisk data. |
| [getEncoding()](#getEncoding--) | Hämtar standardkodningen. |
| [getExtendToNextSheet()](#getExtendToNextSheet--) | Om data ska utökas till nästa blad när rader eller kolumner i data överskrider gränsen. |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | Ignorera data som inte skrivs ut om filen skrivs ut direkt |
| [getKeepPrecision()](#getKeepPrecision--) | Anger om en strängvärde inte ska parsas om längden är 15. |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | Om oparsade data ska behållas i minnet för arbetsboken när den laddas från mallfilen. |
| [getOnlyAuto()](#getOnlyAuto--) | Anger om endast rader vars höjd inte är anpassad ska anpassas. |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | Anger om formeln ska parsas när filen läses. |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | Anger om pivottabellens cachade poster ska parsas när filen laddas. |
| [getPassword()](#getPassword--) | Hämtar arbetsbokens lösenord. |
| [getPreservePaddingSpacesInFormula()](#getPreservePaddingSpacesInFormula--) | Anger om mellanslag och radbrytningar som finns mellan formeltoken ska bevaras när formler hämtas och sätts. |
| [getSeparator()](#getSeparator--) | Hämtar teckenseparator för textfil. |
| [getSeparatorString()](#getSeparatorString--) | Hämtar ett strängvärde som separator. |
| [getTextQualifier()](#getTextQualifier--) | Anger textkvalificeraren för cellvärden. |
| [getTreatConsecutiveDelimitersAsOne()](#getTreatConsecutiveDelimitersAsOne--) | Om på varandra följande avgränsare ska behandlas som en. |
| [getTreatQuotePrefixAsValue()](#getTreatQuotePrefixAsValue--) | Anger om det inledande enkla citattecknet ska tas med som en del av värdet i en cell. |
| [hasFormula()](#hasFormula--) | Anger om texten är en formel om den börjar med "=","Ställer in ett värde som anger om strängen i textfilen konverteras till datumdata. |
| [hasTextQualifier()](#hasTextQualifier--) | Om det finns en textkvalificerare för cellvärdet. |
| [hashCode()](#hashCode--) |  |
| [isMultiEncoded()](#isMultiEncoded--) | Sant betyder att filen innehåller flera kodningar. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | Anger om data automatiskt filtreras när filerna laddas. |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | Kontrollera om data är giltiga i mallfilen. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Om restriktioner för Excel-filen ska kontrolleras när användaren modifierar cellrelaterade objekt. |
| [setConvertDateTimeData(boolean value)](#setConvertDateTimeData-boolean-) | Ställer in ett värde som anger om strängen i textfilen konverteras till numerisk data. |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | Ställer in standardkodningen. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.gridweb.Encoding-) | Ställer in StreamProviderImportHtmlFile för att importera objekt. |
| [setExtendToNextSheet(boolean value)](#setExtendToNextSheet-boolean-) | Om data ska utökas till nästa blad när rader eller kolumner i data överskrider gränsen. |
| [setHasFormula(boolean value)](#setHasFormula-boolean-) | Anger om texten är en formel om den börjar med "=","Ställer in ett värde som anger om strängen i textfilen konverteras till datumdata. |
| [setHasTextQualifier(boolean value)](#setHasTextQualifier-boolean-) | Om det finns en textkvalificerare för cellvärdet. |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | Ignorera data som inte skrivs ut om filen skrivs ut direkt |
| [setKeepPrecision(boolean value)](#setKeepPrecision-boolean-) | Anger om en strängvärde inte ska parsas om längden är 15. |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | Om oparsade data ska behållas i minnet för arbetsboken när den laddas från mallfilen. |
| [setMultiEncoded(boolean value)](#setMultiEncoded-boolean-) | Sant betyder att filen innehåller flera kodningar. |
| [setOnlyAuto(boolean value)](#setOnlyAuto-boolean-) | Anger om endast rader vars höjd inte är anpassad ska anpassas. |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | Anger om formeln ska parsas när filen läses. |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | Anger om pivottabellens cachade poster ska parsas när filen laddas. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Ställer in lösenordet för arbetsboken. |
| [setPreservePaddingSpacesInFormula(boolean value)](#setPreservePaddingSpacesInFormula-boolean-) | Anger om mellanslag och radbrytningar som finns mellan formeltoken ska bevaras när formler hämtas och sätts. |
| [setSeparator(char value)](#setSeparator-char-) | Ställer in teckenseparator för textfil. |
| [setSeparatorString(String value)](#setSeparatorString-java.lang.String-) | Ställer in ett strängvärde som separator. |
| [setTextQualifier(char value)](#setTextQualifier-char-) | Anger textkvalificeraren för cellvärden. |
| [setTreatConsecutiveDelimitersAsOne(boolean value)](#setTreatConsecutiveDelimitersAsOne-boolean-) | Om på varandra följande avgränsare ska behandlas som en. |
| [setTreatQuotePrefixAsValue(boolean value)](#setTreatQuotePrefixAsValue-boolean-) | Anger om det inledande enkla citattecknet ska tas med som en del av värdet i en cell. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridTxtLoadOptions() {#GridTxtLoadOptions--}
```
public GridTxtLoadOptions()
```


Skapar alternativ för att läsa in textfil.

**Remarks**

Standardfiltypen för inläsning är CSV.

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
### getConvertDateTimeData() {#getConvertDateTimeData--}
```
public boolean getConvertDateTimeData()
```


Hämtar ett värde som anger om strängen i textfilen konverteras till datumdata.

**Returns:**
boolean
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```


Hämtar ett värde som anger om strängen i textfilen konverteras till numerisk data.

**Returns:**
boolean
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Hämtar standardkodningen. Gäller endast för csv-filer.

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding)
### getExtendToNextSheet() {#getExtendToNextSheet--}
```
public boolean getExtendToNextSheet()
```


Om data ska utökas till nästa blad när rader eller kolumner överstiger gränsen. Om denna egenskap är sann, kommer extra data att utökas till nästa blad bakom det aktuella (om det aktuella bladet är det sista, kommer ett nytt blad att läggas till i den aktuella arbetsboken). Om denna egenskap är falsk, kommer data som överstiger gränsen att ignoreras. Standardvärdet är falskt;

**Returns:**
boolean
### getIgnoreNotPrinted() {#getIgnoreNotPrinted--}
```
public boolean getIgnoreNotPrinted()
```


Ignorera data som inte skrivs ut om filen skrivs ut direkt

**Remarks**

Endast för xlsx-fil.

**Returns:**
boolean
### getKeepPrecision() {#getKeepPrecision--}
```
public boolean getKeepPrecision()
```


Anger om en strängvärde inte ska parsas om längden är 15.

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
### getSeparator() {#getSeparator--}
```
public char getSeparator()
```


Hämtar teckenseparator för textfil.

**Returns:**
char
### getSeparatorString() {#getSeparatorString--}
```
public String getSeparatorString()
```


Hämtar ett strängvärde som separator.

**Returns:**
java.lang.String
### getTextQualifier() {#getTextQualifier--}
```
public char getTextQualifier()
```


Anger textkvalificeraren för cellvärden. Standardkvalificerare är '"'.

**Remarks**

När denna egenskap sätts, kommer [hasTextQualifier()](../../com.aspose.gridweb/gridtxtloadoptions\#hasTextQualifier--) automatiskt att bli sann.

**Returns:**
char
### getTreatConsecutiveDelimitersAsOne() {#getTreatConsecutiveDelimitersAsOne--}
```
public boolean getTreatConsecutiveDelimitersAsOne()
```


Om på varandra följande avgränsare ska behandlas som en.

**Returns:**
boolean
### getTreatQuotePrefixAsValue() {#getTreatQuotePrefixAsValue--}
```
public boolean getTreatQuotePrefixAsValue()
```


Anger om det inledande enkelfnuttstecknet ska tas med som en del av värdet i en cell. Standardvärdet är sant. Om det är falskt kommer det inledande enkelfnuttet att tas bort från motsvarande cells värde och [GridTableItemStyle.getQuotePrefix()](../../com.aspose.gridweb/gridtableitemstyle\#getQuotePrefix--) kommer att sättas till sant för cellen.

**Returns:**
boolean
### hasFormula() {#hasFormula--}
```
public boolean hasFormula()
```


Anger om texten är en formel om den börjar med "=","Ställer in ett värde som anger om strängen i textfilen konverteras till datumdata.

**Returns:**
boolean
### hasTextQualifier() {#hasTextQualifier--}
```
public boolean hasTextQualifier()
```


Om det finns en textkvalificerare för cellvärdet. Standard är sant.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isMultiEncoded() {#isMultiEncoded--}
```
public boolean isMultiEncoded()
```


Sant betyder att filen innehåller flera kodningar.

**Returns:**
boolean
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

### setConvertDateTimeData(boolean value) {#setConvertDateTimeData-boolean-}
```
public void setConvertDateTimeData(boolean value)
```


Ställer in ett värde som anger om strängen i textfilen konverteras till numerisk data.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


Ställer in standardkodningen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.gridweb.Encoding-}
```
public void setEncoding(Encoding value)
```


Ställer in standardkodningen. Gäller endast för csv-filer.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.gridweb/encoding) |  |

### setExtendToNextSheet(boolean value) {#setExtendToNextSheet-boolean-}
```
public void setExtendToNextSheet(boolean value)
```


Om data ska utökas till nästa blad när rader eller kolumner överstiger gränsen. Om denna egenskap är sann, kommer extra data att utökas till nästa blad bakom det aktuella (om det aktuella bladet är det sista, kommer ett nytt blad att läggas till i den aktuella arbetsboken). Om denna egenskap är falsk, kommer data som överstiger gränsen att ignoreras. Standardvärdet är falskt;

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHasFormula(boolean value) {#setHasFormula-boolean-}
```
public void setHasFormula(boolean value)
```


Anger om texten är en formel om den börjar med "=","Ställer in ett värde som anger om strängen i textfilen konverteras till datumdata.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHasTextQualifier(boolean value) {#setHasTextQualifier-boolean-}
```
public void setHasTextQualifier(boolean value)
```


Om det finns en textkvalificerare för cellvärdet. Standard är sant.

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

### setKeepPrecision(boolean value) {#setKeepPrecision-boolean-}
```
public void setKeepPrecision(boolean value)
```


Anger om en strängvärde inte ska parsas om längden är 15.

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

### setMultiEncoded(boolean value) {#setMultiEncoded-boolean-}
```
public void setMultiEncoded(boolean value)
```


Sant betyder att filen innehåller flera kodningar.

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

### setSeparator(char value) {#setSeparator-char-}
```
public void setSeparator(char value)
```


Ställer in teckenseparator för textfil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | char |  |

### setSeparatorString(String value) {#setSeparatorString-java.lang.String-}
```
public void setSeparatorString(String value)
```


Ställer in ett strängvärde som separator.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setTextQualifier(char value) {#setTextQualifier-char-}
```
public void setTextQualifier(char value)
```


Anger textkvalificeraren för cellvärden. Standardkvalificerare är '"'.

**Remarks**

När denna egenskap sätts, kommer [hasTextQualifier()](../../com.aspose.gridweb/gridtxtloadoptions\#hasTextQualifier--) automatiskt att bli sann.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | char |  |

### setTreatConsecutiveDelimitersAsOne(boolean value) {#setTreatConsecutiveDelimitersAsOne-boolean-}
```
public void setTreatConsecutiveDelimitersAsOne(boolean value)
```


Om på varandra följande avgränsare ska behandlas som en.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setTreatQuotePrefixAsValue(boolean value) {#setTreatQuotePrefixAsValue-boolean-}
```
public void setTreatQuotePrefixAsValue(boolean value)
```


Anger om det inledande enkelfnuttstecknet ska tas med som en del av värdet i en cell. Standardvärdet är sant. Om det är falskt kommer det inledande enkelfnuttet att tas bort från motsvarande cells värde och [GridTableItemStyle.getQuotePrefix()](../../com.aspose.gridweb/gridtableitemstyle\#getQuotePrefix--) kommer att sättas till sant för cellen.

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

