---
title: "GlobalizationSettings"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar globaliseringsinställningarna."
type: docs
url: /sv/java/com.aspose.cells/globalizationsettings/
---

**Inheritance:**
java.lang.Object
```
public class GlobalizationSettings
```

Representerar globaliseringsinställningarna.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [GlobalizationSettings()](#GlobalizationSettings--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [compare(String v1, String v2, boolean ignoreCase)](#compare-java.lang.String-java.lang.String-boolean-) | Jämför två strängvärden enligt vissa sorteringsregler. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllName()](#getAllName--) | Hämtar namnet på "(All)"-etiketten i pivottabellen. |
| [getBooleanValueString(boolean bv)](#getBooleanValueString-boolean-) | Hämtar displaysträngvärdet för cellens booleska värde. |
| [getChartSettings()](#getChartSettings--) | Hämtar globaliseringsinställningarna för diagram. |
| [getClass()](#getClass--) |  |
| [getCollationKey(String v, boolean ignoreCase)](#getCollationKey-java.lang.String-boolean-) | Omvandlar strängen till ett jämförbart objekt enligt vissa sorteringsregler. |
| [getColumnLabelsOfPivotTable()](#getColumnLabelsOfPivotTable--) | Hämtar namnet på "Column Labels"-etiketten i pivottabellen. |
| [getColumnSeparatorOfFormulaArray()](#getColumnSeparatorOfFormulaArray--) | Hämtar separatorn för objekten i matrisens raddata i formeln. |
| [getCommentTitleName(int type)](#getCommentTitleName-int-) | Hämtar den lokalanpassade kommentarsrubrikens namn enligt kommentarsrubriktyp. |
| [getDataFieldHeaderNameOfPivotTable()](#getDataFieldHeaderNameOfPivotTable--) | Hämtar namnet på rubriken för värdeområdesfältet i pivottabellen. |
| [getDefaultSheetName()](#getDefaultSheetName--) | Hämtar standardbladnamnet för att automatiskt lägga till ett arbetsblad. |
| [getEmptyDataName()](#getEmptyDataName--) | Hämtar namnet på "(blank)"-etiketten i pivottabellen. |
| [getErrorValueString(String err)](#getErrorValueString-java.lang.String-) | Hämtar visningssträngvärdet för cellens felvärde |
| [getGrandTotalName(int functionType)](#getGrandTotalName-int-) | Hämtar namnet på totalen för funktionen. |
| [getListSeparator()](#getListSeparator--) | Hämtar separatorn för listor, funktionsparametrar, ...etc. |
| [getLocalBuiltInName(String standardName)](#getLocalBuiltInName-java.lang.String-) | Hämtar den localespecifika texten för inbyggt namn enligt given standardtext. |
| [getLocalFunctionName(String standardName)](#getLocalFunctionName-java.lang.String-) | Hämtar det localespecifika funktionsnamnet enligt givet standardfunktionsnamn. |
| [getMultipleItemsName()](#getMultipleItemsName--) | Hämtar namnet på "(Multiple Items)"-etiketten i pivottabellen. |
| [getPivotGrandTotalName()](#getPivotGrandTotalName--) | Hämtar namnet på "Grand Total"-etiketten i pivottabellen. |
| [getPivotSettings()](#getPivotSettings--) | Hämtar globaliseringsinställningarna för pivottabellen. |
| [getPivotTotalName()](#getPivotTotalName--) | Hämtar namnet på "Total"-etiketten i pivottabellen. |
| [getProtectionNameOfPivotTable()](#getProtectionNameOfPivotTable--) | Hämtar skyddsnamnet i pivottabellen. |
| [getRowLabelsNameOfPivotTable()](#getRowLabelsNameOfPivotTable--) | Hämtar namnet på "Row Labels"-etiketten i pivottabellen. |
| [getRowSeparatorOfFormulaArray()](#getRowSeparatorOfFormulaArray--) | Hämtar separatorn för rader i array‑data i formeln. |
| [getStandardBuiltInName(String localName)](#getStandardBuiltInName-java.lang.String-) | Hämtar standardtexten för inbyggt namn enligt given localespecifik text. |
| [getStandardFunctionName(String localName)](#getStandardFunctionName-java.lang.String-) | Hämtar standardfunktionsnamnet enligt givet localespecifikt funktionsnamn. |
| [getStandardHeaderFooterFontStyleName(String localfontStyleName)](#getStandardHeaderFooterFontStyleName-java.lang.String-) | Hämtar standardengelska teckensnittsstilsnamnet (Regular, Bold, Italic) för Header/Footer enligt givet localespecifikt teckensnittsstilsnamn. |
| [getSubTotalName(int subTotalType)](#getSubTotalName-int-) | Hämtar namnet på [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype)-typen i pivottabellen. |
| [getTableRowTypeOfAll()](#getTableRowTypeOfAll--) | Hämtar typnamnet för tabellrader som består av alla rader i den refererade tabellen. |
| [getTableRowTypeOfCurrent()](#getTableRowTypeOfCurrent--) | Hämtar typnamnet för tabellrader som består av den aktuella raden i den refererade tabellen. |
| [getTableRowTypeOfData()](#getTableRowTypeOfData--) | Hämtar typnamnet för tabellrader som består av dataområdet i den refererade tabellen. |
| [getTableRowTypeOfHeaders()](#getTableRowTypeOfHeaders--) | Hämtar typnamnet för tabellrader som består av tabellhuvudet. |
| [getTableRowTypeOfTotals()](#getTableRowTypeOfTotals--) | Hämtar typnamnet för tabellrader som består av totalraden i den refererade tabellen. |
| [getTotalName(int functionType)](#getTotalName-int-) | Hämtar det totala namnet på funktionen. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setChartSettings(ChartGlobalizationSettings value)](#setChartSettings-com.aspose.cells.ChartGlobalizationSettings-) | Ställer in globaliseringsinställningarna för diagrammet. |
| [setPivotSettings(PivotGlobalizationSettings value)](#setPivotSettings-com.aspose.cells.PivotGlobalizationSettings-) | Ställer in globaliseringsinställningarna för pivottabellen. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GlobalizationSettings() {#GlobalizationSettings--}
```
public GlobalizationSettings()
```


### compare(String v1, String v2, boolean ignoreCase) {#compare-java.lang.String-java.lang.String-boolean-}
```
public int compare(String v1, String v2, boolean ignoreCase)
```


Jämför två strängvärden enligt vissa sorteringsregler.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| v1 | java.lang.String | den första strängen |
| v2 | java.lang.String | den andra strängen |
| ignoreCase | boolean | om skiftlägeskänslighet ska ignoreras vid jämförelse av värden |

**Returns:**
int - Heltal som indikerar det lexikala förhållandet mellan de två jämförelseoperanderna
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
### getAllName() {#getAllName--}
```
public String getAllName()
```


Hämtar namnet på "(All)"-etiketten i pivottabellen.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället metoden GlobalizationSettings.GetColumnLabelsOfPivotTable(). Denna egenskap kommer att tas bort 12 månader senare från och med december 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
java.lang.String - Namnet på "(All)"-etiketten
### getBooleanValueString(boolean bv) {#getBooleanValueString-boolean-}
```
public String getBooleanValueString(boolean bv)
```


Hämtar displaysträngvärdet för cellens booleska värde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| bv | boolean | booleskt värde |

**Returns:**
java.lang.String - Returnerar som standard "TRUE" för sant värde och "FALSE" för falskt värde.
### getChartSettings() {#getChartSettings--}
```
public ChartGlobalizationSettings getChartSettings()
```


Hämtar globaliseringsinställningarna för diagram.

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


Omvandlar strängen till ett jämförbart objekt enligt vissa sorteringsregler.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| v | java.lang.String | Strängvärdet måste jämföras med andra. |
| ignoreCase | boolean | om skiftlägeskänslighet ska ignoreras vid jämförelse av värden |

**Returns:**
java.lang.Comparable - Objekt kan användas för att jämföra eller sortera strängvärden
### getColumnLabelsOfPivotTable() {#getColumnLabelsOfPivotTable--}
```
public String getColumnLabelsOfPivotTable()
```


Hämtar namnet på "Column Labels"-etiketten i pivottabellen.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället metoden PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Denna egenskap kommer att tas bort 12 månader senare från och med december 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
java.lang.String - Namnet på kolumnetiketter
### getColumnSeparatorOfFormulaArray() {#getColumnSeparatorOfFormulaArray--}
```
public char getColumnSeparatorOfFormulaArray()
```


Hämtar separatorn för objekten i matrisens raddata i formeln.

**Returns:**
char
### getCommentTitleName(int type) {#getCommentTitleName-int-}
```
public String getCommentTitleName(int type)
```


Hämtar den lokalanpassade kommentarsrubrikens namn enligt kommentarsrubriktyp.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| type | int | [CommentTitleType](../../com.aspose.cells/commenttitletype). |

**Returns:**
java.lang.String -
### getDataFieldHeaderNameOfPivotTable() {#getDataFieldHeaderNameOfPivotTable--}
```
public String getDataFieldHeaderNameOfPivotTable()
```


Hämtar namnet på rubriken för värdeområdesfältet i pivottabellen.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället metoden PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Denna egenskap kommer att tas bort 12 månader senare från och med december 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
java.lang.String - Namnet på datafältets rubriknamn
### getDefaultSheetName() {#getDefaultSheetName--}
```
public String getDefaultSheetName()
```


Hämtar standardbladnamnet för att automatiskt lägga till ett arbetsblad. Standard är "Sheet".

**Remarks**

Det automatiskt tillagda (t.ex. via [WorksheetCollection.add()](../../com.aspose.cells/worksheetcollection\#add--)) bladets namn blir det angivna namnet plus sekvensnummer. Till exempel kan en tysk användare vilja att bladnamnet blir "Tabellenblatt2" istället för "Sheet2". Då kan användaren implementera den här metoden för att returnera "Tabellenblatt".

**Returns:**
java.lang.String - standardbladnamnet för att automatiskt lägga till ett arbetsblad
### getEmptyDataName() {#getEmptyDataName--}
```
public String getEmptyDataName()
```


Hämtar namnet på "(blank)"-etiketten i pivottabellen.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället metoden PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Denna egenskap kommer att tas bort 12 månader senare från och med december 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
java.lang.String - Namnet på tom data
### getErrorValueString(String err) {#getErrorValueString-java.lang.String-}
```
public String getErrorValueString(String err)
```


Hämtar visningssträngvärdet för cellens felvärde

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| err | java.lang.String | felvärden såsom \#VALUE!,\#NAME? |

**Returns:**
java.lang.String - Returnerar som standard själva felvärdet
### getGrandTotalName(int functionType) {#getGrandTotalName-int-}
```
public String getGrandTotalName(int functionType)
```


Hämtar namnet på totalen för funktionen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| functionType | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). Funktions typen. |

**Returns:**
java.lang.String - Det totala namnet för funktionen.
### getListSeparator() {#getListSeparator--}
```
public char getListSeparator()
```


Hämtar separatorn för listor, funktionsparametrar, ...etc.

**Returns:**
char
### getLocalBuiltInName(String standardName) {#getLocalBuiltInName-java.lang.String-}
```
public String getLocalBuiltInName(String standardName)
```


Hämtar den localespecifika texten för inbyggt namn enligt given standardtext.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| standardName | java.lang.String | Standard(en-US locale) text för inbyggt namn. |

**Returns:**
java.lang.String - Lokalanpassad text. Språkinställningen angavs av arbetsboken för vilken dessa inställningar används.
### getLocalFunctionName(String standardName) {#getLocalFunctionName-java.lang.String-}
```
public String getLocalFunctionName(String standardName)
```


Hämtar det localespecifika funktionsnamnet enligt givet standardfunktionsnamn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| standardName | java.lang.String | Standard(en-US locale) funktionsnamn. |

**Returns:**
java.lang.String - Lokalanpassat funktionsnamn. Språkinställningen angavs av arbetsboken för vilken dessa inställningar används.
### getMultipleItemsName() {#getMultipleItemsName--}
```
public String getMultipleItemsName()
```


Hämtar namnet på "(Multiple Items)"-etiketten i pivottabellen.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället metoden PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Denna egenskap kommer att tas bort 12 månader senare från och med december 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
java.lang.String - Namnet på etiketten "(Multiple Items)"
### getPivotGrandTotalName() {#getPivotGrandTotalName--}
```
public String getPivotGrandTotalName()
```


Hämtar namnet på "Grand Total"-etiketten i pivottabellen.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället metoden PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Denna egenskap kommer att tas bort 12 månader senare från och med december 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
java.lang.String - Namnet på etiketten "Grand Total"
### getPivotSettings() {#getPivotSettings--}
```
public PivotGlobalizationSettings getPivotSettings()
```


Hämtar globaliseringsinställningarna för pivottabellen.

**Returns:**
[PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings)
### getPivotTotalName() {#getPivotTotalName--}
```
public String getPivotTotalName()
```


Hämtar namnet på "Total"-etiketten i pivottabellen. Du måste åsidosätta den här metoden när pivottabellen innehåller två eller fler PivotFields i dataområdet.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället metoden PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Denna egenskap kommer att tas bort 12 månader senare från och med december 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
java.lang.String - Namnet på etiketten "Total"
### getProtectionNameOfPivotTable() {#getProtectionNameOfPivotTable--}
```
public String getProtectionNameOfPivotTable()
```


Hämtar skyddsnamnet i pivottabellen.

**Remarks**

OBS: Den här medlemmen är nu föråldrad. Använd istället metoden PivotGlobalizationSettings.GetTextOfProtectedName(string). Den här egenskapen kommer att tas bort 12 månader senare från och med december 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
java.lang.String - Skyddsnamnet för PivotTable
### getRowLabelsNameOfPivotTable() {#getRowLabelsNameOfPivotTable--}
```
public String getRowLabelsNameOfPivotTable()
```


Hämtar namnet på "Row Labels"-etiketten i pivottabellen.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället metoden PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Denna egenskap kommer att tas bort 12 månader senare från och med december 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
java.lang.String - Namnet på radetiketter
### getRowSeparatorOfFormulaArray() {#getRowSeparatorOfFormulaArray--}
```
public char getRowSeparatorOfFormulaArray()
```


Hämtar separatorn för rader i array‑data i formeln.

**Returns:**
char
### getStandardBuiltInName(String localName) {#getStandardBuiltInName-java.lang.String-}
```
public String getStandardBuiltInName(String localName)
```


Hämtar standardtexten för inbyggt namn enligt given localespecifik text.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| localName | java.lang.String | Språköberoende text för inbyggt namn. Språket specificerades av Workbook för vilken dessa inställningar används. |

**Returns:**
java.lang.String - Standardtext (en-US locale).
### getStandardFunctionName(String localName) {#getStandardFunctionName-java.lang.String-}
```
public String getStandardFunctionName(String localName)
```


Hämtar standardfunktionsnamnet enligt givet localespecifikt funktionsnamn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| localName | java.lang.String | Språköberoende funktionsnamn. Språket specificerades av Workbook för vilken dessa inställningar används. |

**Returns:**
java.lang.String - Standardfunktionsnamn (en-US locale).
### getStandardHeaderFooterFontStyleName(String localfontStyleName) {#getStandardHeaderFooterFontStyleName-java.lang.String-}
```
public String getStandardHeaderFooterFontStyleName(String localfontStyleName)
```


Hämtar standardengelska teckensnittsstilsnamnet (Regular, Bold, Italic) för Header/Footer enligt givet localespecifikt teckensnittsstilsnamn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| localfontStyleName | java.lang.String | Språköberoende teckensnittsstilsnamn för Header/Footer. |

**Returns:**
java.lang.String - Standard engelskt teckensnittsstilsnamn (Regular, Bold, Italic)
### getSubTotalName(int subTotalType) {#getSubTotalName-int-}
```
public String getSubTotalName(int subTotalType)
```


Hämtar namnet på [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype)-typen i pivottabellen.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället metoden PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Denna egenskap kommer att tas bort 12 månader senare från och med december 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| subTotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). Typen [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) |

**Returns:**
java.lang.String - Namnet på typen [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype)
### getTableRowTypeOfAll() {#getTableRowTypeOfAll--}
```
public String getTableRowTypeOfAll()
```


Hämtar typnamnet för tabellrader som består av alla rader i den refererade tabellen. Standard är "All", så i formeln "\\#All" representerar alla rader i den refererade tabellen.

**Returns:**
java.lang.String - typnamnet för tabellrader
### getTableRowTypeOfCurrent() {#getTableRowTypeOfCurrent--}
```
public String getTableRowTypeOfCurrent()
```


Hämtar typnamnet för tabellrader som består av den aktuella raden i den refererade tabellen. Standard är "This Row", så i formeln "\\#This Row" representerar den aktuella raden i den refererade tabellen.

**Returns:**
java.lang.String - typnamnet för tabellrader
### getTableRowTypeOfData() {#getTableRowTypeOfData--}
```
public String getTableRowTypeOfData()
```


Hämtar typnamnet för tabellrader som består av datasegmentet i den refererade tabellen. Standard är "Data", så i formeln "\#Data" representerar datasegmentet i tabellen.

**Returns:**
java.lang.String - typnamnet för tabellrader
### getTableRowTypeOfHeaders() {#getTableRowTypeOfHeaders--}
```
public String getTableRowTypeOfHeaders()
```


Hämtar typnamnet för tabellrader som består av tabellrubriken. Standard är "Headers", så i formeln "\#Headers" representerar tabellrubriken.

**Returns:**
java.lang.String - typnamnet för tabellrader
### getTableRowTypeOfTotals() {#getTableRowTypeOfTotals--}
```
public String getTableRowTypeOfTotals()
```


Hämtar typnamnet för tabellrader som består av totalraden i den refererade tabellen. Standard är "Totals", så i formeln "\\#Totals" representerar totalraden i den refererade tabellen.

**Returns:**
java.lang.String - typnamnet för tabellrader
### getTotalName(int functionType) {#getTotalName-int-}
```
public String getTotalName(int functionType)
```


Hämtar det totala namnet på funktionen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| functionType | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). Funktions typen. |

**Returns:**
java.lang.String - Det totala namnet på funktionen.
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




### setChartSettings(ChartGlobalizationSettings value) {#setChartSettings-com.aspose.cells.ChartGlobalizationSettings-}
```
public void setChartSettings(ChartGlobalizationSettings value)
```


Ställer in globaliseringsinställningarna för diagrammet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [ChartGlobalizationSettings](../../com.aspose.cells/chartglobalizationsettings) |  |

### setPivotSettings(PivotGlobalizationSettings value) {#setPivotSettings-com.aspose.cells.PivotGlobalizationSettings-}
```
public void setPivotSettings(PivotGlobalizationSettings value)
```


Ställer in globaliseringsinställningarna för pivottabellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings) |  |

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

