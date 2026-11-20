---
title: "Workbook"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt ein Root-Objekt zum Erstellen einer Excel-Tabelle dar."
type: docs
url: /de/java/com.aspose.cells/workbook/
---

**Inheritance:**
java.lang.Object
```
public class Workbook
```

Stellt ein Root-Objekt zum Erstellen einer Excel-Tabelle dar.

**Remarks**

Die Workbook‑Klasse bezeichnet eine Excel‑Tabelle. Jede Tabelle kann mehrere Arbeitsblätter enthalten. Die Grundfunktion der Klasse besteht darin, native Excel‑Dateien zu öffnen und zu speichern. Die Klasse verfügt über erweiterte Funktionen wie das Kopieren von Daten aus anderen Workbooks, das Kombinieren zweier Workbooks, das Konvertieren von Excel zu PDF, das Rendern von Excel zu Bild und das Schützen der Excel‑Tabelle.

**Example**

Das folgende Beispiel lädt ein Workbook aus einer Excel‑Datei namens designer.xls und macht die horizontalen und vertikalen Bildlaufleisten unsichtbar. Anschließend ersetzt es zwei Zeichenfolgenwerte jeweils durch einen Integer‑Wert und einen Zeichenfolgenwert innerhalb der Tabelle und speichert schließlich das Workbook als Excel‑xlsx‑Datei.

