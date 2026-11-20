---
title: "PivotGlobalizationSettings"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Globalisierungseinstellungen für PivotTables dar."
type: docs
url: /de/java/com.aspose.cells/pivotglobalizationsettings/
---

**Inheritance:**
java.lang.Object
```
public class PivotGlobalizationSettings
```

Stellt die Globalisierungseinstellungen für PivotTables dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [PivotGlobalizationSettings()](#PivotGlobalizationSettings--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFormatOfDayGroup()](#getFormatOfDayGroup--) | Gibt das Zahlenformat der Pivot‑Tag‑Gruppe zurück. |
| [getNameOfDataField(int function, String name)](#getNameOfDataField-int-java.lang.String-) | Gibt den Anzeigenamen des Daten‑Pivot‑Felds zurück. |
| [getShortTextOf12Months()](#getShortTextOf12Months--) | Gibt alle kurz formatierten Zeichenketten der 12 Monate zurück. |
| [getTextOf24Hours()](#getTextOf24Hours--) | Gibt alle lokal formatierten Zeichenketten der 24 Stunden zurück. |
| [getTextOf4Quarters()](#getTextOf4Quarters--) | Gibt den lokalen Text der 4 Quartale zurück. |
| [getTextOf4Quaters()](#getTextOf4Quaters--) | Gibt den lokalen Text der 4 Quartale zurück. |
| [getTextOfAll()](#getTextOfAll--) | Gibt den Text des Labels "(All)" in der Pivot‑Tabelle zurück. |
| [getTextOfAllPeriods()](#getTextOfAllPeriods--) | Gibt den lokalisierten Text von "All Periods" zurück. |
| [getTextOfColumnLabels()](#getTextOfColumnLabels--) | Gibt den Text des Labels "Column Labels" in der Pivot‑Tabelle zurück. |
| [getTextOfDataFieldHeader()](#getTextOfDataFieldHeader--) | Ruft den Text der Feldkopfzeile des Wertebereichs in der PivotTable ab. |
| [getTextOfDays()](#getTextOfDays--) | Ruft den lokalen Text von "Days" ab. |
| [getTextOfEmptyData()](#getTextOfEmptyData--) | Ruft den Text des Labels "(blank)" in der PivotTable ab. |
| [getTextOfGrandTotal()](#getTextOfGrandTotal--) | Ruft den Text des Labels "Grand Total" in der PivotTable ab. |
| [getTextOfHours()](#getTextOfHours--) | Ruft den lokalen Text von "Hours" ab. |
| [getTextOfMinutes()](#getTextOfMinutes--) | Ruft den lokalen Text von "Minutes" ab. |
| [getTextOfMonths()](#getTextOfMonths--) | Ruft den lokalen Text von "Months" ab. |
| [getTextOfMultipleItems()](#getTextOfMultipleItems--) | Ruft den Text des Labels "(Multiple Items)" in der PivotTable ab. |
| [getTextOfOr()](#getTextOfOr--) | Ruft alle lokal formatierten Zeichenketten von "or" ab. |
| [getTextOfProtectedName(String protectedName)](#getTextOfProtectedName-java.lang.String-) | Ruft den Text für den angegebenen geschützten Namen ab. |
| [getTextOfProtection()](#getTextOfProtection--) | Ermittelt den Schutznamen in der PivotTable. |
| [getTextOfQuarters()](#getTextOfQuarters--) | Ruft den lokalen Text von "Quarters" ab. |
| [getTextOfRange()](#getTextOfRange--) | Ruft den lokalen Text von "Range" ab. |
| [getTextOfRowLabels()](#getTextOfRowLabels--) | Ruft den Text des Labels "Row Labels" in der PivotTable ab. |
| [getTextOfSeconds()](#getTextOfSeconds--) | Ruft den lokalen Text von "Seconds" ab. |
| [getTextOfSubTotal(int subTotalType)](#getTextOfSubTotal-int-) | Ruft den Text des Typs [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) in der PivotTable ab. |
| [getTextOfTotal()](#getTextOfTotal--) | Ruft den Text des Labels "Total" in der PivotTable ab. |
| [getTextOfYears()](#getTextOfYears--) | Ruft den lokalen Text von "Years" ab. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotGlobalizationSettings() {#PivotGlobalizationSettings--}
```
public PivotGlobalizationSettings()
```


### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
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


Ruft das Zahlenformat der Pivot‑Tag‑Gruppe ab. Wird nur verwendet, wenn das Pivot‑Feld nach Tagen gruppiert wird. Der Standardwert ist "d-MMM";

**Returns:**
java.lang.String -
### getNameOfDataField(int function, String name) {#getNameOfDataField-int-java.lang.String-}
```
public String getNameOfDataField(int function, String name)
```


Ruft den Anzeigenamen des Daten‑Pivot‑Feldes ab. Das Standardformat ist "Sum Of Field".

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| function | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). Die Funktion wird verwendet, um Werte des Pivot‑Feldes zusammenzufassen. |
| Name | java.lang.String | Der ursprüngliche Name des Pivot‑Feldes. |

**Returns:**
java.lang.String -
### getShortTextOf12Months() {#getShortTextOf12Months--}
```
public String[] getShortTextOf12Months()
```


Gibt alle kurz formatierten Zeichenketten der 12 Monate zurück.

**Returns:**
java.lang.String[] -
### getTextOf24Hours() {#getTextOf24Hours--}
```
public String[] getTextOf24Hours()
```


Ruft alle lokal formatierten Zeichenketten von 24 Stunden ab. Der Standardwert ist 12 AM, 1 AM, 2 AM, 3 AM, 4 AM, 5 AM, 6 AM, 7 AM, 8 AM, 9 AM, 10 AM, 11 AM, 12 PM, 1 PM, 2 PM, 3 PM, 4 PM, 5 PM, 6 PM, 7 PM, 8 PM, 9 PM, 10 PM, 11 PM.

**Returns:**
java.lang.String[] -
### getTextOf4Quarters() {#getTextOf4Quarters--}
```
public String[] getTextOf4Quarters()
```


Gibt den lokalen Text der 4 Quartale zurück.

**Remarks**

Gibt standardmäßig Quarter1, Quarter2, Quarter3, Quarter4 vor Version 26.9 zurück. Gibt standardmäßig Qtr1, Qtr2, Qtr3, Qtr4 seit Version 26.9 zurück.

**Returns:**
java.lang.String[] -
### getTextOf4Quaters() {#getTextOf4Quaters--}
```
public String[] getTextOf4Quaters()
```


Gibt den lokalen Text der 4 Quartale zurück.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotGlobalizationSettings.GetTextOf4Quarters(). Diese Eigenschaft wird 12 Monate später, seit Juli 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
java.lang.String[] -
### getTextOfAll() {#getTextOfAll--}
```
public String getTextOfAll()
```


Gibt den Text des Labels "(All)" in der Pivot‑Tabelle zurück.

**Returns:**
java.lang.String - Der Text des \"(All)\"-Labels
### getTextOfAllPeriods() {#getTextOfAllPeriods--}
```
public String getTextOfAllPeriods()
```


Gibt den lokalisierten Text von "All Periods" zurück.

**Returns:**
java.lang.String -
### getTextOfColumnLabels() {#getTextOfColumnLabels--}
```
public String getTextOfColumnLabels()
```


Gibt den Text des Labels "Column Labels" in der Pivot‑Tabelle zurück.

**Returns:**
java.lang.String - Der Text der Spaltenbeschriftungen
### getTextOfDataFieldHeader() {#getTextOfDataFieldHeader--}
```
public String getTextOfDataFieldHeader()
```


Ruft den Text der Feldkopfzeile des Wertebereichs in der PivotTable ab.

**Returns:**
java.lang.String - Der Text des Datenfeldkopfnamens
### getTextOfDays() {#getTextOfDays--}
```
public String getTextOfDays()
```


Ruft den lokalen Text von "Days" ab.

**Returns:**
java.lang.String -
### getTextOfEmptyData() {#getTextOfEmptyData--}
```
public String getTextOfEmptyData()
```


Ruft den Text des Labels "(blank)" in der PivotTable ab.

**Returns:**
java.lang.String - Der Text für leere Daten
### getTextOfGrandTotal() {#getTextOfGrandTotal--}
```
public String getTextOfGrandTotal()
```


Ruft den Text des Labels "Grand Total" in der PivotTable ab.

**Returns:**
java.lang.String - Der Text des \"Grand Total\"-Labels
### getTextOfHours() {#getTextOfHours--}
```
public String getTextOfHours()
```


Ruft den lokalen Text von "Hours" ab.

**Returns:**
java.lang.String -
### getTextOfMinutes() {#getTextOfMinutes--}
```
public String getTextOfMinutes()
```


Ruft den lokalen Text von "Minutes" ab.

**Returns:**
java.lang.String -
### getTextOfMonths() {#getTextOfMonths--}
```
public String getTextOfMonths()
```


Ruft den lokalen Text von "Months" ab.

**Returns:**
java.lang.String -
### getTextOfMultipleItems() {#getTextOfMultipleItems--}
```
public String getTextOfMultipleItems()
```


Ruft den Text des Labels "(Multiple Items)" in der PivotTable ab.

**Returns:**
java.lang.String - Der Text des \"(Multiple Items)\"-Labels
### getTextOfOr() {#getTextOfOr--}
```
public String getTextOfOr()
```


Ruft alle lokal formatierten Zeichenketten von "or" ab.

**Returns:**
java.lang.String -
### getTextOfProtectedName(String protectedName) {#getTextOfProtectedName-java.lang.String-}
```
public String getTextOfProtectedName(String protectedName)
```


Ruft den Text für den angegebenen geschützten Namen ab.

**Remarks**

In Ms Excel dürfen einige Namen nicht als Name von PivotFields in einer PivotTable verwendet werden. Sie unterscheiden sich je nach Region; der Benutzer kann sie je nach verwendeter Region ausdrücklich festlegen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| protectedName | java.lang.String | Der geschützte Name in der PivotTable. |

**Returns:**
java.lang.String - Die lokalen geschützten Namen der PivotTable.
### getTextOfProtection() {#getTextOfProtection--}
```
public String getTextOfProtection()
```


Ermittelt den Schutznamen in der PivotTable.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotGlobalizationSettings.GetTextOfProtectedName(string). Diese Eigenschaft wird 12 Monate später, seit März 2023, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
java.lang.String - Der Schutzname der PivotTable
### getTextOfQuarters() {#getTextOfQuarters--}
```
public String getTextOfQuarters()
```


Ruft den lokalen Text von "Quarters" ab.

**Returns:**
java.lang.String -
### getTextOfRange() {#getTextOfRange--}
```
public String getTextOfRange()
```


Ruft den lokalen Text von "Range" ab.

**Returns:**
java.lang.String -
### getTextOfRowLabels() {#getTextOfRowLabels--}
```
public String getTextOfRowLabels()
```


Ruft den Text des Labels "Row Labels" in der PivotTable ab.

**Returns:**
java.lang.String - Der Text der Zeilenbeschriftungen
### getTextOfSeconds() {#getTextOfSeconds--}
```
public String getTextOfSeconds()
```


Ruft den lokalen Text von "Seconds" ab.

**Returns:**
java.lang.String -
### getTextOfSubTotal(int subTotalType) {#getTextOfSubTotal-int-}
```
public String getTextOfSubTotal(int subTotalType)
```


Ruft den Text des Typs [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) in der PivotTable ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| subTotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). Der [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) |

**Returns:**
java.lang.String - Der Text des angegebenen Typs
### getTextOfTotal() {#getTextOfTotal--}
```
public String getTextOfTotal()
```


Gibt den Text des \"Total\"-Labels in der PivotTable zurück. Sie müssen diese Methode überschreiben, wenn die PivotTable zwei oder mehr PivotFields im Datenbereich enthält.

**Returns:**
java.lang.String - Der Text des \"Total\"-Labels
### getTextOfYears() {#getTextOfYears--}
```
public String getTextOfYears()
```


Ruft den lokalen Text von "Years" ab.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

