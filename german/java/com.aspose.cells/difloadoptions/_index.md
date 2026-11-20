---
title: "DifLoadOptions"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Optionen zum Laden einer .dif-Datei dar."
type: docs
url: /de/java/com.aspose.cells/difloadoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LoadOptions](../../com.aspose.cells/loadoptions)
```
public class DifLoadOptions extends LoadOptions
```

Stellt die Optionen zum Laden einer .dif-Datei dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [DifLoadOptions()](#DifLoadOptions--) | Die Optionen. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | Gibt an, ob die Daten beim Laden der Dateien automatisch gefiltert werden. |
| [getAutoFitterOptions()](#getAutoFitterOptions--) | Ermittelt die Auto‑Fit‑Optionen |
| [getCheckDataValid()](#getCheckDataValid--) | Prüft, ob die Daten in der Vorlagendatei gültig sind. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Ob Einschränkungen der Excel‑Datei geprüft werden, wenn der Benutzer zellenbezogene Objekte ändert. |
| [getClass()](#getClass--) |  |
| [getDefaultStyleSettings()](#getDefaultStyleSettings--) | Liest die Standard‑Stileinstellungen zum Initialisieren der Stile der Arbeitsmappe. |
| [getFontConfigs()](#getFontConfigs--) | Liest einzelne Schriftartkonfigurationen. |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | Ignoriert die Daten, die nicht gedruckt werden, wenn die Datei direkt gedruckt wird |
| [getIgnoreUselessShapes()](#getIgnoreUselessShapes--) | Gibt an, ob nutzlose Formen ignoriert werden. |
| [getInterruptMonitor()](#getInterruptMonitor--) | Liest den Unterbrechungsmonitor. |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | Ob nicht geparste Daten im Speicher für die Arbeitsmappe behalten werden, wenn sie aus einer Vorlagendatei geladen wird. |
| [getLanguageCode()](#getLanguageCode--) | Liest die Benutzerschnittstellensprache der Arbeitsmappen‑Version basierend auf dem Ländercode, unter dem die Datei gespeichert wurde. |
| [getLightCellsDataHandler()](#getLightCellsDataHandler--) | Der Datenhandler zur Verarbeitung von Zellen­daten beim Lesen der Vorlagendatei. |
| [getLoadFilter()](#getLoadFilter--) | Der Filter, der angibt, wie Daten geladen werden. |
| [getLoadFormat()](#getLoadFormat--) | Liest das Ladeformat. |
| [getLocale()](#getLocale--) | Liest die regionalen Einstellungen, die für die zu ladende Arbeitsmappe verwendet werden. |
| [getMemorySetting()](#getMemorySetting--) | Liest den Speichermodus für die geladene Arbeitsmappe. |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | Gibt an, ob Formeln beim Lesen der Datei geparst werden. |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | Gibt an, ob Pivot‑Cache‑Datensätze beim Laden der Datei geparst werden. |
| [getPassword()](#getPassword--) | Liest das Passwort der Arbeitsmappe. |
| [getPreservePaddingSpacesInFormula()](#getPreservePaddingSpacesInFormula--) | Gibt an, ob die zwischen Formel‑Token eingefügten Leerzeichen und Zeilenumbrüche beim Abrufen und Setzen von Formeln erhalten bleiben. |
| [getRegion()](#getRegion--) | Liest die regionalen Einstellungen, die für die zu ladende Arbeitsmappe verwendet werden. |
| [getStandardFont()](#getStandardFont--) | Setzt den Standard‑Schriftartnamen. |
| [getStandardFontSize()](#getStandardFontSize--) | Setzt die Standard‑Schriftgröße. |
| [getWarningCallback()](#getWarningCallback--) | Liest den Warn‑Callback. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | Gibt an, ob die Daten beim Laden der Dateien automatisch gefiltert werden. |
| [setAutoFitterOptions(AutoFitterOptions value)](#setAutoFitterOptions-com.aspose.cells.AutoFitterOptions-) | Setzt die Auto‑Fit‑Optionen |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | Prüft, ob die Daten in der Vorlagendatei gültig sind. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Ob Einschränkungen der Excel‑Datei geprüft werden, wenn der Benutzer zellenbezogene Objekte ändert. |
| [setFontConfigs(IndividualFontConfigs value)](#setFontConfigs-com.aspose.cells.IndividualFontConfigs-) | Legt einzelne Schriftartkonfigurationen fest. |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | Ignoriert die Daten, die nicht gedruckt werden, wenn die Datei direkt gedruckt wird |
| [setIgnoreUselessShapes(boolean value)](#setIgnoreUselessShapes-boolean-) | Gibt an, ob nutzlose Formen ignoriert werden. |
| [setInterruptMonitor(AbstractInterruptMonitor value)](#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-) | Legt den Interrupt‑Monitor fest. |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | Ob nicht geparste Daten im Speicher für die Arbeitsmappe behalten werden, wenn sie aus einer Vorlagendatei geladen wird. |
| [setLanguageCode(int value)](#setLanguageCode-int-) | Legt die Sprache der Benutzeroberfläche der Arbeitsmappen‑Version basierend auf dem CountryCode fest, mit dem die Datei gespeichert wurde. |
| [setLightCellsDataHandler(LightCellsDataHandler value)](#setLightCellsDataHandler-com.aspose.cells.LightCellsDataHandler-) | Der Datenhandler zur Verarbeitung von Zellen­daten beim Lesen der Vorlagendatei. |
| [setLoadFilter(LoadFilter value)](#setLoadFilter-com.aspose.cells.LoadFilter-) | Der Filter, der angibt, wie Daten geladen werden. |
| [setLocale(Locale value)](#setLocale-java.util.Locale-) | Legt die regionalen Einstellungen fest, die für die zu ladende Arbeitsmappe verwendet werden. |
| [setMemorySetting(int value)](#setMemorySetting-int-) | Legt den Speichermodus für die geladene Arbeitsmappe fest. |
| [setPaperSize(int type)](#setPaperSize-int-) | Legt die Standard‑Papiergröße für den Druck anhand der Einstellung des Standarddruckers fest. |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | Gibt an, ob Formeln beim Lesen der Datei geparst werden. |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | Gibt an, ob Pivot‑Cache‑Datensätze beim Laden der Datei geparst werden. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Legt das Passwort der Arbeitsmappe fest. |
| [setPreservePaddingSpacesInFormula(boolean value)](#setPreservePaddingSpacesInFormula-boolean-) | Gibt an, ob die zwischen Formel‑Token eingefügten Leerzeichen und Zeilenumbrüche beim Abrufen und Setzen von Formeln erhalten bleiben. |
| [setRegion(int value)](#setRegion-int-) | Legt die regionalen Einstellungen fest, die für die zu ladende Arbeitsmappe verwendet werden. |
| [setStandardFont(String value)](#setStandardFont-java.lang.String-) | Setzt den Standard‑Schriftartnamen. |
| [setStandardFontSize(double value)](#setStandardFontSize-double-) | Setzt die Standard‑Schriftgröße. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Legt die Warn‑Callback‑Funktion fest. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DifLoadOptions() {#DifLoadOptions--}
```
public DifLoadOptions()
```


Die Optionen.

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
### getDefaultStyleSettings() {#getDefaultStyleSettings--}
```
public DefaultStyleSettings getDefaultStyleSettings()
```


Liest die Standard‑Stileinstellungen zum Initialisieren der Stile der Arbeitsmappe.

**Returns:**
[DefaultStyleSettings](../../com.aspose.cells/defaultstylesettings)
### getFontConfigs() {#getFontConfigs--}
```
public IndividualFontConfigs getFontConfigs()
```


Liest einzelne Schriftartkonfigurationen aus. Funktioniert nur für die [Workbook](../../com.aspose.cells/workbook), die diese [LoadOptions](../../com.aspose.cells/loadoptions) zum Laden verwendet.

**Returns:**
[IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs)
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
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Liest den Warn‑Callback.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
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

### setFontConfigs(IndividualFontConfigs value) {#setFontConfigs-com.aspose.cells.IndividualFontConfigs-}
```
public void setFontConfigs(IndividualFontConfigs value)
```


Legt einzelne Schriftkonfigurationen fest. Funktioniert nur für die [Workbook](../../com.aspose.cells/workbook), die diese [LoadOptions](../../com.aspose.cells/loadoptions) zum Laden verwendet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs) |  |

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

