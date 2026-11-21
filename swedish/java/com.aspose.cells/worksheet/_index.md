---
title: "Kalkylblad"
second_title: "Aspose.Cells för Java API-referens"
description: "Inkapslar objektet som representerar ett enskilt kalkylblad."
type: docs
url: /sv/java/com.aspose.cells/worksheet/
---

**Inheritance:**
java.lang.Object
```
public class Worksheet
```

Inkapslar objektet som representerar ett enskilt kalkylblad.

**Example**

Följande exempel visar hur man fryser rutor och infogar hyperlänk till kalkylbladet med .Net eller VB.

```
         Workbook workbook = new Workbook();
 
         Worksheet sheet = workbook.getWorksheets().get(0);
 
         //Freeze panes at "AS40" with 10 rows and 10 columns
         sheet.freezePanes("AS40", 10, 10);
 
         //Add a hyperlink in Cell A1
         sheet.getHyperlinks().add("A1", 1, 1, "http://www.aspose.com");
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [addPageBreaks(String cellName)](#addPageBreaks-java.lang.String-) | Lägger till sidbrytning. |
| [advancedFilter(boolean isFilter, String listRange, String criteriaRange, String copyTo, boolean uniqueRecordOnly)](#advancedFilter-boolean-java.lang.String-java.lang.String-java.lang.String-boolean-) | Filtrerar data med komplexa kriterier. |
| [autoFitColumn(int columnIndex)](#autoFitColumn-int-) | Anpassar automatiskt kolumnbredden. |
| [autoFitColumn(int columnIndex, int firstRow, int lastRow)](#autoFitColumn-int-int-int-) | Anpassar automatiskt kolumnbredden. |
| [autoFitColumns()](#autoFitColumns--) | Anpassar automatiskt alla kolumner i detta kalkylblad. |
| [autoFitColumns(AutoFitterOptions options)](#autoFitColumns-com.aspose.cells.AutoFitterOptions-) | Anpassar automatiskt alla kolumner i detta kalkylblad. |
| [autoFitColumns(int firstColumn, int lastColumn)](#autoFitColumns-int-int-) | Anpassar automatiskt kolumnernas bredd. |
| [autoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options)](#autoFitColumns-int-int-com.aspose.cells.AutoFitterOptions-) | Anpassar automatiskt kolumnernas bredd. |
| [autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn)](#autoFitColumns-int-int-int-int-) | Anpassar automatiskt kolumnernas bredd. |
| [autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn, AutoFitterOptions options)](#autoFitColumns-int-int-int-int-com.aspose.cells.AutoFitterOptions-) | Anpassar automatiskt kolumnernas bredd. |
| [autoFitRow(int rowIndex)](#autoFitRow-int-) | Anpassar automatiskt radhöjden. |
| [autoFitRow(int rowIndex, int firstColumn, int lastColumn)](#autoFitRow-int-int-int-) | Anpassar automatiskt radhöjden. |
| [autoFitRow(int rowIndex, int firstColumn, int lastColumn, AutoFitterOptions options)](#autoFitRow-int-int-int-com.aspose.cells.AutoFitterOptions-) | Anpassar automatiskt radhöjden. |
| [autoFitRow(int startRow, int endRow, int startColumn, int endColumn)](#autoFitRow-int-int-int-int-) | Anpassar automatiskt radhöjden i ett rektangulärt område. |
| [autoFitRows()](#autoFitRows--) | Anpassar automatiskt alla rader i detta kalkylblad. |
| [autoFitRows(boolean onlyAuto)](#autoFitRows-boolean-) | Anpassar automatiskt alla rader i detta kalkylblad. |
| [autoFitRows(AutoFitterOptions options)](#autoFitRows-com.aspose.cells.AutoFitterOptions-) | Anpassar automatiskt alla rader i detta kalkylblad. |
| [autoFitRows(int startRow, int endRow)](#autoFitRows-int-int-) | Anpassar automatiskt radhöjden i ett område. |
| [autoFitRows(int startRow, int endRow, AutoFitterOptions options)](#autoFitRows-int-int-com.aspose.cells.AutoFitterOptions-) | Anpassar automatiskt radhöjden i ett område. |
| [calculateArrayFormula(String formula, CalculationOptions opts)](#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-) | Beräknar en formel som matrisformel. |
| [calculateArrayFormula(String formula, CalculationOptions opts, int maxRowCount, int maxColumnCount)](#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-int-int-) | Beräknar en formel som matrisformel. |
| [calculateArrayFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, int maxRowCount, int maxColumnCount, CalculationData calculationData)](#calculateArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-com.aspose.cells.CalculationOptions-int-int-int-int-com.aspose.cells.CalculationData-) | Beräknar en formel som matrisformel. |
| [calculateFormula(CalculationOptions options, boolean recursive)](#calculateFormula-com.aspose.cells.CalculationOptions-boolean-) | Beräknar alla formler i detta kalkylblad. |
| [calculateFormula(String formula)](#calculateFormula-java.lang.String-) | Beräknar en formel. |
| [calculateFormula(String formula, CalculationOptions opts)](#calculateFormula-java.lang.String-com.aspose.cells.CalculationOptions-) | Beräknar ett formeluttryck direkt. |
| [calculateFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, CalculationData calculationData)](#calculateFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-com.aspose.cells.CalculationOptions-int-int-com.aspose.cells.CalculationData-) | Beräknar ett formeluttryck direkt. |
| [clearComments()](#clearComments--) | Rensar alla kommentarer i designerns kalkylblad. |
| [closeAccessCache(int opts)](#closeAccessCache-int-) | Stänger sessionen som använder cache för att komma åt data i detta kalkylblad. |
| [convertFormulaReferenceStyle(String formula, boolean toR1C1, int baseCellRow, int baseCellColumn)](#convertFormulaReferenceStyle-java.lang.String-boolean-int-int-) | Konverterar formelreferensstilen. |
| [copy(Worksheet sourceSheet)](#copy-com.aspose.cells.Worksheet-) | Kopierar innehåll och format från ett annat kalkylblad. |
| [copy(Worksheet sourceSheet, CopyOptions copyOptions)](#copy-com.aspose.cells.Worksheet-com.aspose.cells.CopyOptions-) | Kopierar innehåll och format från ett annat kalkylblad. |
| [dispose()](#dispose--) | Utför applikationsdefinierade uppgifter som är relaterade till att frigöra, släppa eller återställa ohanterade resurser. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filter(CellArea ca)](#filter-com.aspose.cells.CellArea-) | Filtrerar området. |
| [freezePanes(int row, int column, int freezedRows, int freezedColumns)](#freezePanes-int-int-int-int-) | Fryser rutor vid den angivna cellen i kalkylbladet. |
| [freezePanes(String cellName, int freezedRows, int freezedColumns)](#freezePanes-java.lang.String-int-int-) | Fryser rutor vid den angivna cellen i kalkylbladet. |
| [getActiveCell()](#getActiveCell--) | Hämtar den aktiva cellen i kalkylbladet. |
| [getAdvancedFilter()](#getAdvancedFilter--) | Hämtar inställningarna för avancerat filter. |
| [getAllPictures()](#getAllPictures--) | Hämtar alla bilder, inklusive bilder som är inbäddade i cellen och över cellerna. |
| [getAllowEditRanges()](#getAllowEditRanges--) | Hämtar samlingen för tillåtna redigeringsområden i kalkylbladet. |
| [getAreasOfXmlMapQuery(String path, XmlMap xmlMap)](#getAreasOfXmlMapQuery-java.lang.String-com.aspose.cells.XmlMap-) | Fråga cellområden som mappades/länkades till den specifika sökvägen för xml‑kartan. |
| [getAutoFilter()](#getAutoFilter--) | Representerar autofilter för det angivna kalkylbladet. |
| [getBackgroundImage()](#getBackgroundImage--) | Hämtar kalkylbladets bakgrundsbild. |
| [getCellWatches()](#getCellWatches--) | Hämtar samling av celler i detta kalkylblad som övervakas i 'watch‑fönstret'. |
| [getCells()](#getCells--) | Hämtar [Cells](../../com.aspose.cells/cells)-samlingen. |
| [getCharts()](#getCharts--) | Hämtar en [Chart](../../com.aspose.cells/chart)-samling |
| [getCheckBoxes()](#getCheckBoxes--) | Hämtar en [CheckBox](../../com.aspose.cells/checkbox)-samling. |
| [getClass()](#getClass--) |  |
| [getCodeName()](#getCodeName--) | Hämtar kalkylbladets kodnamn. |
| [getComments()](#getComments--) | Hämtar [Comment](../../com.aspose.cells/comment)-samlingen. |
| [getConditionalFormattings()](#getConditionalFormattings--) | Hämtar ConditionalFormattings i kalkylbladet. |
| [getCustomProperties()](#getCustomProperties--) | Hämtar ett objekt som representerar identifieringsinformationen som är associerad med ett kalkylblad. |
| [getDisplayRightToLeft()](#getDisplayRightToLeft--) | Anger om det angivna kalkylbladet visas från höger till vänster istället för från vänster till höger. |
| [getDisplayZeros()](#getDisplayZeros--) | Sant om nollvärden visas. |
| [getErrorCheckOptions()](#getErrorCheckOptions--) | Hämtar felkontrollinställning som tillämpas på vissa områden. |
| [getFirstVisibleColumn()](#getFirstVisibleColumn--) | Representerar första synliga kolumnindex. |
| [getFirstVisibleRow()](#getFirstVisibleRow--) | Representerar första synliga radindex. |
| [getFreezedPanes()](#getFreezedPanes--) | Hämtar frysade rutor. |
| [getGridlineColor()](#getGridlineColor--) | Hämtar färgen på rutnätslinjen |
| [getHorizontalPageBreaks()](#getHorizontalPageBreaks--) | Hämtar [HorizontalPageBreakCollection](../../com.aspose.cells/horizontalpagebreakcollection)-samlingen. |
| [getHyperlinks()](#getHyperlinks--) | Hämtar [HyperlinkCollection](../../com.aspose.cells/hyperlinkcollection)-samlingen. |
| [getIndex()](#getIndex--) | Hämtar indexet för bladet i kalkylblads‑samlingen. |
| [getListObjects()](#getListObjects--) | Hämtar alla ListObjects i detta kalkylblad. |
| [getName()](#getName--) | Hämtar namnet på kalkylbladet. |
| [getOleObjects()](#getOleObjects--) | Representerar en samling av [OleObject](../../com.aspose.cells/oleobject) i ett kalkylblad. |
| [getOutline()](#getOutline--) | Hämtar konturen i detta kalkylblad. |
| [getPageSetup()](#getPageSetup--) | Representerar sidinställningsbeskrivningen i detta blad. |
| [getPaneState()](#getPaneState--) | Anger om panelen har horisontella eller vertikala delningar, och om dessa delningar är frysta. |
| [getPanes()](#getPanes--) | Hämtar fönsterpanelerna. |
| [getPictures()](#getPictures--) | Hämtar en [Picture](../../com.aspose.cells/picture)-samling. |
| [getPivotTables()](#getPivotTables--) | Hämtar alla pivottabeller i detta kalkylblad. |
| [getPrintingPageBreaks(ImageOrPrintOptions options)](#getPrintingPageBreaks-com.aspose.cells.ImageOrPrintOptions-) | Hämtar automatiska sidbrytningar. |
| [getProtection()](#getProtection--) | Representerar de olika typerna av skyddsalternativ som finns tillgängliga för ett kalkylblad. |
| [getQueryTables()](#getQueryTables--) | Hämtar [QueryTableCollection](../../com.aspose.cells/querytablecollection) i kalkylbladet. |
| [getScenarios()](#getScenarios--) | Hämtar samlingen av [Scenario](../../com.aspose.cells/scenario). |
| [getSelectedAreas()](#getSelectedAreas--) | Hämtar markerade cellområden i designerns kalkylblad. |
| [getSelectedRanges()](#getSelectedRanges--) | Hämtar markerade cellområden i designerns kalkylblad. |
| [getShapes()](#getShapes--) | Returnerar alla ritningsformer i detta kalkylblad. |
| [getShowDataTypeIcons()](#getShowDataTypeIcons--) | Anger om datatypikoner ska visas. |
| [getShowFormulas()](#getShowFormulas--) | Anger om formler eller deras resultat ska visas. |
| [getSlicers()](#getSlicers--) | Hämta Slicer-samlingen i kalkylbladet |
| [getSmartTagSetting()](#getSmartTagSetting--) | Hämtar alla [SmartTagCollection](../../com.aspose.cells/smarttagcollection)-objekt i kalkylbladet. |
| [getSparklineGroups()](#getSparklineGroups--) | Hämtar sparkline-grupperna i kalkylbladet. |
| [getTabColor()](#getTabColor--) | Representerar flikfärgen för kalkylbladet. |
| [getTabId()](#getTabId--) | Anger det interna identifieraren för bladet. |
| [getTextBoxes()](#getTextBoxes--) | Hämtar en [TextBox](../../com.aspose.cells/textbox)-samling. |
| [getTimelines()](#getTimelines--) | Hämta Timeline-samlingen i kalkylbladet |
| [getTransitionEntry()](#getTransitionEntry--) | Anger om alternativet Transition Formula Entry (Lotus-kompatibilitet) är aktiverat. |
| [getTransitionEvaluation()](#getTransitionEvaluation--) | Anger om alternativet Transition Formula Evaluation (Lotus-kompatibilitet) är aktiverat. |
| [getType()](#getType--) | Representerar kalkylbladstyp. |
| [getUniqueId()](#getUniqueId--) | Hämtar det unika ID:t, det är samma som \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\}. |
| [getValidations()](#getValidations--) | Hämtar samlingen av datavalideringsinställningar i kalkylbladet. |
| [getVerticalPageBreaks()](#getVerticalPageBreaks--) | Hämtar [VerticalPageBreakCollection](../../com.aspose.cells/verticalpagebreakcollection)-samlingen. |
| [getViewType()](#getViewType--) | Hämtar vytypen. |
| [getVisibilityType()](#getVisibilityType--) | Anger det synliga tillståndet för detta blad. |
| [getWorkbook()](#getWorkbook--) | Hämtar arbetsboksobjektet som innehåller detta blad. |
| [getZoom()](#getZoom--) | Representerar skalningsfaktorn i procent. |
| [hasAutofilter()](#hasAutofilter--) | Anger om detta kalkylblad har autofilter. |
| [hashCode()](#hashCode--) |  |
| [isGridlinesVisible()](#isGridlinesVisible--) | Hämtar ett värde som anger om rutnätslinjerna är synliga. Standard är true. |
| [isOutlineShown()](#isOutlineShown--) | Anger om konturen ska visas. |
| [isPageBreakPreview()](#isPageBreakPreview--) | Anger om det angivna kalkylbladet visas i normal vy eller sidbrytning förhandsgranskning. |
| [isProtected()](#isProtected--) | Anger om kalkylbladet är skyddat. |
| [isRowColumnHeadersVisible()](#isRowColumnHeadersVisible--) | Hämtar ett värde som anger om kalkylbladet ska visa rad- och kolumnrubriker. |
| [isRulerVisible()](#isRulerVisible--) | Anger om linjalen är synlig. |
| [isSelected()](#isSelected--) | Anger om detta kalkylblad är valt när arbetsboken öppnas. |
| [isVisible()](#isVisible--) | Representerar om kalkylbladet är synligt. |
| [moveTo(int index)](#moveTo-int-) | Flyttar bladet till en annan plats i kalkylarket. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [protect(int type)](#protect-int-) | Skyddar kalkylbladet. |
| [protect(int type, String password, String oldPassword)](#protect-int-java.lang.String-java.lang.String-) | Skyddar kalkylbladet. |
| [refreshPivotTables()](#refreshPivotTables--) | Uppdaterar alla pivottabeller i detta kalkylblad. |
| [refreshPivotTables(PivotTableRefreshOption option)](#refreshPivotTables-com.aspose.cells.PivotTableRefreshOption-) | Uppdaterar alla pivottabeller i detta kalkylblad. |
| [removeAllDrawingObjects()](#removeAllDrawingObjects--) | Tar bort alla ritobjekt i detta kalkylblad. |
| [removeAutoFilter()](#removeAutoFilter--) | Tar bort autofiltret för kalkylbladet. |
| [removeSplit()](#removeSplit--) | Tar bort delat fönster. |
| [replace(String oldString, String newString)](#replace-java.lang.String-java.lang.String-) | Ersätter all celltext med en ny sträng. |
| [selectRange(int startRow, int startColumn, int totalRows, int totalColumns, boolean removeOthers)](#selectRange-int-int-int-int-boolean-) | Markerar ett område. |
| [setActiveCell(String value)](#setActiveCell-java.lang.String-) | Ställer in den aktiva cellen i kalkylbladet. |
| [setBackgroundImage(byte[] value)](#setBackgroundImage-byte---) | Ställer in bakgrundsbild för kalkylbladet. |
| [setCodeName(String value)](#setCodeName-java.lang.String-) | Hämtar kalkylbladets kodnamn. |
| [setDisplayRightToLeft(boolean value)](#setDisplayRightToLeft-boolean-) | Anger om det angivna kalkylbladet visas från höger till vänster istället för från vänster till höger. |
| [setDisplayZeros(boolean value)](#setDisplayZeros-boolean-) | Sant om nollvärden visas. |
| [setFirstVisibleColumn(int value)](#setFirstVisibleColumn-int-) | Representerar första synliga kolumnindex. |
| [setFirstVisibleRow(int value)](#setFirstVisibleRow-int-) | Representerar första synliga radindex. |
| [setGridlineColor(Color value)](#setGridlineColor-com.aspose.cells.Color-) | Ställer in färgen på rutnätslinjen |
| [setGridlinesVisible(boolean value)](#setGridlinesVisible-boolean-) | Ställer in ett värde som anger om rutnätslinjerna är synliga. Standard är true. |
| [setName(String value)](#setName-java.lang.String-) | Ställer in namnet på kalkylbladet. |
| [setOutlineShown(boolean value)](#setOutlineShown-boolean-) | Anger om konturen ska visas. |
| [setPageBreakPreview(boolean value)](#setPageBreakPreview-boolean-) | Anger om det angivna kalkylbladet visas i normal vy eller sidbrytning förhandsgranskning. |
| [setRowColumnHeadersVisible(boolean value)](#setRowColumnHeadersVisible-boolean-) | Ställer in ett värde som indikerar om kalkylbladet ska visa rad- och kolumnrubriker. |
| [setRulerVisible(boolean value)](#setRulerVisible-boolean-) | Anger om linjalen är synlig. |
| [setSelected(boolean value)](#setSelected-boolean-) | Anger om detta kalkylblad är valt när arbetsboken öppnas. |
| [setShowDataTypeIcons(boolean value)](#setShowDataTypeIcons-boolean-) | Anger om datatypikoner ska visas. |
| [setShowFormulas(boolean value)](#setShowFormulas-boolean-) | Anger om formler eller deras resultat ska visas. |
| [setTabColor(Color value)](#setTabColor-com.aspose.cells.Color-) | Representerar flikfärgen för kalkylbladet. |
| [setTabId(int value)](#setTabId-int-) | Anger det interna identifieraren för bladet. |
| [setTransitionEntry(boolean value)](#setTransitionEntry-boolean-) | Anger om alternativet Transition Formula Entry (Lotus-kompatibilitet) är aktiverat. |
| [setTransitionEvaluation(boolean value)](#setTransitionEvaluation-boolean-) | Anger om alternativet Transition Formula Evaluation (Lotus-kompatibilitet) är aktiverat. |
| [setType(int value)](#setType-int-) | Representerar kalkylbladstyp. |
| [setUniqueId(String value)](#setUniqueId-java.lang.String-) | Ställer in det unika ID:t, det är samma som \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\}. |
| [setViewType(int value)](#setViewType-int-) | Ställer in visningstypen. |
| [setVisibilityType(int value)](#setVisibilityType-int-) | Anger det synliga tillståndet för detta blad. |
| [setVisible(boolean value)](#setVisible-boolean-) | Representerar om kalkylbladet är synligt. |
| [setVisible(boolean isVisible, boolean ignoreError)](#setVisible-boolean-boolean-) | Ställer in de synliga alternativen. |
| [setZoom(int value)](#setZoom-int-) | Representerar skalningsfaktorn i procent. |
| [split()](#split--) | Delar fönstret. |
| [startAccessCache(int opts)](#startAccessCache-int-) | Startar sessionen som använder cache för att komma åt data i detta kalkylblad. |
| [toString()](#toString--) | Returnerar en sträng som representerar det aktuella kalkylbladsobjektet. |
| [unFreezePanes()](#unFreezePanes--) | Låser upp paneler i kalkylbladet. |
| [unprotect()](#unprotect--) | Avskyddar kalkylbladet. |
| [unprotect(String password)](#unprotect-java.lang.String-) | Avskyddar kalkylbladet. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
| [xmlMapQuery(String path, XmlMap xmlMap)](#xmlMapQuery-java.lang.String-com.aspose.cells.XmlMap-) | Fråga cellområden som mappades/länkades till den specifika sökvägen för xml‑kartan. |
### addPageBreaks(String cellName) {#addPageBreaks-java.lang.String-}
```
public void addPageBreaks(String cellName)
```


Lägger till sidbrytning.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellNamn | java.lang.String |  |

### advancedFilter(boolean isFilter, String listRange, String criteriaRange, String copyTo, boolean uniqueRecordOnly) {#advancedFilter-boolean-java.lang.String-java.lang.String-java.lang.String-boolean-}
```
public void advancedFilter(boolean isFilter, String listRange, String criteriaRange, String copyTo, boolean uniqueRecordOnly)
```


Filtrerar data med komplexa kriterier.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isFilter | boolean | Indikerar om listan filtreras på plats. |
| listRange | java.lang.String | Listintervallet. |
| criteriaRange | java.lang.String | Kriterieintervallet. |
| copyTo | java.lang.String | Intervallet dit data kopieras. |
| uniqueRecordOnly | boolean | Visar eller kopierar endast unika rader. |

### autoFitColumn(int columnIndex) {#autoFitColumn-int-}
```
public void autoFitColumn(int columnIndex)
```


Anpassar automatiskt kolumnbredden.

**Remarks**

AutoFitColumn är en inexakt funktion.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | int | Kolumnindex. |

### autoFitColumn(int columnIndex, int firstRow, int lastRow) {#autoFitColumn-int-int-int-}
```
public void autoFitColumn(int columnIndex, int firstRow, int lastRow)
```


Anpassar automatiskt kolumnbredden.

**Remarks**

Denna metod anpassar automatiskt en rad baserat på innehållet i ett cellintervall inom raden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | int | Kolumnindex. |
| firstRow | int | Första radens index. |
| lastRow | int | Sista radens index. |

### autoFitColumns() {#autoFitColumns--}
```
public void autoFitColumns()
```


Anpassar automatiskt alla kolumner i detta kalkylblad.

### autoFitColumns(AutoFitterOptions options) {#autoFitColumns-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitColumns(AutoFitterOptions options)
```


