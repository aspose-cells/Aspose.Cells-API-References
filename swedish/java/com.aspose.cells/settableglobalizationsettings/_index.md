---
title: "SettableGlobalizationSettings"
second_title: "Aspose.Cells för Java API-referens"
description: "Implementering av GlobalizationSettings som stödjer användaren att ange/ändra fördefinierade texter."
type: docs
url: /sv/java/com.aspose.cells/settableglobalizationsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.GlobalizationSettings](../../com.aspose.cells/globalizationsettings)
```
public class SettableGlobalizationSettings extends GlobalizationSettings
```

Implementering av GlobalizationSettings som stödjer användaren att ange/ändra fördefinierade texter.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [SettableGlobalizationSettings()](#SettableGlobalizationSettings--) |  |
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
| [getTotalName(int functionType)](#getTotalName-int-) | Hämtar totalnamnet för en specifik funktion. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBooleanValueString(boolean bv, String name)](#setBooleanValueString-boolean-java.lang.String-) | Ställer in visningssträngvärdet för cellens booleska värde |
| [setChartSettings(ChartGlobalizationSettings value)](#setChartSettings-com.aspose.cells.ChartGlobalizationSettings-) | Ställer in globaliseringsinställningarna för diagrammet. |
| [setColumnSeparatorOfFormulaArray(char c)](#setColumnSeparatorOfFormulaArray-char-) | Ställer in separatorn för objekten i arrayens raddata i formeln. |
| [setCommentTitleName(int type, String name)](#setCommentTitleName-int-java.lang.String-) | Hämtar den lokalanpassade kommentarsrubrikens namn enligt kommentarsrubriktyp. |
| [setGrandTotalName(int functionType, String name)](#setGrandTotalName-int-java.lang.String-) | Ställer in namnet på totalsumman för en specifik funktion. |
| [setListSeparator(char c)](#setListSeparator-char-) | Ställer in separatorn för listan, funktionsparametrar, ...etc. |
| [setLocalBuiltInName(String standardName, String localName, boolean bidirectional)](#setLocalBuiltInName-java.lang.String-java.lang.String-boolean-) | Ställer in den lokalanpassade texten för det inbyggda namnet med given standardnamnstext. |
| [setLocalFunctionName(String standardName, String localName, boolean bidirectional)](#setLocalFunctionName-java.lang.String-java.lang.String-boolean-) | Ställer in det lokalanpassade funktionsnamnet som motsvarar det givna standardfunktionsnamnet. |
| [setPivotSettings(PivotGlobalizationSettings value)](#setPivotSettings-com.aspose.cells.PivotGlobalizationSettings-) | Ställer in globaliseringsinställningarna för pivottabellen. |
| [setRowSeparatorOfFormulaArray(char c)](#setRowSeparatorOfFormulaArray-char-) | Ställer in separatorn för rader i arraydata i formeln. |
| [setStandardBuiltInName(String localName, String standardName, boolean bidirectional)](#setStandardBuiltInName-java.lang.String-java.lang.String-boolean-) | Ställer in det lokalanpassade funktionsnamnet enligt det givna standardfunktionsnamnet. |
| [setStandardFunctionName(String localName, String standardName, boolean bidirectional)](#setStandardFunctionName-java.lang.String-java.lang.String-boolean-) | Ställer in det lokalanpassade funktionsnamnet enligt det givna standardfunktionsnamnet. |
| [setStandardHeaderFooterFontStyleName(String localfontStyleName, String standardName)](#setStandardHeaderFooterFontStyleName-java.lang.String-java.lang.String-) | Ställer in det lokalanpassade funktionsnamnet enligt det givna standardfunktionsnamnet. |
| [setTableRowTypeOfAll(String name)](#setTableRowTypeOfAll-java.lang.String-) | Ställer in typnamnet för tabellrader som består av alla rader i den refererade tabellen. |
| [setTableRowTypeOfCurrent(String name)](#setTableRowTypeOfCurrent-java.lang.String-) | Ställer in typnamnet för tabellrader som består av den aktuella raden i den refererade tabellen. |
| [setTableRowTypeOfData(String name)](#setTableRowTypeOfData-java.lang.String-) | Ställer in typnamnet för tabellrader som består av datatområdet i den refererade tabellen. |
| [setTableRowTypeOfHeaders(String name)](#setTableRowTypeOfHeaders-java.lang.String-) | Ställer in typnamnet för tabellrader som består av tabellrubriken. |
| [setTableRowTypeOfTotals(String name)](#setTableRowTypeOfTotals-java.lang.String-) | Ställer in typnamnet för tabellrader som består av totalsraden i den refererade tabellen. |
| [setTotalName(int functionType, String name)](#setTotalName-int-java.lang.String-) | Ställer in totalsnamnet för en specifik funktion. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SettableGlobalizationSettings() {#SettableGlobalizationSettings--}
```
public SettableGlobalizationSettings()
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
| type | int | [CommentTitleType](../../com.aspose.cells/commenttitletype). typ av kommentarstitel |

**Returns:**
java.lang.String - lokalanpassat namn för kommentarstitel
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


Hämtar typnamnet för tabellrader som består av alla rader i den refererade tabellen.

**Returns:**
java.lang.String - typnamnet för tabellrader
### getTableRowTypeOfCurrent() {#getTableRowTypeOfCurrent--}
```
public String getTableRowTypeOfCurrent()
```


Hämtar typnamnet för tabellrader som består av den aktuella raden i den refererade tabellen.

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


Hämtar typnamnet för tabellrader som består av totalraden i den refererade tabellen.

**Returns:**
java.lang.String - typnamnet för tabellrader
### getTotalName(int functionType) {#getTotalName-int-}
```
public String getTotalName(int functionType)
```


Hämtar totalnamnet för en specifik funktion.

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




### setBooleanValueString(boolean bv, String name) {#setBooleanValueString-boolean-java.lang.String-}
```
public void setBooleanValueString(boolean bv, String name)
```


Ställer in visningssträngvärdet för cellens booleska värde

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| bv | boolean | booleskt värde |
| name | java.lang.String | strängvärde för det booleska värdet |

### setChartSettings(ChartGlobalizationSettings value) {#setChartSettings-com.aspose.cells.ChartGlobalizationSettings-}
```
public void setChartSettings(ChartGlobalizationSettings value)
```


Ställer in globaliseringsinställningarna för diagrammet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [ChartGlobalizationSettings](../../com.aspose.cells/chartglobalizationsettings) |  |

### setColumnSeparatorOfFormulaArray(char c) {#setColumnSeparatorOfFormulaArray-char-}
```
public void setColumnSeparatorOfFormulaArray(char c)
```


Ställer in separatorn för objekten i arrayens raddata i formeln.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| c | char | den angivna avgränsaren |

### setCommentTitleName(int type, String name) {#setCommentTitleName-int-java.lang.String-}
```
public void setCommentTitleName(int type, String name)
```


Hämtar den lokalanpassade kommentarsrubrikens namn enligt kommentarsrubriktyp.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| type | int | [CommentTitleType](../../com.aspose.cells/commenttitletype). typ av kommentarstitel |
| name | java.lang.String | språköberoende namn för kommentarstitel |

### setGrandTotalName(int functionType, String name) {#setGrandTotalName-int-java.lang.String-}
```
public void setGrandTotalName(int functionType, String name)
```


Ställer in namnet på totalsumman för en specifik funktion.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| functionType | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). Funktions typen. |
| name | java.lang.String | Det totala namnet på funktionen. |

### setListSeparator(char c) {#setListSeparator-char-}
```
public void setListSeparator(char c)
```


Ställer in separatorn för listan, funktionsparametrar, ...etc.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| c | char | den angivna avgränsaren |

### setLocalBuiltInName(String standardName, String localName, boolean bidirectional) {#setLocalBuiltInName-java.lang.String-java.lang.String-boolean-}
```
public void setLocalBuiltInName(String standardName, String localName, boolean bidirectional)
```


Ställer in den lokalanpassade texten för det inbyggda namnet med given standardnamnstext.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| standardName | java.lang.String | Standard (en-US‑lokal) namntext för inbyggt namn. |
| localName | java.lang.String | Lokalberoende namntext |
| bidirectional | boolean | Om den lokala namntexten ska mappas till standardnamntext automatiskt. Om sant kommer den lokala namntexten att mappas till standardnamntext automatiskt så att användaren inte behöver anropa [setStandardBuiltInName(String,String,boolean)](../../com.aspose.cells/settableglobalizationsettings\#setStandardBuiltInName-String-String-boolean-) igen för samma standard‑ och lokala namnpar. |

### setLocalFunctionName(String standardName, String localName, boolean bidirectional) {#setLocalFunctionName-java.lang.String-java.lang.String-boolean-}
```
public void setLocalFunctionName(String standardName, String localName, boolean bidirectional)
```


Ställer in det lokalanpassade funktionsnamnet som motsvarar det givna standardfunktionsnamnet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| standardName | java.lang.String | Standard(en-US locale) funktionsnamn. |
| localName | java.lang.String | Lokalberoende funktionsnamn |
| bidirectional | boolean | Om det lokala funktionsnamnet ska mappas till standardfunktionsnamn automatiskt. Om sant kommer det lokala namnet att mappas till standardnamnet automatiskt så att användaren inte behöver anropa [setStandardFunctionName(String,String,boolean)](../../com.aspose.cells/settableglobalizationsettings\#setStandardFunctionName-String-String-boolean-) igen för samma standard‑ och lokala namnpar. |

### setPivotSettings(PivotGlobalizationSettings value) {#setPivotSettings-com.aspose.cells.PivotGlobalizationSettings-}
```
public void setPivotSettings(PivotGlobalizationSettings value)
```


Ställer in globaliseringsinställningarna för pivottabellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings) |  |

### setRowSeparatorOfFormulaArray(char c) {#setRowSeparatorOfFormulaArray-char-}
```
public void setRowSeparatorOfFormulaArray(char c)
```


Ställer in separatorn för rader i arraydata i formeln.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| c | char | den angivna avgränsaren |

### setStandardBuiltInName(String localName, String standardName, boolean bidirectional) {#setStandardBuiltInName-java.lang.String-java.lang.String-boolean-}
```
public void setStandardBuiltInName(String localName, String standardName, boolean bidirectional)
```


Ställer in det lokalanpassade funktionsnamnet enligt det givna standardfunktionsnamnet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| localName | java.lang.String | Lokalberoende funktionsnamn |
| standardName | java.lang.String | Standard(en-US locale) funktionsnamn. |
| bidirectional | boolean | Om standardnamntexten ska mappas till lokal namntext automatiskt. Om sant kommer standardnamntexten att mappas till lokal namntext automatiskt så att användaren inte behöver anropa [setLocalBuiltInName(String,String,boolean)](../../com.aspose.cells/settableglobalizationsettings\#setLocalBuiltInName-String-String-boolean-) igen för samma standard‑ och lokala namnpar. |

### setStandardFunctionName(String localName, String standardName, boolean bidirectional) {#setStandardFunctionName-java.lang.String-java.lang.String-boolean-}
```
public void setStandardFunctionName(String localName, String standardName, boolean bidirectional)
```


Ställer in det lokalanpassade funktionsnamnet enligt det givna standardfunktionsnamnet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| localName | java.lang.String | Lokalberoende funktionsnamn |
| standardName | java.lang.String | Standard(en-US locale) funktionsnamn. |
| bidirectional | boolean | Om standardfunktionsnamnet ska mappas till lokalt funktionsnamn automatiskt. Om sant kommer standardnamnet att mappas till lokalt namn automatiskt så att användaren inte behöver anropa [setLocalFunctionName(String,String,boolean)](../../com.aspose.cells/settableglobalizationsettings\#setLocalFunctionName-String-String-boolean-) igen för samma standard‑ och lokala namnpar. |

### setStandardHeaderFooterFontStyleName(String localfontStyleName, String standardName) {#setStandardHeaderFooterFontStyleName-java.lang.String-java.lang.String-}
```
public void setStandardHeaderFooterFontStyleName(String localfontStyleName, String standardName)
```


Ställer in det lokalanpassade funktionsnamnet enligt det givna standardfunktionsnamnet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| localfontStyleName | java.lang.String | Språköberoende teckensnittsstilsnamn för Header/Footer. |
| standardName | java.lang.String | Standard(en-US locale) funktionsnamn. |

### setTableRowTypeOfAll(String name) {#setTableRowTypeOfAll-java.lang.String-}
```
public void setTableRowTypeOfAll(String name)
```


Ställer in typnamnet för tabellrader som består av alla rader i den refererade tabellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | typnamnet för tabellrader |

### setTableRowTypeOfCurrent(String name) {#setTableRowTypeOfCurrent-java.lang.String-}
```
public void setTableRowTypeOfCurrent(String name)
```


Ställer in typnamnet för tabellrader som består av den aktuella raden i den refererade tabellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | typnamnet för tabellrader |

### setTableRowTypeOfData(String name) {#setTableRowTypeOfData-java.lang.String-}
```
public void setTableRowTypeOfData(String name)
```


Ställer in typnamnet för tabellrader som består av datatområdet i den refererade tabellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | typnamnet för tabellrader |

### setTableRowTypeOfHeaders(String name) {#setTableRowTypeOfHeaders-java.lang.String-}
```
public void setTableRowTypeOfHeaders(String name)
```


Ställer in typnamnet för tabellrader som består av tabellrubriken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | typnamnet för tabellrader |

### setTableRowTypeOfTotals(String name) {#setTableRowTypeOfTotals-java.lang.String-}
```
public void setTableRowTypeOfTotals(String name)
```


Ställer in typnamnet för tabellrader som består av totalsraden i den refererade tabellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | typnamnet för tabellrader |

### setTotalName(int functionType, String name) {#setTotalName-int-java.lang.String-}
```
public void setTotalName(int functionType, String name)
```


Ställer in totalsnamnet för en specifik funktion.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| functionType | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). Funktions typen. |
| name | java.lang.String | Det totala namnet för funktionen. |

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

