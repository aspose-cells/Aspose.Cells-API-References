---
title: "CellsHelper"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt Hilfsfunktionen bereit."
type: docs
url: /de/java/com.aspose.cells/cellshelper/
---

**Inheritance:**
java.lang.Object
```
public class CellsHelper
```

Stellt Hilfsfunktionen bereit.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [addAddInFunction(String function, int minCountOfParameters, int maxCountOfParameters, int[] paramersType, int functionValueType)](#addAddInFunction-java.lang.String-int-int-int---int-) | Add‑In‑Funktion hinzufügen. |
| [cellIndexToName(int row, int column)](#cellIndexToName-int-int-) | Ermittelt den Zellenamen anhand seiner Zeilen‑ und Spaltenindizes. |
| [cellNameToIndex(String cellName)](#cellNameToIndex-java.lang.String-) | Ermittelt die Zeilen‑ und Spaltenindizes der Zelle anhand ihres Namens. |
| [columnIndexToName(int column)](#columnIndexToName-int-) | Ermittelt den Spaltennamen anhand des Spaltenindex. |
| [columnNameToIndex(String columnName)](#columnNameToIndex-java.lang.String-) | Ermittelt den Spaltenindex anhand des Spaltennamens. |
| [convertA1FormulaToR1C1(String formula, int row, int column)](#convertA1FormulaToR1C1-java.lang.String-int-int-) | Konvertiert die A1‑Formel der Zelle in die r1c1‑Formel. |
| [convertR1C1FormulaToA1(String r1c1Formula, int row, int column)](#convertR1C1FormulaToA1-java.lang.String-int-int-) | Konvertiert die r1c1‑Formel der Zelle in die A1‑Formel. |
| [createSafeSheetName(String nameProposal)](#createSafeSheetName-java.lang.String-) | Überprüft den angegebenen Blattnamen und erstellt bei Bedarf einen gültigen. |
| [createSafeSheetName(String nameProposal, char replaceChar)](#createSafeSheetName-java.lang.String-char-) | Überprüft den angegebenen Blattnamen und erstellt bei Bedarf einen gültigen. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAltStartPath()](#getAltStartPath--) | Ermittelt den alternativen Startpfad, auf den sich einige externe Formelbezüge beziehen. |
| [getCacheFolder()](#getCacheFolder--) | Ermittelt den Ordner für temporäre Dateien, die als Daten‑Cache verwendet werden können. |
| [getClass()](#getClass--) |  |
| [getCustomImplementationFactory()](#getCustomImplementationFactory--) | Ermittelt die Fabrik zur Erstellung von Instanzen mit spezieller Implementierung. |
| [getDPI()](#getDPI--) | Ermittelt die DPI des Geräts. |
| [getDateTimeFromDouble(double doubleValue, boolean date1904)](#getDateTimeFromDouble-double-boolean-) | Konvertiert den Double‑Wert in den Datums‑Zeit‑Wert. |
| [getDoubleFromDateTime(DateTime dateTime, boolean date1904)](#getDoubleFromDateTime-com.aspose.cells.DateTime-boolean-) | Konvertiert das Datum/Zeit in einen Double‑Wert. |
| [getLibraryPath()](#getLibraryPath--) | Ermittelt den Bibliothekspfad, auf den sich einige externe Formelbezüge beziehen. |
| [getSignificantDigits()](#getSignificantDigits--) | Ermittelt die Anzahl signifikanter Stellen. |
| [getSignificantDigitsType()](#getSignificantDigitsType--) | Ermittelt den Standardtyp signifikanter Stellen für die Ausgabe numerischer Werte. |
| [getStartupPath()](#getStartupPath--) | Ermittelt den Startpfad, auf den sich einige externe Formelbezüge beziehen. |
| [getTextWidth(String text, Font font, double scaling)](#getTextWidth-java.lang.String-com.aspose.cells.Font-double-) | Ermittelt die Textbreite in Punkten. |
| [getUsedColors(Workbook workbook)](#getUsedColors-com.aspose.cells.Workbook-) | Ermittelt alle im Arbeitsbuch verwendeten Farben. |
| [getVersion()](#getVersion--) | Ermittelt die Release‑Version. |
| [hashCode()](#hashCode--) |  |
| [isCloudPlatform()](#isCloudPlatform--) | Bitte setzen Sie diese Eigenschaft auf True, wenn Sie auf einer Cloud‑Plattform wie Azure, AWSLambda usw. ausführen, |
| [mergeFiles(String[] files, String cachedFile, String destFile)](#mergeFiles-java.lang.String---java.lang.String-java.lang.String-) | Führt einige große XLS‑Dateien zu einer XLS‑Datei zusammen. |
| [needQuoteInFormula(String sheetName)](#needQuoteInFormula-java.lang.String-) | Gibt an, ob der Blattname in einfache Anführungszeichen eingeschlossen werden soll. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [rowIndexToName(int row)](#rowIndexToName-int-) | Ermittelt den Zeilennamen anhand des Zeilenindex. |
| [rowNameToIndex(String rowName)](#rowNameToIndex-java.lang.String-) | Ermittelt den Zeilenindex anhand des Zeilennamens. |
| [setAltStartPath(String value)](#setAltStartPath-java.lang.String-) | Legt den alternativen Startpfad fest, auf den sich einige externe Formelbezüge beziehen. |
| [setCacheFolder(String cache)](#setCacheFolder-java.lang.String-) | Legt den Ordner für temporäre Dateien fest, die als Daten-Cache verwendet werden können. |
| [setCloudPlatform(boolean value)](#setCloudPlatform-boolean-) | Bitte setzen Sie diese Eigenschaft auf True, wenn Sie auf einer Cloud‑Plattform wie Azure, AWSLambda usw. ausführen, |
| [setCustomImplementationFactory(CustomImplementationFactory value)](#setCustomImplementationFactory-com.aspose.cells.CustomImplementationFactory-) | Legt die Fabrik zum Erzeugen von Instanzen mit spezieller Implementierung fest. |
| [setDPI(double value)](#setDPI-double-) | Ermittelt die DPI des Geräts. |
| [setLibraryPath(String value)](#setLibraryPath-java.lang.String-) | Legt den Bibliothekspfad fest, auf den sich einige externe Formelbezüge beziehen. |
| [setSignificantDigits(int value)](#setSignificantDigits-int-) | Legt die Anzahl signifikanter Stellen fest. |
| [setSignificantDigitsType(int value)](#setSignificantDigitsType-int-) | Legt den Standardtyp signifikanter Stellen für die Ausgabe numerischer Werte fest. |
| [setStartupPath(String value)](#setStartupPath-java.lang.String-) | Legt den Startpfad fest, auf den sich einige externe Formelbezüge beziehen. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addAddInFunction(String function, int minCountOfParameters, int maxCountOfParameters, int[] paramersType, int functionValueType) {#addAddInFunction-java.lang.String-int-int-int---int-}
```
public static void addAddInFunction(String function, int minCountOfParameters, int maxCountOfParameters, int[] paramersType, int functionValueType)
```


Add‑In‑Funktion hinzufügen.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methoden WorksheetCollection.RegisterAddInFunction(). Diese Methode wird 12 Monate nach Januar 2022 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Funktion | java.lang.String | Der Funktionsname. |
| minCountOfParameters | int | Minimale Anzahl von Parametern, die diese Funktion benötigt |
| maxCountOfParameters | int | Maximale Anzahl von Parametern, die diese Funktion erlaubt. |
| paramersType | int[] | [ParameterType](../../com.aspose.cells/parametertype). Der erwartete Parametertyp der Funktion |
| functionValueType | int | [ParameterType](../../com.aspose.cells/parametertype). Der Funktionswerttyp. |

### cellIndexToName(int row, int column) {#cellIndexToName-int-int-}
```
public static String cellIndexToName(int row, int column)
```


Ermittelt den Zellenamen anhand seiner Zeilen‑ und Spaltenindizes.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex. |
| Spalte | int | Spaltenindex. |

**Returns:**
java.lang.String - Name der Zelle.
### cellNameToIndex(String cellName) {#cellNameToIndex-java.lang.String-}
```
public static int[] cellNameToIndex(String cellName)
```


Ermittelt die Zeilen‑ und Spaltenindizes der Zelle anhand ihres Namens.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellName | java.lang.String | Name der Zelle |

**Returns:**
int[] - [0] ist der Zeilenindex und [1] ist der Spaltenindex.
### columnIndexToName(int column) {#columnIndexToName-int-}
```
public static String columnIndexToName(int column)
```


Ermittelt den Spaltennamen anhand des Spaltenindex.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Spalte | int | Spaltenindex. |

**Returns:**
java.lang.String - Name der Spalte.
### columnNameToIndex(String columnName) {#columnNameToIndex-java.lang.String-}
```
public static int columnNameToIndex(String columnName)
```


Ermittelt den Spaltenindex anhand des Spaltennamens.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnName | java.lang.String | Spaltenname. |

**Returns:**
int - Spaltenindex.
### convertA1FormulaToR1C1(String formula, int row, int column) {#convertA1FormulaToR1C1-java.lang.String-int-int-}
```
public static String convertA1FormulaToR1C1(String formula, int row, int column)
```


Konvertiert die A1‑Formel der Zelle in die r1c1‑Formel.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode Worksheet.ConvertFormulaReferenceStyle() . Diese Eigenschaft wird 12 Monate später, seit August 2023, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| formula | java.lang.String | Die A1-Formel. |
| Zeile | int | Der Zeilenindex der Zelle. |
| Spalte | int | Der Spaltenindex der Zelle. |

**Returns:**
java.lang.String - Die R1C1-Formel.
### convertR1C1FormulaToA1(String r1c1Formula, int row, int column) {#convertR1C1FormulaToA1-java.lang.String-int-int-}
```
public static String convertR1C1FormulaToA1(String r1c1Formula, int row, int column)
```


Konvertiert die r1c1‑Formel der Zelle in die A1‑Formel.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode Worksheet.ConvertFormulaReferenceStyle() . Diese Eigenschaft wird 12 Monate später, seit August 2023, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| r1c1Formula | java.lang.String | Die r1c1-Formel. |
| Zeile | int | Der Zeilenindex der Zelle. |
| Spalte | int | Der Spaltenindex der Zelle. |

**Returns:**
java.lang.String - Die A1-Formel.
### createSafeSheetName(String nameProposal) {#createSafeSheetName-java.lang.String-}
```
public static String createSafeSheetName(String nameProposal)
```


Überprüft den angegebenen Blattnamen und erstellt bei Bedarf einen gültigen. Wenn der angegebene Blattname den Regeln für Excel-Blattnamen entspricht, wird er zurückgegeben. Andernfalls wird die Zeichenkette abgeschnitten, wenn die Länge das Limit überschreitet, und ungültige Zeichen werden durch ' ' ersetzt, dann wird der wiederhergestellte Zeichenkettenwert zurückgegeben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| nameProposal | java.lang.String | zu verwendender Blattname |

**Returns:**
java.lang.String -
### createSafeSheetName(String nameProposal, char replaceChar) {#createSafeSheetName-java.lang.String-char-}
```
public static String createSafeSheetName(String nameProposal, char replaceChar)
```


Überprüft den angegebenen Blattnamen und erstellt bei Bedarf einen gültigen. Wenn der angegebene Blattname den Regeln für Excel-Blattnamen entspricht, wird er zurückgegeben. Andernfalls wird die Zeichenkette abgeschnitten, wenn die Länge das Limit überschreitet, und ungültige Zeichen werden durch das angegebene Zeichen ersetzt, dann wird der wiederhergestellte Zeichenkettenwert zurückgegeben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| nameProposal | java.lang.String | zu verwendender Blattname |
| replaceChar | char | Zeichen, das zum Ersetzen ungültiger Zeichen im angegebenen Blattnamen verwendet wird |

**Returns:**
java.lang.String -
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
### getAltStartPath() {#getAltStartPath--}
```
public static String getAltStartPath()
```


Ermittelt den alternativen Startpfad, auf den sich einige externe Formelbezüge beziehen.

**Returns:**
java.lang.String
### getCacheFolder() {#getCacheFolder--}
```
public static String getCacheFolder()
```


Ermittelt den Ordner für temporäre Dateien, die als Daten‑Cache verwendet werden können.

**Remarks**

Cache-Dateien werden im Allgemeinen für einige Funktionen zur Speicherleistungsoptimierung verwendet, z. B. zum Speichern großer Datensätze in einer xls-Datei oder beim Verwenden des Speichermodus mit Dateicache für das Zellenmodell.

**Returns:**
java.lang.String - Ordner für Cache-Dateien, der angegeben wurde. Wenn keiner angegeben wurde, wird null zurückgegeben und bei Bedarf der temporäre Pfad des Systems verwendet.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCustomImplementationFactory() {#getCustomImplementationFactory--}
```
public static CustomImplementationFactory getCustomImplementationFactory()
```


Ermittelt die Fabrik zur Erstellung von Instanzen mit spezieller Implementierung.

**Returns:**
[CustomImplementationFactory](../../com.aspose.cells/customimplementationfactory)
### getDPI() {#getDPI--}
```
public static double getDPI()
```


Ermittelt die DPI des Geräts.

**Remarks**

**Returns:**
double
### getDateTimeFromDouble(double doubleValue, boolean date1904) {#getDateTimeFromDouble-double-boolean-}
```
public static DateTime getDateTimeFromDouble(double doubleValue, boolean date1904)
```


Konvertiert den Double‑Wert in den Datums‑Zeit‑Wert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| doubleValue | double | Der double-Wert. |
| date1904 | boolean | Datum‑1904‑System. |

**Returns:**
[DateTime](../../com.aspose.cells/datetime) - 
### getDoubleFromDateTime(DateTime dateTime, boolean date1904) {#getDoubleFromDateTime-com.aspose.cells.DateTime-boolean-}
```
public static double getDoubleFromDateTime(DateTime dateTime, boolean date1904)
```


Konvertiert das Datum/Zeit in einen Double‑Wert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dateTime | [DateTime](../../com.aspose.cells/datetime) | Das Datum und die Uhrzeit. |
| date1904 | boolean | Datum‑1904‑System. |

**Returns:**
double -
### getLibraryPath() {#getLibraryPath--}
```
public static String getLibraryPath()
```


Ermittelt den Bibliothekspfad, auf den sich einige externe Formelbezüge beziehen.

**Returns:**
java.lang.String
### getSignificantDigits() {#getSignificantDigits--}
```
public static int getSignificantDigits()
```


Gibt die Anzahl signifikanter Stellen zurück. Der Standardwert ist 17.

**Remarks**

Kann jetzt nur 15 oder 17 sein. HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen [getSignificantDigitsType()](../../com.aspose.cells/cellshelper\#getSignificantDigitsType--). Diese Eigenschaft wird 12 Monate später, seit Juni 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Returns:**
int
### getSignificantDigitsType() {#getSignificantDigitsType--}
```
public static int getSignificantDigitsType()
```


Gibt den Standardtyp signifikanter Stellen für die Ausgabe numerischer Werte zurück. Der Standardwert ist [SignificantDigitsType.G\_17](../../com.aspose.cells/significantdigitstype\#G-17).

Siehe [SignificantDigitsType](../../com.aspose.cells/significantdigitstype).

**Returns:**
int
### getStartupPath() {#getStartupPath--}
```
public static String getStartupPath()
```


Ermittelt den Startpfad, auf den sich einige externe Formelbezüge beziehen.

**Returns:**
java.lang.String
### getTextWidth(String text, Font font, double scaling) {#getTextWidth-java.lang.String-com.aspose.cells.Font-double-}
```
public static double getTextWidth(String text, Font font, double scaling)
```


Ermittelt die Textbreite in Punkten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Text | java.lang.String | Der Text. |
| font | [Font](../../com.aspose.cells/font) | Die Schriftart des Textes. |
| Skalierung | double | Die Skalierung des Textes. |

**Returns:**
double -
### getUsedColors(Workbook workbook) {#getUsedColors-com.aspose.cells.Workbook-}
```
public static Color[] getUsedColors(Workbook workbook)
```


Ermittelt alle im Arbeitsbuch verwendeten Farben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| workbook | [Workbook](../../com.aspose.cells/workbook) | Das Arbeitsmappenobjekt. |

**Returns:**
com.aspose.cells.Color[] - Die verwendeten Farben.
### getVersion() {#getVersion--}
```
public static String getVersion()
```


Ermittelt die Release‑Version.

**Returns:**
java.lang.String - Die Release-Version.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCloudPlatform() {#isCloudPlatform--}
```
public static boolean isCloudPlatform()
```


Bitte setzen Sie diese Eigenschaft auf True, wenn Sie auf einer Cloud‑Plattform wie Azure, AWSLambda usw. ausführen,

**Returns:**
boolean
### mergeFiles(String[] files, String cachedFile, String destFile) {#mergeFiles-java.lang.String---java.lang.String-java.lang.String-}
```
public static void mergeFiles(String[] files, String cachedFile, String destFile)
```


Führt einige große XLS‑Dateien zu einer XLS‑Datei zusammen.

**Remarks**

Diese Methode unterstützt nur das Zusammenführen von Daten, Stil und Formeln in die neue Datei. Die zwischengespeicherte Datei wird verwendet, um einige temporäre Daten zu speichern.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Dateien | java.lang.String[] | Die Dateien. |
| cachedFile | java.lang.String | Die zwischengespeicherte Datei. |
| destFile | java.lang.String | Die Ziel-Datei. |

### needQuoteInFormula(String sheetName) {#needQuoteInFormula-java.lang.String-}
```
public static boolean needQuoteInFormula(String sheetName)
```


Gibt an, ob der Blattname in einfache Anführungszeichen eingeschlossen werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetName | java.lang.String | Der Name des Blatts |

**Returns:**
boolean -
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### rowIndexToName(int row) {#rowIndexToName-int-}
```
public static String rowIndexToName(int row)
```


Ermittelt den Zeilennamen anhand des Zeilenindex.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex. |

**Returns:**
java.lang.String - Name der Zeile.
### rowNameToIndex(String rowName) {#rowNameToIndex-java.lang.String-}
```
public static int rowNameToIndex(String rowName)
```


Ermittelt den Zeilenindex anhand des Zeilennamens.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowName | java.lang.String | Zeilenname. |

**Returns:**
int - Zeilenindex.
### setAltStartPath(String value) {#setAltStartPath-java.lang.String-}
```
public static void setAltStartPath(String value)
```


Legt den alternativen Startpfad fest, auf den sich einige externe Formelbezüge beziehen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setCacheFolder(String cache) {#setCacheFolder-java.lang.String-}
```
public static void setCacheFolder(String cache)
```


Legt den Ordner für temporäre Dateien fest, die als Daten-Cache verwendet werden können.

**Remarks**

Cache-Dateien werden im Allgemeinen für einige Funktionen zur Speicherleistungsoptimierung verwendet, z. B. zum Speichern großer Datensätze in einer xls-Datei oder beim Verwenden des Speichermodus mit Dateicache für das Zellenmodell.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Cache | java.lang.String | Ordner für temporäre Dateien, die als Daten-Cache verwendet werden können. |

### setCloudPlatform(boolean value) {#setCloudPlatform-boolean-}
```
public static void setCloudPlatform(boolean value)
```


Bitte setzen Sie diese Eigenschaft auf True, wenn Sie auf einer Cloud‑Plattform wie Azure, AWSLambda usw. ausführen,

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setCustomImplementationFactory(CustomImplementationFactory value) {#setCustomImplementationFactory-com.aspose.cells.CustomImplementationFactory-}
```
public static void setCustomImplementationFactory(CustomImplementationFactory value)
```


Legt die Fabrik zum Erzeugen von Instanzen mit spezieller Implementierung fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [CustomImplementationFactory](../../com.aspose.cells/customimplementationfactory) |  |

### setDPI(double value) {#setDPI-double-}
```
public static void setDPI(double value)
```


Ermittelt die DPI des Geräts.

**Remarks**

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setLibraryPath(String value) {#setLibraryPath-java.lang.String-}
```
public static void setLibraryPath(String value)
```


Legt den Bibliothekspfad fest, auf den sich einige externe Formelbezüge beziehen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setSignificantDigits(int value) {#setSignificantDigits-int-}
```
public static void setSignificantDigits(int value)
```


Legt die Anzahl signifikanter Stellen fest. Der Standardwert ist 17.

**Remarks**

Kann jetzt nur 15 oder 17 sein. HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen [getSignificantDigitsType()](../../com.aspose.cells/cellshelper\#getSignificantDigitsType--). Diese Eigenschaft wird 12 Monate später, seit Juni 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setSignificantDigitsType(int value) {#setSignificantDigitsType-int-}
```
public static void setSignificantDigitsType(int value)
```


Legt den Standardtyp signifikanter Stellen für die Ausgabe numerischer Werte fest. Der Standardwert ist [SignificantDigitsType.G\_17](../../com.aspose.cells/significantdigitstype\#G-17).

Siehe [SignificantDigitsType](../../com.aspose.cells/significantdigitstype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setStartupPath(String value) {#setStartupPath-java.lang.String-}
```
public static void setStartupPath(String value)
```


Legt den Startpfad fest, auf den sich einige externe Formelbezüge beziehen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

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