Anpassar automatiskt alla kolumner i detta kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | De automatiska anpassningsalternativen |

### autoFitColumns(int firstColumn, int lastColumn) {#autoFitColumns-int-int-}
```
public void autoFitColumns(int firstColumn, int lastColumn)
```


Anpassar automatiskt kolumnernas bredd.

**Remarks**

AutoFitColumn är en inexakt funktion.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstColumn | int | Första kolumnens index. |
| lastColumn | int | Sista kolumnens index. |

### autoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options) {#autoFitColumns-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options)
```


Anpassar automatiskt kolumnernas bredd.

**Remarks**

AutoFitColumn är en inexakt funktion.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstColumn | int | Första kolumnens index. |
| lastColumn | int | Sista kolumnens index. |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | De automatiska anpassningsalternativen |

### autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn) {#autoFitColumns-int-int-int-int-}
```
public void autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn)
```


Anpassar automatiskt kolumnernas bredd.

**Remarks**

AutoFitColumn är en inexakt funktion.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstRow | int | Första radens index. |
| firstColumn | int | Första kolumnens index. |
| lastRow | int | Sista radens index. |
| lastColumn | int | Sista kolumnens index. |

### autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn, AutoFitterOptions options) {#autoFitColumns-int-int-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn, AutoFitterOptions options)
```


