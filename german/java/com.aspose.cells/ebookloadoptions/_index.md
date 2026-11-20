---
title: "EbookLoadOptions"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt Optionen beim Importieren einer E‑Book-Datei dar."
type: docs
url: /de/java/com.aspose.cells/ebookloadoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LoadOptions](../../com.aspose.cells/loadoptions), [com.aspose.cells.AbstractTextLoadOptions](../../com.aspose.cells/abstracttextloadoptions), [com.aspose.cells.HtmlLoadOptions](../../com.aspose.cells/htmlloadoptions)
```
public class EbookLoadOptions extends HtmlLoadOptions
```

Stellt Optionen beim Importieren einer E‑Book-Datei dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [EbookLoadOptions()](#EbookLoadOptions--) | Erstellt eine Option zum Laden der Ebook-Datei. |
| [EbookLoadOptions(int loadFormat)](#EbookLoadOptions-int-) | Erstellt eine Option zum Laden der Ebook-Datei. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAttachedFilesDirectory()](#getAttachedFilesDirectory--) | Das Verzeichnis, in dem die angehängten Dateien gespeichert werden. |
| [getAutoFilter()](#getAutoFilter--) | Gibt an, ob die Daten beim Laden der Dateien automatisch gefiltert werden. |
| [getAutoFitColsAndRows()](#getAutoFitColsAndRows--) | Gibt an, ob Spalten und Zeilen automatisch angepasst werden. |
| [getAutoFitterOptions()](#getAutoFitterOptions--) | Ermittelt die Auto‑Fit‑Optionen |
| [getCheckDataValid()](#getCheckDataValid--) | Prüft, ob die Daten in der Vorlagendatei gültig sind. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Ob Einschränkungen der Excel‑Datei geprüft werden, wenn der Benutzer zellenbezogene Objekte ändert. |
| [getClass()](#getClass--) |  |
| [getConvertDateTimeData()](#getConvertDateTimeData--) | Ruft einen Wert ab, der angibt, ob die Zeichenkette in der Textdatei in Datumsdaten konvertiert wird. |
| [getConvertFormulasData()](#getConvertFormulasData--) | Wenn true, wird die Zeichenkette in eine Formel konvertiert, wenn der Zeichenkettenwert mit dem Zeichen '=' beginnt; der Standardwert ist false. |
| [getConvertNumericData()](#getConvertNumericData--) | Ruft einen Wert ab, der angibt, ob die Zeichenkette in der Textdatei in numerische Daten konvertiert wird. |
| [getDefaultStyleSettings()](#getDefaultStyleSettings--) | Liest die Standard‑Stileinstellungen zum Initialisieren der Stile der Arbeitsmappe. |
| [getDeleteRedundantSpaces()](#getDeleteRedundantSpaces--) | Gibt an, ob überflüssige Leerzeichen gelöscht werden, wenn der Text Zeilenumbrüche mit dem `<br>`‑Tag erzeugt. |
| [getDetectLaTeX()](#getDetectLaTeX--) | Gibt an, ob LaTeX‑Formeln in der HTML‑Datei erkannt werden sollen. |
| [getEncoding()](#getEncoding--) | Ruft die Standardkodierung ab. |
| [getFontConfigs()](#getFontConfigs--) | Liest einzelne Schriftartkonfigurationen. |
| [getHyperlinkLoadMode()](#getHyperlinkLoadMode--) | Legt fest, wie Hyperlinks beim Laden von HTML geladen werden. |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | Ignoriert die Daten, die nicht gedruckt werden, wenn die Datei direkt gedruckt wird |
| [getIgnoreUselessShapes()](#getIgnoreUselessShapes--) | Gibt an, ob nutzlose Formen ignoriert werden. |
| [getInterruptMonitor()](#getInterruptMonitor--) | Liest den Unterbrechungsmonitor. |
| [getKeepPrecision()](#getKeepPrecision--) | Gibt an, ob ein Zeichenkettenwert nicht geparst wird, wenn die Länge 15 beträgt. |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | Ob nicht geparste Daten im Speicher für die Arbeitsmappe behalten werden, wenn sie aus einer Vorlagendatei geladen wird. |
| [getLanguageCode()](#getLanguageCode--) | Liest die Benutzerschnittstellensprache der Arbeitsmappen‑Version basierend auf dem Ländercode, unter dem die Datei gespeichert wurde. |
| [getLightCellsDataHandler()](#getLightCellsDataHandler--) | Der Datenhandler zur Verarbeitung von Zellen­daten beim Lesen der Vorlagendatei. |
| [getLoadFilter()](#getLoadFilter--) | Der Filter, der angibt, wie Daten geladen werden. |
| [getLoadFormat()](#getLoadFormat--) | Liest das Ladeformat. |
| [getLoadFormulas()](#getLoadFormulas--) | Gibt an, ob Formeln importiert werden, wenn die ursprüngliche HTML‑Datei Formeln enthält |
| [getLoadStyleStrategy()](#getLoadStyleStrategy--) | Gibt die Strategie an, mit der Stil für geparste Werte angewendet wird, wenn die Zeichenkette in eine Zahl oder ein Datum/Uhrzeit konvertiert wird. |
| [getLocale()](#getLocale--) | Liest die regionalen Einstellungen, die für die zu ladende Arbeitsmappe verwendet werden. |
| [getMemorySetting()](#getMemorySetting--) | Liest den Speichermodus für die geladene Arbeitsmappe. |
| [getParagrahLayoutMode()](#getParagrahLayoutMode--) | Gibt an, wie HTML-<p>-Elemente beim Laden von HTML gerendert werden. |
| [getParagraphLayoutMode()](#getParagraphLayoutMode--) | Gibt an, wie HTML-<p>-Elemente beim Laden von HTML gerendert werden. |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | Gibt an, ob Formeln beim Lesen der Datei geparst werden. |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | Gibt an, ob Pivot‑Cache‑Datensätze beim Laden der Datei geparst werden. |
| [getPassword()](#getPassword--) | Liest das Passwort der Arbeitsmappe. |
| [getPreservePaddingSpacesInFormula()](#getPreservePaddingSpacesInFormula--) | Gibt an, ob die zwischen Formel‑Token eingefügten Leerzeichen und Zeilenumbrüche beim Abrufen und Setzen von Formeln erhalten bleiben. |
| [getProgId()](#getProgId--) | Ruft die Programm‑ID des Erstellens der Datei ab. |
| [getRegion()](#getRegion--) | Liest die regionalen Einstellungen, die für die zu ladende Arbeitsmappe verwendet werden. |
| [getStandardFont()](#getStandardFont--) | Setzt den Standard‑Schriftartnamen. |
| [getStandardFontSize()](#getStandardFontSize--) | Setzt die Standard‑Schriftgröße. |
| [getStreamProvider()](#getStreamProvider--) | Ruft das StreamProviderImportHtmlFile zum Importieren von Objekten ab. |
| [getSupportDivTag()](#getSupportDivTag--) | Gibt an, ob das Layout des `<div>`‑Tags unterstützt wird, wenn die HTML‑Datei es enthält. |
| [getTableLoadOptions()](#getTableLoadOptions--) | Ruft die Instanz von HtmlTableLoadOptionCollection ab |
| [getWarningCallback()](#getWarningCallback--) | Liest den Warn‑Callback. |
| [hasFormula()](#hasFormula--) | Gibt an, ob der Text eine Formel ist, wenn er mit "=" beginnt. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAttachedFilesDirectory(String value)](#setAttachedFilesDirectory-java.lang.String-) | Das Verzeichnis, in dem die angehängten Dateien gespeichert werden. |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | Gibt an, ob die Daten beim Laden der Dateien automatisch gefiltert werden. |
| [setAutoFitColsAndRows(boolean value)](#setAutoFitColsAndRows-boolean-) | Gibt an, ob Spalten und Zeilen automatisch angepasst werden. |
| [setAutoFitterOptions(AutoFitterOptions value)](#setAutoFitterOptions-com.aspose.cells.AutoFitterOptions-) | Setzt die Auto‑Fit‑Optionen |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | Prüft, ob die Daten in der Vorlagendatei gültig sind. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Ob Einschränkungen der Excel‑Datei geprüft werden, wenn der Benutzer zellenbezogene Objekte ändert. |
| [setConvertDateTimeData(boolean value)](#setConvertDateTimeData-boolean-) | Legt einen Wert fest, der angibt, ob die Zeichenkette in der Textdatei in Datumsdaten konvertiert wird. |
| [setConvertFormulasData(boolean value)](#setConvertFormulasData-boolean-) | Wenn true, wird die Zeichenkette in eine Formel konvertiert, wenn der Zeichenkettenwert mit dem Zeichen '=' beginnt; der Standardwert ist false. |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | Legt einen Wert fest, der angibt, ob die Zeichenkette in der Textdatei in numerische Daten konvertiert wird. |
| [setDeleteRedundantSpaces(boolean value)](#setDeleteRedundantSpaces-boolean-) | Gibt an, ob überflüssige Leerzeichen gelöscht werden, wenn der Text Zeilenumbrüche mit dem `<br>`‑Tag erzeugt. |
| [setDetectLaTeX(boolean value)](#setDetectLaTeX-boolean-) | Gibt an, ob LaTeX‑Formeln in der HTML‑Datei erkannt werden sollen. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | Legt die Standardkodierung fest. |
| [setFontConfigs(IndividualFontConfigs value)](#setFontConfigs-com.aspose.cells.IndividualFontConfigs-) | Legt einzelne Schriftartkonfigurationen fest. |
| [setHasFormula(boolean value)](#setHasFormula-boolean-) | Gibt an, ob der Text eine Formel ist, wenn er mit "=" beginnt. |
| [setHyperlinkLoadMode(int value)](#setHyperlinkLoadMode-int-) | Legt fest, wie Hyperlinks beim Laden von HTML geladen werden. |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | Ignoriert die Daten, die nicht gedruckt werden, wenn die Datei direkt gedruckt wird |
| [setIgnoreUselessShapes(boolean value)](#setIgnoreUselessShapes-boolean-) | Gibt an, ob nutzlose Formen ignoriert werden. |
| [setInterruptMonitor(AbstractInterruptMonitor value)](#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-) | Legt den Interrupt‑Monitor fest. |
| [setKeepPrecision(boolean value)](#setKeepPrecision-boolean-) | Gibt an, ob ein Zeichenkettenwert nicht geparst wird, wenn die Länge 15 beträgt. |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | Ob nicht geparste Daten im Speicher für die Arbeitsmappe behalten werden, wenn sie aus einer Vorlagendatei geladen wird. |
| [setLanguageCode(int value)](#setLanguageCode-int-) | Legt die Sprache der Benutzeroberfläche der Arbeitsmappen‑Version basierend auf dem CountryCode fest, mit dem die Datei gespeichert wurde. |
| [setLightCellsDataHandler(LightCellsDataHandler value)](#setLightCellsDataHandler-com.aspose.cells.LightCellsDataHandler-) | Der Datenhandler zur Verarbeitung von Zellen­daten beim Lesen der Vorlagendatei. |
| [setLoadFilter(LoadFilter value)](#setLoadFilter-com.aspose.cells.LoadFilter-) | Der Filter, der angibt, wie Daten geladen werden. |
| [setLoadFormulas(boolean value)](#setLoadFormulas-boolean-) | Gibt an, ob Formeln importiert werden, wenn die ursprüngliche HTML‑Datei Formeln enthält |
| [setLoadStyleStrategy(int value)](#setLoadStyleStrategy-int-) | Gibt die Strategie an, mit der Stil für geparste Werte angewendet wird, wenn die Zeichenkette in eine Zahl oder ein Datum/Uhrzeit konvertiert wird. |
| [setLocale(Locale value)](#setLocale-java.util.Locale-) | Legt die regionalen Einstellungen fest, die für die zu ladende Arbeitsmappe verwendet werden. |
| [setMemorySetting(int value)](#setMemorySetting-int-) | Legt den Speichermodus für die geladene Arbeitsmappe fest. |
| [setPaperSize(int type)](#setPaperSize-int-) | Legt die Standard‑Papiergröße für den Druck anhand der Einstellung des Standarddruckers fest. |
| [setParagrahLayoutMode(int value)](#setParagrahLayoutMode-int-) | Gibt an, wie HTML-<p>-Elemente beim Laden von HTML gerendert werden. |
| [setParagraphLayoutMode(int value)](#setParagraphLayoutMode-int-) | Gibt an, wie HTML-<p>-Elemente beim Laden von HTML gerendert werden. |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | Gibt an, ob Formeln beim Lesen der Datei geparst werden. |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | Gibt an, ob Pivot‑Cache‑Datensätze beim Laden der Datei geparst werden. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Legt das Passwort der Arbeitsmappe fest. |
| [setPreservePaddingSpacesInFormula(boolean value)](#setPreservePaddingSpacesInFormula-boolean-) | Gibt an, ob die zwischen Formel‑Token eingefügten Leerzeichen und Zeilenumbrüche beim Abrufen und Setzen von Formeln erhalten bleiben. |
| [setRegion(int value)](#setRegion-int-) | Legt die regionalen Einstellungen fest, die für die zu ladende Arbeitsmappe verwendet werden. |
| [setStandardFont(String value)](#setStandardFont-java.lang.String-) | Setzt den Standard‑Schriftartnamen. |
| [setStandardFontSize(double value)](#setStandardFontSize-double-) | Setzt die Standard‑Schriftgröße. |
| [setStreamProvider(IStreamProvider value)](#setStreamProvider-com.aspose.cells.IStreamProvider-) | Legt die StreamProviderImportHtmlFile für das Importieren von Objekten fest. |
| [setSupportDivTag(boolean value)](#setSupportDivTag-boolean-) | Gibt an, ob das Layout des `<div>`‑Tags unterstützt wird, wenn die HTML‑Datei es enthält. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Legt die Warn‑Callback‑Funktion fest. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### EbookLoadOptions() {#EbookLoadOptions--}
```
public EbookLoadOptions()
```


Erstellt eine Option zum Laden der Ebook-Datei.

### EbookLoadOptions(int loadFormat) {#EbookLoadOptions-int-}
```
public EbookLoadOptions(int loadFormat)
```


Erstellt eine Option zum Laden der Ebook-Datei.

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
### getAttachedFilesDirectory() {#getAttachedFilesDirectory--}
```
public String getAttachedFilesDirectory()
```


Das Verzeichnis, in dem die angehängten Dateien gespeichert werden.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft HtmlLoadOptions.StreamProvider. Diese Eigenschaft wird 12 Monate später, seit Dezember 2014, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
java.lang.String
### getAutoFilter() {#getAutoFilter--}
```
public boolean getAutoFilter()
```


Gibt an, ob die Daten beim Laden der Dateien automatisch gefiltert werden.

**Remarks**

Manchmal werden, obwohl der AutoFilter gesetzt ist, die entsprechenden Zeilen in der Datei nicht ausgeblendet. Jetzt funktioniert es nur für SpreadSheetML‑Dateien.

**Returns:**
boolean
### getAutoFitColsAndRows() {#getAutoFitColsAndRows--}
```
public boolean getAutoFitColsAndRows()
```


Gibt an, ob Spalten und Zeilen automatisch angepasst werden. Der Standardwert ist false.

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
### getConvertFormulasData() {#getConvertFormulasData--}
```
public boolean getConvertFormulasData()
```


Wenn true, wird die Zeichenkette in eine Formel konvertiert, wenn der Zeichenkettenwert mit dem Zeichen '=' beginnt; der Standardwert ist false.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft HtmlLoadOptions.HasFormula. Diese Eigenschaft wird 12 Monate später, seit März 2023, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

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
### getDeleteRedundantSpaces() {#getDeleteRedundantSpaces--}
```
public boolean getDeleteRedundantSpaces()
```


Gibt an, ob überflüssige Leerzeichen gelöscht werden, wenn der Text Zeilen mit dem `<br>`‑Tag umbricht. Der Standardwert ist false.

**Returns:**
boolean
### getDetectLaTeX() {#getDetectLaTeX--}
```
public boolean getDetectLaTeX()
```


Gibt an, ob LaTeX‑Formeln in der HTML‑Datei erkannt werden sollen. Der Standardwert ist false.

**Returns:**
boolean
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Ruft die Standardkodierung ab. Gilt nur für CSV‑Dateien.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getFontConfigs() {#getFontConfigs--}
```
public IndividualFontConfigs getFontConfigs()
```


Liest einzelne Schriftartkonfigurationen aus. Funktioniert nur für die [Workbook](../../com.aspose.cells/workbook), die diese [LoadOptions](../../com.aspose.cells/loadoptions) zum Laden verwendet.

**Returns:**
[IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs)
### getHyperlinkLoadMode() {#getHyperlinkLoadMode--}
```
public int getHyperlinkLoadMode()
```


Legt fest, wie Hyperlinks beim Laden von HTML geladen werden.

Siehe [HyperlinkLoadMode](../../com.aspose.cells/hyperlinkloadmode).

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
### getLoadFormulas() {#getLoadFormulas--}
```
public boolean getLoadFormulas()
```


Gibt an, ob Formeln importiert werden, wenn die ursprüngliche HTML‑Datei Formeln enthält

**Returns:**
boolean
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
### getParagrahLayoutMode() {#getParagrahLayoutMode--}
```
public int getParagrahLayoutMode()
```


Gibt an, wie HTML‑<p>‑Elemente beim Laden von HTML gerendert werden. Der Standardwert ist [HtmlParagraphLayoutMode.NORMAL](../../com.aspose.cells/htmlparagraphlayoutmode\#NORMAL).

Siehe [HtmlParagraphLayoutMode](../../com.aspose.cells/htmlparagraphlayoutmode).

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft HtmlLoadOptions.ParagraphLayoutMode. Diese Methode wird 12 Monate später, seit Juli 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
int
### getParagraphLayoutMode() {#getParagraphLayoutMode--}
```
public int getParagraphLayoutMode()
```


Gibt an, wie HTML‑<p>‑Elemente beim Laden von HTML gerendert werden. Der Standardwert ist [HtmlParagraphLayoutMode.NORMAL](../../com.aspose.cells/htmlparagraphlayoutmode\#NORMAL).

Siehe [HtmlParagraphLayoutMode](../../com.aspose.cells/htmlparagraphlayoutmode).

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
### getPreservePaddingSpacesInFormula() {#getPreservePaddingSpacesInFormula--}
```
public boolean getPreservePaddingSpacesInFormula()
```


Gibt an, ob die zwischen Formel‑Token eingefügten Leerzeichen und Zeilenumbrüche beim Lesen und Schreiben von Formeln beibehalten werden sollen. Der Standardwert ist false.

**Remarks**

Nach dem Laden einer Arbeitsmappe aus einer Vorlagendatei mit dieser Option wird [FormulaSettings.getPreservePaddingSpaces()](../../com.aspose.cells/formulasettings\#getPreservePaddingSpaces--) auf denselben Wert wie diese Eigenschaft gesetzt.

**Returns:**
boolean
### getProgId() {#getProgId--}
```
public String getProgId()
```


Ruft die Programm‑ID beim Erstellen der Datei ab. Nur für MHT‑Dateien.

**Returns:**
java.lang.String
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
### getStreamProvider() {#getStreamProvider--}
```
public IStreamProvider getStreamProvider()
```


Ruft das StreamProviderImportHtmlFile zum Importieren von Objekten ab.

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getSupportDivTag() {#getSupportDivTag--}
```
public boolean getSupportDivTag()
```


Gibt an, ob das Layout des `<div>`‑Tags unterstützt wird, wenn die HTML‑Datei es enthält. Der Standardwert ist false.

**Returns:**
boolean
### getTableLoadOptions() {#getTableLoadOptions--}
```
public HtmlTableLoadOptionCollection getTableLoadOptions()
```


Ruft die Instanz von HtmlTableLoadOptionCollection ab

**Returns:**
[HtmlTableLoadOptionCollection](../../com.aspose.cells/htmltableloadoptioncollection)
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




### setAttachedFilesDirectory(String value) {#setAttachedFilesDirectory-java.lang.String-}
```
public void setAttachedFilesDirectory(String value)
```


Das Verzeichnis, in dem die angehängten Dateien gespeichert werden.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft HtmlLoadOptions.StreamProvider. Diese Eigenschaft wird 12 Monate später, seit Dezember 2014, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

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

### setAutoFitColsAndRows(boolean value) {#setAutoFitColsAndRows-boolean-}
```
public void setAutoFitColsAndRows(boolean value)
```


Gibt an, ob Spalten und Zeilen automatisch angepasst werden. Der Standardwert ist false.

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

### setConvertFormulasData(boolean value) {#setConvertFormulasData-boolean-}
```
public void setConvertFormulasData(boolean value)
```


Wenn true, wird die Zeichenkette in eine Formel konvertiert, wenn der Zeichenkettenwert mit dem Zeichen '=' beginnt; der Standardwert ist false.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft HtmlLoadOptions.HasFormula. Diese Eigenschaft wird 12 Monate später, seit März 2023, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

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

### setDeleteRedundantSpaces(boolean value) {#setDeleteRedundantSpaces-boolean-}
```
public void setDeleteRedundantSpaces(boolean value)
```


Gibt an, ob überflüssige Leerzeichen gelöscht werden, wenn der Text Zeilen mit dem `<br>`‑Tag umbricht. Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setDetectLaTeX(boolean value) {#setDetectLaTeX-boolean-}
```
public void setDetectLaTeX(boolean value)
```


Gibt an, ob LaTeX‑Formeln in der HTML‑Datei erkannt werden sollen. Der Standardwert ist false.

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

### setHyperlinkLoadMode(int value) {#setHyperlinkLoadMode-int-}
```
public void setHyperlinkLoadMode(int value)
```


Legt fest, wie Hyperlinks beim Laden von HTML geladen werden.

Siehe [HyperlinkLoadMode](../../com.aspose.cells/hyperlinkloadmode).

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

### setLoadFormulas(boolean value) {#setLoadFormulas-boolean-}
```
public void setLoadFormulas(boolean value)
```


Gibt an, ob Formeln importiert werden, wenn die ursprüngliche HTML‑Datei Formeln enthält

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

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

### setParagrahLayoutMode(int value) {#setParagrahLayoutMode-int-}
```
public void setParagrahLayoutMode(int value)
```


Gibt an, wie HTML‑<p>‑Elemente beim Laden von HTML gerendert werden. Der Standardwert ist [HtmlParagraphLayoutMode.NORMAL](../../com.aspose.cells/htmlparagraphlayoutmode\#NORMAL).

Siehe [HtmlParagraphLayoutMode](../../com.aspose.cells/htmlparagraphlayoutmode).

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft HtmlLoadOptions.ParagraphLayoutMode. Diese Methode wird 12 Monate später, seit Juli 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setParagraphLayoutMode(int value) {#setParagraphLayoutMode-int-}
```
public void setParagraphLayoutMode(int value)
```


Gibt an, wie HTML‑<p>‑Elemente beim Laden von HTML gerendert werden. Der Standardwert ist [HtmlParagraphLayoutMode.NORMAL](../../com.aspose.cells/htmlparagraphlayoutmode\#NORMAL).

Siehe [HtmlParagraphLayoutMode](../../com.aspose.cells/htmlparagraphlayoutmode).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

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

### setStreamProvider(IStreamProvider value) {#setStreamProvider-com.aspose.cells.IStreamProvider-}
```
public void setStreamProvider(IStreamProvider value)
```


Legt die StreamProviderImportHtmlFile für das Importieren von Objekten fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setSupportDivTag(boolean value) {#setSupportDivTag-boolean-}
```
public void setSupportDivTag(boolean value)
```


Gibt an, ob das Layout des `<div>`‑Tags unterstützt wird, wenn die HTML‑Datei es enthält. Der Standardwert ist false.

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

