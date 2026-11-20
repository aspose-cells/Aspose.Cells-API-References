---
title: "SettableGlobalizationSettings"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Implementierung von GlobalizationSettings, die dem Benutzer das Festlegen/Ändern vordefinierter Texte ermöglicht."
type: docs
url: /de/java/com.aspose.cells/settableglobalizationsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.GlobalizationSettings](../../com.aspose.cells/globalizationsettings)
```
public class SettableGlobalizationSettings extends GlobalizationSettings
```

Implementierung von GlobalizationSettings, die dem Benutzer das Festlegen/Ändern vordefinierter Texte ermöglicht.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [SettableGlobalizationSettings()](#SettableGlobalizationSettings--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [compare(String v1, String v2, boolean ignoreCase)](#compare-java.lang.String-java.lang.String-boolean-) | Vergleicht zwei Zeichenkettenwerte gemäß bestimmter Sortierregeln. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllName()](#getAllName--) | Liefert den Namen des "(All)"-Labels in der PivotTable. |
| [getBooleanValueString(boolean bv)](#getBooleanValueString-boolean-) | Liefert den Anzeigetextwert für den booleschen Zellwert. |
| [getChartSettings()](#getChartSettings--) | Liefert die Globalisierungseinstellungen für Diagramme. |
| [getClass()](#getClass--) |  |
| [getCollationKey(String v, boolean ignoreCase)](#getCollationKey-java.lang.String-boolean-) | Transformiert die Zeichenkette in ein vergleichbares Objekt gemäß bestimmter Sortierregeln. |
| [getColumnLabelsOfPivotTable()](#getColumnLabelsOfPivotTable--) | Liefert den Namen des "Column Labels"-Labels in der PivotTable. |
| [getColumnSeparatorOfFormulaArray()](#getColumnSeparatorOfFormulaArray--) | Liefert das Trennzeichen für die Elemente in den Zeilendaten des Arrays in einer Formel. |
| [getCommentTitleName(int type)](#getCommentTitleName-int-) | Liefert den lokalisierungsabhängigen Kommentar‑Titelnamen gemäß dem Typ des Kommentar‑Titels. |
| [getDataFieldHeaderNameOfPivotTable()](#getDataFieldHeaderNameOfPivotTable--) | Liefert den Namen der Feldüberschrift des Wertebereichs in der PivotTable. |
| [getDefaultSheetName()](#getDefaultSheetName--) | Liefert den Standardblattnamen zum automatischen Hinzufügen eines Arbeitsblatts. |
| [getEmptyDataName()](#getEmptyDataName--) | Ermittelt den Namen des "(blank)"-Labels in der PivotTable. |
| [getErrorValueString(String err)](#getErrorValueString-java.lang.String-) | Ermittelt den Anzeigestringwert für den Fehlerwert der Zelle. |
| [getGrandTotalName(int functionType)](#getGrandTotalName-int-) | Ermittelt den Namen des Gesamtsummennamens der Funktion. |
| [getListSeparator()](#getListSeparator--) | Ermittelt das Trennzeichen für Listen, Funktionsparameter, ...usw. |
| [getLocalBuiltInName(String standardName)](#getLocalBuiltInName-java.lang.String-) | Ermittelt den lokalisierungsabhängigen Text für den integrierten Namen gemäß dem angegebenen Standardtext. |
| [getLocalFunctionName(String standardName)](#getLocalFunctionName-java.lang.String-) | Ermittelt den lokalisierungsabhängigen Funktionsnamen gemäß dem angegebenen Standardfunktionsnamen. |
| [getMultipleItemsName()](#getMultipleItemsName--) | Ermittelt den Namen des "(Multiple Items)"-Labels in der PivotTable. |
| [getPivotGrandTotalName()](#getPivotGrandTotalName--) | Ermittelt den Namen des "Grand Total"-Labels in der PivotTable. |
| [getPivotSettings()](#getPivotSettings--) | Ermittelt die Globalisierungseinstellungen für die PivotTable. |
| [getPivotTotalName()](#getPivotTotalName--) | Ermittelt den Namen des "Total"-Labels in der PivotTable. |
| [getProtectionNameOfPivotTable()](#getProtectionNameOfPivotTable--) | Ermittelt den Schutznamen in der PivotTable. |
| [getRowLabelsNameOfPivotTable()](#getRowLabelsNameOfPivotTable--) | Ermittelt den Namen des "Row Labels"-Labels in der PivotTable. |
| [getRowSeparatorOfFormulaArray()](#getRowSeparatorOfFormulaArray--) | Ermittelt das Trennzeichen für Zeilen in Arraydaten in der Formel. |
| [getStandardBuiltInName(String localName)](#getStandardBuiltInName-java.lang.String-) | Ermittelt den Standardtext des integrierten Namens gemäß dem angegebenen lokalisierungsabhängigen Text. |
| [getStandardFunctionName(String localName)](#getStandardFunctionName-java.lang.String-) | Ermittelt den Standardfunktionsnamen gemäß dem angegebenen lokalisierungsabhängigen Funktionsnamen. |
| [getStandardHeaderFooterFontStyleName(String localfontStyleName)](#getStandardHeaderFooterFontStyleName-java.lang.String-) | Ermittelt den standardmäßigen englischen Schriftstilnamen (Regular, Bold, Italic) für Header/Footer gemäß dem angegebenen lokalisierungsabhängigen Schriftstilnamen. |
| [getSubTotalName(int subTotalType)](#getSubTotalName-int-) | Ermittelt den Namen des [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype)-Typs in der PivotTable. |
| [getTableRowTypeOfAll()](#getTableRowTypeOfAll--) | Ermittelt den Typnamen der Tabellenzeilen, die alle Zeilen in der referenzierten Tabelle enthalten. |
| [getTableRowTypeOfCurrent()](#getTableRowTypeOfCurrent--) | Ermittelt den Typnamen der Tabellenzeilen, die die aktuelle Zeile in der referenzierten Tabelle enthalten. |
| [getTableRowTypeOfData()](#getTableRowTypeOfData--) | Ermittelt den Typnamen der Tabellenzeilen, die den Datenbereich der referenzierten Tabelle enthalten. |
| [getTableRowTypeOfHeaders()](#getTableRowTypeOfHeaders--) | Ermittelt den Typnamen der Tabellenzeilen, die die Tabellenkopfzeile enthalten. |
| [getTableRowTypeOfTotals()](#getTableRowTypeOfTotals--) | Ermittelt den Typnamen der Tabellenzeilen, die die Gesamtsummenzeile der referenzierten Tabelle enthalten. |
| [getTotalName(int functionType)](#getTotalName-int-) | Ermittelt den Gesamtnamen einer bestimmten Funktion. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBooleanValueString(boolean bv, String name)](#setBooleanValueString-boolean-java.lang.String-) | Setzt den Anzeigestringwert für den booleschen Wert der Zelle. |
| [setChartSettings(ChartGlobalizationSettings value)](#setChartSettings-com.aspose.cells.ChartGlobalizationSettings-) | Setzt die Globalisierungseinstellungen für das Diagramm. |
| [setColumnSeparatorOfFormulaArray(char c)](#setColumnSeparatorOfFormulaArray-char-) | Legt das Trennzeichen für die Elemente in den Zeilendaten des Arrays in der Formel fest. |
| [setCommentTitleName(int type, String name)](#setCommentTitleName-int-java.lang.String-) | Liefert den lokalisierungsabhängigen Kommentar‑Titelnamen gemäß dem Typ des Kommentar‑Titels. |
| [setGrandTotalName(int functionType, String name)](#setGrandTotalName-int-java.lang.String-) | Legt den Namen des Gesamtsummens für eine bestimmte Funktion fest. |
| [setListSeparator(char c)](#setListSeparator-char-) | Legt das Trennzeichen für Listen, Funktionsparameter, ... usw. fest. |
| [setLocalBuiltInName(String standardName, String localName, boolean bidirectional)](#setLocalBuiltInName-java.lang.String-java.lang.String-boolean-) | Legt den lokalisierungsabhängigen Text für den integrierten Namen mit dem angegebenen Standardnamen fest. |
| [setLocalFunctionName(String standardName, String localName, boolean bidirectional)](#setLocalFunctionName-java.lang.String-java.lang.String-boolean-) | Legt den lokalisierungsabhängigen Funktionsnamen fest, der dem angegebenen Standardfunktionsnamen entspricht. |
| [setPivotSettings(PivotGlobalizationSettings value)](#setPivotSettings-com.aspose.cells.PivotGlobalizationSettings-) | Legt die Globalisierungseinstellungen für die Pivot-Tabelle fest. |
| [setRowSeparatorOfFormulaArray(char c)](#setRowSeparatorOfFormulaArray-char-) | Legt das Trennzeichen für Zeilen in den Array-Daten in der Formel fest. |
| [setStandardBuiltInName(String localName, String standardName, boolean bidirectional)](#setStandardBuiltInName-java.lang.String-java.lang.String-boolean-) | Legt den lokalisierungsabhängigen Funktionsnamen gemäß dem angegebenen Standardfunktionsnamen fest. |
| [setStandardFunctionName(String localName, String standardName, boolean bidirectional)](#setStandardFunctionName-java.lang.String-java.lang.String-boolean-) | Legt den lokalisierungsabhängigen Funktionsnamen gemäß dem angegebenen Standardfunktionsnamen fest. |
| [setStandardHeaderFooterFontStyleName(String localfontStyleName, String standardName)](#setStandardHeaderFooterFontStyleName-java.lang.String-java.lang.String-) | Legt den lokalisierungsabhängigen Funktionsnamen gemäß dem angegebenen Standardfunktionsnamen fest. |
| [setTableRowTypeOfAll(String name)](#setTableRowTypeOfAll-java.lang.String-) | Legt den Typnamen für Tabellenzeilen fest, die alle Zeilen in der referenzierten Tabelle enthalten. |
| [setTableRowTypeOfCurrent(String name)](#setTableRowTypeOfCurrent-java.lang.String-) | Legt den Typnamen für Tabellenzeilen fest, die die aktuelle Zeile in der referenzierten Tabelle enthalten. |
| [setTableRowTypeOfData(String name)](#setTableRowTypeOfData-java.lang.String-) | Legt den Typnamen für Tabellenzeilen fest, die den Datenbereich der referenzierten Tabelle enthalten. |
| [setTableRowTypeOfHeaders(String name)](#setTableRowTypeOfHeaders-java.lang.String-) | Legt den Typnamen für Tabellenzeilen fest, die die Tabellenüberschrift enthalten. |
| [setTableRowTypeOfTotals(String name)](#setTableRowTypeOfTotals-java.lang.String-) | Legt den Typnamen für Tabellenzeilen fest, die die Gesamtsumme‑Zeile der referenzierten Tabelle enthalten. |
| [setTotalName(int functionType, String name)](#setTotalName-int-java.lang.String-) | Legt den Namen der Gesamtsumme für eine bestimmte Funktion fest. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SettableGlobalizationSettings() {#SettableGlobalizationSettings--}
```
public SettableGlobalizationSettings()
```


### compare(String v1, String v2, boolean ignoreCase) {#compare-java.lang.String-java.lang.String-boolean-}
```
public int compare(String v1, String v2, boolean ignoreCase)
```


Vergleicht zwei Zeichenkettenwerte gemäß bestimmter Sortierregeln.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| v1 | java.lang.String | die erste Zeichenkette |
| v2 | java.lang.String | die zweite Zeichenkette |
| ignoreCase | boolean | ob bei Vergleich von Werten die Groß-/Kleinschreibung ignoriert werden soll |

**Returns:**
int - Integer, der die lexikalische Beziehung zwischen den beiden Vergleichswerten angibt
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
### getAllName() {#getAllName--}
```
public String getAllName()
```


Liefert den Namen des "(All)"-Labels in der PivotTable.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Stattdessen verwenden Sie bitte die Methode GlobalizationSettings.GetColumnLabelsOfPivotTable(). Diese Eigenschaft wird 12 Monate nach Dezember 2022 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
java.lang.String - Der Name des "(All)"-Labels
### getBooleanValueString(boolean bv) {#getBooleanValueString-boolean-}
```
public String getBooleanValueString(boolean bv)
```


Liefert den Anzeigetextwert für den booleschen Zellwert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| bv | boolean | boolescher Wert |

**Returns:**
java.lang.String - Gibt standardmäßig "TRUE" für den wahren Wert und "FALSE" für den falschen Wert zurück.
### getChartSettings() {#getChartSettings--}
```
public ChartGlobalizationSettings getChartSettings()
```


Liefert die Globalisierungseinstellungen für Diagramme.

**Returns:**
[ChartGlobalizationSettings](../../com.aspose.cells/chartglobalizationsettings)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCollationKey(String v, boolean ignoreCase) {#getCollationKey-java.lang.String-boolean-}
```
public Comparable getCollationKey(String v, boolean ignoreCase)
```


Transformiert die Zeichenkette in ein vergleichbares Objekt gemäß bestimmter Sortierregeln.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| v | java.lang.String | String-Wert muss mit anderen verglichen werden. |
| ignoreCase | boolean | ob bei Vergleich von Werten die Groß-/Kleinschreibung ignoriert werden soll |

**Returns:**
java.lang.Comparable - Objekt kann verwendet werden, um String-Werte zu vergleichen oder zu sortieren
### getColumnLabelsOfPivotTable() {#getColumnLabelsOfPivotTable--}
```
public String getColumnLabelsOfPivotTable()
```


Liefert den Namen des "Column Labels"-Labels in der PivotTable.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Diese Eigenschaft wird 12 Monate später, seit Dezember 2022, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
java.lang.String - Der Name der Spaltenbeschriftungen
### getColumnSeparatorOfFormulaArray() {#getColumnSeparatorOfFormulaArray--}
```
public char getColumnSeparatorOfFormulaArray()
```


Liefert das Trennzeichen für die Elemente in den Zeilendaten des Arrays in einer Formel.

**Returns:**
char
### getCommentTitleName(int type) {#getCommentTitleName-int-}
```
public String getCommentTitleName(int type)
```


Liefert den lokalisierungsabhängigen Kommentar‑Titelnamen gemäß dem Typ des Kommentar‑Titels.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| type | int | [CommentTitleType](../../com.aspose.cells/commenttitletype). Typ des Kommentar-Titels |

**Returns:**
java.lang.String - lokalisierungsabhängiger Name des Kommentar-Titels
### getDataFieldHeaderNameOfPivotTable() {#getDataFieldHeaderNameOfPivotTable--}
```
public String getDataFieldHeaderNameOfPivotTable()
```


Liefert den Namen der Feldüberschrift des Wertebereichs in der PivotTable.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Diese Eigenschaft wird 12 Monate später, seit Dezember 2022, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
java.lang.String - Der Name des Datenfeld‑Kopfzeilen-Namens
### getDefaultSheetName() {#getDefaultSheetName--}
```
public String getDefaultSheetName()
```


Ermittelt den Standardblattnamen für das automatische Hinzufügen eines Arbeitsblatts. Standard ist "Sheet".

**Remarks**

Der automatisch hinzugefügte (z. B. über [WorksheetCollection.add()](../../com.aspose.cells/worksheetcollection\#add--)) Blattname wird der angegebene Name plus einer laufenden Nummer sein. Zum Beispiel könnte ein deutscher Benutzer den Blattnamen "Tabellenblatt2" anstelle von "Sheet2" wünschen. Dann kann der Benutzer diese Methode implementieren, um "Tabellenblatt" zurückzugeben.

**Returns:**
java.lang.String - der Standardblattname für das automatische Hinzufügen eines Arbeitsblatts
### getEmptyDataName() {#getEmptyDataName--}
```
public String getEmptyDataName()
```


Ermittelt den Namen des "(blank)"-Labels in der PivotTable.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Diese Eigenschaft wird 12 Monate später, seit Dezember 2022, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
java.lang.String - Der Name für leere Daten
### getErrorValueString(String err) {#getErrorValueString-java.lang.String-}
```
public String getErrorValueString(String err)
```


Ermittelt den Anzeigestringwert für den Fehlerwert der Zelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| err | java.lang.String | Fehlerwerte wie \#VALUE!,\#NAME? |

**Returns:**
java.lang.String - Gibt standardmäßig den Fehlerwert selbst zurück
### getGrandTotalName(int functionType) {#getGrandTotalName-int-}
```
public String getGrandTotalName(int functionType)
```


Ermittelt den Namen des Gesamtsummennamens der Funktion.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| functionType | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). Der Funktionstyp. |

**Returns:**
java.lang.String - Der Gesamtsummenname der Funktion.
### getListSeparator() {#getListSeparator--}
```
public char getListSeparator()
```


Ermittelt das Trennzeichen für Listen, Funktionsparameter, ...usw.

**Returns:**
char
### getLocalBuiltInName(String standardName) {#getLocalBuiltInName-java.lang.String-}
```
public String getLocalBuiltInName(String standardName)
```


Ermittelt den lokalisierungsabhängigen Text für den integrierten Namen gemäß dem angegebenen Standardtext.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| standardName | java.lang.String | Standard(en-US locale) Text des integrierten Namens. |

**Returns:**
java.lang.String - Lokalisierungsabhängiger Text. Das Gebietsschema wurde vom Arbeitsbuch angegeben, für das diese Einstellung verwendet wird.
### getLocalFunctionName(String standardName) {#getLocalFunctionName-java.lang.String-}
```
public String getLocalFunctionName(String standardName)
```


Ermittelt den lokalisierungsabhängigen Funktionsnamen gemäß dem angegebenen Standardfunktionsnamen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| standardName | java.lang.String | Standard(en-US locale) Funktionsname. |

**Returns:**
java.lang.String - Lokalisierungsabhängiger Funktionsname. Das Gebietsschema wurde vom Arbeitsbuch angegeben, für das diese Einstellung verwendet wird.
### getMultipleItemsName() {#getMultipleItemsName--}
```
public String getMultipleItemsName()
```


Ermittelt den Namen des "(Multiple Items)"-Labels in der PivotTable.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Diese Eigenschaft wird 12 Monate später, seit Dezember 2022, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
java.lang.String - Der Name des Labels "(Multiple Items)"
### getPivotGrandTotalName() {#getPivotGrandTotalName--}
```
public String getPivotGrandTotalName()
```


Ermittelt den Namen des "Grand Total"-Labels in der PivotTable.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Diese Eigenschaft wird 12 Monate später, seit Dezember 2022, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
java.lang.String - Der Name des \"Grand Total\"-Labels
### getPivotSettings() {#getPivotSettings--}
```
public PivotGlobalizationSettings getPivotSettings()
```


Ermittelt die Globalisierungseinstellungen für die PivotTable.

**Returns:**
[PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings)
### getPivotTotalName() {#getPivotTotalName--}
```
public String getPivotTotalName()
```


Ruft den Namen des \"Total\"-Labels in der PivotTable ab. Sie müssen diese Methode überschreiben, wenn die PivotTable zwei oder mehr PivotFields im Datenbereich enthält.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Diese Eigenschaft wird 12 Monate später, seit Dezember 2022, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
java.lang.String - Der Name des \"Total\"-Labels
### getProtectionNameOfPivotTable() {#getProtectionNameOfPivotTable--}
```
public String getProtectionNameOfPivotTable()
```


Ermittelt den Schutznamen in der PivotTable.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotGlobalizationSettings.GetTextOfProtectedName(string). Diese Eigenschaft wird 12 Monate später, seit Dezember 2022, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
java.lang.String - Der Schutzname der PivotTable
### getRowLabelsNameOfPivotTable() {#getRowLabelsNameOfPivotTable--}
```
public String getRowLabelsNameOfPivotTable()
```


Ermittelt den Namen des "Row Labels"-Labels in der PivotTable.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Diese Eigenschaft wird 12 Monate später, seit Dezember 2022, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
java.lang.String - Der Name der Zeilenbeschriftungen
### getRowSeparatorOfFormulaArray() {#getRowSeparatorOfFormulaArray--}
```
public char getRowSeparatorOfFormulaArray()
```


Ermittelt das Trennzeichen für Zeilen in Arraydaten in der Formel.

**Returns:**
char
### getStandardBuiltInName(String localName) {#getStandardBuiltInName-java.lang.String-}
```
public String getStandardBuiltInName(String localName)
```


Ermittelt den Standardtext des integrierten Namens gemäß dem angegebenen lokalisierungsabhängigen Text.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| localName | java.lang.String | Lokalisierungsabhängiger Text des integrierten Namens. Das Gebietsschema wurde vom Arbeitsbuch angegeben, für das diese Einstellung verwendet wird. |

**Returns:**
java.lang.String - Standard(en-US-Locale) Text.
### getStandardFunctionName(String localName) {#getStandardFunctionName-java.lang.String-}
```
public String getStandardFunctionName(String localName)
```


Ermittelt den Standardfunktionsnamen gemäß dem angegebenen lokalisierungsabhängigen Funktionsnamen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| localName | java.lang.String | Lokalisierungsabhängiger Funktionsname. Das Gebietsschema wurde vom Arbeitsbuch angegeben, für das diese Einstellung verwendet wird. |

**Returns:**
java.lang.String - Standard(en-US-Locale) Funktionsname.
### getStandardHeaderFooterFontStyleName(String localfontStyleName) {#getStandardHeaderFooterFontStyleName-java.lang.String-}
```
public String getStandardHeaderFooterFontStyleName(String localfontStyleName)
```


Ermittelt den standardmäßigen englischen Schriftstilnamen (Regular, Bold, Italic) für Header/Footer gemäß dem angegebenen lokalisierungsabhängigen Schriftstilnamen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| localfontStyleName | java.lang.String | Locale Schriftstilname für Header/Footer. |

**Returns:**
java.lang.String - Standard-Englisch Schriftstilname (Regular, Bold, Italic)
### getSubTotalName(int subTotalType) {#getSubTotalName-int-}
```
public String getSubTotalName(int subTotalType)
```


Ermittelt den Namen des [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype)-Typs in der PivotTable.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Diese Eigenschaft wird 12 Monate später, seit Dezember 2022, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| subTotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). Der [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) Typ |

**Returns:**
java.lang.String - Der Name des [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) Typs
### getTableRowTypeOfAll() {#getTableRowTypeOfAll--}
```
public String getTableRowTypeOfAll()
```


Ermittelt den Typnamen der Tabellenzeilen, die alle Zeilen in der referenzierten Tabelle enthalten.

**Returns:**
java.lang.String - Der Typname der Tabellenzeilen
### getTableRowTypeOfCurrent() {#getTableRowTypeOfCurrent--}
```
public String getTableRowTypeOfCurrent()
```


Ermittelt den Typnamen der Tabellenzeilen, die die aktuelle Zeile in der referenzierten Tabelle enthalten.

**Returns:**
java.lang.String - Der Typname der Tabellenzeilen
### getTableRowTypeOfData() {#getTableRowTypeOfData--}
```
public String getTableRowTypeOfData()
```


Ruft den Typnamen der Tabellenzeilen ab, die aus dem Datenbereich der referenzierten Tabelle bestehen. Standard ist \"Data\", sodass in der Formel \"\\#Data\" der Datenbereich der Tabelle dargestellt wird.

**Returns:**
java.lang.String - Der Typname der Tabellenzeilen
### getTableRowTypeOfHeaders() {#getTableRowTypeOfHeaders--}
```
public String getTableRowTypeOfHeaders()
```


Ruft den Typnamen der Tabellenzeilen ab, die aus der Tabellenkopfzeile bestehen. Standard ist \"Headers\", sodass in der Formel \"\\#Headers\" die Tabellenkopfzeile dargestellt wird.

**Returns:**
java.lang.String - Der Typname der Tabellenzeilen
### getTableRowTypeOfTotals() {#getTableRowTypeOfTotals--}
```
public String getTableRowTypeOfTotals()
```


Ermittelt den Typnamen der Tabellenzeilen, die die Gesamtsummenzeile der referenzierten Tabelle enthalten.

**Returns:**
java.lang.String - Der Typname der Tabellenzeilen
### getTotalName(int functionType) {#getTotalName-int-}
```
public String getTotalName(int functionType)
```


Ermittelt den Gesamtnamen einer bestimmten Funktion.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| functionType | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). Der Funktionstyp. |

**Returns:**
java.lang.String - Der Gesamtname der Funktion.
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




### setBooleanValueString(boolean bv, String name) {#setBooleanValueString-boolean-java.lang.String-}
```
public void setBooleanValueString(boolean bv, String name)
```


Setzt den Anzeigestringwert für den booleschen Wert der Zelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| bv | boolean | boolescher Wert |
| Name | java.lang.String | Zeichenkettenwert des booleschen Werts |

### setChartSettings(ChartGlobalizationSettings value) {#setChartSettings-com.aspose.cells.ChartGlobalizationSettings-}
```
public void setChartSettings(ChartGlobalizationSettings value)
```


Setzt die Globalisierungseinstellungen für das Diagramm.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [ChartGlobalizationSettings](../../com.aspose.cells/chartglobalizationsettings) |  |

### setColumnSeparatorOfFormulaArray(char c) {#setColumnSeparatorOfFormulaArray-char-}
```
public void setColumnSeparatorOfFormulaArray(char c)
```


Legt das Trennzeichen für die Elemente in den Zeilendaten des Arrays in der Formel fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| c | char | der angegebene Trenner |

### setCommentTitleName(int type, String name) {#setCommentTitleName-int-java.lang.String-}
```
public void setCommentTitleName(int type, String name)
```


Liefert den lokalisierungsabhängigen Kommentar‑Titelnamen gemäß dem Typ des Kommentar‑Titels.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| type | int | [CommentTitleType](../../com.aspose.cells/commenttitletype). Typ des Kommentar-Titels |
| Name | java.lang.String | lokalisierungsabhängiger Kommentar-Titelname |

### setGrandTotalName(int functionType, String name) {#setGrandTotalName-int-java.lang.String-}
```
public void setGrandTotalName(int functionType, String name)
```


Legt den Namen des Gesamtsummens für eine bestimmte Funktion fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| functionType | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). Der Funktionstyp. |
| Name | java.lang.String | Der Gesamtsummenname der Funktion. |

### setListSeparator(char c) {#setListSeparator-char-}
```
public void setListSeparator(char c)
```


Legt das Trennzeichen für Listen, Funktionsparameter, ... usw. fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| c | char | der angegebene Trenner |

### setLocalBuiltInName(String standardName, String localName, boolean bidirectional) {#setLocalBuiltInName-java.lang.String-java.lang.String-boolean-}
```
public void setLocalBuiltInName(String standardName, String localName, boolean bidirectional)
```


Legt den lokalisierungsabhängigen Text für den integrierten Namen mit dem angegebenen Standardnamen fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| standardName | java.lang.String | Standard (en-US-Locale) Namens-Text des integrierten Namens. |
| localName | java.lang.String | Lokalisierungsabhängiger Namens-Text |
| bidirectional | boolean | Ob der lokale Namens-Text automatisch auf den Standard-Name-Text abgebildet wird. Falls true, wird der lokale Namens-Text automatisch auf den Standard-Name-Text abgebildet, sodass der Benutzer nicht erneut [setStandardBuiltInName(String,String,boolean)](../../com.aspose.cells/settableglobalizationsettings\#setStandardBuiltInName-String-String-boolean-) für dasselbe Standard‑ und lokale Namenspaar aufrufen muss. |

### setLocalFunctionName(String standardName, String localName, boolean bidirectional) {#setLocalFunctionName-java.lang.String-java.lang.String-boolean-}
```
public void setLocalFunctionName(String standardName, String localName, boolean bidirectional)
```


Legt den lokalisierungsabhängigen Funktionsnamen fest, der dem angegebenen Standardfunktionsnamen entspricht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| standardName | java.lang.String | Standard(en-US locale) Funktionsname. |
| localName | java.lang.String | Lokalisierungsabhängiger Funktionsname |
| bidirectional | boolean | Ob der lokale Funktionsname automatisch auf den Standard‑Funktionsnamen abgebildet wird. Falls true, wird der lokale Name automatisch auf den Standard‑Namen abgebildet, sodass der Benutzer nicht erneut [setStandardFunctionName(String,String,boolean)](../../com.aspose.cells/settableglobalizationsettings\#setStandardFunctionName-String-String-boolean-) für dasselbe Standard‑ und lokale Namenspaar aufrufen muss. |

### setPivotSettings(PivotGlobalizationSettings value) {#setPivotSettings-com.aspose.cells.PivotGlobalizationSettings-}
```
public void setPivotSettings(PivotGlobalizationSettings value)
```


Legt die Globalisierungseinstellungen für die Pivot-Tabelle fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings) |  |

### setRowSeparatorOfFormulaArray(char c) {#setRowSeparatorOfFormulaArray-char-}
```
public void setRowSeparatorOfFormulaArray(char c)
```


Legt das Trennzeichen für Zeilen in den Array-Daten in der Formel fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| c | char | der angegebene Trenner |

### setStandardBuiltInName(String localName, String standardName, boolean bidirectional) {#setStandardBuiltInName-java.lang.String-java.lang.String-boolean-}
```
public void setStandardBuiltInName(String localName, String standardName, boolean bidirectional)
```


Legt den lokalisierungsabhängigen Funktionsnamen gemäß dem angegebenen Standardfunktionsnamen fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| localName | java.lang.String | Lokalisierungsabhängiger Funktionsname |
| standardName | java.lang.String | Standard(en-US locale) Funktionsname. |
| bidirectional | boolean | Ob der Standard‑Namens‑Text automatisch auf den lokalen Namens‑Text abgebildet wird. Falls true, wird der Standard‑Namens‑Text automatisch auf den lokalen Namens‑Text abgebildet, sodass der Benutzer nicht erneut [setLocalBuiltInName(String,String,boolean)](../../com.aspose.cells/settableglobalizationsettings\#setLocalBuiltInName-String-String-boolean-) für dasselbe Standard‑ und lokale Namenspaar aufrufen muss. |

### setStandardFunctionName(String localName, String standardName, boolean bidirectional) {#setStandardFunctionName-java.lang.String-java.lang.String-boolean-}
```
public void setStandardFunctionName(String localName, String standardName, boolean bidirectional)
```


Legt den lokalisierungsabhängigen Funktionsnamen gemäß dem angegebenen Standardfunktionsnamen fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| localName | java.lang.String | Lokalisierungsabhängiger Funktionsname |
| standardName | java.lang.String | Standard(en-US locale) Funktionsname. |
| bidirectional | boolean | Ob der Standard‑Funktionsname automatisch auf den lokalen Funktionsnamen abgebildet wird. Falls true, wird der Standard‑Name automatisch auf den lokalen Namen abgebildet, sodass der Benutzer nicht erneut [setLocalFunctionName(String,String,boolean)](../../com.aspose.cells/settableglobalizationsettings\#setLocalFunctionName-String-String-boolean-) für dasselbe Standard‑ und lokale Namenspaar aufrufen muss. |

### setStandardHeaderFooterFontStyleName(String localfontStyleName, String standardName) {#setStandardHeaderFooterFontStyleName-java.lang.String-java.lang.String-}
```
public void setStandardHeaderFooterFontStyleName(String localfontStyleName, String standardName)
```


Legt den lokalisierungsabhängigen Funktionsnamen gemäß dem angegebenen Standardfunktionsnamen fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| localfontStyleName | java.lang.String | Locale Schriftstilname für Header/Footer. |
| standardName | java.lang.String | Standard(en-US locale) Funktionsname. |

### setTableRowTypeOfAll(String name) {#setTableRowTypeOfAll-java.lang.String-}
```
public void setTableRowTypeOfAll(String name)
```


Legt den Typnamen für Tabellenzeilen fest, die alle Zeilen in der referenzierten Tabelle enthalten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | der Typname der Tabellenzeilen |

### setTableRowTypeOfCurrent(String name) {#setTableRowTypeOfCurrent-java.lang.String-}
```
public void setTableRowTypeOfCurrent(String name)
```


Legt den Typnamen für Tabellenzeilen fest, die die aktuelle Zeile in der referenzierten Tabelle enthalten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | der Typname der Tabellenzeilen |

### setTableRowTypeOfData(String name) {#setTableRowTypeOfData-java.lang.String-}
```
public void setTableRowTypeOfData(String name)
```


Legt den Typnamen für Tabellenzeilen fest, die den Datenbereich der referenzierten Tabelle enthalten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | der Typname der Tabellenzeilen |

### setTableRowTypeOfHeaders(String name) {#setTableRowTypeOfHeaders-java.lang.String-}
```
public void setTableRowTypeOfHeaders(String name)
```


Legt den Typnamen für Tabellenzeilen fest, die die Tabellenüberschrift enthalten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | der Typname der Tabellenzeilen |

### setTableRowTypeOfTotals(String name) {#setTableRowTypeOfTotals-java.lang.String-}
```
public void setTableRowTypeOfTotals(String name)
```


Legt den Typnamen für Tabellenzeilen fest, die die Gesamtsumme‑Zeile der referenzierten Tabelle enthalten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | der Typname der Tabellenzeilen |

### setTotalName(int functionType, String name) {#setTotalName-int-java.lang.String-}
```
public void setTotalName(int functionType, String name)
```


Legt den Namen der Gesamtsumme für eine bestimmte Funktion fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| functionType | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). Der Funktionstyp. |
| Name | java.lang.String | Der Gesamtname der Funktion. |

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