Anpassar automatiskt kolumnernas bredd.

**Remarks**

AutoFitColumn är en inexakt funktion.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstRow | int | Första radens index. |
| firstColumn | int | Första kolumnens index. |
| lastRow | int | Sista radens index. |
| lastColumn | int | Sista kolumnens index. |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | De automatiska anpassningsalternativen |

### autoFitRow(int rowIndex) {#autoFitRow-int-}
```
public void autoFitRow(int rowIndex)
```


Anpassar automatiskt radhöjden.

**Remarks**

AutoFitRow är en inexakt funktion.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | int | Radindex. |

### autoFitRow(int rowIndex, int firstColumn, int lastColumn) {#autoFitRow-int-int-int-}
```
public void autoFitRow(int rowIndex, int firstColumn, int lastColumn)
```


Anpassar automatiskt radhöjden.

**Remarks**

Denna metod anpassar automatiskt en rad baserat på innehållet i ett cellintervall inom raden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | int | Radindex. |
| firstColumn | int | Första kolumnens index. |
| lastColumn | int | Sista kolumnens index. |

### autoFitRow(int rowIndex, int firstColumn, int lastColumn, AutoFitterOptions options) {#autoFitRow-int-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitRow(int rowIndex, int firstColumn, int lastColumn, AutoFitterOptions options)
```


Anpassar automatiskt radhöjden.

**Remarks**

Denna metod anpassar automatiskt en rad baserat på innehållet i ett cellintervall inom raden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | int | Radindex. |
| firstColumn | int | Första kolumnens index. |
| lastColumn | int | Sista kolumnens index. |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | Alternativen för automatisk anpassning |

### autoFitRow(int startRow, int endRow, int startColumn, int endColumn) {#autoFitRow-int-int-int-int-}
```
public void autoFitRow(int startRow, int endRow, int startColumn, int endColumn)
```


Anpassar automatiskt radhöjden i ett rektangulärt område.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRad | int | Startradens index. |
| slutRad | int | Slutradens index. |
| startColumn | int | Startkolumnens index. |
| endColumn | int | Slutkolumnens index. |

### autoFitRows() {#autoFitRows--}
```
public void autoFitRows()
```


Anpassar automatiskt alla rader i detta kalkylblad.

### autoFitRows(boolean onlyAuto) {#autoFitRows-boolean-}
```
public void autoFitRows(boolean onlyAuto)
```


Anpassar automatiskt alla rader i detta kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| onlyAuto | boolean | True, endast autofitar radens höjd när radens höjd inte är anpassad. |

### autoFitRows(AutoFitterOptions options) {#autoFitRows-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitRows(AutoFitterOptions options)
```