```
         //Open a designer file
         String designerFile = "designer.xls";
         Workbook workbook = new Workbook(designerFile);
 
         //Set scroll bars
         workbook.getSettings().setHScrollBarVisible(false);
         workbook.getSettings().setVScrollBarVisible(false);
 
         //Replace the placeholder string with new values
         int newInt = 100;
         workbook.replace("OldInt", newInt);
 
         String newString = "Hello!";
         workbook.replace("OldString", newString);
         workbook.save("result.xlsx");
```
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [Workbook()](#Workbook--) | Initialisiert eine neue Instanz der [Workbook](../../com.aspose.cells/workbook)-Klasse. |
| [Workbook(int fileFormatType)](#Workbook-int-) | Initialisiert eine neue Instanz der [Workbook](../../com.aspose.cells/workbook)-Klasse. |
| [Workbook(LoadOptions loadOptions)](#Workbook-com.aspose.cells.LoadOptions-) | Initialisiert eine neue leere Instanz der [Workbook](../../com.aspose.cells/workbook)-Klasse mit Optionen |
| [Workbook(String file)](#Workbook-java.lang.String-) | Initialisiert eine neue Instanz der [Workbook](../../com.aspose.cells/workbook)-Klasse und öffnet eine Datei. |
| [Workbook(InputStream stream)](#Workbook-java.io.InputStream-) | Initialisiert eine neue Instanz der [Workbook](../../com.aspose.cells/workbook)-Klasse und öffnet einen Stream. |
| [Workbook(String file, LoadOptions loadOptions)](#Workbook-java.lang.String-com.aspose.cells.LoadOptions-) | Initialisiert eine neue Instanz der [Workbook](../../com.aspose.cells/workbook)-Klasse und öffnet eine Datei. |
| [Workbook(InputStream stream, LoadOptions loadOptions)](#Workbook-java.io.InputStream-com.aspose.cells.LoadOptions-) | Initialisiert eine neue Instanz der [Workbook](../../com.aspose.cells/workbook)-Klasse und öffnet einen Stream |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [acceptAllRevisions()](#acceptAllRevisions--) | Akzeptiert alle nachverfolgten Änderungen im Workbook. |
| [addDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)](#addDigitalSignature-com.aspose.cells.DigitalSignatureCollection-) | Fügt einer OOXML‑Tabellendatei (Excel2007 und neuer) eine digitale Signatur hinzu. |
| [calculateFormula()](#calculateFormula--) | Berechnet das Ergebnis von Formeln. |
| [calculateFormula(boolean ignoreError)](#calculateFormula-boolean-) | Berechnet das Ergebnis von Formeln. |
| [calculateFormula(CalculationOptions options)](#calculateFormula-com.aspose.cells.CalculationOptions-) | Formeln in diesem Workbook werden berechnet. |
| [changePalette(Color color, int index)](#changePalette-com.aspose.cells.Color-int-) | Ändert die Palette für die Tabellenkalkulation am angegebenen Index. |
| [closeAccessCache(int opts)](#closeAccessCache-int-) | Schließt die Sitzung, die Caches verwendet, um auf Daten zuzugreifen. |
| [combine(Workbook secondWorkbook)](#combine-com.aspose.cells.Workbook-) | Kombiniert ein weiteres Workbook-Objekt. |
| [copy(Workbook source)](#copy-com.aspose.cells.Workbook-) | Kopiert Daten aus einem Quell-Workbook-Objekt. |
| [copy(Workbook source, CopyOptions copyOptions)](#copy-com.aspose.cells.Workbook-com.aspose.cells.CopyOptions-) | Kopiert ein weiteres Workbook-Objekt. |
| [copyTheme(Workbook source)](#copyTheme-com.aspose.cells.Workbook-) | Kopiert das Theme aus einer anderen Arbeitsmappe. |
| [createBuiltinStyle(int type)](#createBuiltinStyle-int-) | Erstellt einen integrierten Stil anhand des angegebenen Typs. |
| [createCellsColor()](#createCellsColor--) | Erstellt ein [CellsColor](../../com.aspose.cells/cellscolor)-Objekt. |
| [createStyle()](#createStyle--) | Erstellt einen neuen Stil. |
| [createStyle(boolean cloneDefaultStyle)](#createStyle-boolean-) | Erstellt einen neuen Stil. |
| [customTheme(String themeName, Color[] colors)](#customTheme-java.lang.String-com.aspose.cells.Color---) | Passt das Theme an. |
| [dispose()](#dispose--) | Führt anwendungsspezifische Aufgaben aus, die mit dem Freigeben, Freisetzen oder Zurücksetzen nicht verwalteter Ressourcen verbunden sind. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportXml(String mapName, OutputStream stream)](#exportXml-java.lang.String-java.io.OutputStream-) | Exportiert XML-Daten, die durch die angegebene XML-Map verknüpft sind. |
| [exportXml(String mapName, String path)](#exportXml-java.lang.String-java.lang.String-) | Exportiert XML-Daten, die durch die angegebene XML-Map verknüpft sind. |
| [getAbsolutePath()](#getAbsolutePath--) | Ermittelt den absoluten Pfad der Datei. |
| [getBuiltInDocumentProperties()](#getBuiltInDocumentProperties--) | Gibt eine [DocumentProperty](../../com.aspose.cells/documentproperty)-Sammlung zurück, die alle integrierten Dokumenteigenschaften der Kalkulationstabelle darstellt. |
| [getCellsDataTableFactory()](#getCellsDataTableFactory--) | Ermittelt die Fabrik zum Erstellen von ICellsDataTable aus benutzerdefinierten Objekten. |
| [getClass()](#getClass--) |  |
| [getColors()](#getColors--) | Gibt die Farben in der Palette für die Tabellenkalkulation zurück. |
| [getContentTypeProperties()](#getContentTypeProperties--) | Ermittelt die Liste der [ContentTypeProperty](../../com.aspose.cells/contenttypeproperty)-Objekte in der Arbeitsmappe. |
| [getCountOfStylesInPool()](#getCountOfStylesInPool--) | Ermittelt die Anzahl der Stile im Stil-Pool. |
| [getCustomDocumentProperties()](#getCustomDocumentProperties--) | Gibt eine [DocumentProperty](../../com.aspose.cells/documentproperty)-Sammlung zurück, die alle benutzerdefinierten Dokumenteigenschaften der Kalkulationstabelle darstellt. |
| [getCustomXmlParts()](#getCustomXmlParts--) | Stellt einen Custom XML Data Storage Part dar (benutzerdefinierte XML-Daten innerhalb eines Pakets). |
| [getDataConnections()](#getDataConnections--) | Ermittelt die [ExternalConnection](../../com.aspose.cells/externalconnection)-Sammlung. |
| [getDataMashup()](#getDataMashup--) | Ermittelt Mashup-Daten. |
| [getDataModel()](#getDataModel--) | Ermittelt das Datenmodell in der Arbeitsmappe. |
| [getDataSorter()](#getDataSorter--) | Ermittelt ein DataSorter-Objekt zum Sortieren von Daten. |
| [getDefaultStyle()](#getDefaultStyle--) | Ermittelt das Standard-[Style](../../com.aspose.cells/style)-Objekt der Arbeitsmappe. |
| [getDigitalSignature()](#getDigitalSignature--) | Ermittelt die digitale Signatur aus der Datei. |
| [getFileFormat()](#getFileFormat--) | Ermittelt das Dateiformat. |
| [getFileName()](#getFileName--) | Ermittelt den aktuellen Dateinamen. |
| [getFonts()](#getFonts--) | Ermittelt alle Schriftarten im Stil-Pool. |
| [getInterruptMonitor()](#getInterruptMonitor--) | Liest den Unterbrechungsmonitor. |
| [getMatchingColor(Color rawColor)](#getMatchingColor-com.aspose.cells.Color-) | Findet die am besten passende Farbe in der aktuellen Palette. |
| [getNamedStyle(String name)](#getNamedStyle-java.lang.String-) | Ruft den benannten Stil im Stilpool ab. |
| [getRibbonXml()](#getRibbonXml--) | Ruft die XML-Datei ab, die die Ribbon-Benutzeroberfläche definiert. |
| [getSettings()](#getSettings--) | Stellt die Arbeitsmappeneinstellungen dar. |
| [getStyleInPool(int index)](#getStyleInPool-int-) | Ruft den Stil im Stilpool ab. |
| [getTheme()](#getTheme--) | Ruft den Namen des Designs ab. |
| [getThemeColor(int type)](#getThemeColor-int-) | Ruft die Designfarbe ab. |
| [getVbaProject()](#getVbaProject--) | Ruft das [getVbaProject()](../../com.aspose.cells/workbook\#getVbaProject--) in einer Tabellenkalkulation ab. |
| [getWorksheets()](#getWorksheets--) | Ruft die [WorksheetCollection](../../com.aspose.cells/worksheetcollection)-Sammlung in der Tabellenkalkulation ab. |
| [hasCustomFunction()](#hasCustomFunction--) | Erkennt, ob in dieser Arbeitsmappe benutzerdefinierte Funktionen verwendet werden, z. B. in Zellformeln oder definierten Namen... |
| [hasExernalLinks()](#hasExernalLinks--) | Gibt an, ob diese Arbeitsmappe externe Verknüpfungen zu anderen Datenquellen enthält. |
| [hasMacro()](#hasMacro--) | Gibt an, ob diese Tabellenkalkulation Makros/VBA enthält. |
| [hasRevisions()](#hasRevisions--) | Ermittelt, ob die Arbeitsmappe nachverfolgte Änderungen enthält |
| [hashCode()](#hashCode--) |  |
| [importXml(InputStream stream, String sheetName, int row, int col)](#importXml-java.io.InputStream-java.lang.String-int-int-) | Importiert/Aktualisiert eine XML-Datendatei in die Arbeitsmappe. |
| [importXml(String url, String sheetName, int row, int col)](#importXml-java.lang.String-java.lang.String-int-int-) | Importiert/Aktualisiert eine XML-Datendatei in die Arbeitsmappe. |
| [isColorInPalette(Color color)](#isColorInPalette-com.aspose.cells.Color-) | Prüft, ob eine Farbe in der Palette der Tabellenkalkulation enthalten ist. |
| [isDigitallySigned()](#isDigitallySigned--) | Gibt an, ob diese Tabellenkalkulation digital signiert ist. |
| [isLicensed()](#isLicensed--) | Gibt an, ob eine Lizenz festgelegt ist. |
| [isWorkbookProtectedWithPassword()](#isWorkbookProtectedWithPassword--) | Gibt an, ob Struktur oder Fenster mit einem Kennwort geschützt ist. |
| [mergeNamedStyles(Workbook source)](#mergeNamedStyles-com.aspose.cells.Workbook-) | Führt benannte Stile aus der anderen Excel-Datei zusammen. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [parseFormulas(boolean ignoreError)](#parseFormulas-boolean-) | Parst alle Formeln, die beim Laden aus einer Vorlagendatei oder beim Setzen in eine Zelle nicht geparst wurden. |
| [protect(int protectionType, String password)](#protect-int-java.lang.String-) | Schützt eine Arbeitsmappe. |
| [protectSharedWorkbook(String password)](#protectSharedWorkbook-java.lang.String-) | Schützt eine freigegebene Arbeitsmappe. |
| [refreshAll()](#refreshAll--) | Aktualisiert verknüpfte Formen, alle Pivot-Tabellen und Diagramme mit der Pivot-Quelle. |
| [refreshDynamicArrayFormulas(boolean calculate)](#refreshDynamicArrayFormulas-boolean-) | Aktualisiert dynamische Array-Formeln (erweitern sich in einen neuen Bereich benachbarter Zellen gemäß den aktuellen Daten). Andere Formeln in der Arbeitsmappe werden nicht rekursiv berechnet, selbst wenn sie von dynamischen Array-Formeln verwendet werden. |
| [refreshDynamicArrayFormulas(boolean calculate, CalculationOptions copts)](#refreshDynamicArrayFormulas-boolean-com.aspose.cells.CalculationOptions-) | Aktualisiert dynamische Array-Formeln (erweitern sich in einen neuen Bereich benachbarter Zellen gemäß den aktuellen Daten) |
| [removeDigitalSignature()](#removeDigitalSignature--) | Entfernt die digitale Signatur aus dieser Tabellenkalkulation. |
| [removeExternalLinks()](#removeExternalLinks--) | Entfernt alle externen Links in der Arbeitsmappe. |
| [removeMacro()](#removeMacro--) | Entfernt VBA/Makro aus dieser Tabellenkalkulation. |
| [removePersonalInformation()](#removePersonalInformation--) | Entfernt persönliche Informationen. |
| [removeUnusedStyles()](#removeUnusedStyles--) | Entfernt alle ungenutzten Stile. |
| [replace(boolean boolValue, Object newValue)](#replace-boolean-java.lang.Object-) | Ersetzt die Werte der Zellen durch neue Daten. |
| [replace(int intValue, Object newValue)](#replace-int-java.lang.Object-) | Ersetzt die Werte der Zellen durch neue Daten. |
| [replace(String placeHolder, double newValue)](#replace-java.lang.String-double-) | Ersetzt den Wert einer Zelle durch ein neues Double. |
| [replace(String placeHolder, double[] newValues, boolean isVertical)](#replace-java.lang.String-double---boolean-) | Ersetzt die Werte der Zellen durch ein Double-Array. |
| [replace(String placeHolder, int newValue)](#replace-java.lang.String-int-) | Ersetzt den Wert einer Zelle durch einen neuen Integer. |
| [replace(String placeHolder, int[] newValues, boolean isVertical)](#replace-java.lang.String-int---boolean-) | Ersetzt die Werte der Zellen durch ein Integer-Array. |
| [replace(String placeHolder, String newValue)](#replace-java.lang.String-java.lang.String-) | Ersetzt den Wert einer Zelle durch einen neuen String. |
| [replace(String placeHolder, String newValue, ReplaceOptions options)](#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-) | Ersetzt den Wert einer Zelle durch einen neuen String. |
| [replace(String placeHolder, String[] newValues, boolean isVertical)](#replace-java.lang.String-java.lang.String---boolean-) | Ersetzt den Wert einer Zelle durch ein neues String-Array. |
| [save(OutputStream stream, SaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.cells.SaveOptions-) | Speichert die Arbeitsmappe in den Stream. |
| [save(OutputStream stream, int saveFormat)](#save-java.io.OutputStream-int-) | Speichert die Arbeitsmappe in den Stream. |
| [save(String fileName)](#save-java.lang.String-) | Speichert die Arbeitsmappe auf die Festplatte. |
| [save(String fileName, SaveOptions saveOptions)](#save-java.lang.String-com.aspose.cells.SaveOptions-) | Speichert die Arbeitsmappe auf die Festplatte. |
| [save(String fileName, int saveFormat)](#save-java.lang.String-int-) | Speichert die Arbeitsmappe auf die Festplatte. |
| [setAbsolutePath(String value)](#setAbsolutePath-java.lang.String-) | Legt den absoluten Pfad der Datei fest. |
| [setDefaultStyle(Style value)](#setDefaultStyle-com.aspose.cells.Style-) | Legt das Standard-[Style](../../com.aspose.cells/style)-Objekt der Arbeitsmappe fest. |
| [setDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)](#setDigitalSignature-com.aspose.cells.DigitalSignatureCollection-) | Setzt die digitale Signatur für eine Tabellenkalkulationsdatei (Excel2007 und neuer). |
| [setEncryptionOptions(int encryptionType, int keyLength)](#setEncryptionOptions-int-int-) | Verschlüsselungsoptionen festlegen. |
| [setFileFormat(int value)](#setFileFormat-int-) | Legt das Dateiformat fest. |
| [setFileName(String value)](#setFileName-java.lang.String-) | Legt den aktuellen Dateinamen fest. |
| [setInterruptMonitor(AbstractInterruptMonitor value)](#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-) | Legt den Interrupt‑Monitor fest. |
| [setRibbonXml(String value)](#setRibbonXml-java.lang.String-) | Legt die XML-Datei fest, die die Ribbon-Benutzeroberfläche definiert. |
| [setThemeColor(int type, Color color)](#setThemeColor-int-com.aspose.cells.Color-) | Legt die Themenfarbe fest. |
| [startAccessCache(int opts)](#startAccessCache-int-) | Startet die Sitzung, die Caches zum Zugriff auf Daten verwendet. |
| [toString()](#toString--) |  |
| [unprotect(String password)](#unprotect-java.lang.String-) | Entfernt den Schutz einer Arbeitsmappe. |
| [unprotectSharedWorkbook(String password)](#unprotectSharedWorkbook-java.lang.String-) | Entfernt den Schutz einer freigegebenen Arbeitsmappe. |
| [updateCustomFunctionDefinition(CustomFunctionDefinition definition)](#updateCustomFunctionDefinition-com.aspose.cells.CustomFunctionDefinition-) | Aktualisiert die Definition benutzerdefinierter Funktionen. |
| [updateLinkedDataSource(Workbook[] externalWorkbooks)](#updateLinkedDataSource-com.aspose.cells.Workbook---) | Wenn diese Arbeitsmappe externe Verknüpfungen zu anderen Datenquellen enthält, wird Aspose.Cells versuchen, die neuesten Daten aus den angegebenen Quellen abzurufen. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Workbook() {#Workbook--}
```
public Workbook()
```


Initialisiert eine neue Instanz der [Workbook](../../com.aspose.cells/workbook)-Klasse.

**Remarks**

Der Standard-Dateiformattyp ist Xlsx. Wenn Sie andere Dateitypen erstellen möchten, verwenden Sie bitte Workbook(FileFormatType).

**Example**

Der folgende Code zeigt, wie der Workbook-Konstruktor verwendet wird, um eine neue Instanz der Klasse zu erstellen und zu initialisieren.

```
         Workbook workbook = new Workbook();
```

### Workbook(int fileFormatType) {#Workbook-int-}
```
public Workbook(int fileFormatType)
```


Initialisiert eine neue Instanz der [Workbook](../../com.aspose.cells/workbook)-Klasse.

**Remarks**

Der Standard-Dateiformattyp ist Excel97To2003.

**Example**

Der folgende Code zeigt, wie der Workbook-Konstruktor verwendet wird, um eine neue Instanz der Klasse mit verschiedenen Dateiformattypen zu erstellen und zu initialisieren.

```
         Workbook workbook = new Workbook(FileFormatType.XLSX);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileFormatType | int | [FileFormatType](../../com.aspose.cells/fileformattype). Das neue Dateiformat. |

### Workbook(LoadOptions loadOptions) {#Workbook-com.aspose.cells.LoadOptions-}
```
public Workbook(LoadOptions loadOptions)
```


Initialisiert eine neue leere Instanz der [Workbook](../../com.aspose.cells/workbook)-Klasse mit Optionen

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| loadOptions | [LoadOptions](../../com.aspose.cells/loadoptions) | Die Optionen. |

### Workbook(String file) {#Workbook-java.lang.String-}
```
public Workbook(String file)
```


Initialisiert eine neue Instanz der [Workbook](../../com.aspose.cells/workbook)-Klasse und öffnet eine Datei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Datei | java.lang.String | Der Dateiname. |

### Workbook(InputStream stream) {#Workbook-java.io.InputStream-}
```
public Workbook(InputStream stream)
```


Initialisiert eine neue Instanz der [Workbook](../../com.aspose.cells/workbook)-Klasse und öffnet einen Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.InputStream | Der Stream. |

### Workbook(String file, LoadOptions loadOptions) {#Workbook-java.lang.String-com.aspose.cells.LoadOptions-}
```
public Workbook(String file, LoadOptions loadOptions)
```


Initialisiert eine neue Instanz der [Workbook](../../com.aspose.cells/workbook)-Klasse und öffnet eine Datei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Datei | java.lang.String | Der Dateiname. |
| loadOptions | [LoadOptions](../../com.aspose.cells/loadoptions) | Die Ladeoptionen |

### Workbook(InputStream stream, LoadOptions loadOptions) {#Workbook-java.io.InputStream-com.aspose.cells.LoadOptions-}
```
public Workbook(InputStream stream, LoadOptions loadOptions)
```


Initialisiert eine neue Instanz der [Workbook](../../com.aspose.cells/workbook)-Klasse und öffnet einen Stream

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.InputStream | Der Stream. |
| loadOptions | [LoadOptions](../../com.aspose.cells/loadoptions) | Die Ladeoptionen |

### acceptAllRevisions() {#acceptAllRevisions--}
```
public void acceptAllRevisions()
```


Akzeptiert alle nachverfolgten Änderungen im Workbook.

### addDigitalSignature(DigitalSignatureCollection digitalSignatureCollection) {#addDigitalSignature-com.aspose.cells.DigitalSignatureCollection-}
```
public void addDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```


Fügt einer OOXML‑Tabellendatei (Excel2007 und neuer) eine digitale Signatur hinzu.

**Remarks**

Unterstützt nur das Hinzufügen einer Xmldsig-Digitalunterschrift zu einer OOXML-Tabellendatei

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| digitalSignatureCollection | [DigitalSignatureCollection](../../com.aspose.cells/digitalsignaturecollection) |  |

### calculateFormula() {#calculateFormula--}
```
public void calculateFormula()
```


Berechnet das Ergebnis von Formeln.

**Remarks**

Für alle unterstützten Formeln siehe die Liste unter https://docs.aspose.com/display/cellsnet/Supported+Formula+Functions

### calculateFormula(boolean ignoreError) {#calculateFormula-boolean-}
```
public void calculateFormula(boolean ignoreError)
```


Berechnet das Ergebnis von Formeln.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ignoreError | boolean | Gibt an, ob Fehler bei der Berechnung von Formeln ausgeblendet werden sollen. Der Fehler kann eine nicht unterstützte Funktion, externe Verknüpfungen usw. sein. |

### calculateFormula(CalculationOptions options) {#calculateFormula-com.aspose.cells.CalculationOptions-}
```
public void calculateFormula(CalculationOptions options)
```


Formeln in diesem Workbook werden berechnet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| options | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Optionen für die Berechnung |

### changePalette(Color color, int index) {#changePalette-com.aspose.cells.Color-int-}
```
public void changePalette(Color color, int index)
```


Ändert die Palette für die Tabellenkalkulation am angegebenen Index.

**Remarks**

Die Palette hat 56 Einträge, jeder dargestellt durch einen RGB-Wert.

Wenn Sie eine Farbe festlegen, die nicht in der Palette enthalten ist, wird sie nicht wirksam.

Wenn Sie also eine benutzerdefinierte Farbe festlegen möchten, ändern Sie zuerst die Palette.

Die folgende ist die Standardfarbpalette.

| Color | Rot | Grün | Blau |
| ------- | --- | ----- | ---- |
| Schwarz | 0 | 0 | 0 |
| Weiß | 255 | 255 | 255 |
| Rot | 255 | 0 | 0 |
| Limette | 0 | 255 | 0 |
| Blau | 0 | 0 | 255 |
| Gelb | 255 | 255 | 0 |
| Magenta | 255 | 0 | 255 |
| Cyan | 0 | 255 | 255 |
| Kastanienbraun | 128 | 0 | 0 |
| Grün | 0 | 128 | 0 |
| Marineblau | 0 | 0 | 128 |
| Oliv | 128 | 128 | 0 |
| Lila | 128 | 0 | 128 |
| Türkis | 0 | 128 | 128 |
| Silber | 192 | 192 | 192 |
| Grau | 128 | 128 | 128 |
| Farbe17 | 153 | 153 | 255 |
| Farbe18 | 153 | 51 | 102 |
| Farbe19 | 255 | 255 | 204 |
| Farbe20 | 204 | 255 | 255 |
| Farbe21 | 102 | 0 | 102 |
| Farbe22 | 255 | 128 | 128 |
| Farbe23 | 0 | 102 | 204 |
| Farbe24 | 204 | 204 | 255 |
| Farbe25 | 0 | 0 | 128 |
| Farbe26 | 255 | 0 | 255 |
| Farbe27 | 255 | 255 | 0 |
| Farbe28 | 0 | 255 | 255 |
| Farbe29 | 128 | 0 | 128 |
| Farbe30 | 128 | 0 | 0 |
| Farbe31 | 0 | 128 | 128 |
| Farbe32 | 0 | 0 | 255 |
| Farbe33 | 0 | 204 | 255 |
| Farbe34 | 204 | 255 | 255 |
| Farbe35 | 204 | 255 | 204 |
| Farbe36 | 255 | 255 | 153 |
| Farbe37 | 153 | 204 | 255 |
| Farbe38 | 255 | 153 | 204 |
| Farbe39 | 204 | 153 | 255 |
| Farbe40 | 255 | 204 | 153 |
| Farbe41 | 51 | 102 | 255 |
| Farbe42 | 51 | 204 | 204 |
| Farbe43 | 153 | 204 | 0 |
| Farbe44 | 255 | 204 | 0 |
| Farbe45 | 255 | 153 | 0 |
| Farbe46 | 255 | 102 | 0 |
| Farbe47 | 102 | 102 | 153 |
| Farbe48 | 150 | 150 | 150 |
| Farbe49 | 0 | 51 | 102 |
| Color50 | 51 | 153 | 102 |
| Color51 | 0 | 51 | 0 |
| Color52 | 51 | 51 | 0 |
| Color53 | 153 | 51 | 0 |
| Color54 | 153 | 51 | 102 |
| Color55 | 51 | 51 | 153 |
| Color56 | 51 | 51 | 51 |

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Farbstruktur. |
| Index | int | Palettenindex, 0 - 55. |

### closeAccessCache(int opts) {#closeAccessCache-int-}
```
public void closeAccessCache(int opts)
```


Schließt die Sitzung, die Caches verwendet, um auf Daten zuzugreifen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| opts | int | [AccessCacheOptions](../../com.aspose.cells/accesscacheoptions). Optionen für den Datenzugriff |

### combine(Workbook secondWorkbook) {#combine-com.aspose.cells.Workbook-}
```
public void combine(Workbook secondWorkbook)
```


Kombiniert ein weiteres Workbook-Objekt.

**Remarks**

Excel, ODS, CSV und andere Dateien zu einer Datei zusammenführen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| secondWorkbook | [Workbook](../../com.aspose.cells/workbook) | Ein weiteres Workbook-Objekt. |

### copy(Workbook source) {#copy-com.aspose.cells.Workbook-}
```
public void copy(Workbook source)
```


Kopiert Daten aus einem Quell-Workbook-Objekt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | [Workbook](../../com.aspose.cells/workbook) | Quell-Workbook-Objekt. |

### copy(Workbook source, CopyOptions copyOptions) {#copy-com.aspose.cells.Workbook-com.aspose.cells.CopyOptions-}
```
public void copy(Workbook source, CopyOptions copyOptions)
```


Kopiert ein weiteres Workbook-Objekt.

**Remarks**

Es ist sehr einfach, eine Excel-Datei zu klonen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | [Workbook](../../com.aspose.cells/workbook) | Quell-Workbook-Objekt. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | Die Optionen zum Kopieren eines anderen Workbooks. |

### copyTheme(Workbook source) {#copyTheme-com.aspose.cells.Workbook-}
```
public void copyTheme(Workbook source)
```


Kopiert das Theme aus einer anderen Arbeitsmappe.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | [Workbook](../../com.aspose.cells/workbook) | Quell-Workbook. |

### createBuiltinStyle(int type) {#createBuiltinStyle-int-}
```
public Style createBuiltinStyle(int type)
```


Erstellt einen integrierten Stil anhand des angegebenen Typs.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| type | int | [BuiltinStyleType](../../com.aspose.cells/builtinstyletype). Der integrierte Stiltyp. |

**Returns:**
[Style](../../com.aspose.cells/style) - [Style](../../com.aspose.cells/style) object
### createCellsColor() {#createCellsColor--}
```
public CellsColor createCellsColor()
```


Erstellt ein [CellsColor](../../com.aspose.cells/cellscolor)-Objekt.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor) - Returns a [CellsColor](../../com.aspose.cells/cellscolor) object.
### createStyle() {#createStyle--}
```
public Style createStyle()
```


Erstellt einen neuen Stil.

**Returns:**
[Style](../../com.aspose.cells/style) - Returns a style object.
### createStyle(boolean cloneDefaultStyle) {#createStyle-boolean-}
```
public Style createStyle(boolean cloneDefaultStyle)
```


Erstellt einen neuen Stil.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cloneDefaultStyle | boolean | Gibt an, ob der Standardstil geklont wird |

**Returns:**
[Style](../../com.aspose.cells/style) - Returns a style object.
### customTheme(String themeName, Color[] colors) {#customTheme-java.lang.String-com.aspose.cells.Color---}
```
public void customTheme(String themeName, Color[] colors)
```


Passt das Theme an.

**Remarks**

Die Länge der Farben sollte 12 betragen.

| Array-Index | Thema-Typ |
| ----------- | ------------------ |
| 0 | Backgournd1 |
| 1 | Text1 |
| 2 | Hintergrund2 |
| 3 | Text2 |
| 4 | Akzent1 |
| 5 | Akzent2 |
| 6 | Akzent3 |
| 7 | Akzent4 |
| 8 | Akzent5 |
| 9 | Akzent6 |
| 10 | Hyperlink |
| 11 | Verfolgter Hyperlink |

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| themeName | java.lang.String | Der Themenname |
| colors | [Color\[\]](../../com.aspose.cells/color) | Die Themenfarben |

### dispose() {#dispose--}
```
public void dispose()
```


Führt anwendungsspezifische Aufgaben aus, die mit dem Freigeben, Freisetzen oder Zurücksetzen nicht verwalteter Ressourcen verbunden sind.

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
### exportXml(String mapName, OutputStream stream) {#exportXml-java.lang.String-java.io.OutputStream-}
```
public void exportXml(String mapName, OutputStream stream)
```


Exportiert XML-Daten, die durch die angegebene XML-Map verknüpft sind.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| mapName | java.lang.String | Name der XML-Karte, die exportiert werden muss |
| stream | java.io.OutputStream | der Export-Stream |

### exportXml(String mapName, String path) {#exportXml-java.lang.String-java.lang.String-}
```
public void exportXml(String mapName, String path)
```


Exportiert XML-Daten, die durch die angegebene XML-Map verknüpft sind.

**Example**

Der folgende Code exportierte die Daten, die mit der ersten XmlMap verknüpft sind.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         //Make sure that the source xlsx file contains a XmlMap.
         XmlMap xmlMap = wb.getWorksheets().getXmlMaps().get(0);
 
         wb.exportXml(xmlMap.getName(), "output.xml");
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| mapName | java.lang.String | Name der XML-Karte, die exportiert werden muss |
| Pfad | java.lang.String | der Exportpfad |

### getAbsolutePath() {#getAbsolutePath--}
```
public String getAbsolutePath()
```


Ermittelt den absoluten Pfad der Datei.

**Remarks**

Nur für externe Links verwendet.

**Returns:**
java.lang.String
### getBuiltInDocumentProperties() {#getBuiltInDocumentProperties--}
```
public BuiltInDocumentPropertyCollection getBuiltInDocumentProperties()
```


Gibt eine [DocumentProperty](../../com.aspose.cells/documentproperty)-Sammlung zurück, die alle integrierten Dokumenteigenschaften der Kalkulationstabelle darstellt.

**Remarks**

Eine neue Eigenschaft kann nicht zur Liste der integrierten Dokumenteigenschaften hinzugefügt werden. Sie können nur eine integrierte Eigenschaft abrufen und ihren Wert ändern. Die folgende Liste enthält die Namen der integrierten Eigenschaften:

Titel

Betreff

Autor

Stichwörter

Kommentare

Vorlage

Letzter Autor

Revisionsnummer

Anwendungsname

Letztes Druckdatum

Erstellungsdatum

Letzter Speicherzeitpunkt

Gesamte Bearbeitungszeit

Anzahl der Seiten

Anzahl der Wörter

Anzahl der Zeichen

Sicherheit

Kategorie

Format

Manager

Unternehmen

Anzahl der Bytes

Anzahl der Zeilen

Anzahl der Absätze

Anzahl der Folien

Anzahl der Notizen

Anzahl der ausgeblendeten Folien

Anzahl der Multimedia‑Clips

**Example**

```
         Workbook workbook = new Workbook();
         DocumentProperty doc = workbook.getBuiltInDocumentProperties().get("Author");
         doc.setValue("John Smith");
```

**Returns:**
[BuiltInDocumentPropertyCollection](../../com.aspose.cells/builtindocumentpropertycollection)
### getCellsDataTableFactory() {#getCellsDataTableFactory--}
```
public CellsDataTableFactory getCellsDataTableFactory()
```


Ermittelt die Fabrik zum Erstellen von ICellsDataTable aus benutzerdefinierten Objekten.

**Returns:**
[CellsDataTableFactory](../../com.aspose.cells/cellsdatatablefactory)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColors() {#getColors--}
```
public Color[] getColors()
```


Gibt die Farben in der Palette für die Tabellenkalkulation zurück.

**Remarks**

Die Palette hat 56 Einträge, jeder dargestellt durch einen RGB-Wert.

**Returns:**
com.aspose.cells.Color[]
### getContentTypeProperties() {#getContentTypeProperties--}
```
public ContentTypePropertyCollection getContentTypeProperties()
```


Ermittelt die Liste der [ContentTypeProperty](../../com.aspose.cells/contenttypeproperty)-Objekte in der Arbeitsmappe.

**Returns:**
[ContentTypePropertyCollection](../../com.aspose.cells/contenttypepropertycollection)
### getCountOfStylesInPool() {#getCountOfStylesInPool--}
```
public int getCountOfStylesInPool()
```


Ermittelt die Anzahl der Stile im Stil-Pool.

**Returns:**
int
### getCustomDocumentProperties() {#getCustomDocumentProperties--}
```
public CustomDocumentPropertyCollection getCustomDocumentProperties()
```


Gibt eine [DocumentProperty](../../com.aspose.cells/documentproperty)-Sammlung zurück, die alle benutzerdefinierten Dokumenteigenschaften der Kalkulationstabelle darstellt.

**Example**

```
         Workbook excel = new Workbook();
         excel.getCustomDocumentProperties().add("Checked by", "Jane");
```

**Returns:**
[CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection)
### getCustomXmlParts() {#getCustomXmlParts--}
```
public CustomXmlPartCollection getCustomXmlParts()
```


Stellt einen Custom XML Data Storage Part dar (benutzerdefinierte XML-Daten innerhalb eines Pakets).

**Returns:**
[CustomXmlPartCollection](../../com.aspose.cells/customxmlpartcollection)
### getDataConnections() {#getDataConnections--}
```
public ExternalConnectionCollection getDataConnections()
```


Ermittelt die [ExternalConnection](../../com.aspose.cells/externalconnection)-Sammlung.

**Returns:**
[ExternalConnectionCollection](../../com.aspose.cells/externalconnectioncollection)
### getDataMashup() {#getDataMashup--}
```
public DataMashup getDataMashup()
```


Ermittelt Mashup-Daten.

**Returns:**
[DataMashup](../../com.aspose.cells/datamashup)
### getDataModel() {#getDataModel--}
```
public DataModel getDataModel()
```


Ermittelt das Datenmodell in der Arbeitsmappe.

**Returns:**
[DataModel](../../com.aspose.cells/datamodel)
### getDataSorter() {#getDataSorter--}
```
public DataSorter getDataSorter()
```


Ermittelt ein DataSorter-Objekt zum Sortieren von Daten.

**Returns:**
[DataSorter](../../com.aspose.cells/datasorter)
### getDefaultStyle() {#getDefaultStyle--}
```
public Style getDefaultStyle()
```


Ermittelt das Standard-[Style](../../com.aspose.cells/style)-Objekt der Arbeitsmappe.

**Remarks**

Die DefaultStyle-Eigenschaft ist nützlich, um einen Stil für die gesamte Arbeitsmappe zu implementieren.

**Example**

Der folgende Code erstellt und instanziiert eine neue Arbeitsmappe und weist ihr einen Standard-[Style](../../com.aspose.cells/style) zu.

```
         Workbook workbook = new Workbook();
         Style defaultStyle = workbook.getDefaultStyle();
         defaultStyle.getFont().setName("Tahoma");
         workbook.setDefaultStyle(defaultStyle);
```

**Returns:**
[Style](../../com.aspose.cells/style)
### getDigitalSignature() {#getDigitalSignature--}
```
public DigitalSignatureCollection getDigitalSignature()
```


Ermittelt die digitale Signatur aus der Datei.

**Returns:**
[DigitalSignatureCollection](../../com.aspose.cells/digitalsignaturecollection)
### getFileFormat() {#getFileFormat--}
```
public int getFileFormat()
```


Ermittelt das Dateiformat.

Siehe [FileFormatType](../../com.aspose.cells/fileformattype).

**Returns:**
int
### getFileName() {#getFileName--}
```
public String getFileName()
```


Ermittelt den aktuellen Dateinamen.

**Remarks**

Wenn die Datei per Stream geöffnet wird und es externe Formelbezüge gibt, geben Sie bitte den Dateinamen an.

**Returns:**
java.lang.String
### getFonts() {#getFonts--}
```
public Font[] getFonts()
```


Ermittelt alle Schriftarten im Stil-Pool.

**Returns:**
com.aspose.cells.Font[]
### getInterruptMonitor() {#getInterruptMonitor--}
```
public AbstractInterruptMonitor getInterruptMonitor()
```


Liest den Unterbrechungsmonitor.

**Returns:**
[AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor)
### getMatchingColor(Color rawColor) {#getMatchingColor-com.aspose.cells.Color-}
```
public Color getMatchingColor(Color rawColor)
```


Findet die am besten passende Farbe in der aktuellen Palette.

**Remarks**

In der Farbpalette von Excel 97-2003 gibt es nur 56 Farben. Wenn die Farbe nicht in der Palette vorhanden ist, wird eine ähnliche Farbe gesetzt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rawColor | [Color](../../com.aspose.cells/color) | Rohfarbe. |

**Returns:**
[Color](../../com.aspose.cells/color) - Best matching color.
### getNamedStyle(String name) {#getNamedStyle-java.lang.String-}
```
public Style getNamedStyle(String name)
```


Ruft den benannten Stil im Stilpool ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | Name des Stils |

**Returns:**
[Style](../../com.aspose.cells/style) - named style, maybe null.
### getRibbonXml() {#getRibbonXml--}
```
public String getRibbonXml()
```


Ruft die XML-Datei ab, die die Ribbon-Benutzeroberfläche definiert.

**Returns:**
java.lang.String
### getSettings() {#getSettings--}
```
public WorkbookSettings getSettings()
```


Stellt die Arbeitsmappeneinstellungen dar.

**Returns:**
[WorkbookSettings](../../com.aspose.cells/workbooksettings)
### getStyleInPool(int index) {#getStyleInPool-int-}
```
public Style getStyleInPool(int index)
```


Ruft den Stil im Stil-Pool ab. Alle Stile in der Arbeitsmappe werden in einen Pool gesammelt. In den Zellen gibt es nur einen einfachen Referenzindex.

**Remarks**

Wenn der zurückgegebene Stil geändert wird, ändert sich der Stil aller Zellen (die auf diesen Stil verweisen).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der Index. |

**Returns:**
[Style](../../com.aspose.cells/style) - The style in the pool corresponds to given index, may be null.
### getTheme() {#getTheme--}
```
public String getTheme()
```


Ruft den Namen des Designs ab.

**Returns:**
java.lang.String
### getThemeColor(int type) {#getThemeColor-int-}
```
public Color getThemeColor(int type)
```


Ruft die Designfarbe ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| type | int | [ThemeColorType](../../com.aspose.cells/themecolortype). Der Theme-Farbtyp. |

**Returns:**
[Color](../../com.aspose.cells/color) - The theme color.
### getVbaProject() {#getVbaProject--}
```
public VbaProject getVbaProject()
```


Ruft das [getVbaProject()](../../com.aspose.cells/workbook\#getVbaProject--) in einer Tabellenkalkulation ab.

**Returns:**
[VbaProject](../../com.aspose.cells/vbaproject)
### getWorksheets() {#getWorksheets--}
```
public WorksheetCollection getWorksheets()
```


Ruft die [WorksheetCollection](../../com.aspose.cells/worksheetcollection)-Sammlung in der Tabellenkalkulation ab.

**Returns:**
[WorksheetCollection](../../com.aspose.cells/worksheetcollection) - [WorksheetCollection](../../com.aspose.cells/worksheetcollection) collection
### hasCustomFunction() {#hasCustomFunction--}
```
public boolean hasCustomFunction()
```


Erkennt, ob in dieser Arbeitsmappe benutzerdefinierte Funktionen verwendet werden, z. B. in Zellformeln oder definierten Namen...

**Returns:**
boolean
### hasExernalLinks() {#hasExernalLinks--}
```
public boolean hasExernalLinks()
```


Gibt an, ob diese Arbeitsmappe externe Verknüpfungen zu anderen Datenquellen enthält.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen ExternalLinkCollection.Count, um zu prüfen, ob es externe Links in dieser Arbeitsmappe gibt. Diese Methode wird 12 Monate nach Dezember 2021 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Returns:**
boolescher Wert – Ob diese Arbeitsmappe externe Links zu anderen Datenquellen enthält.
### hasMacro() {#hasMacro--}
```
public boolean hasMacro()
```


Gibt an, ob diese Tabellenkalkulation Makros/VBA enthält.

**Returns:**
boolean
### hasRevisions() {#hasRevisions--}
```
public boolean hasRevisions()
```


Ermittelt, ob die Arbeitsmappe nachverfolgte Änderungen enthält

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### importXml(InputStream stream, String sheetName, int row, int col) {#importXml-java.io.InputStream-java.lang.String-int-int-}
```
public void importXml(InputStream stream, String sheetName, int row, int col)
```


Importiert/Aktualisiert eine XML-Datendatei in die Arbeitsmappe.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.InputStream | der XML-Dateistream. |
| sheetName | java.lang.String | der Zielblattname. |
| Zeile | int | die Zielzeile. |
| Spalte | int | die Zielspalte. |

### importXml(String url, String sheetName, int row, int col) {#importXml-java.lang.String-java.lang.String-int-int-}
```
public void importXml(String url, String sheetName, int row, int col)
```


Importiert/Aktualisiert eine XML-Datendatei in die Arbeitsmappe.

**Example**

Der folgende Code importiert XML-Daten in das Arbeitsblatt 'Sheet 1' bei Zelle A1.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         wb.importXml("xml.xml", "Sheet1", 0, 0);
 
         wb.save("output.xlsx");
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| URL | java.lang.String | die URL/Pfad der XML-Datei. |
| sheetName | java.lang.String | der Zielblattname. |
| Zeile | int | die Zielzeile |
| Spalte | int | die Zielspalte |

### isColorInPalette(Color color) {#isColorInPalette-com.aspose.cells.Color-}
```
public boolean isColorInPalette(Color color)
```


Prüft, ob eine Farbe in der Palette der Tabellenkalkulation enthalten ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Farbstruktur. |

**Returns:**
boolean - Gibt true zurück, wenn diese Farbe in der Palette ist. Andernfalls wird false zurückgegeben
### isDigitallySigned() {#isDigitallySigned--}
```
public boolean isDigitallySigned()
```


Gibt an, ob diese Tabellenkalkulation digital signiert ist.

**Returns:**
boolean
### isLicensed() {#isLicensed--}
```
public boolean isLicensed()
```


Gibt an, ob eine Lizenz festgelegt ist.

**Returns:**
boolean
### isWorkbookProtectedWithPassword() {#isWorkbookProtectedWithPassword--}
```
public boolean isWorkbookProtectedWithPassword()
```


Gibt an, ob Struktur oder Fenster mit einem Kennwort geschützt ist.

**Returns:**
boolean
### mergeNamedStyles(Workbook source) {#mergeNamedStyles-com.aspose.cells.Workbook-}
```
public void mergeNamedStyles(Workbook source)
```


Führt benannte Stile aus der anderen Excel-Datei zusammen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | [Workbook](../../com.aspose.cells/workbook) | Die andere Datei |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### parseFormulas(boolean ignoreError) {#parseFormulas-boolean-}
```
public void parseFormulas(boolean ignoreError)
```


Parst alle Formeln, die beim Laden aus einer Vorlagendatei oder beim Setzen in eine Zelle nicht geparst wurden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ignoreError | boolean | Ob Fehler bei ungültiger Formel ignoriert werden sollen. Bei einer ungültigen Formel wird, wenn Fehler ignoriert werden, diese Formel übersprungen und der Vorgang fährt mit dem Parsen anderer Formeln fort, andernfalls wird eine Ausnahme ausgelöst. |

### protect(int protectionType, String password) {#protect-int-java.lang.String-}
```
public void protect(int protectionType, String password)
```


Schützt eine Arbeitsmappe.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| protectionType | int | [ProtectionType](../../com.aspose.cells/protectiontype). Schutztyp. |
| Passwort | java.lang.String | Passwort zum Schutz der Arbeitsmappe. |

### protectSharedWorkbook(String password) {#protectSharedWorkbook-java.lang.String-}
```
public void protectSharedWorkbook(String password)
```


Schützt eine freigegebene Arbeitsmappe.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Passwort | java.lang.String | Passwort zum Schutz der Arbeitsmappe. |

### refreshAll() {#refreshAll--}
```
public void refreshAll()
```


Aktualisiert verknüpfte Formen, alle Pivot-Tabellen und Diagramme mit der Pivot-Quelle.

### refreshDynamicArrayFormulas(boolean calculate) {#refreshDynamicArrayFormulas-boolean-}
```
public void refreshDynamicArrayFormulas(boolean calculate)
```


Aktualisiert dynamische Array-Formeln (erweitern sich in einen neuen Bereich benachbarter Zellen gemäß den aktuellen Daten). Andere Formeln in der Arbeitsmappe werden nicht rekursiv berechnet, selbst wenn sie von dynamischen Array-Formeln verwendet werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| berechnen | boolean | Ob die Zellwerte für diese dynamischen Array-Formeln berechnet und aktualisiert werden |

### refreshDynamicArrayFormulas(boolean calculate, CalculationOptions copts) {#refreshDynamicArrayFormulas-boolean-com.aspose.cells.CalculationOptions-}
```
public void refreshDynamicArrayFormulas(boolean calculate, CalculationOptions copts)
```


Aktualisiert dynamische Array-Formeln (erweitern sich in einen neuen Bereich benachbarter Zellen gemäß den aktuellen Daten)

**Remarks**

Aus Performancegründen aktualisieren wir nicht automatisch alle dynamischen Array-Formeln, wenn sich die Formel selbst oder die referenzierten Daten ändern. Der Benutzer muss diese Methode daher nach Vorgängen, die dynamische Array-Formeln beeinflussen können, manuell aufrufen, z. b. beim Importieren/Setzen von Zellwerten, Einfügen/Löschen von Zeilen/Spalten/Bereichen usw.

Für die meisten Formeln mit Funktionen muss zur Berechnung des Spill‑Bereichs auch die Formel berechnet werden, daher wird im Allgemeinen der wahre Wert für das \"calculate\"‑Flag bevorzugt. Ist die Formel einfach, z. B. ein Bereichsverweis oder ein Array (zum Beispiel \"=C1:E5\", \"=\\{1,2;3,4\\}\", ...), eine einfache Funktion auf einem Bereich oder Array (zum Beispiel \"=ABS(C1:E5)\", \"=1+\\{1,2;3,4\\}\", ...), und werden alle Formeln später berechnet (wie z. B. durch [calculateFormula(CalculationOptions)](../../com.aspose.cells/workbook\\#calculateFormula-CalculationOptions-)), kann die Verwendung des falschen Werts für das \"calculate\"‑Flag die doppelte Berechnung vermeiden und die Leistung verbessern.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| berechnen | boolean | Ob die Zellwerte für diese dynamischen Array-Formeln berechnet und aktualisiert werden |
| copts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Die Optionen zur Berechnung von Formeln |

### removeDigitalSignature() {#removeDigitalSignature--}
```
public void removeDigitalSignature()
```


Entfernt die digitale Signatur aus dieser Tabellenkalkulation.

### removeExternalLinks() {#removeExternalLinks--}
```
public void removeExternalLinks()
```


Entfernt alle externen Links in der Arbeitsmappe.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode ExternalLinkCollection.Clear(). Diese Methode wird 12 Monate nach Dezember 2021 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### removeMacro() {#removeMacro--}
```
public void removeMacro()
```


Entfernt VBA/Makro aus dieser Tabellenkalkulation.

### removePersonalInformation() {#removePersonalInformation--}
```
public void removePersonalInformation()
```


Entfernt persönliche Informationen.

### removeUnusedStyles() {#removeUnusedStyles--}
```
public void removeUnusedStyles()
```


Entfernt alle ungenutzten Stile.

### replace(boolean boolValue, Object newValue) {#replace-boolean-java.lang.Object-}
```
public int replace(boolean boolValue, Object newValue)
```


Ersetzt die Werte der Zellen durch neue Daten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| boolValue | boolean | Der boolesche Wert, der ersetzt werden soll. |
| newValue | java.lang.Object | Neuer Wert. Kann ein String, Integer, Double oder DateTime‑Wert sein. |

**Returns:**
int
### replace(int intValue, Object newValue) {#replace-int-java.lang.Object-}
```
public int replace(int intValue, Object newValue)
```


Ersetzt die Werte der Zellen durch neue Daten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| intValue | int | Der ganzzahlige Wert, der ersetzt werden soll. |
| newValue | java.lang.Object | Neuer Wert. Kann ein String, Integer, Double oder DateTime‑Wert sein. |

**Returns:**
int
### replace(String placeHolder, double newValue) {#replace-java.lang.String-double-}
```
public int replace(String placeHolder, double newValue)
```


Ersetzt den Wert einer Zelle durch ein neues Double.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         double newValue = 100.0;
         workbook.replace("AnOldValue", newValue);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| placeHolder | java.lang.String | Zellenplatzhalter |
| newValue | double | Double‑Wert zum Ersetzen |

**Returns:**
int
### replace(String placeHolder, double[] newValues, boolean isVertical) {#replace-java.lang.String-double---boolean-}
```
public int replace(String placeHolder, double[] newValues, boolean isVertical)
```


Ersetzt die Werte der Zellen durch ein Double-Array.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         double[] newValues = new double[]{1.23, 2.56, 3.14159};
         workbook.replace("AnOldValue", newValues, true);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| placeHolder | java.lang.String | Zellenplatzhalter |
| newValues | double[] | Double‑Array zum Ersetzen |
| isVertical | boolean | True - Vertikal, False - Horizontal |

**Returns:**
int
### replace(String placeHolder, int newValue) {#replace-java.lang.String-int-}
```
public int replace(String placeHolder, int newValue)
```


Ersetzt den Wert einer Zelle durch einen neuen Integer.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         int newValue = 100;
         workbook.replace("AnOldValue", newValue);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| placeHolder | java.lang.String | Zellenplatzhalter |
| newValue | int | Ganzzahlwert zum Ersetzen |

**Returns:**
int
### replace(String placeHolder, int[] newValues, boolean isVertical) {#replace-java.lang.String-int---boolean-}
```
public int replace(String placeHolder, int[] newValues, boolean isVertical)
```


Ersetzt die Werte der Zellen durch ein Integer-Array.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         int[] newValues = new int[]{1, 2, 3};
         workbook.replace("AnOldValue", newValues, true);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| placeHolder | java.lang.String | Zellenplatzhalter |
| newValues | int[] | Integer-Array zum Ersetzen |
| isVertical | boolean | True - Vertikal, False - Horizontal |

**Returns:**
int
### replace(String placeHolder, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public int replace(String placeHolder, String newValue)
```


Ersetzt den Wert einer Zelle durch einen neuen String.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         workbook.replace("AnOldValue", "NewValue");
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| placeHolder | java.lang.String | Zellenplatzhalter |
| newValue | java.lang.String | String-Wert zum Ersetzen |

**Returns:**
int
### replace(String placeHolder, String newValue, ReplaceOptions options) {#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-}
```
public int replace(String placeHolder, String newValue, ReplaceOptions options)
```


Ersetzt den Wert einer Zelle durch einen neuen String.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| placeHolder | java.lang.String | Zellenplatzhalter |
| newValue | java.lang.String | String-Wert zum Ersetzen |
| options | [ReplaceOptions](../../com.aspose.cells/replaceoptions) | Die Ersetzungsoptionen |

**Returns:**
int
### replace(String placeHolder, String[] newValues, boolean isVertical) {#replace-java.lang.String-java.lang.String---boolean-}
```
public int replace(String placeHolder, String[] newValues, boolean isVertical)
```


Ersetzt den Wert einer Zelle durch ein neues String-Array.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         String[] newValues = new String[]{"Tom", "Alice", "Jerry"};
         workbook.replace("AnOldValue", newValues, true);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| placeHolder | java.lang.String | Zellenplatzhalter |
| newValues | java.lang.String[] | String-Array zum Ersetzen |
| isVertical | boolean | True - Vertikal, False - Horizontal |

**Returns:**
int
### save(OutputStream stream, SaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.cells.SaveOptions-}
```
public void save(OutputStream stream, SaveOptions saveOptions)
```


Speichert die Arbeitsmappe in den Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.OutputStream | Der Dateistream. |
| saveOptions | [SaveOptions](../../com.aspose.cells/saveoptions) | Die Speicheroptionen. |

### save(OutputStream stream, int saveFormat) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int saveFormat)
```


Speichert die Arbeitsmappe in den Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.OutputStream | Der Dateistream. |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). Der Typ des Speicherdateiformats. |

### save(String fileName) {#save-java.lang.String-}
```
public void save(String fileName)
```


Speichert die Arbeitsmappe auf die Festplatte.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | java.lang.String |  |

### save(String fileName, SaveOptions saveOptions) {#save-java.lang.String-com.aspose.cells.SaveOptions-}
```
public void save(String fileName, SaveOptions saveOptions)
```


Speichert die Arbeitsmappe auf die Festplatte.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | java.lang.String | Der Dateiname. |
| saveOptions | [SaveOptions](../../com.aspose.cells/saveoptions) | Die Speicheroptionen. |

### save(String fileName, int saveFormat) {#save-java.lang.String-int-}
```
public void save(String fileName, int saveFormat)
```


Speichert die Arbeitsmappe auf die Festplatte.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | java.lang.String | Der Dateiname. |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). Der Typ des Speicherformats. |

### setAbsolutePath(String value) {#setAbsolutePath-java.lang.String-}
```
public void setAbsolutePath(String value)
```


Legt den absoluten Pfad der Datei fest.

**Remarks**

Nur für externe Links verwendet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setDefaultStyle(Style value) {#setDefaultStyle-com.aspose.cells.Style-}
```
public void setDefaultStyle(Style value)
```


Legt das Standard-[Style](../../com.aspose.cells/style)-Objekt der Arbeitsmappe fest.

**Remarks**

Die DefaultStyle-Eigenschaft ist nützlich, um einen Stil für die gesamte Arbeitsmappe zu implementieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setDigitalSignature(DigitalSignatureCollection digitalSignatureCollection) {#setDigitalSignature-com.aspose.cells.DigitalSignatureCollection-}
```
public void setDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```


Setzt die digitale Signatur für eine Tabellenkalkulationsdatei (Excel2007 und neuer).

**Remarks**

Unterstützt nur das Hinzufügen von Xmldsig-Digitaler Signatur.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| digitalSignatureCollection | [DigitalSignatureCollection](../../com.aspose.cells/digitalsignaturecollection) |  |

### setEncryptionOptions(int encryptionType, int keyLength) {#setEncryptionOptions-int-int-}
```
public void setEncryptionOptions(int encryptionType, int keyLength)
```


Verschlüsselungsoptionen festlegen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| encryptionType | int | [EncryptionType](../../com.aspose.cells/encryptiontype). Der Verschlüsselungstyp. |
| keyLength | int | Die Schlüssellänge. |

### setFileFormat(int value) {#setFileFormat-int-}
```
public void setFileFormat(int value)
```


Legt das Dateiformat fest.

Siehe [FileFormatType](../../com.aspose.cells/fileformattype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setFileName(String value) {#setFileName-java.lang.String-}
```
public void setFileName(String value)
```


Legt den aktuellen Dateinamen fest.

**Remarks**

Wenn die Datei per Stream geöffnet wird und es externe Formelbezüge gibt, geben Sie bitte den Dateinamen an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setInterruptMonitor(AbstractInterruptMonitor value) {#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-}
```
public void setInterruptMonitor(AbstractInterruptMonitor value)
```


Legt den Interrupt‑Monitor fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor) |  |

### setRibbonXml(String value) {#setRibbonXml-java.lang.String-}
```
public void setRibbonXml(String value)
```


Legt die XML-Datei fest, die die Ribbon-Benutzeroberfläche definiert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setThemeColor(int type, Color color) {#setThemeColor-int-com.aspose.cells.Color-}
```
public void setThemeColor(int type, Color color)
```


Legt die Themenfarbe fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| type | int | [ThemeColorType](../../com.aspose.cells/themecolortype). Der Theme-Farbtyp. |
| color | [Color](../../com.aspose.cells/color) | die Themenfarbe |

### startAccessCache(int opts) {#startAccessCache-int-}
```
public void startAccessCache(int opts)
```


Startet die Sitzung, die Caches zum Zugriff auf Daten verwendet.

**Remarks**

Wenn der Cache des angegebenen Datenzugriffs erfordert, dass einige Datenmodelle im Arbeitsblatt "read-only" sind, dann werden die entsprechenden Datenmodelle in jedem Arbeitsblatt dieser Arbeitsmappe als "read-only" betrachtet und der Benutzer sollte keines davon ändern.

Nach dem Abschluss des Datenzugriffs sollte [closeAccessCache(int)](../../com.aspose.cells/workbook\#closeAccessCache-int-) mit denselben Optionen aufgerufen werden, um alle Caches zu leeren und den normalen Zugriffsmodus wiederherzustellen.



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| opts | int | [AccessCacheOptions](../../com.aspose.cells/accesscacheoptions). Optionen für den Datenzugriff |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### unprotect(String password) {#unprotect-java.lang.String-}
```
public void unprotect(String password)
```


Entfernt den Schutz einer Arbeitsmappe.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Passwort | java.lang.String | Passwort zum Aufheben des Schutzes der Arbeitsmappe. |

### unprotectSharedWorkbook(String password) {#unprotectSharedWorkbook-java.lang.String-}
```
public void unprotectSharedWorkbook(String password)
```


Entfernt den Schutz einer freigegebenen Arbeitsmappe.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Passwort | java.lang.String | Passwort zum Aufheben des Schutzes der Arbeitsmappe. |

### updateCustomFunctionDefinition(CustomFunctionDefinition definition) {#updateCustomFunctionDefinition-com.aspose.cells.CustomFunctionDefinition-}
```
public void updateCustomFunctionDefinition(CustomFunctionDefinition definition)
```


Aktualisiert die Definition benutzerdefinierter Funktionen.

**Remarks**

Diese Methode kann für einige spezielle Szenarien verwendet werden. Zum Beispiel, wenn der Benutzer benötigt, dass einige Parameter benutzerdefinierter Funktionen im Array‑Modus berechnet werden, kann der Benutzer seine eigene Definition mit implementierter [CustomFunctionDefinition.getArrayModeParameters(String)](../../com.aspose.cells/customfunctiondefinition\#getArrayModeParameters-String-) für diese Funktionen bereitstellen. Nachdem die Formeldaten aktualisiert wurden, werden die angegebenen Parameter beim Berechnen der entsprechenden benutzerdefinierten Funktionen automatisch im Array‑Modus berechnet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| definition | [CustomFunctionDefinition](../../com.aspose.cells/customfunctiondefinition) | Spezielle Definition benutzerdefinierter Funktionen für die speziellen Anforderungen des Benutzers. |

### updateLinkedDataSource(Workbook[] externalWorkbooks) {#updateLinkedDataSource-com.aspose.cells.Workbook---}
```
public void updateLinkedDataSource(Workbook[] externalWorkbooks)
```


Wenn diese Arbeitsmappe externe Verknüpfungen zu anderen Datenquellen enthält, wird Aspose.Cells versuchen, die neuesten Daten aus den angegebenen Quellen abzurufen.

**Remarks**

Wenn der entsprechende externe Link für eine Arbeitsmappe nicht gefunden werden kann, wird diese Arbeitsmappe ignoriert. Wenn Sie später eine Formel mit einem neuen externen Link setzen, den Sie mit der ignorierten Arbeitsmappe verknüpfen möchten, kann die Verknüpfung nicht durchgeführt werden, bis Sie diese Methode erneut mit diesen Arbeitsmappen aufrufen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| externalWorkbooks | [Workbook\[\]](../../com.aspose.cells/workbook) | Arbeitsmappen, die zum Aktualisieren der Daten externer Links, auf die sich diese Arbeitsmappe bezieht, verwendet werden. Die Zuordnung dieser Arbeitsmappen zu den externen Links wird durch [getFileName()](../../com.aspose.cells/workbook\#getFileName--) und [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--) bestimmt. Bitte stellen Sie daher sicher, dass [getFileName()](../../com.aspose.cells/workbook\#getFileName--) für jede Arbeitsmappe mit dem richtigen Wert angegeben wurde, damit sie mit dem entsprechenden externen Link verknüpft werden können. |

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

