---
title: "SettablePivotGlobalizationSettings"
second_title: "Aspose.Cells för Java API-referens"
description: "Implementering av PivotGlobalizationSettings som stödjer användaren att ange/ändra fördefinierade texter."
type: docs
url: /sv/java/com.aspose.cells/settablepivotglobalizationsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings)
```
public class SettablePivotGlobalizationSettings extends PivotGlobalizationSettings
```

Implementering av PivotGlobalizationSettings som stödjer användaren att ange/ändra fördefinierade texter.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [SettablePivotGlobalizationSettings()](#SettablePivotGlobalizationSettings--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFormatOfDayGroup()](#getFormatOfDayGroup--) | Hämtar talformatet för pivottagets daggrupp. |
| [getNameOfDataField(int function, String name)](#getNameOfDataField-int-java.lang.String-) | Hämtar visningsnamnet för datapivottfältet. |
| [getShortTextOf12Months()](#getShortTextOf12Months--) | Hämtar alla kortformaterade strängar för 12 månader. |
| [getTextOf24Hours()](#getTextOf24Hours--) | Hämtar alla lokalt formaterade strängar för 24 timmar. |
| [getTextOf4Quarters()](#getTextOf4Quarters--) | Hämtar den lokala texten för 4 kvartal. |
| [getTextOf4Quaters()](#getTextOf4Quaters--) | Hämtar den lokala texten för 4 kvartal. |
| [getTextOfAll()](#getTextOfAll--) | Hämtar texten för etiketten "(All)" i pivottabellen. |
| [getTextOfAllPeriods()](#getTextOfAllPeriods--) | Hämtar den lokalanpassade texten för "All Periods". |
| [getTextOfColumnLabels()](#getTextOfColumnLabels--) | Hämtar texten för etiketten "Column Labels" i pivottabellen. |
| [getTextOfDataFieldHeader()](#getTextOfDataFieldHeader--) | Hämtar texten för rubriken för värdeområdesfältet i pivottabellen. |
| [getTextOfDays()](#getTextOfDays--) | Hämtar den lokala texten för "Days". |
| [getTextOfEmptyData()](#getTextOfEmptyData--) | Hämtar texten för etiketten "(blank)" i pivottabellen. |
| [getTextOfGrandTotal()](#getTextOfGrandTotal--) | Hämtar texten för etiketten "Grand Total" i pivottabellen. |
| [getTextOfHours()](#getTextOfHours--) | Hämtar den lokala texten för "Hours". |
| [getTextOfMinutes()](#getTextOfMinutes--) | Hämtar den lokala texten för "Minutes". |
| [getTextOfMonths()](#getTextOfMonths--) | Hämtar den lokala texten för "Months". |
| [getTextOfMultipleItems()](#getTextOfMultipleItems--) | Hämtar texten för etiketten "(Multiple Items)" i pivottabellen. |
| [getTextOfOr()](#getTextOfOr--) | Hämtar alla lokalt formaterade strängar för "or". |
| [getTextOfProtectedName(String protectedName)](#getTextOfProtectedName-java.lang.String-) | Hämtar texten för angivet skyddat namn. |
| [getTextOfProtection()](#getTextOfProtection--) | Hämtar skyddsnamnet i pivottabellen. |
| [getTextOfQuarters()](#getTextOfQuarters--) | Hämta den lokala texten för "Quarters". |
| [getTextOfRange()](#getTextOfRange--) | Hämtar den lokala texten för "Range" |
| [getTextOfRowLabels()](#getTextOfRowLabels--) | Hämtar texten för etiketten "Row Labels" i pivottabellen. |
| [getTextOfSeconds()](#getTextOfSeconds--) | Hämtar den lokala texten för "Seconds" |
| [getTextOfSubTotal(int subTotalType)](#getTextOfSubTotal-int-) | Hämtar texten för typen [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) i pivottabellen. |
| [getTextOfTotal()](#getTextOfTotal--) | Hämtar texten för etiketten "Total" i pivottabellen. |
| [getTextOfYears()](#getTextOfYears--) | Hämtar den lokala texten för "Years". |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setTextOfAll(String text)](#setTextOfAll-java.lang.String-) | Ställer in texten för "(All)"‑etiketten i PivotTable. |
| [setTextOfColumnLabels(String text)](#setTextOfColumnLabels-java.lang.String-) | Hämtar texten för etiketten "Column Labels" i pivottabellen. |
| [setTextOfDataFieldHeader(String text)](#setTextOfDataFieldHeader-java.lang.String-) | Ställer in texten för fältets rubrik i värdeområdet i PivotTable. |
| [setTextOfEmptyData(String text)](#setTextOfEmptyData-java.lang.String-) | Ställer in texten för "(blank)"‑etiketten i PivotTable. |
| [setTextOfGrandTotal(String text)](#setTextOfGrandTotal-java.lang.String-) | Ställer in texten för "Grand Total"‑etiketten i PivotTable. |
| [setTextOfMultipleItems(String text)](#setTextOfMultipleItems-java.lang.String-) | Ställer in texten för "(Multiple Items)"‑etiketten i PivotTable. |
| [setTextOfProtectedName(String protectedName, String text)](#setTextOfProtectedName-java.lang.String-java.lang.String-) | Ställer in texten för ett specifikt skyddat namn. |
| [setTextOfRowLabels(String text)](#setTextOfRowLabels-java.lang.String-) | Ställer in texten för "Row Labels"‑etiketten i PivotTable. |
| [setTextOfSubTotal(int subTotalType, String text)](#setTextOfSubTotal-int-java.lang.String-) | Ställer in texten för typen [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) i PivotTable. |
| [setTextOfTotal(String text)](#setTextOfTotal-java.lang.String-) | Ställer in texten för "Total"‑etiketten i PivotTable. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SettablePivotGlobalizationSettings() {#SettablePivotGlobalizationSettings--}
```
public SettablePivotGlobalizationSettings()
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFormatOfDayGroup() {#getFormatOfDayGroup--}
```
public String getFormatOfDayGroup()
```


Hämtar talformatet för pivottagsgrupp. Används endast när pivottfältet grupperas efter dagar. Standardvärdet är "d-MMM";

**Returns:**
java.lang.String -
### getNameOfDataField(int function, String name) {#getNameOfDataField-int-java.lang.String-}
```
public String getNameOfDataField(int function, String name)
```


Hämtar visningsnamnet för datapivottfältet. Standardformatet är "Sum Of Field".

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| function | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). Funktionen används för att sammanfatta värden i pivottfältet. |
| name | java.lang.String | Det ursprungliga namnet på pivottfältet. |

**Returns:**
java.lang.String -
### getShortTextOf12Months() {#getShortTextOf12Months--}
```
public String[] getShortTextOf12Months()
```


Hämtar alla kortformaterade strängar för 12 månader.

**Returns:**
java.lang.String[] -
### getTextOf24Hours() {#getTextOf24Hours--}
```
public String[] getTextOf24Hours()
```


Hämtar alla lokalt formaterade strängar för 24 timmar. Standardvärdet är 12 AM, 1 AM, 2 AM, 3 AM, 4 AM, 5 AM, 6 AM, 7 AM, 8 AM, 9 AM, 10 AM, 11 AM, 12 PM, 1 PM, 2 PM, 3 PM, 4 PM, 5 PM, 6 PM, 7 PM, 8 PM, 9 PM, 10 PM, 11 PM.

**Returns:**
java.lang.String[] -
### getTextOf4Quarters() {#getTextOf4Quarters--}
```
public String[] getTextOf4Quarters()
```


Hämtar den lokala texten för 4 kvartal.

**Remarks**

Returnerar som standard Quarter1, Quarter2, Quarter3, Quarter4 före 26.9. Returnerar som standard Qtr1, Qtr2, Qtr3, Qtr4 sedan 26.9.

**Returns:**
java.lang.String[] -
### getTextOf4Quaters() {#getTextOf4Quaters--}
```
public String[] getTextOf4Quaters()
```


Hämtar den lokala texten för 4 kvartal.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället PivotGlobalizationSettings.GetTextOf4Quarters()‑metoden. Denna egenskap kommer att tas bort 12 månader senare från och med juli 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
java.lang.String[] -
### getTextOfAll() {#getTextOfAll--}
```
public String getTextOfAll()
```


Hämtar texten för etiketten "(All)" i pivottabellen.

**Returns:**
java.lang.String - Texten för "(All)"‑etiketten
### getTextOfAllPeriods() {#getTextOfAllPeriods--}
```
public String getTextOfAllPeriods()
```


Hämtar den lokalanpassade texten för "All Periods".

**Returns:**
java.lang.String -
### getTextOfColumnLabels() {#getTextOfColumnLabels--}
```
public String getTextOfColumnLabels()
```


Hämtar texten för etiketten "Column Labels" i pivottabellen.

**Returns:**
java.lang.String - Texten för kolumnetiketter
### getTextOfDataFieldHeader() {#getTextOfDataFieldHeader--}
```
public String getTextOfDataFieldHeader()
```


Hämtar texten för rubriken för värdeområdesfältet i pivottabellen.

**Returns:**
java.lang.String - Texten för rubriken på datafältet
### getTextOfDays() {#getTextOfDays--}
```
public String getTextOfDays()
```


Hämtar den lokala texten för "Days".

**Returns:**
java.lang.String -
### getTextOfEmptyData() {#getTextOfEmptyData--}
```
public String getTextOfEmptyData()
```


Hämtar texten för etiketten "(blank)" i pivottabellen.

**Returns:**
java.lang.String - Texten för tom data
### getTextOfGrandTotal() {#getTextOfGrandTotal--}
```
public String getTextOfGrandTotal()
```


Hämtar texten för etiketten "Grand Total" i pivottabellen.

**Returns:**
java.lang.String - Texten för "Grand Total"‑etiketten
### getTextOfHours() {#getTextOfHours--}
```
public String getTextOfHours()
```


Hämtar den lokala texten för "Hours".

**Returns:**
java.lang.String -
### getTextOfMinutes() {#getTextOfMinutes--}
```
public String getTextOfMinutes()
```


Hämtar den lokala texten för "Minutes".

**Returns:**
java.lang.String -
### getTextOfMonths() {#getTextOfMonths--}
```
public String getTextOfMonths()
```


Hämtar den lokala texten för "Months".

**Returns:**
java.lang.String -
### getTextOfMultipleItems() {#getTextOfMultipleItems--}
```
public String getTextOfMultipleItems()
```


Hämtar texten för etiketten "(Multiple Items)" i pivottabellen.

**Returns:**
java.lang.String - Texten för "(Multiple Items)"‑etiketten
### getTextOfOr() {#getTextOfOr--}
```
public String getTextOfOr()
```


Hämtar alla lokalt formaterade strängar för "or".

**Returns:**
java.lang.String -
### getTextOfProtectedName(String protectedName) {#getTextOfProtectedName-java.lang.String-}
```
public String getTextOfProtectedName(String protectedName)
```


Hämtar texten för angivet skyddat namn.

**Remarks**

I Ms Excel är vissa namn inte tillåtna att användas som namn på PivotFields i en PivotTable. De varierar mellan olika regioner, och användaren kan ange dem explicit enligt den använda regionen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| protectedName | java.lang.String | Det skyddade namnet i PivotTable. |

**Returns:**
java.lang.String - De lokala skyddade namnen i PivotTable.
### getTextOfProtection() {#getTextOfProtection--}
```
public String getTextOfProtection()
```


Hämtar skyddsnamnet i pivottabellen.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället PivotGlobalizationSettings.GetTextOfProtectedName(string)-metoden. Denna egenskap kommer att tas bort 12 månader senare från och med mars 2023. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
java.lang.String - Skyddsnamnet för PivotTable
### getTextOfQuarters() {#getTextOfQuarters--}
```
public String getTextOfQuarters()
```


Hämta den lokala texten för "Quarters".

**Returns:**
java.lang.String -
### getTextOfRange() {#getTextOfRange--}
```
public String getTextOfRange()
```


Hämtar den lokala texten för "Range"

**Returns:**
java.lang.String -
### getTextOfRowLabels() {#getTextOfRowLabels--}
```
public String getTextOfRowLabels()
```


Hämtar texten för etiketten "Row Labels" i pivottabellen.

**Returns:**
java.lang.String - Texten för radetiketter
### getTextOfSeconds() {#getTextOfSeconds--}
```
public String getTextOfSeconds()
```


Hämtar den lokala texten för "Seconds"

**Returns:**
java.lang.String -
### getTextOfSubTotal(int subTotalType) {#getTextOfSubTotal-int-}
```
public String getTextOfSubTotal(int subTotalType)
```


Hämtar texten för typen [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) i pivottabellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| subTotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). Den [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) |

**Returns:**
java.lang.String - Texten för given typ
### getTextOfTotal() {#getTextOfTotal--}
```
public String getTextOfTotal()
```


Hämtar texten för "Total"‑etiketten i PivotTable. Du måste åsidosätta den här metoden när PivotTable innehåller två eller fler PivotFields i dataområdet.

**Returns:**
java.lang.String - Texten för "Total"‑etiketten
### getTextOfYears() {#getTextOfYears--}
```
public String getTextOfYears()
```


Hämtar den lokala texten för "Years".

**Returns:**
java.lang.String -
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




### setTextOfAll(String text) {#setTextOfAll-java.lang.String-}
```
public void setTextOfAll(String text)
```


Ställer in texten för "(All)"‑etiketten i PivotTable.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| text | java.lang.String | anpassad text |

### setTextOfColumnLabels(String text) {#setTextOfColumnLabels-java.lang.String-}
```
public void setTextOfColumnLabels(String text)
```


Hämtar texten för etiketten "Column Labels" i pivottabellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| text | java.lang.String | Texten för kolumnetiketter |

### setTextOfDataFieldHeader(String text) {#setTextOfDataFieldHeader-java.lang.String-}
```
public void setTextOfDataFieldHeader(String text)
```


Ställer in texten för fältets rubrik i värdeområdet i PivotTable.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| text | java.lang.String | Texten för datafältets rubriknamn |

### setTextOfEmptyData(String text) {#setTextOfEmptyData-java.lang.String-}
```
public void setTextOfEmptyData(String text)
```


Ställer in texten för "(blank)"‑etiketten i PivotTable.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| text | java.lang.String | Texten för tom data |

### setTextOfGrandTotal(String text) {#setTextOfGrandTotal-java.lang.String-}
```
public void setTextOfGrandTotal(String text)
```


Ställer in texten för "Grand Total"‑etiketten i PivotTable.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| text | java.lang.String | anpassad text |

### setTextOfMultipleItems(String text) {#setTextOfMultipleItems-java.lang.String-}
```
public void setTextOfMultipleItems(String text)
```


Ställer in texten för "(Multiple Items)"‑etiketten i PivotTable.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| text | java.lang.String | anpassad text |

### setTextOfProtectedName(String protectedName, String text) {#setTextOfProtectedName-java.lang.String-java.lang.String-}
```
public void setTextOfProtectedName(String protectedName, String text)
```


Ställer in texten för ett specifikt skyddat namn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| protectedName | java.lang.String | Det skyddade namnet i PivotTable. |
| text | java.lang.String | De lokala skyddade namnen för PivotTable. |

### setTextOfRowLabels(String text) {#setTextOfRowLabels-java.lang.String-}
```
public void setTextOfRowLabels(String text)
```


Ställer in texten för "Row Labels"‑etiketten i PivotTable.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| text | java.lang.String | Texten för radetiketter |

### setTextOfSubTotal(int subTotalType, String text) {#setTextOfSubTotal-int-java.lang.String-}
```
public void setTextOfSubTotal(int subTotalType, String text)
```


Ställer in texten för typen [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) i PivotTable.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| subTotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). Den [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) |
| text | java.lang.String | Texten för given typ |

### setTextOfTotal(String text) {#setTextOfTotal-java.lang.String-}
```
public void setTextOfTotal(String text)
```


Ställer in texten för "Total"‑etiketten i PivotTable.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| text | java.lang.String | anpassad text |

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