Anpassar automatiskt alla rader i detta kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | Alternativen för automatisk anpassning |

### autoFitRows(int startRow, int endRow) {#autoFitRows-int-int-}
```
public void autoFitRows(int startRow, int endRow)
```


Anpassar automatiskt radhöjden i ett område.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRad | int | Startradens index. |
| slutRad | int | Slutradens index. |

### autoFitRows(int startRow, int endRow, AutoFitterOptions options) {#autoFitRows-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitRows(int startRow, int endRow, AutoFitterOptions options)
```


Anpassar automatiskt radhöjden i ett område.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRad | int | Startradens index. |
| slutRad | int | Slutradens index. |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | Alternativen för automatisk anpassning. |

### calculateArrayFormula(String formula, CalculationOptions opts) {#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-}
```
public Object[][] calculateArrayFormula(String formula, CalculationOptions opts)
```


Beräknar en formel som matrisformel.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formula | java.lang.String | Formel att beräkna. |
| opts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Alternativ för att beräkna formel |

**Returns:**
java.lang.Object[][]
### calculateArrayFormula(String formula, CalculationOptions opts, int maxRowCount, int maxColumnCount) {#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-int-int-}
```
public Object[][] calculateArrayFormula(String formula, CalculationOptions opts, int maxRowCount, int maxColumnCount)
```


Beräknar en formel som matrisformel.

**Remarks**

Formeln kommer att tas som en dynamisk array-formel för att beräkna dimensionen och resultatet. Användarspecificerad maximal dimension används för fall där det beräknade resultatet är en stor datamängd (till exempel kan det beräknade resultatet motsvara en hel rad- eller kolumndata) men användaren inte behöver så stor en array enligt affärskrav eller av prestandaskäl.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formula | java.lang.String | Formel att beräkna. |
| opts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Alternativ för att beräkna formel |
| maxRowCount | int | det maximala radantalet för resulterande data. Om det är icke-positivt eller större än det faktiska radantalet, används det faktiska radantalet. |
| maxColumnCount | int | det maximala kolumnantalet för resulterande data. Om det är icke-positivt eller större än det faktiska radantalet, används det faktiska kolumnantalet. |

**Returns:**
java.lang.Object[][] - Beräknat formelresultat.
### calculateArrayFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, int maxRowCount, int maxColumnCount, CalculationData calculationData) {#calculateArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-com.aspose.cells.CalculationOptions-int-int-int-int-com.aspose.cells.CalculationData-}
```
public Object[][] calculateArrayFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, int maxRowCount, int maxColumnCount, CalculationData calculationData)
```


Beräknar en formel som matrisformel.

**Remarks**

Formeln kommer att tas som en dynamisk array-formel för att beräkna dimensionen och resultatet. Användarspecificerad maximal dimension används för fall där det beräknade resultatet är en stor datamängd (till exempel kan det beräknade resultatet motsvara en hel rad- eller kolumndata) men användaren inte behöver så stor en array enligt affärskrav eller av prestandaskäl.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formula | java.lang.String | Formel att beräkna. |
| pOpts | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Alternativ för att tolka formel |
| cOpts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Alternativ för att beräkna formel |
| baseCellRow | int | Radindex för bascellen. |
| baseCellColumn | int | Kolumnindex för bascellen. |
| maxRowCount | int | Det maximala antalet rader i den resulterande datan. Om det är noll eller negativt eller större än det faktiska antalet rader, används det faktiska antalet rader. |
| maxColumnCount | int | Det maximala antalet kolumner i den resulterande datan. Om det är noll eller negativt eller större än det faktiska antalet kolumner, används det faktiska antalet kolumner. |
| calculationData | [CalculationData](../../com.aspose.cells/calculationdata) | Beräkningsdata. Den används när användaren behöver beräkna vissa statiska formler vid implementering av en anpassad beräkningsmotor. För sådana situationer måste användaren ange den med beräkningsdata som tillhandahålls för [AbstractCalculationEngine.calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-). |

**Returns:**
java.lang.Object[][] - Beräknat formelresultat.
### calculateFormula(CalculationOptions options, boolean recursive) {#calculateFormula-com.aspose.cells.CalculationOptions-boolean-}
```
public void calculateFormula(CalculationOptions options, boolean recursive)
```


Beräknar alla formler i detta kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| options | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Alternativ för beräkning |
| rekursiv | boolean | True betyder att om kalkylbladets celler beror på celler i andra kalkylblad, kommer de beroende cellerna i de andra kalkylbladen också att beräknas. False betyder att alla formler i kalkylbladet har beräknats och värdena är korrekta. |

### calculateFormula(String formula) {#calculateFormula-java.lang.String-}
```
public Object calculateFormula(String formula)
```


Beräknar en formel.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formula | java.lang.String | Formel att beräkna. |

**Returns:**
java.lang.Object - Beräknat formelresultat.
### calculateFormula(String formula, CalculationOptions opts) {#calculateFormula-java.lang.String-com.aspose.cells.CalculationOptions-}
```
public Object calculateFormula(String formula, CalculationOptions opts)
```


Beräknar ett formeluttryck direkt.

**Remarks**

Formeln kommer att beräknas precis som om den hade satts i cell A1. Och formeln kommer att behandlas som en normal formel. Om du behöver att formeln beräknas som en matrisformel och få en matris för det beräknade resultatet, använd [calculateArrayFormula(String,CalculationOptions)](../../com.aspose.cells/worksheet\#calculateArrayFormula-String-CalculationOptions-) istället.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formula | java.lang.String | Formel att beräkna. |
| opts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Alternativ för att beräkna formel |

**Returns:**
java.lang.Object - Beräknat resultat av given formel. Det returnerade objektet kan vara av möjliga typer som [Cell.getValue()](../../com.aspose.cells/cell\#getValue--), eller ReferredArea.
### calculateFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, CalculationData calculationData) {#calculateFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-com.aspose.cells.CalculationOptions-int-int-com.aspose.cells.CalculationData-}
```
public Object calculateFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, CalculationData calculationData)
```


Beräknar ett formeluttryck direkt.

**Remarks**

Formeln kommer att beräknas precis som om den hade satts i den angivna bascellen. Och formeln kommer att behandlas som en normal formel. Om du behöver att formeln beräknas som en matrisformel och få en matris för det beräknade resultatet, använd [calculateArrayFormula(String,FormulaParseOptions,CalculationOptions,int,int,int,int,CalculationData)](../../com.aspose.cells/worksheet\#calculateArrayFormula-String-FormulaParseOptions-CalculationOptions-int-int-int-int-CalculationData-) istället.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formula | java.lang.String | Formel att beräkna. |
| pOpts | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Alternativ för att tolka formel. |
| cOpts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Alternativ för att beräkna formel. |
| baseCellRow | int | Radindex för bascellen. |
| baseCellColumn | int | Kolumnindex för bascellen. |
| calculationData | [CalculationData](../../com.aspose.cells/calculationdata) | Beräkningsdata. Den används när användaren behöver beräkna vissa statiska formler vid implementering av en anpassad beräkningsmotor. För sådana situationer måste användaren ange den med beräkningsdata som tillhandahålls för [AbstractCalculationEngine.calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-). |

**Returns:**
java.lang.Object - Beräknat resultat av given formel. Det returnerade objektet kan vara av möjliga typer som [Cell.getValue()](../../com.aspose.cells/cell\#getValue--), eller ReferredArea.
### clearComments() {#clearComments--}
```
public void clearComments()
```


Rensar alla kommentarer i designerns kalkylblad.

### closeAccessCache(int opts) {#closeAccessCache-int-}
```
public void closeAccessCache(int opts)
```


Stänger sessionen som använder cache för att komma åt data i detta kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| opts | int | [AccessCacheOptions](../../com.aspose.cells/accesscacheoptions). alternativ för dataåtkomst |

### convertFormulaReferenceStyle(String formula, boolean toR1C1, int baseCellRow, int baseCellColumn) {#convertFormulaReferenceStyle-java.lang.String-boolean-int-int-}
```
public String convertFormulaReferenceStyle(String formula, boolean toR1C1, int baseCellRow, int baseCellColumn)
```


Konverterar formelreferensstilen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formula | java.lang.String | Formeln som ska konverteras. |
| toR1C1 | boolean | Vilken referensstil formeln ska konverteras till. Om den ursprungliga formeln är i A1-referensstil, bör detta värde vara true så att formeln konverteras från A1 till R1C1-referensstil; om den ursprungliga formeln är i R1C1-referensstil, bör detta värde vara false så att formeln konverteras från R1C1 till A1-referensstil; |
| baseCellRow | int | Radindex för bascellen. |
| baseCellColumn | int | Kolumnindex för bascellen. |

**Returns:**
java.lang.String - Den konverterade formeln.
### copy(Worksheet sourceSheet) {#copy-com.aspose.cells.Worksheet-}
```
public void copy(Worksheet sourceSheet)
```


Kopierar innehåll och format från ett annat kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceSheet | [Worksheet](../../com.aspose.cells/worksheet) | Källkalkylblad. |

### copy(Worksheet sourceSheet, CopyOptions copyOptions) {#copy-com.aspose.cells.Worksheet-com.aspose.cells.CopyOptions-}
```
public void copy(Worksheet sourceSheet, CopyOptions copyOptions)
```


Kopierar innehåll och format från ett annat kalkylblad.

**Remarks**

Du kan kopiera data från ett annat kalkylblad i samma fil eller en annan fil. Denna metod stöder dock inte kopiering av ritobjekt, såsom kommentarer, bilder och diagram.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceSheet | [Worksheet](../../com.aspose.cells/worksheet) | Källkalkylblad. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) |  |

### dispose() {#dispose--}
```
public void dispose()
```


Utför applikationsdefinierade uppgifter som är relaterade till att frigöra, släppa eller återställa ohanterade resurser.

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
### filter(CellArea ca) {#filter-com.aspose.cells.CellArea-}
```
public void filter(CellArea ca)
```


Filtrerar området.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Området |

### freezePanes(int row, int column, int freezedRows, int freezedColumns) {#freezePanes-int-int-int-int-}
```
public void freezePanes(int row, int column, int freezedRows, int freezedColumns)
```


Fryser rutor vid den angivna cellen i kalkylbladet.

**Remarks**

Radindex och kolumnindex kan inte alla vara noll. Antalet rader och antalet kolumner kan inte heller alla vara noll.

De två första parametrarna anger den frysta positionen och de två sista parametrarna anger området som är fryst i det vänstra övre fönstret.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindex. |
| kolumn | int | Kolumnindex. |
| freezedRows | int | Antal synliga rader i övre fönstret, högst lika med radindex. |
| freezedColumns | int | Antalet synliga kolumner i vänsterpanelen, högst kolumnindexet. |

### freezePanes(String cellName, int freezedRows, int freezedColumns) {#freezePanes-java.lang.String-int-int-}
```
public void freezePanes(String cellName, int freezedRows, int freezedColumns)
```


Fryser rutor vid den angivna cellen i kalkylbladet.

**Remarks**

Radindex och kolumnindex kan inte alla vara noll. Antalet rader och antalet kolumner kan inte heller alla vara noll.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellNamn | java.lang.String | Cellnamn. |
| freezedRows | int | Antal synliga rader i övre fönstret, högst lika med radindex. |
| freezedColumns | int | Antalet synliga kolumner i vänsterpanelen, högst kolumnindexet. |

### getActiveCell() {#getActiveCell--}
```
public String getActiveCell()
```


Hämtar den aktiva cellen i kalkylbladet.

**Returns:**
java.lang.String
### getAdvancedFilter() {#getAdvancedFilter--}
```
public AdvancedFilter getAdvancedFilter()
```


Hämtar inställningarna för avancerat filter.

**Returns:**
[AdvancedFilter](../../com.aspose.cells/advancedfilter) - 
### getAllPictures() {#getAllPictures--}
```
public Picture[] getAllPictures()
```


Hämtar alla bilder, inklusive bilder som är inbäddade i cellen och över cellerna.

**Returns:**
com.aspose.cells.Picture[] -
### getAllowEditRanges() {#getAllowEditRanges--}
```
public ProtectedRangeCollection getAllowEditRanges()
```


Hämtar samlingen för tillåtna redigeringsområden i kalkylbladet.

**Returns:**
[ProtectedRangeCollection](../../com.aspose.cells/protectedrangecollection)
### getAreasOfXmlMapQuery(String path, XmlMap xmlMap) {#getAreasOfXmlMapQuery-java.lang.String-com.aspose.cells.XmlMap-}
```
public CellArea[] getAreasOfXmlMapQuery(String path, XmlMap xmlMap)
```


Fråga cellområden som mappades/länkades till den specifika sökvägen för xml‑kartan.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sökväg | java.lang.String | xml-elementets sökväg |
| xmlMap | [XmlMap](../../com.aspose.cells/xmlmap) | Ange en xml-karta om du vill fråga efter den specifika sökvägen inom en specifik karta. |

**Returns:**
com.aspose.cells.CellArea[] - [CellArea](../../com.aspose.cells/cellarea) lista som är mappad/länkad till den specifika sökvägen i xml-kartan, en tom lista returneras om inget är mappat/länkat.
### getAutoFilter() {#getAutoFilter--}
```
public AutoFilter getAutoFilter()
```


Representerar autofilter för det angivna kalkylbladet.

**Returns:**
[AutoFilter](../../com.aspose.cells/autofilter)
### getBackgroundImage() {#getBackgroundImage--}
```
public byte[] getBackgroundImage()
```


Hämtar kalkylbladets bakgrundsbild.

**Returns:**
byte[]
### getCellWatches() {#getCellWatches--}
```
public CellWatchCollection getCellWatches()
```


Hämtar samling av celler i detta kalkylblad som övervakas i 'watch‑fönstret'.

**Returns:**
[CellWatchCollection](../../com.aspose.cells/cellwatchcollection)
### getCells() {#getCells--}
```
public Cells getCells()
```


Hämtar [Cells](../../com.aspose.cells/cells)-samlingen.

**Returns:**
[Cells](../../com.aspose.cells/cells)
### getCharts() {#getCharts--}
```
public ChartCollection getCharts()
```


Hämtar en [Chart](../../com.aspose.cells/chart)-samling

**Returns:**
[ChartCollection](../../com.aspose.cells/chartcollection)
### getCheckBoxes() {#getCheckBoxes--}
```
public CheckBoxCollection getCheckBoxes()
```


Hämtar en [CheckBox](../../com.aspose.cells/checkbox)-samling.

**Returns:**
[CheckBoxCollection](../../com.aspose.cells/checkboxcollection)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCodeName() {#getCodeName--}
```
public String getCodeName()
```


Hämtar kalkylbladets kodnamn.

**Returns:**
java.lang.String
### getComments() {#getComments--}
```
public CommentCollection getComments()
```


Hämtar [Comment](../../com.aspose.cells/comment)-samlingen.

**Returns:**
[CommentCollection](../../com.aspose.cells/commentcollection)
### getConditionalFormattings() {#getConditionalFormattings--}
```
public ConditionalFormattingCollection getConditionalFormattings()
```


Hämtar ConditionalFormattings i kalkylbladet.

**Returns:**
[ConditionalFormattingCollection](../../com.aspose.cells/conditionalformattingcollection)
### getCustomProperties() {#getCustomProperties--}
```
public CustomPropertyCollection getCustomProperties()
```


Hämtar ett objekt som representerar identifieringsinformationen som är associerad med ett kalkylblad.

**Remarks**

Worksheet.CustomProperties erbjuder en föredragen mekanism för att lagra godtyckliga data. Den stödjer äldre tredjepartsdokumentkomponenter samt situationer som har ett strikt behov av binära delar.

**Returns:**
[CustomPropertyCollection](../../com.aspose.cells/custompropertycollection)
### getDisplayRightToLeft() {#getDisplayRightToLeft--}
```
public boolean getDisplayRightToLeft()
```


Indikerar om det angivna kalkylbladet visas från höger till vänster istället för från vänster till höger. Standard är falskt.

**Returns:**
boolean
### getDisplayZeros() {#getDisplayZeros--}
```
public boolean getDisplayZeros()
```


Sant om nollvärden visas.

**Returns:**
boolean
### getErrorCheckOptions() {#getErrorCheckOptions--}
```
public ErrorCheckOptionCollection getErrorCheckOptions()
```


Hämtar felkontrollinställning som tillämpas på vissa områden.

**Returns:**
[ErrorCheckOptionCollection](../../com.aspose.cells/errorcheckoptioncollection)
### getFirstVisibleColumn() {#getFirstVisibleColumn--}
```
public int getFirstVisibleColumn()
```


Representerar första synliga kolumnindex.

**Returns:**
int
### getFirstVisibleRow() {#getFirstVisibleRow--}
```
public int getFirstVisibleRow()
```


Representerar första synliga radindex.

**Returns:**
int
### getFreezedPanes() {#getFreezedPanes--}
```
public int[] getFreezedPanes()
```


Hämtar frysade rutor.

**Returns:**
int[] - Returnerar null betyder att kalkylbladet inte är fryst 0:Radindex;1:kolumn;2:frysta rader;3:frysta rader
### getGridlineColor() {#getGridlineColor--}
```
public Color getGridlineColor()
```


Hämtar färgen på rutnätslinjen

**Returns:**
[Color](../../com.aspose.cells/color)
### getHorizontalPageBreaks() {#getHorizontalPageBreaks--}
```
public HorizontalPageBreakCollection getHorizontalPageBreaks()
```


Hämtar [HorizontalPageBreakCollection](../../com.aspose.cells/horizontalpagebreakcollection)-samlingen.

**Returns:**
[HorizontalPageBreakCollection](../../com.aspose.cells/horizontalpagebreakcollection)
### getHyperlinks() {#getHyperlinks--}
```
public HyperlinkCollection getHyperlinks()
```


Hämtar [HyperlinkCollection](../../com.aspose.cells/hyperlinkcollection)-samlingen.

**Returns:**
[HyperlinkCollection](../../com.aspose.cells/hyperlinkcollection)
### getIndex() {#getIndex--}
```
public int getIndex()
```


Hämtar indexet för bladet i kalkylblads‑samlingen.

**Returns:**
int
### getListObjects() {#getListObjects--}
```
public ListObjectCollection getListObjects()
```


Hämtar alla ListObjects i detta kalkylblad.

**Returns:**
[ListObjectCollection](../../com.aspose.cells/listobjectcollection)
### getName() {#getName--}
```
public String getName()
```


Hämtar namnet på kalkylbladet.

**Remarks**

Den maximala längden för bladnamn är 31. Du kan inte tilldela samma namn (skiftlägesokänsligt) till två kalkylblad. Till exempel kan du inte sätta "SheetName1" på det första kalkylbladet och sätta "SHEETNAME1" på det andra kalkylbladet.

**Returns:**
java.lang.String
### getOleObjects() {#getOleObjects--}
```
public OleObjectCollection getOleObjects()
```


Representerar en samling av [OleObject](../../com.aspose.cells/oleobject) i ett kalkylblad.

**Returns:**
[OleObjectCollection](../../com.aspose.cells/oleobjectcollection)
### getOutline() {#getOutline--}
```
public Outline getOutline()
```


Hämtar konturen i detta kalkylblad.

**Returns:**
[Outline](../../com.aspose.cells/outline)
### getPageSetup() {#getPageSetup--}
```
public PageSetup getPageSetup()
```


Representerar sidinställningsbeskrivningen i detta blad.

**Returns:**
[PageSetup](../../com.aspose.cells/pagesetup)
### getPaneState() {#getPaneState--}
```
public int getPaneState()
```


Anger om panelen har horisontella eller vertikala delningar, och om dessa delningar är frysta.

See [PaneStateType](../../com.aspose.cells/panestatetype).

**Returns:**
int
### getPanes() {#getPanes--}
```
public PaneCollection getPanes()
```


Hämtar fönsterpanelerna.

**Remarks**

Om fönstret inte är delat eller fryst.

**Returns:**
[PaneCollection](../../com.aspose.cells/panecollection)
### getPictures() {#getPictures--}
```
public PictureCollection getPictures()
```


Hämtar en [Picture](../../com.aspose.cells/picture)-samling.

**Returns:**
[PictureCollection](../../com.aspose.cells/picturecollection)
### getPivotTables() {#getPivotTables--}
```
public PivotTableCollection getPivotTables()
```


Hämtar alla pivottabeller i detta kalkylblad.

**Returns:**
[PivotTableCollection](../../com.aspose.cells/pivottablecollection)
### getPrintingPageBreaks(ImageOrPrintOptions options) {#getPrintingPageBreaks-com.aspose.cells.ImageOrPrintOptions-}
```
public CellArea[] getPrintingPageBreaks(ImageOrPrintOptions options)
```


Hämtar automatiska sidbrytningar.

**Remarks**

Varje cellområde representerar ett papper.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | Utskriftsalternativen |

**Returns:**
com.aspose.cells.CellArea[] - De automatiska sidbrytningsområdena.
### getProtection() {#getProtection--}
```
public Protection getProtection()
```


Representerar de olika typerna av skyddsalternativ som finns tillgängliga för ett kalkylblad. Stöder avancerade skyddsalternativ i ExcelXP och senare versioner.

**Remarks**

Denna egenskap kan skydda kalkylblad i alla versioner av Excel-filer och stödjer avancerade skyddsalternativ i ExcelXP och senare versioner.

**Returns:**
[Protection](../../com.aspose.cells/protection)
### getQueryTables() {#getQueryTables--}
```
public QueryTableCollection getQueryTables()
```


Hämtar [QueryTableCollection](../../com.aspose.cells/querytablecollection) i kalkylbladet.

**Returns:**
[QueryTableCollection](../../com.aspose.cells/querytablecollection)
### getScenarios() {#getScenarios--}
```
public ScenarioCollection getScenarios()
```


Hämtar samlingen av [Scenario](../../com.aspose.cells/scenario).

**Returns:**
[ScenarioCollection](../../com.aspose.cells/scenariocollection)
### getSelectedAreas() {#getSelectedAreas--}
```
public Range[] getSelectedAreas()
```


Hämtar markerade cellområden i designerns kalkylblad.

**Returns:**
com.aspose.cells.Range[] - Returnerar alla markerade områden.
### getSelectedRanges() {#getSelectedRanges--}
```
public ArrayList getSelectedRanges()
```


Hämtar markerade cellområden i designerns kalkylblad.

**Remarks**

OBS: Denna metod är nu föråldrad. Använd i stället Worksheet.GetSelectedAreas()‑metoden. Denna egenskap kommer att tas bort 12 månader senare från och med mars 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
java.util.ArrayList - En ArrayList som innehåller markerade områden.
### getShapes() {#getShapes--}
```
public ShapeCollection getShapes()
```


Returnerar alla ritningsformer i detta kalkylblad.

**Returns:**
[ShapeCollection](../../com.aspose.cells/shapecollection)
### getShowDataTypeIcons() {#getShowDataTypeIcons--}
```
public boolean getShowDataTypeIcons()
```


Anger om datatypikoner ska visas.

**Returns:**
boolean
### getShowFormulas() {#getShowFormulas--}
```
public boolean getShowFormulas()
```


Anger om formler eller deras resultat ska visas.

**Returns:**
boolean
### getSlicers() {#getSlicers--}
```
public SlicerCollection getSlicers()
```


Hämta Slicer-samlingen i kalkylbladet

**Returns:**
[SlicerCollection](../../com.aspose.cells/slicercollection)
### getSmartTagSetting() {#getSmartTagSetting--}
```
public SmartTagSetting getSmartTagSetting()
```


Hämtar alla [SmartTagCollection](../../com.aspose.cells/smarttagcollection)-objekt i kalkylbladet.

**Returns:**
[SmartTagSetting](../../com.aspose.cells/smarttagsetting)
### getSparklineGroups() {#getSparklineGroups--}
```
public SparklineGroupCollection getSparklineGroups()
```


Hämtar sparkline-grupperna i kalkylbladet.

**Returns:**
[SparklineGroupCollection](../../com.aspose.cells/sparklinegroupcollection)
### getTabColor() {#getTabColor--}
```
public Color getTabColor()
```


Representerar flikfärgen för kalkylbladet.

**Remarks**

Denna funktion stöds endast i ExcelXP (Excel2002) och senare versioner. Om du sparar filen som Excel97- eller Excel2000-format kommer den att utelämnas.

**Returns:**
[Color](../../com.aspose.cells/color)
### getTabId() {#getTabId--}
```
public int getTabId()
```


Anger det interna identifieraren för bladet.

**Returns:**
int
### getTextBoxes() {#getTextBoxes--}
```
public TextBoxCollection getTextBoxes()
```


Hämtar en [TextBox](../../com.aspose.cells/textbox)-samling.

**Returns:**
[TextBoxCollection](../../com.aspose.cells/textboxcollection)
### getTimelines() {#getTimelines--}
```
public TimelineCollection getTimelines()
```


Hämta Timeline-samlingen i kalkylbladet

**Returns:**
[TimelineCollection](../../com.aspose.cells/timelinecollection)
### getTransitionEntry() {#getTransitionEntry--}
```
public boolean getTransitionEntry()
```


Anger om alternativet Transition Formula Entry (Lotus-kompatibilitet) är aktiverat.

**Returns:**
boolean
### getTransitionEvaluation() {#getTransitionEvaluation--}
```
public boolean getTransitionEvaluation()
```


Anger om alternativet Transition Formula Evaluation (Lotus-kompatibilitet) är aktiverat.

**Returns:**
boolean
### getType() {#getType--}
```
public int getType()
```


Representerar kalkylbladstyp.

See [SheetType](../../com.aspose.cells/sheettype).

**Returns:**
int
### getUniqueId() {#getUniqueId--}
```
public String getUniqueId()
```


Hämtar det unika ID:t, det är samma som \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\}.

**Returns:**
java.lang.String
### getValidations() {#getValidations--}
```
public ValidationCollection getValidations()
```


Hämtar samlingen av datavalideringsinställningar i kalkylbladet.

**Returns:**
[ValidationCollection](../../com.aspose.cells/validationcollection)
### getVerticalPageBreaks() {#getVerticalPageBreaks--}
```
public VerticalPageBreakCollection getVerticalPageBreaks()
```


Hämtar [VerticalPageBreakCollection](../../com.aspose.cells/verticalpagebreakcollection)-samlingen.

**Returns:**
[VerticalPageBreakCollection](../../com.aspose.cells/verticalpagebreakcollection)
### getViewType() {#getViewType--}
```
public int getViewType()
```


Hämtar vytypen.

See [ViewType](../../com.aspose.cells/viewtype).

**Returns:**
int
### getVisibilityType() {#getVisibilityType--}
```
public int getVisibilityType()
```


Anger det synliga tillståndet för detta blad.

See [VisibilityType](../../com.aspose.cells/visibilitytype).

**Returns:**
int
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


Hämtar arbetsboksobjektet som innehåller detta blad.

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### getZoom() {#getZoom--}
```
public int getZoom()
```


Representerar skalningsfaktorn i procent. Den bör vara mellan 10 och 400.

**Remarks**

Ange vytypen först.

**Returns:**
int
### hasAutofilter() {#hasAutofilter--}
```
public boolean hasAutofilter()
```


Anger om detta kalkylblad har autofilter.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isGridlinesVisible() {#isGridlinesVisible--}
```
public boolean isGridlinesVisible()
```


Hämtar ett värde som anger om rutnätslinjerna är synliga. Standard är true.

**Returns:**
boolean
### isOutlineShown() {#isOutlineShown--}
```
public boolean isOutlineShown()
```


Anger om konturen ska visas.

**Returns:**
boolean
### isPageBreakPreview() {#isPageBreakPreview--}
```
public boolean isPageBreakPreview()
```


Anger om det angivna kalkylbladet visas i normal vy eller sidbrytning förhandsgranskning.

**Returns:**
boolean
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


Anger om kalkylbladet är skyddat.

**Returns:**
boolean
### isRowColumnHeadersVisible() {#isRowColumnHeadersVisible--}
```
public boolean isRowColumnHeadersVisible()
```


Hämtar ett värde som indikerar om kalkylbladet ska visa rad- och kolumnrubriker. Standard är true.

**Returns:**
boolean
### isRulerVisible() {#isRulerVisible--}
```
public boolean isRulerVisible()
```


Anger om linjalen är synlig. Denna egenskap tillämpas endast för förhandsgranskning av sidbrytningar.

**Returns:**
boolean
### isSelected() {#isSelected--}
```
public boolean isSelected()
```


Anger om detta kalkylblad är valt när arbetsboken öppnas.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Representerar om kalkylbladet är synligt.

**Returns:**
boolean
### moveTo(int index) {#moveTo-int-}
```
public void moveTo(int index)
```


Flyttar bladet till en annan plats i kalkylarket.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Destinationsbladets index. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### protect(int type) {#protect-int-}
```
public void protect(int type)
```


Skyddar kalkylbladet.

**Remarks**

Denna metod skyddar kalkylbladet utan lösenord. Den kan skydda kalkylbladet i alla versioner av Excel-filen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| type | int | [ProtectionType](../../com.aspose.cells/protectiontype). Skyddstyp. |

### protect(int type, String password, String oldPassword) {#protect-int-java.lang.String-java.lang.String-}
```
public void protect(int type, String password, String oldPassword)
```


Skyddar kalkylbladet.

**Remarks**

Denna metod kan skydda kalkylbladet i alla versioner av Excel-filen.

**Example**

```
         //Instantiating a Workbook object
         Workbook excel = new Workbook("template.xlsx");
         //Accessing the first worksheet in the Excel file
         Worksheet worksheet = excel.getWorksheets().get(0);
         //Protecting the worksheet with a password
         worksheet.protect(ProtectionType.ALL, "aspose", null);
         //Saving the modified Excel file in default (that is Excel 20003) format
         excel.save("output.xls");
         //Closing the file stream to free all resources
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| type | int | [ProtectionType](../../com.aspose.cells/protectiontype). Skyddstyp. |
| lösenord | java.lang.String | Lösenord. |
| oldPassword | java.lang.String | Om kalkylbladet redan är skyddat med ett lösenord, ange det gamla lösenordet. Annars kan du sätta ett null‑värde eller en tom sträng för den här parametern. |

