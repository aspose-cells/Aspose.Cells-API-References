---
title: "WorksheetCollection"
second_title: "Aspose.Cells för Java API-referens"
description: "Inkapslar en samling av objekt."
type: docs
url: /sv/java/com.aspose.cells/worksheetcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class WorksheetCollection extends CollectionBase
```

Innesluter en samling av [Worksheet](../../com.aspose.cells/worksheet)-objekt.

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
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add()](#add--) | Lägger till ett kalkylblad i samlingen. |
| [add(int type)](#add-int-) | Lägger till ett kalkylblad i samlingen. |
| [add(Object o)](#add-java.lang.Object-) | Lägger till ett objekt i CollectionBase-instansen. |
| [add(String sheetName)](#add-java.lang.String-) | Lägger till ett kalkylblad i samlingen. |
| [addCopy(Worksheet[] source, String[] destSheetNames)](#addCopy-com.aspose.cells.Worksheet---java.lang.String---) | Kopiera en grupp av kalkylblad. |
| [addCopy(int sheetIndex)](#addCopy-int-) | Lägger till ett kalkylblad i samlingen och kopierar data från ett befintligt kalkylblad. |
| [addCopy(String sheetName)](#addCopy-java.lang.String-) | Lägger till ett kalkylblad i samlingen och kopierar data från ett befintligt kalkylblad. |
| [clear()](#clear--) | Rensa alla kalkylblad. |
| [clearPivottables()](#clearPivottables--) | Rensar pivottabeller från kalkylbladet. |
| [contains(Object o)](#contains-java.lang.Object-) | Returnerar om instansen innehåller detta objekt |
| [createRange(String address, int sheetIndex)](#createRange-java.lang.String-int-) | Skapar ett [Range](../../com.aspose.cells/range)-objekt från en adress för området. |
| [createUnionRange(String address, int sheetIndex)](#createUnionRange-java.lang.String-int-) | Skapar ett [Range](../../com.aspose.cells/range)-objekt från en adress för området. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Hämtar [Worksheet](../../com.aspose.cells/worksheet)-elementet på det angivna indexet. |
| [get(String sheetName)](#get-java.lang.String-) | Hämtar [Worksheet](../../com.aspose.cells/worksheet)-elementet med det angivna namnet. |
| [getActiveSheetIndex()](#getActiveSheetIndex--) | Representerar indexet för det aktiva kalkylbladet när kalkylbladet öppnas. |
| [getActiveSheetName()](#getActiveSheetName--) | Representerar namnet på det aktiva kalkylbladet när kalkylbladet öppnas. |
| [getBuiltInDocumentProperties()](#getBuiltInDocumentProperties--) | Returnerar en [DocumentProperty](../../com.aspose.cells/documentproperty) samling som representerar alla inbyggda dokumentegenskaper i kalkylbladet. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Hämtar antalet element som finns i CollectionBase-instansen. |
| [getCustomDocumentProperties()](#getCustomDocumentProperties--) | Returnerar en [DocumentProperty](../../com.aspose.cells/documentproperty) samling som representerar alla anpassade dokumentegenskaper i kalkylbladet. |
| [getDxfs()](#getDxfs--) | Hämtar huvudposterna för differensialformatering. |
| [getExternalLinks()](#getExternalLinks--) | Representerar externa länkar i en arbetsbok. |
| [getNamedRanges()](#getNamedRanges--) | Hämtar alla fördefinierade namngivna områden i kalkylbladet. |
| [getNamedRangesAndTables()](#getNamedRangesAndTables--) | Hämtar alla fördefinierade namngivna områden i kalkylbladet. |
| [getNames()](#getNames--) | Hämtar samlingen av alla Name-objekt i kalkylbladet. |
| [getOleSize()](#getOleSize--) | Hämtar den visade storleken när Workbook-filen används som ett Ole-objekt. |
| [getPivotCaches()](#getPivotCaches--) | Hämtar alla [PivotCache](../../com.aspose.cells/pivotcache). |
| [getRangeByName(String rangeName)](#getRangeByName-java.lang.String-) | Hämtar Range-objektet efter fördefinierat namn. |
| [getRangeByName(String rangeName, int currentSheetIndex, boolean includeTable)](#getRangeByName-java.lang.String-int-boolean-) | Hämtar [Range](../../com.aspose.cells/range) efter fördefinierat namn eller tabellens namn |
| [getRevisionLogs()](#getRevisionLogs--) | Representerar revisionsloggar. |
| [getSensitivityLabels()](#getSensitivityLabels--) | Representerar alla känslighetsetiketter. |
| [getSheetByCodeName(String codeName)](#getSheetByCodeName-java.lang.String-) | Hämtar kalkylbladet efter kodnamnet. |
| [getTableStyles()](#getTableStyles--) | Hämtar [getTableStyles()](../../com.aspose.cells/worksheetcollection\#getTableStyles--) objektet. |
| [getThreadedCommentAuthors()](#getThreadedCommentAuthors--) | Hämtar listan över trådade kommentarsförfattare. |
| [getWebExtensionTaskPanes()](#getWebExtensionTaskPanes--) | Hämtar listan över uppgiftspaneler. |
| [getWebExtensions()](#getWebExtensions--) | Hämtar listan över uppgiftspaneler. |
| [getXmlMaps()](#getXmlMaps--) | Hämtar XML-kartorna i arbetsboken. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen. |
| [insert(int index, int sheetType)](#insert-int-int-) | Infoga ett kalkylblad. |
| [insert(int index, int sheetType, String sheetName)](#insert-int-int-java.lang.String-) | Infoga ett kalkylblad. |
| [isRefreshAllConnections()](#isRefreshAllConnections--) | Anger om alla anslutningar ska uppdateras vid öppning av filen i MS Excel. |
| [iterator()](#iterator--) | Returnerar en enumerator som itererar genom CollectionBase-instansen. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshAll()](#refreshAll--) | Uppdatera alla pivottabeller och diagram med pivottabellskälla. |
| [refreshPivotTables()](#refreshPivotTables--) | Uppdaterar alla PivotTables i Excel-filen. |
| [refreshPivotTables(PivotTableRefreshOption option)](#refreshPivotTables-com.aspose.cells.PivotTableRefreshOption-) | Uppdaterar alla PivotTables i Excel-filen. |
| [registerAddInFunction(int id, String functionName)](#registerAddInFunction-int-java.lang.String-) | Lägger till tilläggsfunktion i arbetsboken |
| [registerAddInFunction(String addInFile, String functionName, boolean lib)](#registerAddInFunction-java.lang.String-java.lang.String-boolean-) | Lägger till tilläggsfunktion i arbetsboken |
| [removeAt(int index)](#removeAt-int-) | Tar bort elementet på ett angivet index. |
| [removeAt(String name)](#removeAt-java.lang.String-) | Tar bort elementet med ett angivet namn. |
| [setActiveSheetIndex(int value)](#setActiveSheetIndex-int-) | Representerar indexet för det aktiva kalkylbladet när kalkylbladet öppnas. |
| [setActiveSheetName(String value)](#setActiveSheetName-java.lang.String-) | Representerar namnet på det aktiva kalkylbladet när kalkylbladet öppnas. |
| [setOleSize(int startRow, int endRow, int startColumn, int endColumn)](#setOleSize-int-int-int-int-) | Ställer in visad storlek när arbetsbokfilen används som ett Ole-objekt. |
| [setOleSize(Object value)](#setOleSize-java.lang.Object-) | Ställer in visad storlek när arbetsbokfilen används som ett Ole-objekt. |
| [setRefreshAllConnections(boolean value)](#setRefreshAllConnections-boolean-) | Anger om alla anslutningar ska uppdateras vid öppning av filen i MS Excel. |
| [setXmlMaps(XmlMapCollection value)](#setXmlMaps-com.aspose.cells.XmlMapCollection-) | Ställer in XML-kartorna i arbetsboken. |
| [sortNames()](#sortNames--) | Sorterar de definierade namnen. |
| [swapSheet(int sheetIndex1, int sheetIndex2)](#swapSheet-int-int-) | Byter plats på de två bladen. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add() {#add--}
```
public int add()
```


Lägger till ett kalkylblad i samlingen.

**Returns:**
int - [Worksheet](../../com.aspose.cells/worksheet) objektindex.
### add(int type) {#add-int-}
```
public int add(int type)
```


Lägger till ett kalkylblad i samlingen.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| type | int | [SheetType](../../com.aspose.cells/sheettype). Kalkylbladstyp. |

**Returns:**
int - [Worksheet](../../com.aspose.cells/worksheet) objektindex.
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Lägger till ett objekt i CollectionBase-instansen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | java.lang.Object | Objektet som ska läggas till i CollectionBase-instansen. |

**Returns:**
int - Positionen där det nya elementet infördes.
### add(String sheetName) {#add-java.lang.String-}
```
public Worksheet add(String sheetName)
```


Lägger till ett kalkylblad i samlingen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetName | java.lang.String | Kalkylbladsnamn |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - [Worksheet](../../com.aspose.cells/worksheet) object.
### addCopy(Worksheet[] source, String[] destSheetNames) {#addCopy-com.aspose.cells.Worksheet---java.lang.String---}
```
public void addCopy(Worksheet[] source, String[] destSheetNames)
```


Kopiera en grupp av kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| source | [Worksheet\[\]](../../com.aspose.cells/worksheet) | Källkalkylbladen. |
| destSheetNames | java.lang.String[] | Namnen på de kopierade bladen. |

### addCopy(int sheetIndex) {#addCopy-int-}
```
public int addCopy(int sheetIndex)
```


Lägger till ett kalkylblad i samlingen och kopierar data från ett befintligt kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetIndex | int | Index för källkalkylblad. |

**Returns:**
int - [Worksheet](../../com.aspose.cells/worksheet) objektindex.
### addCopy(String sheetName) {#addCopy-java.lang.String-}
```
public int addCopy(String sheetName)
```


Lägger till ett kalkylblad i samlingen och kopierar data från ett befintligt kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetName | java.lang.String | Namn på källkalkylblad. |

**Returns:**
int - [Worksheet](../../com.aspose.cells/worksheet) objektindex.
### clear() {#clear--}
```
public void clear()
```


Rensa alla kalkylblad.

**Remarks**

En arbetsbok måste innehålla ett kalkylblad.

### clearPivottables() {#clearPivottables--}
```
public void clearPivottables()
```


Rensar pivottabeller från kalkylbladet.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Returnerar om instansen innehåller detta objekt

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | java.lang.Object | testobjekt |

**Returns:**
boolean - Om instansen innehåller detta objekt
### createRange(String address, int sheetIndex) {#createRange-java.lang.String-int-}
```
public Range createRange(String address, int sheetIndex)
```


Skapar ett [Range](../../com.aspose.cells/range)-objekt från en adress för området.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| adress | java.lang.String | Adressen för området. |
| sheetIndex | int | Bladets index. |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### createUnionRange(String address, int sheetIndex) {#createUnionRange-java.lang.String-int-}
```
public UnionRange createUnionRange(String address, int sheetIndex)
```


Skapar ett [Range](../../com.aspose.cells/range)-objekt från en adress för området.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| adress | java.lang.String | Adressen för området. |
| sheetIndex | int | Bladets index. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - A [Range](../../com.aspose.cells/range) object
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
### get(int index) {#get-int-}
```
public Worksheet get(int index)
```


Hämtar [Worksheet](../../com.aspose.cells/worksheet)-elementet på det angivna indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Det nollbaserade indexet för elementet. |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - The element at the specified index.
### get(String sheetName) {#get-java.lang.String-}
```
public Worksheet get(String sheetName)
```


Hämtar [Worksheet](../../com.aspose.cells/worksheet)-elementet med det angivna namnet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetName | java.lang.String | Kalkylbladsnamn |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - The element with the specified name.
### getActiveSheetIndex() {#getActiveSheetIndex--}
```
public int getActiveSheetIndex()
```


Representerar indexet för det aktiva kalkylbladet när kalkylbladet öppnas.

**Remarks**

Bladindex är nollbaserat.

**Returns:**
int
### getActiveSheetName() {#getActiveSheetName--}
```
public String getActiveSheetName()
```


Representerar namnet på det aktiva kalkylbladet när kalkylbladet öppnas.

**Returns:**
java.lang.String
### getBuiltInDocumentProperties() {#getBuiltInDocumentProperties--}
```
public BuiltInDocumentPropertyCollection getBuiltInDocumentProperties()
```


Returnerar en [DocumentProperty](../../com.aspose.cells/documentproperty) samling som representerar alla inbyggda dokumentegenskaper i kalkylbladet.

**Remarks**

En ny egenskap kan inte läggas till i listan över inbyggda dokumentegenskaper. Du kan bara hämta en inbyggd egenskap och ändra dess värde. Följande är listan över namn på inbyggda egenskaper:

Titel

Ämne

Författare

Nyckelord

Kommentarer

Mall

Senaste författare

Revisionsnummer

Programnamn

Senaste utskriftsdatum

Skapandedatum

Senaste sparningstid

Total redigeringstid

Antal sidor

Antal ord

Antal tecken

Säkerhet

Kategori

Format

Ansvarig

Företag

Antal byte

Antal rader

Antal stycken

Antal bilder

Antal anteckningar

Antal dolda bilder

Antal multimedieklipp

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


Hämtar antalet element som finns i CollectionBase-instansen.

**Returns:**
int - Antalet element som finns i CollectionBase-instansen.
### getCustomDocumentProperties() {#getCustomDocumentProperties--}
```
public CustomDocumentPropertyCollection getCustomDocumentProperties()
```


Returnerar en [DocumentProperty](../../com.aspose.cells/documentproperty) samling som representerar alla anpassade dokumentegenskaper i kalkylbladet.

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


Hämtar huvudposterna för differensialformatering.

**Returns:**
[DxfCollection](../../com.aspose.cells/dxfcollection)
### getExternalLinks() {#getExternalLinks--}
```
public ExternalLinkCollection getExternalLinks()
```


Representerar externa länkar i en arbetsbok.

**Returns:**
[ExternalLinkCollection](../../com.aspose.cells/externallinkcollection)
### getNamedRanges() {#getNamedRanges--}
```
public Range[] getNamedRanges()
```


Hämtar alla fördefinierade namngivna områden i kalkylbladet.

**Returns:**
com.aspose.cells.Range[] - En array av Range-objekt. Om den definierade Name-referensen är extern eller har flera intervall, returneras inget Range-objekt för detta Name.

Returnerar null om det namngivna intervallet inte finns.
### getNamedRangesAndTables() {#getNamedRangesAndTables--}
```
public Range[] getNamedRangesAndTables()
```


Hämtar alla fördefinierade namngivna områden i kalkylbladet.

**Returns:**
com.aspose.cells.Range[] - En array av Range-objekt.

Returnerar null om det namngivna intervallet inte finns.
### getNames() {#getNames--}
```
public NameCollection getNames()
```


Hämtar samlingen av alla Name-objekt i kalkylbladet.

**Returns:**
[NameCollection](../../com.aspose.cells/namecollection)
### getOleSize() {#getOleSize--}
```
public Object getOleSize()
```


Hämtar den visade storleken när Workbook-filen används som ett Ole-objekt.

**Remarks**

Null betyder ingen ole-storleksinställning.

**Returns:**
java.lang.Object
### getPivotCaches() {#getPivotCaches--}
```
public PivotCacheCollection getPivotCaches()
```


Hämtar alla [PivotCache](../../com.aspose.cells/pivotcache).

**Returns:**
[PivotCacheCollection](../../com.aspose.cells/pivotcachecollection)
### getRangeByName(String rangeName) {#getRangeByName-java.lang.String-}
```
public Range getRangeByName(String rangeName)
```


Hämtar Range-objektet efter fördefinierat namn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rangeName | java.lang.String | Namn på intervallet. |

**Returns:**
[Range](../../com.aspose.cells/range) - Range object.

Returnerar null om det namngivna intervallet inte finns.
### getRangeByName(String rangeName, int currentSheetIndex, boolean includeTable) {#getRangeByName-java.lang.String-int-boolean-}
```
public Range getRangeByName(String rangeName, int currentSheetIndex, boolean includeTable)
```


Hämtar [Range](../../com.aspose.cells/range) efter fördefinierat namn eller tabellens namn

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rangeName | java.lang.String | Namn på intervallet eller tabellens namn. |
| currentSheetIndex | int | Bladindexet. -1 representerar globalt. |
| includeTable | boolean | Indikerar om alla tabeller ska kontrolleras. |

**Returns:**
[Range](../../com.aspose.cells/range) - 
### getRevisionLogs() {#getRevisionLogs--}
```
public RevisionLogCollection getRevisionLogs()
```


Representerar revisionsloggar.

**Returns:**
[RevisionLogCollection](../../com.aspose.cells/revisionlogcollection)
### getSensitivityLabels() {#getSensitivityLabels--}
```
public SensitivityLabelCollection getSensitivityLabels()
```


Representerar alla känslighetsetiketter.

**Returns:**
[SensitivityLabelCollection](../../com.aspose.cells/sensitivitylabelcollection)
### getSheetByCodeName(String codeName) {#getSheetByCodeName-java.lang.String-}
```
public Worksheet getSheetByCodeName(String codeName)
```


Hämtar kalkylbladet efter kodnamnet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| codeName | java.lang.String | Arbetsbladets kodnamn. |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - The element with the specified code name.
### getTableStyles() {#getTableStyles--}
```
public TableStyleCollection getTableStyles()
```


Hämtar [getTableStyles()](../../com.aspose.cells/worksheetcollection\#getTableStyles--) objektet.

**Returns:**
[TableStyleCollection](../../com.aspose.cells/tablestylecollection)
### getThreadedCommentAuthors() {#getThreadedCommentAuthors--}
```
public ThreadedCommentAuthorCollection getThreadedCommentAuthors()
```


Hämtar listan över trådade kommentarsförfattare.

**Returns:**
[ThreadedCommentAuthorCollection](../../com.aspose.cells/threadedcommentauthorcollection)
### getWebExtensionTaskPanes() {#getWebExtensionTaskPanes--}
```
public WebExtensionTaskPaneCollection getWebExtensionTaskPanes()
```


Hämtar listan över uppgiftspaneler.

**Returns:**
[WebExtensionTaskPaneCollection](../../com.aspose.cells/webextensiontaskpanecollection)
### getWebExtensions() {#getWebExtensions--}
```
public WebExtensionCollection getWebExtensions()
```


Hämtar listan över uppgiftspaneler.

**Returns:**
[WebExtensionCollection](../../com.aspose.cells/webextensioncollection)
### getXmlMaps() {#getXmlMaps--}
```
public XmlMapCollection getXmlMaps()
```


Hämtar XML-kartorna i arbetsboken.

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


Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | java.lang.Object | Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen. |

**Returns:**
int - Indexet för värdet om det hittas i listan; annars -1.
### insert(int index, int sheetType) {#insert-int-int-}
```
public Worksheet insert(int index, int sheetType)
```


Infoga ett kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Bladindexet |
| sheetType | int | [SheetType](../../com.aspose.cells/sheettype). Bladtypen. |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - Returns an inserted worksheet.
### insert(int index, int sheetType, String sheetName) {#insert-int-int-java.lang.String-}
```
public Worksheet insert(int index, int sheetType, String sheetName)
```


Infoga ett kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Bladindexet |
| sheetType | int | [SheetType](../../com.aspose.cells/sheettype). Bladtypen. |
| sheetName | java.lang.String | Bladnamnet. |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - Returns an inserted worksheet.
### isRefreshAllConnections() {#isRefreshAllConnections--}
```
public boolean isRefreshAllConnections()
```


Anger om alla anslutningar ska uppdateras vid öppning av filen i MS Excel.

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


Returnerar en enumerator som itererar genom CollectionBase-instansen.

**Returns:**
java.util.Iterator - En iterator för CollectionBase-instansen.
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


Uppdatera alla pivottabeller och diagram med pivottabellskälla.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället Workbook.RefreshAll()-metoden. Denna metod kommer att tas bort 12 månader senare från och med april 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### refreshPivotTables() {#refreshPivotTables--}
```
public void refreshPivotTables()
```


Uppdaterar alla PivotTables i Excel-filen.

### refreshPivotTables(PivotTableRefreshOption option) {#refreshPivotTables-com.aspose.cells.PivotTableRefreshOption-}
```
public boolean refreshPivotTables(PivotTableRefreshOption option)
```


Uppdaterar alla PivotTables i Excel-filen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) | Alternativet för att uppdatera datakällan för pivottabellerna. |

**Returns:**
boolean
### registerAddInFunction(int id, String functionName) {#registerAddInFunction-int-java.lang.String-}
```
public String registerAddInFunction(int id, String functionName)
```


Lägger till tilläggsfunktion i arbetsboken

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| id | int | ID för den data som innehåller tilläggsfunktioner, kan erhållas genom det första anropet av [registerAddInFunction(String,String,boolean)](../../com.aspose.cells/worksheetcollection\#registerAddInFunction-String-String-boolean-) för samma tilläggsfil. |
| functionName | java.lang.String | tilläggsfunktionens namn |

**Returns:**
java.lang.String - URL för tilläggsfilen som innehåller tilläggsfunktioner
### registerAddInFunction(String addInFile, String functionName, boolean lib) {#registerAddInFunction-java.lang.String-java.lang.String-boolean-}
```
public int registerAddInFunction(String addInFile, String functionName, boolean lib)
```


Lägger till tilläggsfunktion i arbetsboken

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| addInFile | java.lang.String | filen innehåller tilläggsfunktionerna |
| functionName | java.lang.String | tilläggsfunktionens namn |
| lib | boolean | om den angivna addin-filen finns i katalogen eller underkatalogen för Workbook Add-In library. Denna flagga träder i kraft och gör skillnad när given addInFile är en relativ sökväg: true betyder att sökvägen är relativ till Add-In library och false betyder att sökvägen är relativ till denna Workbook. |

**Returns:**
int - ID för den data som innehåller given addin-funktion
### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Tar bort elementet på ett angivet index.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Indexvärdet för elementet som ska tas bort. |

### removeAt(String name) {#removeAt-java.lang.String-}
```
public void removeAt(String name)
```


Tar bort elementet med ett angivet namn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Namnet på elementet som ska tas bort. |

### setActiveSheetIndex(int value) {#setActiveSheetIndex-int-}
```
public void setActiveSheetIndex(int value)
```


Representerar indexet för det aktiva kalkylbladet när kalkylbladet öppnas.

**Remarks**

Bladindex är nollbaserat.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setActiveSheetName(String value) {#setActiveSheetName-java.lang.String-}
```
public void setActiveSheetName(String value)
```


Representerar namnet på det aktiva kalkylbladet när kalkylbladet öppnas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setOleSize(int startRow, int endRow, int startColumn, int endColumn) {#setOleSize-int-int-int-int-}
```
public void setOleSize(int startRow, int endRow, int startColumn, int endColumn)
```


Ställer in visad storlek när arbetsbokfilen används som ett Ole-objekt.

**Remarks**

Denna metod används vanligtvis för att justera visningsstorleken i ppt-fil eller doc-fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRad | int | Startradens index. |
| slutRad | int | Slutradens index. |
| startColumn | int | Startkolumnens index. |
| endColumn | int | Slutkolumnens index. |

### setOleSize(Object value) {#setOleSize-java.lang.Object-}
```
public void setOleSize(Object value)
```


Ställer in visad storlek när arbetsbokfilen används som ett Ole-objekt.

**Remarks**

Null betyder ingen ole-storleksinställning.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.Object |  |

### setRefreshAllConnections(boolean value) {#setRefreshAllConnections-boolean-}
```
public void setRefreshAllConnections(boolean value)
```


Anger om alla anslutningar ska uppdateras vid öppning av filen i MS Excel.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setXmlMaps(XmlMapCollection value) {#setXmlMaps-com.aspose.cells.XmlMapCollection-}
```
public void setXmlMaps(XmlMapCollection value)
```


Ställer in XML-kartorna i arbetsboken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [XmlMapCollection](../../com.aspose.cells/xmlmapcollection) |  |

### sortNames() {#sortNames--}
```
public void sortNames()
```


Sorterar de definierade namnen.

**Remarks**

Om du skapar ett stort antal namngivna områden i Excel-filen, anropa denna metod efter att alla namngivna områden har skapats och innan du sparar.

### swapSheet(int sheetIndex1, int sheetIndex2) {#swapSheet-int-int-}
```
public void swapSheet(int sheetIndex1, int sheetIndex2)
```


Byter plats på de två bladen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetIndex1 | int | Det första kalkylbladet. |
| sheetIndex2 | int | Det andra kalkylbladet. |

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

