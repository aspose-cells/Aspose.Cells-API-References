---
title: "GridTxtLoadOptions"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Optionen zum Laden einer Textdatei dar."
type: docs
url: /de/java/com.aspose.gridweb/gridtxtloadoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.GridLoadOptions](../../com.aspose.gridweb/gridloadoptions)
```
public class GridTxtLoadOptions extends GridLoadOptions
```

Stellt die Optionen zum Laden einer Textdatei dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [GridTxtLoadOptions()](#GridTxtLoadOptions--) | Erstellt die Optionen zum Laden einer Textdatei. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | Gibt an, ob die Daten beim Laden der Dateien automatisch gefiltert werden. |
| [getCheckDataValid()](#getCheckDataValid--) | Prüft, ob die Daten in der Vorlagendatei gültig sind. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Ob Einschränkungen der Excel‑Datei geprüft werden, wenn der Benutzer zellenbezogene Objekte ändert. |
| [getClass()](#getClass--) |  |
| [getConvertDateTimeData()](#getConvertDateTimeData--) | Ruft einen Wert ab, der angibt, ob die Zeichenkette in der Textdatei in Datumsdaten konvertiert wird. |
| [getConvertNumericData()](#getConvertNumericData--) | Ruft einen Wert ab, der angibt, ob die Zeichenkette in der Textdatei in numerische Daten konvertiert wird. |
| [getEncoding()](#getEncoding--) | Ruft die Standardkodierung ab. |
| [getExtendToNextSheet()](#getExtendToNextSheet--) | Ob Daten auf das nächste Blatt erweitert werden, wenn die Zeilen- oder Spaltenanzahl das Limit überschreitet. |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | Ignoriert die Daten, die nicht gedruckt werden, wenn die Datei direkt gedruckt wird |
| [getKeepPrecision()](#getKeepPrecision--) | Gibt an, ob ein Zeichenkettenwert nicht geparst wird, wenn die Länge 15 beträgt. |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | Ob nicht geparste Daten im Speicher für die Arbeitsmappe behalten werden, wenn sie aus einer Vorlagendatei geladen wird. |
| [getOnlyAuto()](#getOnlyAuto--) | Gibt an, ob nur die Zeilen angepasst werden, deren Höhe nicht benutzerdefiniert ist. |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | Gibt an, ob Formeln beim Lesen der Datei geparst werden. |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | Gibt an, ob Pivot‑Cache‑Datensätze beim Laden der Datei geparst werden. |
| [getPassword()](#getPassword--) | Liest das Passwort der Arbeitsmappe. |
| [getPreservePaddingSpacesInFormula()](#getPreservePaddingSpacesInFormula--) | Gibt an, ob die zwischen Formel‑Token eingefügten Leerzeichen und Zeilenumbrüche beim Abrufen und Setzen von Formeln erhalten bleiben. |
| [getSeparator()](#getSeparator--) | Liest das Zeichen-Trennzeichen der Textdatei aus. |
| [getSeparatorString()](#getSeparatorString--) | Liest einen Zeichenkettenwert als Trennzeichen aus. |
| [getTextQualifier()](#getTextQualifier--) | Gibt den Textqualifizierer für Zellwerte an. |
| [getTreatConsecutiveDelimitersAsOne()](#getTreatConsecutiveDelimitersAsOne--) | Ob aufeinanderfolgende Trennzeichen als eines behandelt werden sollen. |
| [getTreatQuotePrefixAsValue()](#getTreatQuotePrefixAsValue--) | Gibt an, ob das führende einfache Anführungszeichen als Teil des Wertes einer Zelle betrachtet werden soll. |
| [hasFormula()](#hasFormula--) | Gibt an, ob der Text eine Formel ist, wenn er mit "=" beginnt. |
| [hasTextQualifier()](#hasTextQualifier--) | Ob ein Textqualifizierer für den Zellwert vorhanden ist. |
| [hashCode()](#hashCode--) |  |
| [isMultiEncoded()](#isMultiEncoded--) | True bedeutet, dass die Datei mehrere Codierungen enthält. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | Gibt an, ob die Daten beim Laden der Dateien automatisch gefiltert werden. |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | Prüft, ob die Daten in der Vorlagendatei gültig sind. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Ob Einschränkungen der Excel‑Datei geprüft werden, wenn der Benutzer zellenbezogene Objekte ändert. |
| [setConvertDateTimeData(boolean value)](#setConvertDateTimeData-boolean-) | Legt einen Wert fest, der angibt, ob die Zeichenkette in der Textdatei in Datumsdaten konvertiert wird. |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | Legt einen Wert fest, der angibt, ob die Zeichenkette in der Textdatei in numerische Daten konvertiert wird. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.gridweb.Encoding-) | Legt die Standardkodierung fest. |
| [setExtendToNextSheet(boolean value)](#setExtendToNextSheet-boolean-) | Ob Daten auf das nächste Blatt erweitert werden, wenn die Zeilen- oder Spaltenanzahl das Limit überschreitet. |
| [setHasFormula(boolean value)](#setHasFormula-boolean-) | Gibt an, ob der Text eine Formel ist, wenn er mit "=" beginnt. |
| [setHasTextQualifier(boolean value)](#setHasTextQualifier-boolean-) | Ob ein Textqualifizierer für den Zellwert vorhanden ist. |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | Ignoriert die Daten, die nicht gedruckt werden, wenn die Datei direkt gedruckt wird |
| [setKeepPrecision(boolean value)](#setKeepPrecision-boolean-) | Gibt an, ob ein Zeichenkettenwert nicht geparst wird, wenn die Länge 15 beträgt. |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | Ob nicht geparste Daten im Speicher für die Arbeitsmappe behalten werden, wenn sie aus einer Vorlagendatei geladen wird. |
| [setMultiEncoded(boolean value)](#setMultiEncoded-boolean-) | True bedeutet, dass die Datei mehrere Codierungen enthält. |
| [setOnlyAuto(boolean value)](#setOnlyAuto-boolean-) | Gibt an, ob nur die Zeilen angepasst werden, deren Höhe nicht benutzerdefiniert ist. |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | Gibt an, ob Formeln beim Lesen der Datei geparst werden. |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | Gibt an, ob Pivot‑Cache‑Datensätze beim Laden der Datei geparst werden. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Legt das Passwort der Arbeitsmappe fest. |
| [setPreservePaddingSpacesInFormula(boolean value)](#setPreservePaddingSpacesInFormula-boolean-) | Gibt an, ob die zwischen Formel‑Token eingefügten Leerzeichen und Zeilenumbrüche beim Abrufen und Setzen von Formeln erhalten bleiben. |
| [setSeparator(char value)](#setSeparator-char-) | Legt das Zeichentrennzeichen der Textdatei fest. |
| [setSeparatorString(String value)](#setSeparatorString-java.lang.String-) | Legt einen Zeichenkettenwert als Trennzeichen fest. |
| [setTextQualifier(char value)](#setTextQualifier-char-) | Gibt den Textqualifizierer für Zellwerte an. |
| [setTreatConsecutiveDelimitersAsOne(boolean value)](#setTreatConsecutiveDelimitersAsOne-boolean-) | Ob aufeinanderfolgende Trennzeichen als eines behandelt werden sollen. |
| [setTreatQuotePrefixAsValue(boolean value)](#setTreatQuotePrefixAsValue-boolean-) | Gibt an, ob das führende einfache Anführungszeichen als Teil des Wertes einer Zelle betrachtet werden soll. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridTxtLoadOptions() {#GridTxtLoadOptions--}
```
public GridTxtLoadOptions()
```


Erstellt die Optionen zum Laden einer Textdatei.

**Remarks**

Der Standard-Ladetyp ist CSV.

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
### getAutoFilter() {#getAutoFilter--}
```
public boolean getAutoFilter()
```


Gibt an, ob die Daten beim Laden der Dateien automatisch gefiltert werden.

**Remarks**

Manchmal werden, obwohl der AutoFilter gesetzt ist, die entsprechenden Zeilen in der Datei nicht ausgeblendet. Jetzt funktioniert es nur für SpreadSheetML‑Dateien.

**Returns:**
boolean
### getCheckDataValid() {#getCheckDataValid--}
```
public boolean getCheckDataValid()
```


Prüft, ob die Daten in der Vorlagendatei gültig sind.

**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Ob die Beschränkungen der Excel‑Datei überprüft werden, wenn der Benutzer zellbezogene Objekte ändert. Zum Beispiel erlaubt Excel nicht das Eingeben eines Zeichenkettenwertes, der länger als 32 KB ist. Wenn Sie einen Wert länger als 32 KB, etwa über Cell.PutValue(string), eingeben und diese Eigenschaft true ist, erhalten Sie eine Ausnahme. Ist die Eigenschaft false, akzeptieren wir den eingegebenen Zeichenkettenwert als Zellenwert, sodass Sie später den vollständigen Zeichenkettenwert für andere Dateiformate wie CSV ausgeben können. Wenn Sie jedoch einen Wert festgelegt haben, der für das Excel‑Dateiformat ungültig ist, sollten Sie die Arbeitsmappe später nicht im Excel‑Format speichern. Andernfalls kann es zu unerwarteten Fehlern in der erzeugten Excel‑Datei kommen.

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


Ruft einen Wert ab, der angibt, ob die Zeichenkette in der Textdatei in Datumsdaten konvertiert wird.

**Returns:**
boolean
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```


Ruft einen Wert ab, der angibt, ob die Zeichenkette in der Textdatei in numerische Daten konvertiert wird.

**Returns:**
boolean
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Ruft die Standardkodierung ab. Gilt nur für CSV‑Dateien.

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding)
### getExtendToNextSheet() {#getExtendToNextSheet--}
```
public boolean getExtendToNextSheet()
```


Ob Daten auf das nächste Blatt erweitert werden, wenn die Zeilen oder Spalten die Grenze überschreiten. Ist diese Eigenschaft true, werden zusätzliche Daten auf das nächste Blatt hinter dem aktuellen Blatt erweitert (wenn das aktuelle Blatt das letzte ist, wird ein neues Blatt an die aktuelle Arbeitsmappe angehängt). Ist diese Eigenschaft false, werden die die Grenze überschreitenden Daten ignoriert. Default ist false;

**Returns:**
boolean
### getIgnoreNotPrinted() {#getIgnoreNotPrinted--}
```
public boolean getIgnoreNotPrinted()
```


Ignoriert die Daten, die nicht gedruckt werden, wenn die Datei direkt gedruckt wird

**Remarks**

Nur für xlsx‑Dateien.

**Returns:**
boolean
### getKeepPrecision() {#getKeepPrecision--}
```
public boolean getKeepPrecision()
```


Gibt an, ob ein Zeichenkettenwert nicht geparst wird, wenn die Länge 15 beträgt.

**Returns:**
boolean
### getKeepUnparsedData() {#getKeepUnparsedData--}
```
public boolean getKeepUnparsedData()
```


Ob die nicht geparsten Daten im Speicher für die Arbeitsmappe behalten werden, wenn sie aus einer Vorlagendatei geladen wird. Standard ist true.

**Remarks**

Für Szenarien, in denen der Benutzer nur Inhalte aus einer Vorlagendatei lesen muss und die Arbeitsmappe nicht zurückspeichern muss, kann das Setzen dieser Eigenschaft auf false die Leistung verbessern, insbesondere in Kombination mit einer Art LoadFilter.

**Returns:**
boolean
### getOnlyAuto() {#getOnlyAuto--}
```
public boolean getOnlyAuto()
```


Gibt an, ob nur die Zeilen angepasst werden, deren Höhe nicht benutzerdefiniert ist.

**Returns:**
boolean
### getParsingFormulaOnOpen() {#getParsingFormulaOnOpen--}
```
public boolean getParsingFormulaOnOpen()
```


Gibt an, ob Formeln beim Lesen der Datei geparst werden.

**Remarks**

Gilt nur für Excel‑Dateien Xlsx, Xltx, Xltm und Xlsm, weil die Formeln in den Dateien als Zeichenkettenformel gespeichert werden.

**Returns:**
boolean
### getParsingPivotCachedRecords() {#getParsingPivotCachedRecords--}
```
public boolean getParsingPivotCachedRecords()
```


Gibt an, ob beim Laden der Datei Pivot‑Cache‑Datensätze geparst werden. Der Standardwert ist false.

**Remarks**

Gilt nur für Excel‑Dateien Xlsx, Xltx, Xltm, Xlsm und xlsb.

**Returns:**
boolean
### getPassword() {#getPassword--}
```
public String getPassword()
```


Liest das Passwort der Arbeitsmappe.

**Returns:**
java.lang.String
### getPreservePaddingSpacesInFormula() {#getPreservePaddingSpacesInFormula--}
```
public boolean getPreservePaddingSpacesInFormula()
```


Gibt an, ob die zwischen Formel‑Token eingefügten Leerzeichen und Zeilenumbrüche beim Lesen und Schreiben von Formeln beibehalten werden sollen. Der Standardwert ist false.

**Remarks**

Nach dem Laden einer Arbeitsmappe aus einer Vorlagendatei mit dieser Option wird [GridWorkbookSettings.getPreservePaddingSpaces()](../../com.aspose.gridweb/gridworkbooksettings\\#getPreservePaddingSpaces--) auf denselben Wert wie diese Eigenschaft gesetzt.

**Returns:**
boolean
### getSeparator() {#getSeparator--}
```
public char getSeparator()
```


Liest das Zeichen-Trennzeichen der Textdatei aus.

**Returns:**
char
### getSeparatorString() {#getSeparatorString--}
```
public String getSeparatorString()
```


Liest einen Zeichenkettenwert als Trennzeichen aus.

**Returns:**
java.lang.String
### getTextQualifier() {#getTextQualifier--}
```
public char getTextQualifier()
```


Gibt den Textqualifizierer für Zellwerte an. Der Standard‑Qualifizierer ist '\"'.

**Remarks**

Beim Setzen dieser Eigenschaft wird [hasTextQualifier()](../../com.aspose.gridweb/gridtxtloadoptions\#hasTextQualifier--) automatisch auf true gesetzt.

**Returns:**
char
### getTreatConsecutiveDelimitersAsOne() {#getTreatConsecutiveDelimitersAsOne--}
```
public boolean getTreatConsecutiveDelimitersAsOne()
```


Ob aufeinanderfolgende Trennzeichen als eines behandelt werden sollen.

**Returns:**
boolean
### getTreatQuotePrefixAsValue() {#getTreatQuotePrefixAsValue--}
```
public boolean getTreatQuotePrefixAsValue()
```


Gibt an, ob das führende einfache Anführungszeichen als Teil des Zellwertes betrachtet werden soll. Default ist true. Ist es false, wird das führende einfache Anführungszeichen aus dem entsprechenden Zellwert entfernt und [GridTableItemStyle.getQuotePrefix()](../../com.aspose.gridweb/gridtableitemstyle\#getQuotePrefix--) wird für die Zelle auf true gesetzt.

**Returns:**
boolean
### hasFormula() {#hasFormula--}
```
public boolean hasFormula()
```


Gibt an, ob der Text eine Formel ist, wenn er mit "=" beginnt.

**Returns:**
boolean
### hasTextQualifier() {#hasTextQualifier--}
```
public boolean hasTextQualifier()
```


Ob es einen Textqualifizierer für den Zellenwert gibt. Standard ist true.

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


True bedeutet, dass die Datei mehrere Codierungen enthält.

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


Gibt an, ob die Daten beim Laden der Dateien automatisch gefiltert werden.

**Remarks**

Manchmal werden, obwohl der AutoFilter gesetzt ist, die entsprechenden Zeilen in der Datei nicht ausgeblendet. Jetzt funktioniert es nur für SpreadSheetML‑Dateien.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setCheckDataValid(boolean value) {#setCheckDataValid-boolean-}
```
public void setCheckDataValid(boolean value)
```


Prüft, ob die Daten in der Vorlagendatei gültig sind.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Ob die Beschränkungen der Excel‑Datei überprüft werden, wenn der Benutzer zellbezogene Objekte ändert. Zum Beispiel erlaubt Excel nicht das Eingeben eines Zeichenkettenwertes, der länger als 32 KB ist. Wenn Sie einen Wert länger als 32 KB, etwa über Cell.PutValue(string), eingeben und diese Eigenschaft true ist, erhalten Sie eine Ausnahme. Ist die Eigenschaft false, akzeptieren wir den eingegebenen Zeichenkettenwert als Zellenwert, sodass Sie später den vollständigen Zeichenkettenwert für andere Dateiformate wie CSV ausgeben können. Wenn Sie jedoch einen Wert festgelegt haben, der für das Excel‑Dateiformat ungültig ist, sollten Sie die Arbeitsmappe später nicht im Excel‑Format speichern. Andernfalls kann es zu unerwarteten Fehlern in der erzeugten Excel‑Datei kommen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setConvertDateTimeData(boolean value) {#setConvertDateTimeData-boolean-}
```
public void setConvertDateTimeData(boolean value)
```


Legt einen Wert fest, der angibt, ob die Zeichenkette in der Textdatei in Datumsdaten konvertiert wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


Legt einen Wert fest, der angibt, ob die Zeichenkette in der Textdatei in numerische Daten konvertiert wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.gridweb.Encoding-}
```
public void setEncoding(Encoding value)
```


Legt die Standardkodierung fest. Gilt nur für CSV‑Dateien.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.gridweb/encoding) |  |

### setExtendToNextSheet(boolean value) {#setExtendToNextSheet-boolean-}
```
public void setExtendToNextSheet(boolean value)
```


Ob Daten auf das nächste Blatt erweitert werden, wenn die Zeilen oder Spalten die Grenze überschreiten. Ist diese Eigenschaft true, werden zusätzliche Daten auf das nächste Blatt hinter dem aktuellen Blatt erweitert (wenn das aktuelle Blatt das letzte ist, wird ein neues Blatt an die aktuelle Arbeitsmappe angehängt). Ist diese Eigenschaft false, werden die die Grenze überschreitenden Daten ignoriert. Default ist false;

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setHasFormula(boolean value) {#setHasFormula-boolean-}
```
public void setHasFormula(boolean value)
```


Gibt an, ob der Text eine Formel ist, wenn er mit "=" beginnt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setHasTextQualifier(boolean value) {#setHasTextQualifier-boolean-}
```
public void setHasTextQualifier(boolean value)
```


Ob es einen Textqualifizierer für den Zellenwert gibt. Standard ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setIgnoreNotPrinted(boolean value) {#setIgnoreNotPrinted-boolean-}
```
public void setIgnoreNotPrinted(boolean value)
```


Ignoriert die Daten, die nicht gedruckt werden, wenn die Datei direkt gedruckt wird

**Remarks**

Nur für xlsx‑Dateien.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setKeepPrecision(boolean value) {#setKeepPrecision-boolean-}
```
public void setKeepPrecision(boolean value)
```


Gibt an, ob ein Zeichenkettenwert nicht geparst wird, wenn die Länge 15 beträgt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setKeepUnparsedData(boolean value) {#setKeepUnparsedData-boolean-}
```
public void setKeepUnparsedData(boolean value)
```


Ob die nicht geparsten Daten im Speicher für die Arbeitsmappe behalten werden, wenn sie aus einer Vorlagendatei geladen wird. Standard ist true.

**Remarks**

Für Szenarien, in denen der Benutzer nur Inhalte aus einer Vorlagendatei lesen muss und die Arbeitsmappe nicht zurückspeichern muss, kann das Setzen dieser Eigenschaft auf false die Leistung verbessern, insbesondere in Kombination mit einer Art LoadFilter.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setMultiEncoded(boolean value) {#setMultiEncoded-boolean-}
```
public void setMultiEncoded(boolean value)
```


True bedeutet, dass die Datei mehrere Codierungen enthält.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setOnlyAuto(boolean value) {#setOnlyAuto-boolean-}
```
public void setOnlyAuto(boolean value)
```


Gibt an, ob nur die Zeilen angepasst werden, deren Höhe nicht benutzerdefiniert ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setParsingFormulaOnOpen(boolean value) {#setParsingFormulaOnOpen-boolean-}
```
public void setParsingFormulaOnOpen(boolean value)
```


Gibt an, ob Formeln beim Lesen der Datei geparst werden.

**Remarks**

Gilt nur für Excel‑Dateien Xlsx, Xltx, Xltm und Xlsm, weil die Formeln in den Dateien als Zeichenkettenformel gespeichert werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setParsingPivotCachedRecords(boolean value) {#setParsingPivotCachedRecords-boolean-}
```
public void setParsingPivotCachedRecords(boolean value)
```


Gibt an, ob beim Laden der Datei Pivot‑Cache‑Datensätze geparst werden. Der Standardwert ist false.

**Remarks**

Gilt nur für Excel‑Dateien Xlsx, Xltx, Xltm, Xlsm und xlsb.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


Legt das Passwort der Arbeitsmappe fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setPreservePaddingSpacesInFormula(boolean value) {#setPreservePaddingSpacesInFormula-boolean-}
```
public void setPreservePaddingSpacesInFormula(boolean value)
```


Gibt an, ob die zwischen Formel‑Token eingefügten Leerzeichen und Zeilenumbrüche beim Lesen und Schreiben von Formeln beibehalten werden sollen. Der Standardwert ist false.

**Remarks**

Nach dem Laden einer Arbeitsmappe aus einer Vorlagendatei mit dieser Option wird [GridWorkbookSettings.getPreservePaddingSpaces()](../../com.aspose.gridweb/gridworkbooksettings\\#getPreservePaddingSpaces--) auf denselben Wert wie diese Eigenschaft gesetzt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSeparator(char value) {#setSeparator-char-}
```
public void setSeparator(char value)
```


Legt das Zeichentrennzeichen der Textdatei fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | char |  |

### setSeparatorString(String value) {#setSeparatorString-java.lang.String-}
```
public void setSeparatorString(String value)
```


Legt einen Zeichenkettenwert als Trennzeichen fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setTextQualifier(char value) {#setTextQualifier-char-}
```
public void setTextQualifier(char value)
```


Gibt den Textqualifizierer für Zellwerte an. Der Standard‑Qualifizierer ist '\"'.

**Remarks**

Beim Setzen dieser Eigenschaft wird [hasTextQualifier()](../../com.aspose.gridweb/gridtxtloadoptions\#hasTextQualifier--) automatisch auf true gesetzt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | char |  |

### setTreatConsecutiveDelimitersAsOne(boolean value) {#setTreatConsecutiveDelimitersAsOne-boolean-}
```
public void setTreatConsecutiveDelimitersAsOne(boolean value)
```


Ob aufeinanderfolgende Trennzeichen als eines behandelt werden sollen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setTreatQuotePrefixAsValue(boolean value) {#setTreatQuotePrefixAsValue-boolean-}
```
public void setTreatQuotePrefixAsValue(boolean value)
```


Gibt an, ob das führende einfache Anführungszeichen als Teil des Zellwertes betrachtet werden soll. Default ist true. Ist es false, wird das führende einfache Anführungszeichen aus dem entsprechenden Zellwert entfernt und [GridTableItemStyle.getQuotePrefix()](../../com.aspose.gridweb/gridtableitemstyle\#getQuotePrefix--) wird für die Zelle auf true gesetzt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

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