### refreshPivotTables() {#refreshPivotTables--}
```
public void refreshPivotTables()
```


Uppdaterar alla pivottabeller i detta kalkylblad.

### refreshPivotTables(PivotTableRefreshOption option) {#refreshPivotTables-com.aspose.cells.PivotTableRefreshOption-}
```
public boolean refreshPivotTables(PivotTableRefreshOption option)
```


Uppdaterar alla pivottabeller i detta kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) | Alternativet för att uppdatera datakällan för pivottabellen. |

**Returns:**
boolean
### removeAllDrawingObjects() {#removeAllDrawingObjects--}
```
public void removeAllDrawingObjects()
```


Tar bort alla ritobjekt i detta kalkylblad.

### removeAutoFilter() {#removeAutoFilter--}
```
public void removeAutoFilter()
```


Tar bort autofiltret för kalkylbladet.

### removeSplit() {#removeSplit--}
```
public void removeSplit()
```


Tar bort delat fönster.

### replace(String oldString, String newString) {#replace-java.lang.String-java.lang.String-}
```
public int replace(String oldString, String newString)
```


Ersätter all celltext med en ny sträng.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| oldString | java.lang.String | Gammalt strängvärde. |
| newString | java.lang.String | Nytt strängvärde. |

**Returns:**
int
### selectRange(int startRow, int startColumn, int totalRows, int totalColumns, boolean removeOthers) {#selectRange-int-int-int-int-boolean-}
```
public void selectRange(int startRow, int startColumn, int totalRows, int totalColumns, boolean removeOthers)
```


