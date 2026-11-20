---
title: "TxtLoadOptions"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Optionen zum Laden einer Textdatei dar."
type: docs
url: /de/java/com.aspose.cells/txtloadoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LoadOptions](../../com.aspose.cells/loadoptions), [com.aspose.cells.AbstractTextLoadOptions](../../com.aspose.cells/abstracttextloadoptions)
```
public class TxtLoadOptions extends AbstractTextLoadOptions
```

Stellt die Optionen zum Laden einer Textdatei dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [TxtLoadOptions()](#TxtLoadOptions--) | Erstellt die Optionen zum Laden einer Textdatei. |
| [TxtLoadOptions(int loadFormat)](#TxtLoadOptions-int-) | Erstellt die Optionen zum Laden einer Textdatei. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | Gibt an, ob die Daten beim Laden der Dateien automatisch gefiltert werden. |
| [getAutoFitterOptions()](#getAutoFitterOptions--) | Ermittelt die Auto‑Fit‑Optionen |
| [getCheckDataValid()](#getCheckDataValid--) | Prüft, ob die Daten in der Vorlagendatei gültig sind. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Ob Einschränkungen der Excel‑Datei geprüft werden, wenn der Benutzer zellenbezogene Objekte ändert. |
| [getClass()](#getClass--) |  |
| [getConvertDateTimeData()](#getConvertDateTimeData--) | Ruft einen Wert ab, der angibt, ob die Zeichenkette in der Textdatei in Datumsdaten konvertiert wird. |
| [getConvertNumericData()](#getConvertNumericData--) | Ruft einen Wert ab, der angibt, ob die Zeichenkette in der Textdatei in numerische Daten konvertiert wird. |
| [getDefaultStyleSettings()](#getDefaultStyleSettings--) | Liest die Standard‑Stileinstellungen zum Initialisieren der Stile der Arbeitsmappe. |
| [getEncoding()](#getEncoding--) | Ruft die Standardkodierung ab. |
| [getExtendToNextSheet()](#getExtendToNextSheet--) | Ob Daten auf das nächste Blatt erweitert werden, wenn die Zeilen- oder Spaltenanzahl das Limit überschreitet. |
| [getFontConfigs()](#getFontConfigs--) | Liest einzelne Schriftartkonfigurationen. |
| [getHeaderColumnsCount()](#getHeaderColumnsCount--) | Die Anzahl der Kopfzeilen-Spalten, die für erweiterte Blätter wiederholt werden sollen. |
| [getHeaderRowsCount()](#getHeaderRowsCount--) | Die Anzahl der Kopfzeilen-Zeilen, die für erweiterte Blätter wiederholt werden sollen. |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | Ignoriert die Daten, die nicht gedruckt werden, wenn die Datei direkt gedruckt wird |
| [getIgnoreUselessShapes()](#getIgnoreUselessShapes--) | Gibt an, ob nutzlose Formen ignoriert werden. |
| [getInterruptMonitor()](#getInterruptMonitor--) | Liest den Unterbrechungsmonitor. |
| [getKeepPrecision()](#getKeepPrecision--) | Gibt an, ob ein Zeichenkettenwert nicht geparst wird, wenn die Länge 15 beträgt. |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | Ob nicht geparste Daten im Speicher für die Arbeitsmappe behalten werden, wenn sie aus einer Vorlagendatei geladen wird. |
| [getLanguageCode()](#getLanguageCode--) | Liest die Benutzerschnittstellensprache der Arbeitsmappen‑Version basierend auf dem Ländercode, unter dem die Datei gespeichert wurde. |
| [getLightCellsDataHandler()](#getLightCellsDataHandler--) | Der Datenhandler zur Verarbeitung von Zellen­daten beim Lesen der Vorlagendatei. |
| [getLoadFilter()](#getLoadFilter--) | Der Filter, der angibt, wie Daten geladen werden. |
| [getLoadFormat()](#getLoadFormat--) | Liest das Ladeformat. |
| [getLoadStyleStrategy()](#getLoadStyleStrategy--) | Gibt die Strategie an, mit der Stil für geparste Werte angewendet wird, wenn die Zeichenkette in eine Zahl oder ein Datum/Uhrzeit konvertiert wird. |
| [getLocale()](#getLocale--) | Liest die regionalen Einstellungen, die für die zu ladende Arbeitsmappe verwendet werden. |
| [getMaxColumnCount()](#getMaxColumnCount--) | Die maximale Anzahl von Spalten, die für ein Blatt importiert werden können. |
| [getMaxRowCount()](#getMaxRowCount--) | Die maximale Anzahl von Zeilen, die für ein Blatt importiert werden können. |
| [getMemorySetting()](#getMemorySetting--) | Liest den Speichermodus für die geladene Arbeitsmappe. |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | Gibt an, ob Formeln beim Lesen der Datei geparst werden. |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | Gibt an, ob Pivot‑Cache‑Datensätze beim Laden der Datei geparst werden. |
| [getPassword()](#getPassword--) | Liest das Passwort der Arbeitsmappe. |
| [getPreferredParsers()](#getPreferredParsers--) | Liest bevorzugte Wertparser zum Laden einer Textdatei aus. |
| [getPreservePaddingSpacesInFormula()](#getPreservePaddingSpacesInFormula--) | Gibt an, ob die zwischen Formel‑Token eingefügten Leerzeichen und Zeilenumbrüche beim Abrufen und Setzen von Formeln erhalten bleiben. |
| [getRegion()](#getRegion--) | Liest die regionalen Einstellungen, die für die zu ladende Arbeitsmappe verwendet werden. |
| [getSeparator()](#getSeparator--) | Liest das Zeichen-Trennzeichen der Textdatei aus. |
| [getSeparatorString()](#getSeparatorString--) | Liest einen Zeichenkettenwert als Trennzeichen aus. |
| [getStandardFont()](#getStandardFont--) | Setzt den Standard‑Schriftartnamen. |
| [getStandardFontSize()](#getStandardFontSize--) | Setzt die Standard‑Schriftgröße. |
| [getTextQualifier()](#getTextQualifier--) | Gibt den Textqualifizierer für Zellwerte an. |
| [getTreatConsecutiveDelimitersAsOne()](#getTreatConsecutiveDelimitersAsOne--) | Ob aufeinanderfolgende Trennzeichen als eines behandelt werden sollen. |
| [getTreatQuotePrefixAsValue()](#getTreatQuotePrefixAsValue--) | Gibt an, ob das führende einfache Anführungszeichen als Teil des Wertes einer Zelle betrachtet werden soll. |
| [getWarningCallback()](#getWarningCallback--) | Liest den Warn‑Callback. |
| [hasFormula()](#hasFormula--) | Gibt an, ob der Text eine Formel ist, wenn er mit "=" beginnt. |
| [hasTextQualifier()](#hasTextQualifier--) | Ob ein Textqualifizierer für den Zellwert vorhanden ist. |
| [hashCode()](#hashCode--) |  |
| [isMultiEncoded()](#isMultiEncoded--) | True bedeutet, dass die Datei mehrere Codierungen enthält. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | Gibt an, ob die Daten beim Laden der Dateien automatisch gefiltert werden. |
| [setAutoFitterOptions(AutoFitterOptions value)](#setAutoFitterOptions-com.aspose.cells.AutoFitterOptions-) | Setzt die Auto‑Fit‑Optionen |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | Prüft, ob die Daten in der Vorlagendatei gültig sind. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Ob Einschränkungen der Excel‑Datei geprüft werden, wenn der Benutzer zellenbezogene Objekte ändert. |
| [setConvertDateTimeData(boolean value)](#setConvertDateTimeData-boolean-) | Legt einen Wert fest, der angibt, ob die Zeichenkette in der Textdatei in Datumsdaten konvertiert wird. |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | Legt einen Wert fest, der angibt, ob die Zeichenkette in der Textdatei in numerische Daten konvertiert wird. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | Legt die Standardkodierung fest. |
| [setExtendToNextSheet(boolean value)](#setExtendToNextSheet-boolean-) | Ob Daten auf das nächste Blatt erweitert werden, wenn die Zeilen- oder Spaltenanzahl das Limit überschreitet. |
| [setFontConfigs(IndividualFontConfigs value)](#setFontConfigs-com.aspose.cells.IndividualFontConfigs-) | Legt einzelne Schriftartkonfigurationen fest. |
| [setHasFormula(boolean value)](#setHasFormula-boolean-) | Gibt an, ob der Text eine Formel ist, wenn er mit "=" beginnt. |
| [setHasTextQualifier(boolean value)](#setHasTextQualifier-boolean-) | Ob ein Textqualifizierer für den Zellwert vorhanden ist. |
| [setHeaderColumnsCount(int value)](#setHeaderColumnsCount-int-) | Die Anzahl der Kopfzeilen-Spalten, die für erweiterte Blätter wiederholt werden sollen. |
| [setHeaderRowsCount(int value)](#setHeaderRowsCount-int-) | Die Anzahl der Kopfzeilen-Zeilen, die für erweiterte Blätter wiederholt werden sollen. |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | Ignoriert die Daten, die nicht gedruckt werden, wenn die Datei direkt gedruckt wird |
| [setIgnoreUselessShapes(boolean value)](#setIgnoreUselessShapes-boolean-) | Gibt an, ob nutzlose Formen ignoriert werden. |
| [setInterruptMonitor(AbstractInterruptMonitor value)](#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-) | Legt den Interrupt‑Monitor fest. |
| [setKeepPrecision(boolean value)](#setKeepPrecision-boolean-) | Gibt an, ob ein Zeichenkettenwert nicht geparst wird, wenn die Länge 15 beträgt. |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | Ob nicht geparste Daten im Speicher für die Arbeitsmappe behalten werden, wenn sie aus einer Vorlagendatei geladen wird. |
| [setLanguageCode(int value)](#setLanguageCode-int-) | Legt die Sprache der Benutzeroberfläche der Arbeitsmappen‑Version basierend auf dem CountryCode fest, mit dem die Datei gespeichert wurde. |
| [setLightCellsDataHandler(LightCellsDataHandler value)](#setLightCellsDataHandler-com.aspose.cells.LightCellsDataHandler-) | Der Datenhandler zur Verarbeitung von Zellen­daten beim Lesen der Vorlagendatei. |
| [setLoadFilter(LoadFilter value)](#setLoadFilter-com.aspose.cells.LoadFilter-) | Der Filter, der angibt, wie Daten geladen werden. |
| [setLoadStyleStrategy(int value)](#setLoadStyleStrategy-int-) | Gibt die Strategie an, mit der Stil für geparste Werte angewendet wird, wenn die Zeichenkette in eine Zahl oder ein Datum/Uhrzeit konvertiert wird. |
| [setLocale(Locale value)](#setLocale-java.util.Locale-) | Legt die regionalen Einstellungen fest, die für die zu ladende Arbeitsmappe verwendet werden. |
| [setMaxColumnCount(int value)](#setMaxColumnCount-int-) | Die maximale Anzahl von Spalten, die für ein Blatt importiert werden können. |
| [setMaxRowCount(int value)](#setMaxRowCount-int-) | Die maximale Anzahl von Zeilen, die für ein Blatt importiert werden können. |
| [setMemorySetting(int value)](#setMemorySetting-int-) | Legt den Speichermodus für die geladene Arbeitsmappe fest. |
| [setMultiEncoded(boolean value)](#setMultiEncoded-boolean-) | True bedeutet, dass die Datei mehrere Codierungen enthält. |
| [setPaperSize(int type)](#setPaperSize-int-) | Legt die Standard‑Papiergröße für den Druck anhand der Einstellung des Standarddruckers fest. |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | Gibt an, ob Formeln beim Lesen der Datei geparst werden. |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | Gibt an, ob Pivot‑Cache‑Datensätze beim Laden der Datei geparst werden. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Legt das Passwort der Arbeitsmappe fest. |
| [setPreferredParsers(ICustomParser[] value)](#setPreferredParsers-com.aspose.cells.ICustomParser---) | Legt bevorzugte Wertparser zum Laden von Textdateien fest. |
| [setPreservePaddingSpacesInFormula(boolean value)](#setPreservePaddingSpacesInFormula-boolean-) | Gibt an, ob die zwischen Formel‑Token eingefügten Leerzeichen und Zeilenumbrüche beim Abrufen und Setzen von Formeln erhalten bleiben. |
| [setRegion(int value)](#setRegion-int-) | Legt die regionalen Einstellungen fest, die für die zu ladende Arbeitsmappe verwendet werden. |
| [setSeparator(char value)](#setSeparator-char-) | Legt das Zeichentrennzeichen der Textdatei fest. |
| [setSeparatorString(String value)](#setSeparatorString-java.lang.String-) | Legt einen Zeichenkettenwert als Trennzeichen fest. |
| [setStandardFont(String value)](#setStandardFont-java.lang.String-) | Setzt den Standard‑Schriftartnamen. |
| [setStandardFontSize(double value)](#setStandardFontSize-double-) | Setzt die Standard‑Schriftgröße. |
| [setTextQualifier(char value)](#setTextQualifier-char-) | Gibt den Textqualifizierer für Zellwerte an. |
| [setTreatConsecutiveDelimitersAsOne(boolean value)](#setTreatConsecutiveDelimitersAsOne-boolean-) | Ob aufeinanderfolgende Trennzeichen als eines behandelt werden sollen. |
| [setTreatQuotePrefixAsValue(boolean value)](#setTreatQuotePrefixAsValue-boolean-) | Gibt an, ob das führende einfache Anführungszeichen als Teil des Wertes einer Zelle betrachtet werden soll. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Legt die Warn‑Callback‑Funktion fest. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### TxtLoadOptions() {#TxtLoadOptions--}
```
public TxtLoadOptions()
```


Erstellt die Optionen zum Laden einer Textdatei.

**Remarks**

Der Standard-Ladetyp ist CSV.

### TxtLoadOptions(int loadFormat) {#TxtLoadOptions-int-}
```
public TxtLoadOptions(int loadFormat)
```


Erstellt die Optionen zum Laden einer Textdatei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| loadFormat | int | [LoadFormat](../../com.aspose.cells/loadformat). Das Ladeformat |

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
### getAutoFitterOptions() {#getAutoFitterOptions--}
```
public AutoFitterOptions getAutoFitterOptions()
```


Ermittelt die Auto‑Fit‑Optionen

**Remarks**

Nur derzeit für xlsx‑ und SpreadsheetML‑Dateien.

**Returns:**
[AutoFitterOptions](../../com.aspose.cells/autofitteroptions)
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


Ruft einen Wert ab, der angibt, ob die Zeichenfolge in der Textdatei in Datumsdaten konvertiert wird. Der Standardwert ist true.

**Returns:**
boolean
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```


Ruft einen Wert ab, der angibt, ob die Zeichenfolge in der Textdatei in numerische Daten konvertiert wird. Der Standardwert ist true.

**Returns:**
boolean
### getDefaultStyleSettings() {#getDefaultStyleSettings--}
```
public DefaultStyleSettings getDefaultStyleSettings()
```


Liest die Standard‑Stileinstellungen zum Initialisieren der Stile der Arbeitsmappe.

**Returns:**
[DefaultStyleSettings](../../com.aspose.cells/defaultstylesettings)
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Ruft die Standardkodierung ab. Gilt nur für CSV‑Dateien.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getExtendToNextSheet() {#getExtendToNextSheet--}
```
public boolean getExtendToNextSheet()
```


Ob Daten auf das nächste Blatt erweitert werden, wenn die Zeilen oder Spalten die Grenze überschreiten. Standard ist false.

**Remarks**

Wenn diese Eigenschaft true ist, werden zusätzliche Daten in das nächste Blatt hinter dem aktuellen Blatt eingefügt (wenn das aktuelle Blatt das letzte ist, wird ein neues Blatt zum aktuellen Arbeitsbuch hinzugefügt). Wenn diese Eigenschaft false ist, werden die die Grenze überschreitenden Daten ignoriert.

**Returns:**
boolean
### getFontConfigs() {#getFontConfigs--}
```
public IndividualFontConfigs getFontConfigs()
```


Liest einzelne Schriftartkonfigurationen aus. Funktioniert nur für die [Workbook](../../com.aspose.cells/workbook), die diese [LoadOptions](../../com.aspose.cells/loadoptions) zum Laden verwendet.

**Returns:**
[IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs)
### getHeaderColumnsCount() {#getHeaderColumnsCount--}
```
public int getHeaderColumnsCount()
```


Die Anzahl der Kopfzeilen-Spalten, die für erweiterte Blätter wiederholt werden sollen.

**Remarks**

Die durch diese Eigenschaft angegebenen Kopfzeilen‑Spalten werden für die erweiterten Blätter dupliziert. Diese Eigenschaft wirkt nur, wenn [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\\#getExtendToNextSheet--) true ist.

**Returns:**
int
### getHeaderRowsCount() {#getHeaderRowsCount--}
```
public int getHeaderRowsCount()
```


Die Anzahl der Kopfzeilen-Zeilen, die für erweiterte Blätter wiederholt werden sollen.

**Remarks**

Die durch diese Eigenschaft angegebenen Kopfzeilen‑Zeilen werden für die erweiterten Blätter dupliziert. Diese Eigenschaft wirkt nur, wenn [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\\#getExtendToNextSheet--) true ist.

**Returns:**
int
### getIgnoreNotPrinted() {#getIgnoreNotPrinted--}
```
public boolean getIgnoreNotPrinted()
```


Ignoriert die Daten, die nicht gedruckt werden, wenn die Datei direkt gedruckt wird

**Remarks**

Nur für xlsx‑Dateien.

**Returns:**
boolean
### getIgnoreUselessShapes() {#getIgnoreUselessShapes--}
```
public boolean getIgnoreUselessShapes()
```


Gibt an, ob nutzlose Formen ignoriert werden.

**Remarks**

Funktioniert nur für xlsx‑, xlsb‑ und xlsm‑Dateien. Es gibt viele überlappende identische Formen, die in einigen Dateien nutzlos sind; wir können sie beim Laden der Dateien ignorieren.

**Returns:**
boolean
### getInterruptMonitor() {#getInterruptMonitor--}
```
public AbstractInterruptMonitor getInterruptMonitor()
```


Liest den Unterbrechungsmonitor.

**Returns:**
[AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor)
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
### getLanguageCode() {#getLanguageCode--}
```
public int getLanguageCode()
```


Liest die Benutzerschnittstellensprache der Arbeitsmappen‑Version basierend auf dem Ländercode, unter dem die Datei gespeichert wurde.

Siehe [CountryCode](../../com.aspose.cells/countrycode).

**Returns:**
int
### getLightCellsDataHandler() {#getLightCellsDataHandler--}
```
public LightCellsDataHandler getLightCellsDataHandler()
```


Der Datenhandler zur Verarbeitung von Zellen­daten beim Lesen der Vorlagendatei.

**Returns:**
[LightCellsDataHandler](../../com.aspose.cells/lightcellsdatahandler)
### getLoadFilter() {#getLoadFilter--}
```
public LoadFilter getLoadFilter()
```


Der Filter, der angibt, wie Daten geladen werden.

**Returns:**
[LoadFilter](../../com.aspose.cells/loadfilter)
### getLoadFormat() {#getLoadFormat--}
```
public int getLoadFormat()
```


Liest das Ladeformat.

Siehe [LoadFormat](../../com.aspose.cells/loadformat).

**Returns:**
int
### getLoadStyleStrategy() {#getLoadStyleStrategy--}
```
public int getLoadStyleStrategy()
```


Gibt die Strategie an, mit der Stil für geparste Werte angewendet wird, wenn die Zeichenkette in eine Zahl oder ein Datum/Uhrzeit konvertiert wird.

Siehe [TxtLoadStyleStrategy](../../com.aspose.cells/txtloadstylestrategy).

**Returns:**
int
### getLocale() {#getLocale--}
```
public Locale getLocale()
```


Liest die regionalen Einstellungen, die für die zu ladende Arbeitsmappe verwendet werden.

**Remarks**

Diese Eigenschaft hat die gleiche Wirkung wie [getRegion()](../../com.aspose.cells/loadoptions\#getRegion--) beim Festlegen regionaler Einstellungen.

**Returns:**
java.util.Locale
### getMaxColumnCount() {#getMaxColumnCount--}
```
public int getMaxColumnCount()
```


Die maximale Anzahl von Spalten, die für ein Blatt importiert werden können.

**Remarks**

Spalten, die dieses Limit überschreiten, werden je nach [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\\#getExtendToNextSheet--) ignoriert oder auf das nächste Blatt erweitert. Diese Anzahl schließt die Kopfzeilen‑Spalten ein ([getHeaderColumnsCount()](../../com.aspose.cells/txtloadoptions\\#getHeaderColumnsCount--)). Der Maximalwert ist das Spaltenlimit des jeweiligen Dateiformats, zum Beispiel beträgt es für xlsx‑Dateien 16384. Wenn diese Eigenschaft nicht angegeben wurde oder der angegebene Wert nicht positiv ist, wird ebenfalls das maximale Limit verwendet.

**Returns:**
int
### getMaxRowCount() {#getMaxRowCount--}
```
public int getMaxRowCount()
```


Die maximale Anzahl von Zeilen, die für ein Blatt importiert werden können.

**Remarks**

Zeilen, die dieses Limit überschreiten, werden je nach [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\\#getExtendToNextSheet--) ignoriert oder auf das nächste Blatt erweitert. Diese Anzahl schließt die Kopfzeilen‑Zeilen ein ([getHeaderRowsCount()](../../com.aspose.cells/txtloadoptions\\#getHeaderRowsCount--)). Der maximal zulässige Wert ist das Zeilenlimit des jeweiligen Dateiformats, zum Beispiel beträgt er für xlsx‑Dateien 1048576. Wenn diese Eigenschaft nicht angegeben wurde oder der angegebene Wert nicht positiv ist, wird ebenfalls das maximale Limit verwendet.

**Returns:**
int
### getMemorySetting() {#getMemorySetting--}
```
public int getMemorySetting()
```


Liest den Speichermodus für die geladene Arbeitsmappe.

Siehe [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Weitere Details zum Speichermodus finden Sie unter [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--).

**Returns:**
int
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
### getPreferredParsers() {#getPreferredParsers--}
```
public ICustomParser[] getPreferredParsers()
```


Liest bevorzugte Wertparser zum Laden einer Textdatei aus.

**Remarks**

parsers[0] ist der Parser, der für die erste Spalte in der Textvorlagendatei verwendet wird, parsers[1] ist der Parser für die zweite Spalte, … usw. Der letzte (parsers[parsers.length-1]) wird für alle übrigen Spalten ab parsers.length-1 verwendet. Wenn ein Element null ist, wird die entsprechende Spalte vom Standard‑Parser von Aspose.Cells geparst.

**Returns:**
com.aspose.cells.ICustomParser[]
### getPreservePaddingSpacesInFormula() {#getPreservePaddingSpacesInFormula--}
```
public boolean getPreservePaddingSpacesInFormula()
```


Gibt an, ob die zwischen Formel‑Token eingefügten Leerzeichen und Zeilenumbrüche beim Lesen und Schreiben von Formeln beibehalten werden sollen. Der Standardwert ist false.

**Remarks**

Nach dem Laden einer Arbeitsmappe aus einer Vorlagendatei mit dieser Option wird [FormulaSettings.getPreservePaddingSpaces()](../../com.aspose.cells/formulasettings\#getPreservePaddingSpaces--) auf denselben Wert wie diese Eigenschaft gesetzt.

**Returns:**
boolean
### getRegion() {#getRegion--}
```
public int getRegion()
```


Liest die regionalen Einstellungen, die für die zu ladende Arbeitsmappe verwendet werden.

Siehe [CountryCode](../../com.aspose.cells/countrycode).

**Remarks**

Die regionalen Einstellungen können zum Initialisieren einiger Funktionen der Arbeitsmappe verwendet werden, z. B. Schriften, Designs usw. Für textbasierte Dateiformate wie CSV, HTML, … wird die regionale Einstellung außerdem verwendet, um Zahlenformate zu erkennen und Textwerte in numerische oder Datums‑/Uhrzeitwerte für Zellen zu konvertieren. Diese Einstellung bleibt für die später erstellte Arbeitsmappe erhalten, das heißt, [WorkbookSettings.getRegion()](../../com.aspose.cells/workbooksettings\#getRegion--) der Arbeitsmappe verwendet dieselbe Region wie diese Eigenschaft.

**Returns:**
int
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
### getStandardFont() {#getStandardFont--}
```
public String getStandardFont()
```


Setzt den Standard‑Schriftartnamen.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen DefaultStyleSettings. Diese Eigenschaft wird 12 Monate nach März 2022 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Returns:**
java.lang.String
### getStandardFontSize() {#getStandardFontSize--}
```
public double getStandardFontSize()
```


Setzt die Standard‑Schriftgröße.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen DefaultStyleSettings. Diese Eigenschaft wird 12 Monate nach März 2022 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Returns:**
double
### getTextQualifier() {#getTextQualifier--}
```
public char getTextQualifier()
```


Gibt den Textqualifizierer für Zellwerte an. Der Standard‑Qualifizierer ist '\"'.

**Remarks**

Beim Setzen dieser Eigenschaft wird [hasTextQualifier()](../../com.aspose.cells/txtloadoptions\\#hasTextQualifier--) automatisch true.

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


Gibt an, ob das führende einfache Anführungszeichen als Teil des Werts einer Zelle betrachtet werden soll. Standard ist true. Wenn es false ist, wird das führende einfache Anführungszeichen aus dem entsprechenden Zellenwert entfernt und [Style.getQuotePrefix()](../../com.aspose.cells/style\\#getQuotePrefix--) wird für die Zelle auf true gesetzt.

**Returns:**
boolean
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Liest den Warn‑Callback.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
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

### setAutoFitterOptions(AutoFitterOptions value) {#setAutoFitterOptions-com.aspose.cells.AutoFitterOptions-}
```
public void setAutoFitterOptions(AutoFitterOptions value)
```


Setzt die Auto‑Fit‑Optionen

**Remarks**

Nur derzeit für xlsx‑ und SpreadsheetML‑Dateien.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) |  |

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


Legt einen Wert fest, der angibt, ob die Zeichenfolge in der Textdatei in Datumsdaten konvertiert wird. Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


Legt einen Wert fest, der angibt, ob die Zeichenfolge in der Textdatei in numerische Daten konvertiert wird. Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


Legt die Standardkodierung fest. Gilt nur für CSV‑Dateien.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setExtendToNextSheet(boolean value) {#setExtendToNextSheet-boolean-}
```
public void setExtendToNextSheet(boolean value)
```


Ob Daten auf das nächste Blatt erweitert werden, wenn die Zeilen oder Spalten die Grenze überschreiten. Standard ist false.

**Remarks**

Wenn diese Eigenschaft true ist, werden zusätzliche Daten in das nächste Blatt hinter dem aktuellen Blatt eingefügt (wenn das aktuelle Blatt das letzte ist, wird ein neues Blatt zum aktuellen Arbeitsbuch hinzugefügt). Wenn diese Eigenschaft false ist, werden die die Grenze überschreitenden Daten ignoriert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setFontConfigs(IndividualFontConfigs value) {#setFontConfigs-com.aspose.cells.IndividualFontConfigs-}
```
public void setFontConfigs(IndividualFontConfigs value)
```


Legt einzelne Schriftkonfigurationen fest. Funktioniert nur für die [Workbook](../../com.aspose.cells/workbook), die diese [LoadOptions](../../com.aspose.cells/loadoptions) zum Laden verwendet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs) |  |

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

### setHeaderColumnsCount(int value) {#setHeaderColumnsCount-int-}
```
public void setHeaderColumnsCount(int value)
```


Die Anzahl der Kopfzeilen-Spalten, die für erweiterte Blätter wiederholt werden sollen.

**Remarks**

Die durch diese Eigenschaft angegebenen Kopfzeilen‑Spalten werden für die erweiterten Blätter dupliziert. Diese Eigenschaft wirkt nur, wenn [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\\#getExtendToNextSheet--) true ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setHeaderRowsCount(int value) {#setHeaderRowsCount-int-}
```
public void setHeaderRowsCount(int value)
```


Die Anzahl der Kopfzeilen-Zeilen, die für erweiterte Blätter wiederholt werden sollen.

**Remarks**

Die durch diese Eigenschaft angegebenen Kopfzeilen‑Zeilen werden für die erweiterten Blätter dupliziert. Diese Eigenschaft wirkt nur, wenn [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\\#getExtendToNextSheet--) true ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

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

### setIgnoreUselessShapes(boolean value) {#setIgnoreUselessShapes-boolean-}
```
public void setIgnoreUselessShapes(boolean value)
```


Gibt an, ob nutzlose Formen ignoriert werden.

**Remarks**

Funktioniert nur für xlsx‑, xlsb‑ und xlsm‑Dateien. Es gibt viele überlappende identische Formen, die in einigen Dateien nutzlos sind; wir können sie beim Laden der Dateien ignorieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setInterruptMonitor(AbstractInterruptMonitor value) {#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-}
```
public void setInterruptMonitor(AbstractInterruptMonitor value)
```


Legt den Interrupt‑Monitor fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor) |  |

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

### setLanguageCode(int value) {#setLanguageCode-int-}
```
public void setLanguageCode(int value)
```


Legt die Sprache der Benutzeroberfläche der Arbeitsmappen‑Version basierend auf dem CountryCode fest, mit dem die Datei gespeichert wurde.

Siehe [CountryCode](../../com.aspose.cells/countrycode).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setLightCellsDataHandler(LightCellsDataHandler value) {#setLightCellsDataHandler-com.aspose.cells.LightCellsDataHandler-}
```
public void setLightCellsDataHandler(LightCellsDataHandler value)
```


Der Datenhandler zur Verarbeitung von Zellen­daten beim Lesen der Vorlagendatei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [LightCellsDataHandler](../../com.aspose.cells/lightcellsdatahandler) |  |

### setLoadFilter(LoadFilter value) {#setLoadFilter-com.aspose.cells.LoadFilter-}
```
public void setLoadFilter(LoadFilter value)
```


Der Filter, der angibt, wie Daten geladen werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [LoadFilter](../../com.aspose.cells/loadfilter) |  |

### setLoadStyleStrategy(int value) {#setLoadStyleStrategy-int-}
```
public void setLoadStyleStrategy(int value)
```


Gibt die Strategie an, mit der Stil für geparste Werte angewendet wird, wenn die Zeichenkette in eine Zahl oder ein Datum/Uhrzeit konvertiert wird.

Siehe [TxtLoadStyleStrategy](../../com.aspose.cells/txtloadstylestrategy).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setLocale(Locale value) {#setLocale-java.util.Locale-}
```
public void setLocale(Locale value)
```


Legt die regionalen Einstellungen fest, die für die zu ladende Arbeitsmappe verwendet werden.

**Remarks**

Diese Eigenschaft hat die gleiche Wirkung wie [getRegion()](../../com.aspose.cells/loadoptions\#getRegion--) beim Festlegen regionaler Einstellungen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Locale |  |

### setMaxColumnCount(int value) {#setMaxColumnCount-int-}
```
public void setMaxColumnCount(int value)
```


Die maximale Anzahl von Spalten, die für ein Blatt importiert werden können.

**Remarks**

Spalten, die dieses Limit überschreiten, werden je nach [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\\#getExtendToNextSheet--) ignoriert oder auf das nächste Blatt erweitert. Diese Anzahl schließt die Kopfzeilen‑Spalten ein ([getHeaderColumnsCount()](../../com.aspose.cells/txtloadoptions\\#getHeaderColumnsCount--)). Der Maximalwert ist das Spaltenlimit des jeweiligen Dateiformats, zum Beispiel beträgt es für xlsx‑Dateien 16384. Wenn diese Eigenschaft nicht angegeben wurde oder der angegebene Wert nicht positiv ist, wird ebenfalls das maximale Limit verwendet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setMaxRowCount(int value) {#setMaxRowCount-int-}
```
public void setMaxRowCount(int value)
```


Die maximale Anzahl von Zeilen, die für ein Blatt importiert werden können.

**Remarks**

Zeilen, die dieses Limit überschreiten, werden je nach [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\\#getExtendToNextSheet--) ignoriert oder auf das nächste Blatt erweitert. Diese Anzahl schließt die Kopfzeilen‑Zeilen ein ([getHeaderRowsCount()](../../com.aspose.cells/txtloadoptions\\#getHeaderRowsCount--)). Der maximal zulässige Wert ist das Zeilenlimit des jeweiligen Dateiformats, zum Beispiel beträgt er für xlsx‑Dateien 1048576. Wenn diese Eigenschaft nicht angegeben wurde oder der angegebene Wert nicht positiv ist, wird ebenfalls das maximale Limit verwendet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setMemorySetting(int value) {#setMemorySetting-int-}
```
public void setMemorySetting(int value)
```


Legt den Speichermodus für die geladene Arbeitsmappe fest.

Siehe [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Weitere Details zum Speichermodus finden Sie unter [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setMultiEncoded(boolean value) {#setMultiEncoded-boolean-}
```
public void setMultiEncoded(boolean value)
```


True bedeutet, dass die Datei mehrere Codierungen enthält.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setPaperSize(int type) {#setPaperSize-int-}
```
public void setPaperSize(int type)
```


Legt die Standard‑Papiergröße für den Druck anhand der Einstellung des Standarddruckers fest.

**Remarks**

Wenn keine Einstellung für die Papiergröße vorhanden ist, verwendet MS Excel die Standardeinstellung des Druckers.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| type | int | [PaperSizeType](../../com.aspose.cells/papersizetype). Die Standardpapiergröße. |

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

### setPreferredParsers(ICustomParser[] value) {#setPreferredParsers-com.aspose.cells.ICustomParser---}
```
public void setPreferredParsers(ICustomParser[] value)
```


Legt bevorzugte Wertparser zum Laden von Textdateien fest.

**Remarks**

parsers[0] ist der Parser, der für die erste Spalte in der Textvorlagendatei verwendet wird, parsers[1] ist der Parser für die zweite Spalte, … usw. Der letzte (parsers[parsers.length-1]) wird für alle übrigen Spalten ab parsers.length-1 verwendet. Wenn ein Element null ist, wird die entsprechende Spalte vom Standard‑Parser von Aspose.Cells geparst.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [ICustomParser\[\]](../../com.aspose.cells/icustomparser) |  |

### setPreservePaddingSpacesInFormula(boolean value) {#setPreservePaddingSpacesInFormula-boolean-}
```
public void setPreservePaddingSpacesInFormula(boolean value)
```


Gibt an, ob die zwischen Formel‑Token eingefügten Leerzeichen und Zeilenumbrüche beim Lesen und Schreiben von Formeln beibehalten werden sollen. Der Standardwert ist false.

**Remarks**

Nach dem Laden einer Arbeitsmappe aus einer Vorlagendatei mit dieser Option wird [FormulaSettings.getPreservePaddingSpaces()](../../com.aspose.cells/formulasettings\#getPreservePaddingSpaces--) auf denselben Wert wie diese Eigenschaft gesetzt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setRegion(int value) {#setRegion-int-}
```
public void setRegion(int value)
```


Legt die regionalen Einstellungen fest, die für die zu ladende Arbeitsmappe verwendet werden.

Siehe [CountryCode](../../com.aspose.cells/countrycode).

**Remarks**

Die regionalen Einstellungen können zum Initialisieren einiger Funktionen der Arbeitsmappe verwendet werden, z. B. Schriften, Designs usw. Für textbasierte Dateiformate wie CSV, HTML, … wird die regionale Einstellung außerdem verwendet, um Zahlenformate zu erkennen und Textwerte in numerische oder Datums‑/Uhrzeitwerte für Zellen zu konvertieren. Diese Einstellung bleibt für die später erstellte Arbeitsmappe erhalten, das heißt, [WorkbookSettings.getRegion()](../../com.aspose.cells/workbooksettings\#getRegion--) der Arbeitsmappe verwendet dieselbe Region wie diese Eigenschaft.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

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

### setStandardFont(String value) {#setStandardFont-java.lang.String-}
```
public void setStandardFont(String value)
```


Setzt den Standard‑Schriftartnamen.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen DefaultStyleSettings. Diese Eigenschaft wird 12 Monate nach März 2022 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setStandardFontSize(double value) {#setStandardFontSize-double-}
```
public void setStandardFontSize(double value)
```


Setzt die Standard‑Schriftgröße.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen DefaultStyleSettings. Diese Eigenschaft wird 12 Monate nach März 2022 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setTextQualifier(char value) {#setTextQualifier-char-}
```
public void setTextQualifier(char value)
```


Gibt den Textqualifizierer für Zellwerte an. Der Standard‑Qualifizierer ist '\"'.

**Remarks**

Beim Setzen dieser Eigenschaft wird [hasTextQualifier()](../../com.aspose.cells/txtloadoptions\\#hasTextQualifier--) automatisch true.

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


Gibt an, ob das führende einfache Anführungszeichen als Teil des Werts einer Zelle betrachtet werden soll. Standard ist true. Wenn es false ist, wird das führende einfache Anführungszeichen aus dem entsprechenden Zellenwert entfernt und [Style.getQuotePrefix()](../../com.aspose.cells/style\\#getQuotePrefix--) wird für die Zelle auf true gesetzt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```


Legt die Warn‑Callback‑Funktion fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |

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

