---
title: "WorksheetCollection"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Kapselt eine Sammlung von Objekten."
type: docs
url: /de/java/com.aspose.cells/worksheetcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class WorksheetCollection extends CollectionBase
```

Kapselt eine Sammlung von [Worksheet](../../com.aspose.cells/worksheet)-Objekten.

**Example**

```
         Workbook workbook = new Workbook();
 
         WorksheetCollection sheets = workbook.getWorksheets();
 
         //Add a worksheet
         sheets.add();
 
         //Change the name of a worksheet
         sheets.get(0).setName("First Sheet");
 
         //Set the active sheet to the second worksheet
         sheets.setActiveSheetIndex(1);
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add()](#add--) | Fügt der Sammlung ein Arbeitsblatt hinzu. |
| [add(int type)](#add-int-) | Fügt der Sammlung ein Arbeitsblatt hinzu. |
| [add(Object o)](#add-java.lang.Object-) | Fügt ein Element zur CollectionBase-Instanz hinzu. |
| [add(String sheetName)](#add-java.lang.String-) | Fügt der Sammlung ein Arbeitsblatt hinzu. |
| [addCopy(Worksheet[] source, String[] destSheetNames)](#addCopy-com.aspose.cells.Worksheet---java.lang.String---) | Kopiert eine Gruppe von Arbeitsblättern. |
| [addCopy(int sheetIndex)](#addCopy-int-) | Fügt der Sammlung ein Arbeitsblatt hinzu und kopiert Daten von einem bestehenden Arbeitsblatt. |
| [addCopy(String sheetName)](#addCopy-java.lang.String-) | Fügt der Sammlung ein Arbeitsblatt hinzu und kopiert Daten von einem bestehenden Arbeitsblatt. |
| [clear()](#clear--) | Alle Arbeitsblätter löschen. |
| [clearPivottables()](#clearPivottables--) | Löscht Pivot-Tabellen aus der Tabelle. |
| [contains(Object o)](#contains-java.lang.Object-) | Gibt zurück, ob die Instanz dieses Objekt enthält |
| [createRange(String address, int sheetIndex)](#createRange-java.lang.String-int-) | Erstellt ein [Range](../../com.aspose.cells/range)-Objekt aus einer Bereichsadresse. |
| [createUnionRange(String address, int sheetIndex)](#createUnionRange-java.lang.String-int-) | Erstellt ein [Range](../../com.aspose.cells/range)-Objekt aus einer Bereichsadresse. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Liefert das [Worksheet](../../com.aspose.cells/worksheet)-Element am angegebenen Index. |
| [get(String sheetName)](#get-java.lang.String-) | Liefert das [Worksheet](../../com.aspose.cells/worksheet)-Element mit dem angegebenen Namen. |
| [getActiveSheetIndex()](#getActiveSheetIndex--) | Stellt den Index des aktiven Arbeitsblatts dar, wenn die Tabelle geöffnet wird. |
| [getActiveSheetName()](#getActiveSheetName--) | Stellt den Namen des aktiven Arbeitsblatts dar, wenn die Tabelle geöffnet wird. |
| [getBuiltInDocumentProperties()](#getBuiltInDocumentProperties--) | Gibt eine [DocumentProperty](../../com.aspose.cells/documentproperty)-Sammlung zurück, die alle integrierten Dokumenteigenschaften der Kalkulationstabelle darstellt. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ermittelt die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente. |
| [getCustomDocumentProperties()](#getCustomDocumentProperties--) | Gibt eine [DocumentProperty](../../com.aspose.cells/documentproperty)-Sammlung zurück, die alle benutzerdefinierten Dokumenteigenschaften der Kalkulationstabelle darstellt. |
| [getDxfs()](#getDxfs--) | Liefert die Master-Differenzformatierungsdatensätze. |
| [getExternalLinks()](#getExternalLinks--) | Stellt externe Links in einer Arbeitsmappe dar. |
| [getNamedRanges()](#getNamedRanges--) | Ermittelt alle vordefinierten benannten Bereiche im Tabellenblatt. |
| [getNamedRangesAndTables()](#getNamedRangesAndTables--) | Ermittelt alle vordefinierten benannten Bereiche im Tabellenblatt. |
| [getNames()](#getNames--) | Ermittelt die Sammlung aller Name-Objekte im Tabellenblatt. |
| [getOleSize()](#getOleSize--) | Ermittelt die angezeigte Größe, wenn die Arbeitsmappendatei als Ole-Objekt verwendet wird. |
| [getPivotCaches()](#getPivotCaches--) | Ermittelt alle [PivotCache](../../com.aspose.cells/pivotcache). |
| [getRangeByName(String rangeName)](#getRangeByName-java.lang.String-) | Ermittelt das Range-Objekt anhand eines vordefinierten Namens. |
| [getRangeByName(String rangeName, int currentSheetIndex, boolean includeTable)](#getRangeByName-java.lang.String-int-boolean-) | Ermittelt [Range](../../com.aspose.cells/range) anhand eines vordefinierten Namens oder des Tabellennamens |
| [getRevisionLogs()](#getRevisionLogs--) | Stellt Revisionsprotokolle dar. |
| [getSensitivityLabels()](#getSensitivityLabels--) | Stellt alle Sensitivitätskennzeichnungen dar. |
| [getSheetByCodeName(String codeName)](#getSheetByCodeName-java.lang.String-) | Ermittelt das Arbeitsblatt anhand des Codenamens. |
| [getTableStyles()](#getTableStyles--) | Ermittelt das [getTableStyles()](../../com.aspose.cells/worksheetcollection\#getTableStyles--) Objekt. |
| [getThreadedCommentAuthors()](#getThreadedCommentAuthors--) | Ermittelt die Liste der Autoren von Threaded-Kommentaren. |
| [getWebExtensionTaskPanes()](#getWebExtensionTaskPanes--) | Ermittelt die Liste der Task-Panes. |
| [getWebExtensions()](#getWebExtensions--) | Ermittelt die Liste der Task-Panes. |
| [getXmlMaps()](#getXmlMaps--) | Ermittelt die XML-Maps im Arbeitsbuch. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz. |
| [insert(int index, int sheetType)](#insert-int-int-) | Fügt ein Arbeitsblatt ein. |
| [insert(int index, int sheetType, String sheetName)](#insert-int-int-java.lang.String-) | Fügt ein Arbeitsblatt ein. |
| [isRefreshAllConnections()](#isRefreshAllConnections--) | Gibt an, ob beim Öffnen der Datei in MS Excel alle Verbindungen aktualisiert werden. |
| [iterator()](#iterator--) | Gibt einen Enumerator zurück, der die CollectionBase-Instanz durchläuft. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshAll()](#refreshAll--) | Aktualisiert alle Pivot-Tabellen und Diagramme mit der Pivot-Quelle. |
| [refreshPivotTables()](#refreshPivotTables--) | Aktualisiert alle PivotTables in der Excel-Datei. |
| [refreshPivotTables(PivotTableRefreshOption option)](#refreshPivotTables-com.aspose.cells.PivotTableRefreshOption-) | Aktualisiert alle PivotTables in der Excel-Datei. |
| [registerAddInFunction(int id, String functionName)](#registerAddInFunction-int-java.lang.String-) | Fügt dem Arbeitsbuch eine Add-In-Funktion hinzu |
| [registerAddInFunction(String addInFile, String functionName, boolean lib)](#registerAddInFunction-java.lang.String-java.lang.String-boolean-) | Fügt dem Arbeitsbuch eine Add-In-Funktion hinzu |
| [removeAt(int index)](#removeAt-int-) | Entfernt das Element an einem angegebenen Index. |
| [removeAt(String name)](#removeAt-java.lang.String-) | Entfernt das Element mit einem angegebenen Namen. |
| [setActiveSheetIndex(int value)](#setActiveSheetIndex-int-) | Stellt den Index des aktiven Arbeitsblatts dar, wenn die Tabelle geöffnet wird. |
| [setActiveSheetName(String value)](#setActiveSheetName-java.lang.String-) | Stellt den Namen des aktiven Arbeitsblatts dar, wenn die Tabelle geöffnet wird. |
| [setOleSize(int startRow, int endRow, int startColumn, int endColumn)](#setOleSize-int-int-int-int-) | Legt die angezeigte Größe fest, wenn die Arbeitsmappendatei als Ole-Objekt verwendet wird. |
| [setOleSize(Object value)](#setOleSize-java.lang.Object-) | Legt die angezeigte Größe fest, wenn die Arbeitsmappendatei als Ole-Objekt verwendet wird. |
| [setRefreshAllConnections(boolean value)](#setRefreshAllConnections-boolean-) | Gibt an, ob beim Öffnen der Datei in MS Excel alle Verbindungen aktualisiert werden. |
| [setXmlMaps(XmlMapCollection value)](#setXmlMaps-com.aspose.cells.XmlMapCollection-) | Legt die XML-Maps im Arbeitsbuch fest. |
| [sortNames()](#sortNames--) | Sortiert die definierten Namen. |
| [swapSheet(int sheetIndex1, int sheetIndex2)](#swapSheet-int-int-) | Vertauscht die beiden Blätter. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add() {#add--}
```
public int add()
```


Fügt der Sammlung ein Arbeitsblatt hinzu.

**Returns:**
int - [Worksheet](../../com.aspose.cells/worksheet) Objektindex.
### add(int type) {#add-int-}
```
public int add(int type)
```


Fügt der Sammlung ein Arbeitsblatt hinzu.

**Example**

```
         Workbook workbook = new Workbook();
         workbook.getWorksheets().add(SheetType.CHART);
         	Cells cells = workbook.getWorksheets().get(0).getCells();
         	cells.get("c2").putValue(5000);
         	cells.get("c3").putValue(3000);
         	cells.get("c4").putValue(4000);
         	cells.get("c5").putValue(5000);
         	cells.get("c6").putValue(6000);
         	ChartCollection charts = workbook.getWorksheets().get(1).getCharts();
         	int chartIndex = charts.add(ChartType.COLUMN, 10,10,20,20);
         	Chart chart = charts.get(chartIndex);
         	chart.getNSeries().add("Sheet1!C2:C6", true);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| type | int | [SheetType](../../com.aspose.cells/sheettype). Arbeitsblatttyp. |

**Returns:**
int - [Worksheet](../../com.aspose.cells/worksheet) Objektindex.
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Fügt ein Element zur CollectionBase-Instanz hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | Das Objekt, das zur CollectionBase-Instanz hinzugefügt werden soll. |

**Returns:**
int - Die Position, an der das neue Element eingefügt wurde.
### add(String sheetName) {#add-java.lang.String-}
```
public Worksheet add(String sheetName)
```


Fügt der Sammlung ein Arbeitsblatt hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetName | java.lang.String | Arbeitsblattname |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - [Worksheet](../../com.aspose.cells/worksheet) object.
### addCopy(Worksheet[] source, String[] destSheetNames) {#addCopy-com.aspose.cells.Worksheet---java.lang.String---}
```
public void addCopy(Worksheet[] source, String[] destSheetNames)
```


Kopiert eine Gruppe von Arbeitsblättern.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | [Worksheet\[\]](../../com.aspose.cells/worksheet) | Die Quellarbeitsblätter. |
| destSheetNames | java.lang.String[] | Die Namen der kopierten Arbeitsblätter. |

### addCopy(int sheetIndex) {#addCopy-int-}
```
public int addCopy(int sheetIndex)
```


Fügt der Sammlung ein Arbeitsblatt hinzu und kopiert Daten von einem bestehenden Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetIndex | int | Index des Quellarbeitsblatts. |

**Returns:**
int - [Worksheet](../../com.aspose.cells/worksheet) Objektindex.
### addCopy(String sheetName) {#addCopy-java.lang.String-}
```
public int addCopy(String sheetName)
```


Fügt der Sammlung ein Arbeitsblatt hinzu und kopiert Daten von einem bestehenden Arbeitsblatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetName | java.lang.String | Name des Quellarbeitsblatts. |

**Returns:**
int - [Worksheet](../../com.aspose.cells/worksheet) Objektindex.
### clear() {#clear--}
```
public void clear()
```


Alle Arbeitsblätter löschen.

**Remarks**

Ein Arbeitsbuch muss ein Arbeitsblatt enthalten.

### clearPivottables() {#clearPivottables--}
```
public void clearPivottables()
```


Löscht Pivot-Tabellen aus der Tabelle.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Gibt zurück, ob die Instanz dieses Objekt enthält

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | Testobjekt |

**Returns:**
boolean - Ob die Instanz dieses Objekt enthält
### createRange(String address, int sheetIndex) {#createRange-java.lang.String-int-}
```
public Range createRange(String address, int sheetIndex)
```


Erstellt ein [Range](../../com.aspose.cells/range)-Objekt aus einer Bereichsadresse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Adresse | java.lang.String | Die Adresse des Bereichs. |
| sheetIndex | int | Der Blattindex. |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### createUnionRange(String address, int sheetIndex) {#createUnionRange-java.lang.String-int-}
```
public UnionRange createUnionRange(String address, int sheetIndex)
```


Erstellt ein [Range](../../com.aspose.cells/range)-Objekt aus einer Bereichsadresse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Adresse | java.lang.String | Die Adresse des Bereichs. |
| sheetIndex | int | Der Blattindex. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - A [Range](../../com.aspose.cells/range) object
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
### get(int index) {#get-int-}
```
public Worksheet get(int index)
```


Liefert das [Worksheet](../../com.aspose.cells/worksheet)-Element am angegebenen Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der nullbasierte Index des Elements. |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - The element at the specified index.
### get(String sheetName) {#get-java.lang.String-}
```
public Worksheet get(String sheetName)
```


Liefert das [Worksheet](../../com.aspose.cells/worksheet)-Element mit dem angegebenen Namen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetName | java.lang.String | Arbeitsblattname |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - The element with the specified name.
### getActiveSheetIndex() {#getActiveSheetIndex--}
```
public int getActiveSheetIndex()
```


Stellt den Index des aktiven Arbeitsblatts dar, wenn die Tabelle geöffnet wird.

**Remarks**

Der Arbeitsblattindex ist nullbasiert.

**Returns:**
int
### getActiveSheetName() {#getActiveSheetName--}
```
public String getActiveSheetName()
```


Stellt den Namen des aktiven Arbeitsblatts dar, wenn die Tabelle geöffnet wird.

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
         DocumentProperty doc = workbook.getWorksheets().getBuiltInDocumentProperties().get("Author");
         doc.setValue("John Smith");
```

**Returns:**
[BuiltInDocumentPropertyCollection](../../com.aspose.cells/builtindocumentpropertycollection)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


Ermittelt die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente.

**Returns:**
int - Die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente.
### getCustomDocumentProperties() {#getCustomDocumentProperties--}
```
public CustomDocumentPropertyCollection getCustomDocumentProperties()
```


Gibt eine [DocumentProperty](../../com.aspose.cells/documentproperty)-Sammlung zurück, die alle benutzerdefinierten Dokumenteigenschaften der Kalkulationstabelle darstellt.

**Example**

```
         Workbook workbook = new Workbook();
         workbook.getWorksheets().getCustomDocumentProperties().add("Checked by", "Jane");
```

**Returns:**
[CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection)
### getDxfs() {#getDxfs--}
```
public DxfCollection getDxfs()
```


Liefert die Master-Differenzformatierungsdatensätze.

**Returns:**
[DxfCollection](../../com.aspose.cells/dxfcollection)
### getExternalLinks() {#getExternalLinks--}
```
public ExternalLinkCollection getExternalLinks()
```


Stellt externe Links in einer Arbeitsmappe dar.

**Returns:**
[ExternalLinkCollection](../../com.aspose.cells/externallinkcollection)
### getNamedRanges() {#getNamedRanges--}
```
public Range[] getNamedRanges()
```


Ermittelt alle vordefinierten benannten Bereiche im Tabellenblatt.

**Returns:**
com.aspose.cells.Range[] - Ein Array von Range‑Objekten. Wenn die Referenz des definierten Namens extern ist oder mehrere Bereiche hat, wird kein Range‑Objekt für diesen Namen zurückgegeben.

Gibt null zurück, wenn der benannte Bereich nicht existiert.
### getNamedRangesAndTables() {#getNamedRangesAndTables--}
```
public Range[] getNamedRangesAndTables()
```


Ermittelt alle vordefinierten benannten Bereiche im Tabellenblatt.

**Returns:**
com.aspose.cells.Range[] - Ein Array von Range‑Objekten.

Gibt null zurück, wenn der benannte Bereich nicht existiert.
### getNames() {#getNames--}
```
public NameCollection getNames()
```


Ermittelt die Sammlung aller Name-Objekte im Tabellenblatt.

**Returns:**
[NameCollection](../../com.aspose.cells/namecollection)
### getOleSize() {#getOleSize--}
```
public Object getOleSize()
```


Ermittelt die angezeigte Größe, wenn die Arbeitsmappendatei als Ole-Objekt verwendet wird.

**Remarks**

Null bedeutet keine OLE‑Größeneinstellung.

**Returns:**
java.lang.Object
### getPivotCaches() {#getPivotCaches--}
```
public PivotCacheCollection getPivotCaches()
```


Ermittelt alle [PivotCache](../../com.aspose.cells/pivotcache).

**Returns:**
[PivotCacheCollection](../../com.aspose.cells/pivotcachecollection)
### getRangeByName(String rangeName) {#getRangeByName-java.lang.String-}
```
public Range getRangeByName(String rangeName)
```


Ermittelt das Range-Objekt anhand eines vordefinierten Namens.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rangeName | java.lang.String | Name des Bereichs. |

**Returns:**
[Range](../../com.aspose.cells/range) - Range object.

Gibt null zurück, wenn der benannte Bereich nicht existiert.
### getRangeByName(String rangeName, int currentSheetIndex, boolean includeTable) {#getRangeByName-java.lang.String-int-boolean-}
```
public Range getRangeByName(String rangeName, int currentSheetIndex, boolean includeTable)
```


Ermittelt [Range](../../com.aspose.cells/range) anhand eines vordefinierten Namens oder des Tabellennamens

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rangeName | java.lang.String | Name des Bereichs oder Tabellenname. |
| currentSheetIndex | int | Der Blattindex. -1 steht für global. |
| includeTable | boolean | Gibt an, ob alle Tabellen geprüft werden. |

**Returns:**
[Range](../../com.aspose.cells/range) - 
### getRevisionLogs() {#getRevisionLogs--}
```
public RevisionLogCollection getRevisionLogs()
```


Stellt Revisionsprotokolle dar.

**Returns:**
[RevisionLogCollection](../../com.aspose.cells/revisionlogcollection)
### getSensitivityLabels() {#getSensitivityLabels--}
```
public SensitivityLabelCollection getSensitivityLabels()
```


Stellt alle Sensitivitätskennzeichnungen dar.

**Returns:**
[SensitivityLabelCollection](../../com.aspose.cells/sensitivitylabelcollection)
### getSheetByCodeName(String codeName) {#getSheetByCodeName-java.lang.String-}
```
public Worksheet getSheetByCodeName(String codeName)
```


Ermittelt das Arbeitsblatt anhand des Codenamens.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| codeName | java.lang.String | Arbeitsblatt-Code-Name. |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - The element with the specified code name.
### getTableStyles() {#getTableStyles--}
```
public TableStyleCollection getTableStyles()
```


Ermittelt das [getTableStyles()](../../com.aspose.cells/worksheetcollection\#getTableStyles--) Objekt.

**Returns:**
[TableStyleCollection](../../com.aspose.cells/tablestylecollection)
### getThreadedCommentAuthors() {#getThreadedCommentAuthors--}
```
public ThreadedCommentAuthorCollection getThreadedCommentAuthors()
```


Ermittelt die Liste der Autoren von Threaded-Kommentaren.

**Returns:**
[ThreadedCommentAuthorCollection](../../com.aspose.cells/threadedcommentauthorcollection)
### getWebExtensionTaskPanes() {#getWebExtensionTaskPanes--}
```
public WebExtensionTaskPaneCollection getWebExtensionTaskPanes()
```


Ermittelt die Liste der Task-Panes.

**Returns:**
[WebExtensionTaskPaneCollection](../../com.aspose.cells/webextensiontaskpanecollection)
### getWebExtensions() {#getWebExtensions--}
```
public WebExtensionCollection getWebExtensions()
```


Ermittelt die Liste der Task-Panes.

**Returns:**
[WebExtensionCollection](../../com.aspose.cells/webextensioncollection)
### getXmlMaps() {#getXmlMaps--}
```
public XmlMapCollection getXmlMaps()
```


Ermittelt die XML-Maps im Arbeitsbuch.

**Returns:**
[XmlMapCollection](../../com.aspose.cells/xmlmapcollection)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz. |

**Returns:**
int - Der Index des Wertes, falls in der Liste gefunden; sonst -1.
### insert(int index, int sheetType) {#insert-int-int-}
```
public Worksheet insert(int index, int sheetType)
```


Fügt ein Arbeitsblatt ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der Blattindex |
| sheetType | int | [SheetType](../../com.aspose.cells/sheettype). Der Blatttyp. |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - Returns an inserted worksheet.
### insert(int index, int sheetType, String sheetName) {#insert-int-int-java.lang.String-}
```
public Worksheet insert(int index, int sheetType, String sheetName)
```


Fügt ein Arbeitsblatt ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der Blattindex |
| sheetType | int | [SheetType](../../com.aspose.cells/sheettype). Der Blatttyp. |
| sheetName | java.lang.String | Der Blattname. |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - Returns an inserted worksheet.
### isRefreshAllConnections() {#isRefreshAllConnections--}
```
public boolean isRefreshAllConnections()
```


Gibt an, ob beim Öffnen der Datei in MS Excel alle Verbindungen aktualisiert werden.

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


Gibt einen Enumerator zurück, der die CollectionBase-Instanz durchläuft.

**Returns:**
java.util.Iterator - Ein Iterator für die CollectionBase-Instanz.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refreshAll() {#refreshAll--}
```
public void refreshAll()
```


Aktualisiert alle Pivot-Tabellen und Diagramme mit der Pivot-Quelle.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode Workbook.RefreshAll(). Diese Methode wird 12 Monate später, seit April 2026, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### refreshPivotTables() {#refreshPivotTables--}
```
public void refreshPivotTables()
```


Aktualisiert alle PivotTables in der Excel-Datei.

### refreshPivotTables(PivotTableRefreshOption option) {#refreshPivotTables-com.aspose.cells.PivotTableRefreshOption-}
```
public boolean refreshPivotTables(PivotTableRefreshOption option)
```


Aktualisiert alle PivotTables in der Excel-Datei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) | Die Option zum Aktualisieren der Datenquelle der Pivot-Tabellen. |

**Returns:**
boolean
### registerAddInFunction(int id, String functionName) {#registerAddInFunction-int-java.lang.String-}
```
public String registerAddInFunction(int id, String functionName)
```


Fügt dem Arbeitsbuch eine Add-In-Funktion hinzu

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| id | int | ID der Daten, die Add-In-Funktionen enthalten, kann durch den ersten Aufruf von [registerAddInFunction(String,String,boolean)](../../com.aspose.cells/worksheetcollection\#registerAddInFunction-String-String-boolean-) für dieselbe Add-In-Datei erhalten werden. |
| functionName | java.lang.String | der Add-In-Funktionsname |

**Returns:**
java.lang.String - URL der Add-In-Datei, die Add-In-Funktionen enthält
### registerAddInFunction(String addInFile, String functionName, boolean lib) {#registerAddInFunction-java.lang.String-java.lang.String-boolean-}
```
public int registerAddInFunction(String addInFile, String functionName, boolean lib)
```


Fügt dem Arbeitsbuch eine Add-In-Funktion hinzu

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| addInFile | java.lang.String | die Datei enthält die Add-In-Funktionen |
| functionName | java.lang.String | der Add-In-Funktionsname |
| lib | boolean | ob die angegebene Add-In-Datei im Verzeichnis oder Unterverzeichnis der Workbook-Add-In-Bibliothek liegt. Dieses Flag tritt in Kraft und macht einen Unterschied, wenn die angegebene addInFile ein relativer Pfad ist: true bedeutet, der Pfad ist relativ zur Add-In-Bibliothek, und false bedeutet, der Pfad ist relativ zu diesem Workbook. |

**Returns:**
int - ID der Daten, die die angegebene Add-In-Funktion enthalten
### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Entfernt das Element an einem angegebenen Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der Indexwert des zu entfernenden Elements. |

### removeAt(String name) {#removeAt-java.lang.String-}
```
public void removeAt(String name)
```


Entfernt das Element mit einem angegebenen Namen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | Der Name des zu entfernenden Elements. |

### setActiveSheetIndex(int value) {#setActiveSheetIndex-int-}
```
public void setActiveSheetIndex(int value)
```


Stellt den Index des aktiven Arbeitsblatts dar, wenn die Tabelle geöffnet wird.

**Remarks**

Der Arbeitsblattindex ist nullbasiert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setActiveSheetName(String value) {#setActiveSheetName-java.lang.String-}
```
public void setActiveSheetName(String value)
```


Stellt den Namen des aktiven Arbeitsblatts dar, wenn die Tabelle geöffnet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setOleSize(int startRow, int endRow, int startColumn, int endColumn) {#setOleSize-int-int-int-int-}
```
public void setOleSize(int startRow, int endRow, int startColumn, int endColumn)
```


Legt die angezeigte Größe fest, wenn die Arbeitsmappendatei als Ole-Objekt verwendet wird.

**Remarks**

Diese Methode wird allgemein verwendet, um die Anzeigegröße in PPT- oder DOC-Dateien anzupassen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | int | Startzeilenindex. |
| endRow | int | Endzeilenindex. |
| startColumn | int | Startspaltenindex. |
| endColumn | int | Endspaltenindex. |

### setOleSize(Object value) {#setOleSize-java.lang.Object-}
```
public void setOleSize(Object value)
```


Legt die angezeigte Größe fest, wenn die Arbeitsmappendatei als Ole-Objekt verwendet wird.

**Remarks**

Null bedeutet keine OLE‑Größeneinstellung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.Object |  |

### setRefreshAllConnections(boolean value) {#setRefreshAllConnections-boolean-}
```
public void setRefreshAllConnections(boolean value)
```


Gibt an, ob beim Öffnen der Datei in MS Excel alle Verbindungen aktualisiert werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setXmlMaps(XmlMapCollection value) {#setXmlMaps-com.aspose.cells.XmlMapCollection-}
```
public void setXmlMaps(XmlMapCollection value)
```


Legt die XML-Maps im Arbeitsbuch fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [XmlMapCollection](../../com.aspose.cells/xmlmapcollection) |  |

### sortNames() {#sortNames--}
```
public void sortNames()
```


Sortiert die definierten Namen.

**Remarks**

Wenn Sie eine große Anzahl benannter Bereiche in der Excel-Datei erstellen, rufen Sie diese Methode bitte auf, nachdem alle benannten Bereiche erstellt wurden und bevor Sie speichern.

### swapSheet(int sheetIndex1, int sheetIndex2) {#swapSheet-int-int-}
```
public void swapSheet(int sheetIndex1, int sheetIndex2)
```


Vertauscht die beiden Blätter.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetIndex1 | int | Das erste Arbeitsblatt. |
| sheetIndex2 | int | Das zweite Arbeitsblatt. |

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