Markerar ett område.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRad | int | Startrad. |
| startColumn | int | Startkolumn |
| totalRows | int | Antalet rader. |
| totalColumns | int | Antalet kolumner |
| removeOthers | boolean | True betyder att ta bort andra markerade områden och endast välja detta område. |

### setActiveCell(String value) {#setActiveCell-java.lang.String-}
```
public void setActiveCell(String value)
```


Ställer in den aktiva cellen i kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setBackgroundImage(byte[] value) {#setBackgroundImage-byte---}
```
public void setBackgroundImage(byte[] value)
```


Ställer in bakgrundsbild för kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | byte[] |  |

### setCodeName(String value) {#setCodeName-java.lang.String-}
```
public void setCodeName(String value)
```


Hämtar kalkylbladets kodnamn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setDisplayRightToLeft(boolean value) {#setDisplayRightToLeft-boolean-}
```
public void setDisplayRightToLeft(boolean value)
```


Indikerar om det angivna kalkylbladet visas från höger till vänster istället för från vänster till höger. Standard är falskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setDisplayZeros(boolean value) {#setDisplayZeros-boolean-}
```
public void setDisplayZeros(boolean value)
```


Sant om nollvärden visas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setFirstVisibleColumn(int value) {#setFirstVisibleColumn-int-}
```
public void setFirstVisibleColumn(int value)
```


Representerar första synliga kolumnindex.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setFirstVisibleRow(int value) {#setFirstVisibleRow-int-}
```
public void setFirstVisibleRow(int value)
```


Representerar första synliga radindex.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setGridlineColor(Color value) {#setGridlineColor-com.aspose.cells.Color-}
```
public void setGridlineColor(Color value)
```


Ställer in färgen på rutnätslinjen

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setGridlinesVisible(boolean value) {#setGridlinesVisible-boolean-}
```
public void setGridlinesVisible(boolean value)
```


Ställer in ett värde som anger om rutnätslinjerna är synliga. Standard är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Ställer in namnet på kalkylbladet.

**Remarks**

Den maximala längden för bladnamn är 31. Du kan inte tilldela samma namn (skiftlägesokänsligt) till två kalkylblad. Till exempel kan du inte sätta "SheetName1" på det första kalkylbladet och sätta "SHEETNAME1" på det andra kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setOutlineShown(boolean value) {#setOutlineShown-boolean-}
```
public void setOutlineShown(boolean value)
```


Anger om konturen ska visas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setPageBreakPreview(boolean value) {#setPageBreakPreview-boolean-}
```
public void setPageBreakPreview(boolean value)
```


Anger om det angivna kalkylbladet visas i normal vy eller sidbrytning förhandsgranskning.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setRowColumnHeadersVisible(boolean value) {#setRowColumnHeadersVisible-boolean-}
```
public void setRowColumnHeadersVisible(boolean value)
```


Ställer in ett värde som indikerar om kalkylbladet ska visa rad- och kolumnrubriker. Standard är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setRulerVisible(boolean value) {#setRulerVisible-boolean-}
```
public void setRulerVisible(boolean value)
```


Anger om linjalen är synlig. Denna egenskap tillämpas endast för förhandsgranskning av sidbrytningar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSelected(boolean value) {#setSelected-boolean-}
```
public void setSelected(boolean value)
```


Anger om detta kalkylblad är valt när arbetsboken öppnas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowDataTypeIcons(boolean value) {#setShowDataTypeIcons-boolean-}
```
public void setShowDataTypeIcons(boolean value)
```


Anger om datatypikoner ska visas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowFormulas(boolean value) {#setShowFormulas-boolean-}
```
public void setShowFormulas(boolean value)
```


Anger om formler eller deras resultat ska visas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setTabColor(Color value) {#setTabColor-com.aspose.cells.Color-}
```
public void setTabColor(Color value)
```


Representerar flikfärgen för kalkylbladet.

**Remarks**

Denna funktion stöds endast i ExcelXP (Excel2002) och senare versioner. Om du sparar filen som Excel97- eller Excel2000-format kommer den att utelämnas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setTabId(int value) {#setTabId-int-}
```
public void setTabId(int value)
```


Anger det interna identifieraren för bladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setTransitionEntry(boolean value) {#setTransitionEntry-boolean-}
```
public void setTransitionEntry(boolean value)
```


Anger om alternativet Transition Formula Entry (Lotus-kompatibilitet) är aktiverat.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setTransitionEvaluation(boolean value) {#setTransitionEvaluation-boolean-}
```
public void setTransitionEvaluation(boolean value)
```


Anger om alternativet Transition Formula Evaluation (Lotus-kompatibilitet) är aktiverat.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Representerar kalkylbladstyp.

See [SheetType](../../com.aspose.cells/sheettype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setUniqueId(String value) {#setUniqueId-java.lang.String-}
```
public void setUniqueId(String value)
```


Ställer in det unika ID:t, det är samma som \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\}.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setViewType(int value) {#setViewType-int-}
```
public void setViewType(int value)
```


Ställer in visningstypen.

See [ViewType](../../com.aspose.cells/viewtype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setVisibilityType(int value) {#setVisibilityType-int-}
```
public void setVisibilityType(int value)
```


Anger det synliga tillståndet för detta blad.

See [VisibilityType](../../com.aspose.cells/visibilitytype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Representerar om kalkylbladet är synligt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setVisible(boolean isVisible, boolean ignoreError) {#setVisible-boolean-boolean-}
```
public void setVisible(boolean isVisible, boolean ignoreError)
```


Ställer in de synliga alternativen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isVisible | boolean | Om kalkylbladet är synligt |
| ignoreError | boolean | Om felet ska ignoreras om detta alternativ inte är giltigt. |

### setZoom(int value) {#setZoom-int-}
```
public void setZoom(int value)
```


Representerar skalningsfaktorn i procent. Den bör vara mellan 10 och 400.

**Remarks**

Ange vytypen först.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### split() {#split--}
```
public void split()
```


Delar fönstret.

### startAccessCache(int opts) {#startAccessCache-int-}
```
public void startAccessCache(int opts)
```


Startar sessionen som använder cache för att komma åt data i detta kalkylblad.

**Remarks**

Efter att ha avslutat åtkomsten till data bör [closeAccessCache(int)](../../com.aspose.cells/worksheet\#closeAccessCache-int-) anropas med samma alternativ för att rensa alla cacheminnen och återställa normalt åtkomstläge.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| opts | int | [AccessCacheOptions](../../com.aspose.cells/accesscacheoptions). alternativ för dataåtkomst |

### toString() {#toString--}
```
public String toString()
```


Returnerar en sträng som representerar det aktuella kalkylbladsobjektet.

**Returns:**
java.lang.String -
### unFreezePanes() {#unFreezePanes--}
```
public void unFreezePanes()
```


Låser upp paneler i kalkylbladet.

### unprotect() {#unprotect--}
```
public void unprotect()
```


Avskyddar kalkylbladet.

**Remarks**

Denna metod tar bort skyddet från ett kalkylblad som är skyddat utan lösenord.

### unprotect(String password) {#unprotect-java.lang.String-}
```
public void unprotect(String password)
```


Avskyddar kalkylbladet.

**Remarks**

Om kalkylbladet är skyddat utan lösenord kan du sätta ett null‑värde eller en tom sträng till lösenordsparametern.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| lösenord | java.lang.String | Password |

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

### xmlMapQuery(String path, XmlMap xmlMap) {#xmlMapQuery-java.lang.String-com.aspose.cells.XmlMap-}
```
public ArrayList xmlMapQuery(String path, XmlMap xmlMap)
```


Fråga cellområden som mappades/länkades till den specifika sökvägen för xml‑kartan.

**Remarks**

OBS: Denna metod är nu föråldrad. Använd istället metoden Worksheet.GetAreasOfXmlMapQuery(). Denna egenskap kommer att tas bort 12 månader senare från och med augusti 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sökväg | java.lang.String | xml-elementets sökväg |
| xmlMap | [XmlMap](../../com.aspose.cells/xmlmap) | Ange en xml-karta om du vill fråga efter den specifika sökvägen inom en specifik karta. |

**Returns:**
java.util.ArrayList – [CellArea](../../com.aspose.cells/cellarea) lista som är mappad/länkad till den specifika sökvägen för xml‑kartan, en tom lista returneras om inget är mappat/länkat.
