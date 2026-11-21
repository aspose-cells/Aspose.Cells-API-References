---
title: "PivotTable"
second_title: "Aspose.Cells för Java API-referens"
description: "Sammanfattande beskrivning för PivotTable."
type: docs
url: /sv/java/com.aspose.cells/pivottable/
---

**Inheritance:**
java.lang.Object
```
public class PivotTable
```

Sammanfattande beskrivning för PivotTable.

**Example**

```
         Workbook book = new Workbook();
         Worksheet sheet = book.getWorksheets().get(0);
         Cells cells = sheet.getCells();
         cells.get(0, 0).setValue("fruit");
         cells.get(1, 0).setValue("grape");
         cells.get(2, 0).setValue("blueberry");
         cells.get(3, 0).setValue("kiwi");
         cells.get(4, 0).setValue("cherry");
         cells.get(5, 0).setValue("grape");
         cells.get(6, 0).setValue("blueberry");
         cells.get(7, 0).setValue("kiwi");
         cells.get(8, 0).setValue("cherry");
 
         cells.get(0, 1).setValue("year");
         cells.get(1, 1).setValue(2020);
         cells.get(2, 1).setValue(2020);
         cells.get(3, 1).setValue(2020);
         cells.get(4, 1).setValue(2020);
         cells.get(5, 1).setValue(2021);
         cells.get(6, 1).setValue(2021);
         cells.get(7, 1).setValue(2021);
         cells.get(8, 1).setValue(2021);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
         cells.get(5, 2).setValue(90);
         cells.get(6, 2).setValue(100);
         cells.get(7, 2).setValue(110);
         cells.get(8, 2).setValue(120);
 
         PivotTableCollection pivots = sheet.getPivotTables();
 
         PivotTable pivot = pivots.add("=Sheet1!A1:C9", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         //Change PivotField's attributes
         PivotField rowField = pivot.getRowFields().get(0);
         rowField.setDisplayName("custom display name");
 
         //Add PivotFilter
         PivotFilter filter = pivot.getRowFields().get(0).filterTop10(0, PivotFilterType.PERCENT, false, 2);
 
 
         //Add PivotFormatCondition
         int formatIndex = pivot.getConditionalFormats().add();
         PivotConditionalFormat pfc = pivot.getConditionalFormats().get(formatIndex);
         pfc.addCellArea(pivot.getDataBodyRange());
         FormatConditionCollection fcc = pfc.getFormatConditions();
         int ii = fcc.addCondition(FormatConditionType.CELL_VALUE, OperatorType.GREATER_OR_EQUAL, "100", null);
 
         FormatCondition fc = fcc.get(ii);
 
         fc.getStyle().setBackgroundColor(Color.getRed());
 
          PivotTableCalculateOption calculateOption = new PivotTableCalculateOption();
          calculateOption.setRefreshData(true);
          calculateOption.setRefreshCharts(true);
          pivot.calculateData(calculateOption); 
 
         //do your business
 
         book.save("out.xlsx");
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [addCalculatedField(String name, String formula)](#addCalculatedField-java.lang.String-java.lang.String-) | Lägger till ett beräknat fält i pivotfältet och drar det till dataområdet. |
| [addCalculatedField(String name, String formula, boolean dragToDataArea)](#addCalculatedField-java.lang.String-java.lang.String-boolean-) | Lägger till ett beräknat fält i pivotfältet. |
| [addFieldToArea(int fieldType, PivotField pivotField)](#addFieldToArea-int-com.aspose.cells.PivotField-) | Lägger till fältet i det specifika området. |
| [addFieldToArea(int fieldType, int baseFieldIndex)](#addFieldToArea-int-int-) | Lägger till fältet i det specifika området. |
| [addFieldToArea(int fieldType, String fieldName)](#addFieldToArea-int-java.lang.String-) | Lägger till fältet i det specifika området. |
| [calculateData()](#calculateData--) | Beräknar data från pivottabellen till celler. |
| [calculateData(PivotTableCalculateOption option)](#calculateData-com.aspose.cells.PivotTableCalculateOption-) | Beräknar pivottabell med alternativ. |
| [calculateRange()](#calculateRange--) | Beräknar pivottabellens område. |
| [changeDataSource(String[] source)](#changeDataSource-java.lang.String---) | Ändra datakälla för pivottabellen. |
| [clearAll()](#clearAll--) | Ta bort alla fält från regioner. |
| [clearData()](#clearData--) | Rensa data och formatering i PivotTable-vyn. |
| [clearFilters()](#clearFilters--) | Rensar alla filter i denna pivottabell. |
| [copyStyle(PivotTable pivotTable)](#copyStyle-com.aspose.cells.PivotTable-) | Kopierar namngiven stil från en annan pivottabell. |
| [dispose()](#dispose--) | Utför applikationsdefinierade uppgifter som är relaterade till att frigöra, släppa eller återställa ohanterade resurser. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportViewToJson(PivotViewToJsonOptions options)](#exportViewToJson-com.aspose.cells.PivotViewToJsonOptions-) | Exporterar pivottvyn som JSON. |
| [fields(int fieldType)](#fields-int-) | Hämtar de specifika fälten efter fälttypen. |
| [format(CellArea ca, Style style)](#format-com.aspose.cells.CellArea-com.aspose.cells.Style-) | Formaterar markerat område i pivottabellen. |
| [format(PivotArea pivotArea, Style style)](#format-com.aspose.cells.PivotArea-com.aspose.cells.Style-) | Formaterar markerat område i pivottabellen. |
| [format(int row, int column, Style style)](#format-int-int-com.aspose.cells.Style-) | Formaterar cellen i pivottabellområdet |
| [formatAll(Style style)](#formatAll-com.aspose.cells.Style-) | Formatera alla celler i pivottabellområdet |
| [formatRow(int row, Style style)](#formatRow-int-com.aspose.cells.Style-) | Formatera raddata i pivottabellområdet |
| [getAllowMultipleFiltersPerField()](#getAllowMultipleFiltersPerField--) | Anger ett booleskt värde som indikerar om fälten i en pivottabell kan ha flera filter inställda på dem. |
| [getAltTextDescription()](#getAltTextDescription--) | Hämtar beskrivningen av alternativtexten. |
| [getAltTextTitle()](#getAltTextTitle--) | Hämtar titeln på alternativtexten. |
| [getAutoFormatType()](#getAutoFormatType--) | Hämtar den automatiska formattypen för pivottabellen. |
| [getAutofitColumnWidthOnUpdate()](#getAutofitColumnWidthOnUpdate--) | Anger om kolumnbredden ska anpassas automatiskt vid uppdatering |
| [getBaseFields()](#getBaseFields--) | Returnerar alla grundläggande pivotfält i pivottabellen. |
| [getButtonArea(int axisType)](#getButtonArea-int-) | Hämtar området som innehåller fältknappen. |
| [getCellByDisplayName(String displayName)](#getCellByDisplayName-java.lang.String-) | Hämtar [Cell](../../com.aspose.cells/cell)-objektet efter visningsnamnet för PivotField. |
| [getChildren()](#getChildren--) | Hämtar de underordnade pivottabellerna som använder denna pivottabells data som datakälla. |
| [getClass()](#getClass--) |  |
| [getColumnFields()](#getColumnFields--) | Returnerar ett PivotFields-objekt som för närvarande visas som kolumnfält. |
| [getColumnGrand()](#getColumnGrand--) | Anger om pivottabellsrapporten visar totalsummor för kolumner. |
| [getColumnHeaderCaption()](#getColumnHeaderCaption--) | Hämtar den anpassade rubriken för kolumnrubriken i pivottabellen. |
| [getColumnRange()](#getColumnRange--) | Returnerar ett CellArea-objekt som representerar det område som innehåller kolumnområdet i pivottabellsrapporten. |
| [getConditionalFormats()](#getConditionalFormats--) | Hämtar de villkorliga formaten för pivottabellen. |
| [getCustomListSort()](#getCustomListSort--) | Anger om inbyggda anpassade listor ska beaktas vid sortering av data. |
| [getDataBodyRange()](#getDataBodyRange--) | Returnerar ett [CellArea](../../com.aspose.cells/cellarea)-objekt som representerar det område som innehåller dataområdet i listan mellan rubrikraden och infogningsraden. |
| [getDataField()](#getDataField--) | Hämtar ett [PivotField](../../com.aspose.cells/pivotfield)-objekt som representerar alla datafält i en pivottabell. |
| [getDataFieldHeaderName()](#getDataFieldHeaderName--) | Hämtar namnet på fältets rubrik i värdeområdet i PivotTable. |
| [getDataFields()](#getDataFields--) | Hämtar en [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) som representerar alla datafält i en PivotTable. |
| [getDataSource()](#getDataSource--) | Hämtar datakällan för pivottabellen. |
| [getDependentPivotTables()](#getDependentPivotTables--) | Hämtar alla [PivotTable](../../com.aspose.cells/pivottable)s som använder denna PivotTable som sin datakälla. |
| [getDisplayErrorString()](#getDisplayErrorString--) | Anger om PivotTable-rapporten visar en anpassad sträng i celler som innehåller fel. |
| [getDisplayImmediateItems()](#getDisplayImmediateItems--) | Anger om objekt i rad- och kolumnområdena är synliga när dataområdet i PivotTable är tomt. |
| [getDisplayNullString()](#getDisplayNullString--) | Anger om PivotTable-rapporten visar en anpassad sträng om värdet är null. |
| [getEnableDataValueEditing()](#getEnableDataValueEditing--) | Specificerar ett booleskt värde som anger om användaren får redigera cellerna i dataområdet i pivottabellen. |
| [getEnableDrilldown()](#getEnableDrilldown--) | Anger om drilldown är aktiverat. |
| [getEnableFieldDialog()](#getEnableFieldDialog--) | Anger om dialogrutan PivotTable Field är tillgänglig när användaren dubbelklickar på PivotTable-fältet. |
| [getEnableFieldList()](#getEnableFieldList--) | Anger om fältlistan för PivotTable är tillgänglig i Excel-vyn. |
| [getEnableWizard()](#getEnableWizard--) | Anger om PivotTable-guiden är tillgänglig. |
| [getErrorString()](#getErrorString--) | Hämtar strängen som visas i celler som innehåller fel när egenskapen DisplayErrorString är sann. Standardvärdet är en tom sträng. |
| [getExternalConnectionDataSource()](#getExternalConnectionDataSource--) | Hämtar den externa anslutningsdatakällan. |
| [getFieldListSortAscending()](#getFieldListSortAscending--) | Anger om fält i PivotTable är sorterade i icke‑standardordning i fältlistan. |
| [getFields(int fieldType)](#getFields-int-) | Hämtar den specifika pivotfältlistan efter region. |
| [getFilterArea()](#getFilterArea--) | Hämtar området för filterregionen. |
| [getGrandTotalName()](#getGrandTotalName--) | Returnerar etiketten som visas i rubriken för totalkolumnen eller totalraden. |
| [getHorizontalBreaks()](#getHorizontalBreaks--) | Hämtar pivottabellens radindexlista för horisontella sidbrytningar. |
| [getHorizontalPageBreaks()](#getHorizontalPageBreaks--) | Hämtar horisontella sidbrytningar för denna pivottabell. |
| [getIndent()](#getIndent--) | Specificerar indenteringsökningen för kompakt axel och kan användas för att ställa in rapportlayouten till kompakt form. |
| [getItemPrintTitles()](#getItemPrintTitles--) | Anger om PivotItem-namn ska upprepas högst upp på varje utskriven sida. |
| [getManualUpdate()](#getManualUpdate--) | Anger om PivotTable-rapporten endast beräknas om användaren begär det. |
| [getMergeLabels()](#getMergeLabels--) | Hämtar om rad-/kolumnfältetiketter som sträcker sig över flera celler ska slås ihop. |
| [getMissingItemsLimit()](#getMissingItemsLimit--) | Anger ett booleskt värde som indikerar om fälten i en pivottabell kan ha flera filter inställda på dem. |
| [getName()](#getName--) | Hämtar namnet på PivotTable. |
| [getNamesOfSourceDataConnections()](#getNamesOfSourceDataConnections--) | Hämtar namnen på externa källdatakopplingar. |
| [getNullString()](#getNullString--) | Hämtar strängen som visas i celler som innehåller null‑värden när egenskapen DisplayNullString är sann. Standardvärdet är en tom sträng. |
| [getPageFieldOrder()](#getPageFieldOrder--) | Hämtar den ordning i vilken sidfält läggs till i PivotTable‑rapportens layout. |
| [getPageFieldWrapCount()](#getPageFieldWrapCount--) | Hämtar antalet sidfält i varje kolumn eller rad i PivotTable‑rapporten. |
| [getPageFields()](#getPageFields--) | Returnerar en [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) som för närvarande visas som sidfält. |
| [getPivotCache()](#getPivotCache--) | Hämtar datakällan. |
| [getPivotFilters()](#getPivotFilters--) | Returnerar alla filter i pivottabellen. |
| [getPivotFormatConditions()](#getPivotFormatConditions--) | Hämtar formatvillkoren för pivottabellen. |
| [getPivotFormats()](#getPivotFormats--) | Hämtar alla cellformat som tillämpas på denna pivottabell. |
| [getPivotTableStyle()](#getPivotTableStyle--) | Hämtar [TableStyle](../../com.aspose.cells/tablestyle)-inställningarna för denna pivottabell. |
| [getPivotTableStyleName()](#getPivotTableStyleName--) | Hämtar stilnamnet för pivottabellen. |
| [getPivotTableStyleType()](#getPivotTableStyleType--) | Hämtar den inbyggda pivottabellstilen. |
| [getPivotTablesWithSamePivotCache()](#getPivotTablesWithSamePivotCache--) | Hämtar alla pivottabeller med samma pivot‑cache. |
| [getPreserveCellFormattingOnUpdate()](#getPreserveCellFormattingOnUpdate--) | Anger om cellformatering ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) ska bevaras när pivottabellen uppdateras eller beräknas om. |
| [getPreserveFormatting()](#getPreserveFormatting--) | Anger om cellformatering ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) bevaras när pivottabellen uppdateras eller beräknas om. |
| [getPrintDrill()](#getPrintDrill--) | Anger ett booleskt värde som visar om drill‑indikatorer ska skrivas ut. |
| [getPrintTitles()](#getPrintTitles--) | Anger om utskriftsrubrikerna för kalkylbladet är inställda baserat på PivotTable‑rapporten. |
| [getRefreshDataOnOpeningFile()](#getRefreshDataOnOpeningFile--) | Anger om data ska uppdateras när filen öppnas. |
| [getRefreshDate()](#getRefreshDate--) | Hämtar det senaste datumet och tiden då pivottabellen uppdaterades. |
| [getRefreshedByWho()](#getRefreshedByWho--) | Hämtar namnet på den senaste användaren som uppdaterade denna pivottabell. |
| [getRepeatItemsOnEachPrintedPage()](#getRepeatItemsOnEachPrintedPage--) | Anger om rubriker för pivot‑objekt i radområdet upprepas på varje utskriven sida för pivottfält i tabellform. |
| [getRowFields()](#getRowFields--) | Returnerar en [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) som för närvarande visas som radfält. |
| [getRowGrand()](#getRowGrand--) | Anger om totalsummor för rader i denna pivottabell ska visas. |
| [getRowHeaderCaption()](#getRowHeaderCaption--) | Hämtar anpassad rubrik för radhuvudet i denna pivottabell. |
| [getRowRange()](#getRowRange--) | Returnerar ett CellArea‑objekt som representerar det område som innehåller radområdet i PivotTable‑rapporten. |
| [getSaveData()](#getSaveData--) | Anger om data för PivotTable-rapporten sparas med arbetsboken. |
| [getShowColumnGrandTotals()](#getShowColumnGrandTotals--) | Anger om sammanlagda totaler för kolumnerna i denna pivottabell ska visas. |
| [getShowDataTips()](#getShowDataTips--) | Anger om verktygstips ska visas för pivottabellens dataceller. |
| [getShowDrill()](#getShowDrill--) | Hämtar om expandera/kollapsa-knappar visas. |
| [getShowEmptyCol()](#getShowEmptyCol--) | Anger om tomma kolumner ska inkluderas i tabellen. |
| [getShowEmptyRow()](#getShowEmptyRow--) | Anger om tomma rader ska inkluderas i tabellen. |
| [getShowHeaders()](#getShowHeaders--) | Om datafältetiketter och pivottfältetiketter ska visas på radaxeln och kolumnaxeln i pivottabellsvyn. |
| [getShowMemberPropertyTips()](#getShowMemberPropertyTips--) | Specificerar ett booleskt värde som anger om medlemsegenskapsinformation ska utelämnas från pivottabellens verktygstips. |
| [getShowPivotStyleColumnHeader()](#getShowPivotStyleColumnHeader--) | Anger om kolumnrubriken i pivottabellen ska ha stilen tillämpad. |
| [getShowPivotStyleColumnStripes()](#getShowPivotStyleColumnStripes--) | Anger om ränderformatering tillämpas för kolumnen. |
| [getShowPivotStyleLastColumn()](#getShowPivotStyleLastColumn--) | Anger om kolumnformatering har tillämpats. |
| [getShowPivotStyleRowHeader()](#getShowPivotStyleRowHeader--) | Anger om radrubriken i pivottabellen ska ha stilen tillämpad. |
| [getShowPivotStyleRowStripes()](#getShowPivotStyleRowStripes--) | Anger om radränderformatering tillämpas. |
| [getShowRowGrandTotals()](#getShowRowGrandTotals--) | Anger om sammanlagda totaler för raderna i pivottabellen ska visas. |
| [getShowRowHeaderCaption()](#getShowRowHeaderCaption--) | Anger om radrubrikens rubrik visas i pivottabellrapporten Anger om fältetiketter och filterrullgardiner visas. |
| [getShowValuesRow()](#getShowValuesRow--) | Anger om värderad rad visas. |
| [getSource()](#getSource--) | Hämta datakällan för denna pivottabell. |
| [getSource(boolean isOriginal)](#getSource-boolean-) | Hämta datakällan för denna pivottabell. |
| [getSourceDataConnections()](#getSourceDataConnections--) | Hämtar de externa anslutningsdatakällorna. |
| [getSourceType()](#getSourceType--) | Hämtar datakälltyp för pivottabellen. |
| [getSubtotalHiddenPageItems()](#getSubtotalHiddenPageItems--) | Anger om dolda sidfältsposter i pivottabellrapporten inkluderas i rad- och kolumnsubtotals, blocktotaler och sammanlagda totaler. |
| [getTableRange1()](#getTableRange1--) | Returnerar ett CellArea-objekt som representerar området som innehåller hela pivottabellrapporten, men inkluderar inte sidfält. |
| [getTableRange2()](#getTableRange2--) | Returnerar ett CellArea-objekt som representerar området som innehåller hela pivottabellrapporten, inkluderar sidfält. |
| [getTag()](#getTag--) | Hämtar en användardefinierad sträng som är associerad med denna pivottabellsvy. |
| [getTopRightArea()](#getTopRightArea--) | Representerar det tomma området högst upp till höger i pivottabellen (uppe till vänster för RTL-ark). |
| [getValuesField()](#getValuesField--) | Hämtar ett [PivotField](../../com.aspose.cells/pivotfield)-objekt som representerar alla datafält i en pivottabell. |
| [hasBlankRows()](#hasBlankRows--) | Anger om tomma rader ska läggas till. |
| [hashCode()](#hashCode--) |  |
| [isAutoFormat()](#isAutoFormat--) | Anger om pivottabellrapporten är automatiskt formaterad. |
| [isExcel2003Compatible()](#isExcel2003Compatible--) | Anger om pivottabellen är kompatibel med Excel2003 vid uppdatering av pivottabellen; om true måste en sträng vara högst 255 tecken, så om strängen är längre än 255 tecken kommer den att trunkeras. Om false har en sträng inte den nämnda begränsningen. |
| [isGridDropZones()](#isGridDropZones--) | Anger om pivottabellrapporten visar klassisk pivottabelllayout. |
| [isMultipleFieldFilters()](#isMultipleFieldFilters--) | Anger ett booleskt värde som indikerar om fälten i en pivottabell kan ha flera filter inställda på dem. |
| [isSelected()](#isSelected--) | Anger om denna pivottabell är markerad. |
| [move(int row, int column)](#move-int-int-) | Flyttar pivottabellen till en annan plats i kalkylbladet. |
| [move(String destCellName)](#move-java.lang.String-) | Flyttar pivottabellen till en annan plats i kalkylbladet. |
| [moveItem(int region, String[] nodes, boolean absolute, int offset)](#moveItem-int-java.lang.String---boolean-int-) | Flytta ett objekt upp eller ner. |
| [moveTo(int row, int column)](#moveTo-int-int-) | Flyttar pivottabellen till en annan plats i kalkylbladet. |
| [moveTo(int sheetIndex, int row, int column)](#moveTo-int-int-int-) | Flyttar pivottabellen till en annan plats i kalkylbladet. |
| [moveTo(String destCellName)](#moveTo-java.lang.String-) | Flyttar pivottabellen till en annan plats i kalkylbladet. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refresh()](#refresh--) | Uppdatera [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) från datakällan och beräkna data och stil för pivotsyn. |
| [refresh(PivotTableRefreshOption option)](#refresh-com.aspose.cells.PivotTableRefreshOption-) | Uppdatera [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) från datakällan och beräkna data och stil för pivotsyn. |
| [refreshData()](#refreshData--) | Uppdaterar data från dess datakälla till pivottcachen. |
| [refreshData(PivotTableRefreshOption option)](#refreshData-com.aspose.cells.PivotTableRefreshOption-) | Uppdaterar pivottabellens data och inställningar från dess datakälla med alternativ. |
| [removeField(int fieldType, PivotField pivotField)](#removeField-int-com.aspose.cells.PivotField-) | Ta bort fält från specifikt fältområde |
| [removeField(int fieldType, int baseFieldIndex)](#removeField-int-int-) | Tar bort ett fält från ett specifikt pivottabellområde. |
| [removeField(int fieldType, String fieldName)](#removeField-int-java.lang.String-) | Tar bort ett fält från specifikt fältområde. |
| [selectArea(CellArea ca)](#selectArea-com.aspose.cells.CellArea-) | Välj ett område i pivottabellvyn. |
| [setAllowMultipleFiltersPerField(boolean value)](#setAllowMultipleFiltersPerField-boolean-) | Anger ett booleskt värde som indikerar om fälten i en pivottabell kan ha flera filter inställda på dem. |
| [setAltTextDescription(String value)](#setAltTextDescription-java.lang.String-) | Hämtar beskrivningen av alternativtexten. |
| [setAltTextTitle(String value)](#setAltTextTitle-java.lang.String-) | Ställer in titeln för alternativ text. |
| [setAutoFormat(boolean value)](#setAutoFormat-boolean-) | Anger om pivottabellrapporten är automatiskt formaterad. |
| [setAutoFormatType(int value)](#setAutoFormatType-int-) | Ställer in den automatiska formateringstypen för pivottabellen. |
| [setAutofitColumnWidthOnUpdate(boolean value)](#setAutofitColumnWidthOnUpdate-boolean-) | Anger om kolumnbredden ska anpassas automatiskt vid uppdatering |
| [setColumnGrand(boolean value)](#setColumnGrand-boolean-) | Anger om pivottabellsrapporten visar totalsummor för kolumner. |
| [setColumnHeaderCaption(String value)](#setColumnHeaderCaption-java.lang.String-) | Ställer in den anpassade rubriken för kolumnhuvudet i pivottabellen. |
| [setCustomListSort(boolean value)](#setCustomListSort-boolean-) | Anger om inbyggda anpassade listor ska beaktas vid sortering av data. |
| [setDataFieldHeaderName(String value)](#setDataFieldHeaderName-java.lang.String-) | Ställer in namnet på värdeområdets fälthuvud i pivottabellen. |
| [setDataSource(String[] value)](#setDataSource-java.lang.String---) | Ställer in datakällan för pivottabellen. |
| [setDisplayErrorString(boolean value)](#setDisplayErrorString-boolean-) | Anger om PivotTable-rapporten visar en anpassad sträng i celler som innehåller fel. |
| [setDisplayImmediateItems(boolean value)](#setDisplayImmediateItems-boolean-) | Anger om objekt i rad- och kolumnområdena är synliga när dataområdet i PivotTable är tomt. |
| [setDisplayNullString(boolean value)](#setDisplayNullString-boolean-) | Anger om PivotTable-rapporten visar en anpassad sträng om värdet är null. |
| [setEnableDataValueEditing(boolean value)](#setEnableDataValueEditing-boolean-) | Specificerar ett booleskt värde som anger om användaren får redigera cellerna i dataområdet i pivottabellen. |
| [setEnableDrilldown(boolean value)](#setEnableDrilldown-boolean-) | Anger om drilldown är aktiverat. |
| [setEnableFieldDialog(boolean value)](#setEnableFieldDialog-boolean-) | Anger om dialogrutan PivotTable Field är tillgänglig när användaren dubbelklickar på PivotTable-fältet. |
| [setEnableFieldList(boolean value)](#setEnableFieldList-boolean-) | Anger om fältlistan för PivotTable är tillgänglig i Excel-vyn. |
| [setEnableWizard(boolean value)](#setEnableWizard-boolean-) | Anger om PivotTable-guiden är tillgänglig. |
| [setErrorString(String value)](#setErrorString-java.lang.String-) | Hämtar strängen som visas i celler som innehåller fel när egenskapen DisplayErrorString är sann. Standardvärdet är en tom sträng. |
| [setExcel2003Compatible(boolean value)](#setExcel2003Compatible-boolean-) | Anger om pivottabellen är kompatibel med Excel2003 vid uppdatering av pivottabellen; om true måste en sträng vara högst 255 tecken, så om strängen är längre än 255 tecken kommer den att trunkeras. Om false har en sträng inte den nämnda begränsningen. |
| [setFieldListSortAscending(boolean value)](#setFieldListSortAscending-boolean-) | Anger om fält i PivotTable är sorterade i icke‑standardordning i fältlistan. |
| [setGrandTotalName(String value)](#setGrandTotalName-java.lang.String-) | Returnerar etiketten som visas i rubriken för totalkolumnen eller totalraden. |
| [setGridDropZones(boolean value)](#setGridDropZones-boolean-) | Anger om pivottabellrapporten visar klassisk pivottabelllayout. |
| [setHasBlankRows(boolean value)](#setHasBlankRows-boolean-) | Anger om tomma rader ska läggas till. |
| [setIndent(int value)](#setIndent-int-) | Specificerar indenteringsökningen för kompakt axel och kan användas för att ställa in rapportlayouten till kompakt form. |
| [setItemPrintTitles(boolean value)](#setItemPrintTitles-boolean-) | Anger om PivotItem-namn ska upprepas högst upp på varje utskriven sida. |
| [setManualUpdate(boolean value)](#setManualUpdate-boolean-) | Anger om PivotTable-rapporten endast beräknas om användaren begär det. |
| [setMergeLabels(boolean value)](#setMergeLabels-boolean-) | Anger om rad-/kolumnfältetiketter som sträcker sig över flera celler ska slås ihop. |
| [setMissingItemsLimit(int value)](#setMissingItemsLimit-int-) | Anger ett booleskt värde som indikerar om fälten i en pivottabell kan ha flera filter inställda på dem. |
| [setMultipleFieldFilters(boolean value)](#setMultipleFieldFilters-boolean-) | Anger ett booleskt värde som indikerar om fälten i en pivottabell kan ha flera filter inställda på dem. |
| [setName(String value)](#setName-java.lang.String-) | Hämtar namnet på PivotTable. |
| [setNullString(String value)](#setNullString-java.lang.String-) | Hämtar strängen som visas i celler som innehåller null‑värden när egenskapen DisplayNullString är sann. Standardvärdet är en tom sträng. |
| [setPageFieldOrder(int value)](#setPageFieldOrder-int-) | Anger den ordning i vilken sidfält läggs till i pivottabellrapportens layout. |
| [setPageFieldWrapCount(int value)](#setPageFieldWrapCount-int-) | Hämtar antalet sidfält i varje kolumn eller rad i PivotTable‑rapporten. |
| [setPivotTableStyle(TableStyle value)](#setPivotTableStyle-com.aspose.cells.TableStyle-) | Hämtar [TableStyle](../../com.aspose.cells/tablestyle)-inställningarna för denna pivottabell. |
| [setPivotTableStyleName(String value)](#setPivotTableStyleName-java.lang.String-) | Ställer in stilnamnet för pivottabellen. |
| [setPivotTableStyleType(int value)](#setPivotTableStyleType-int-) | Ställer in den inbyggda pivottabellstilen. |
| [setPreserveCellFormattingOnUpdate(boolean value)](#setPreserveCellFormattingOnUpdate-boolean-) | Anger om cellformatering ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) ska bevaras när pivottabellen uppdateras eller beräknas om. |
| [setPreserveFormatting(boolean value)](#setPreserveFormatting-boolean-) | Anger om cellformatering ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) bevaras när pivottabellen uppdateras eller beräknas om. |
| [setPrintDrill(boolean value)](#setPrintDrill-boolean-) | Anger ett booleskt värde som visar om drill‑indikatorer ska skrivas ut. |
| [setPrintTitles(boolean value)](#setPrintTitles-boolean-) | Anger om utskriftsrubrikerna för kalkylbladet är inställda baserat på PivotTable‑rapporten. |
| [setRefreshDataOnOpeningFile(boolean value)](#setRefreshDataOnOpeningFile-boolean-) | Anger om data ska uppdateras när filen öppnas. |
| [setRepeatItemsOnEachPrintedPage(boolean value)](#setRepeatItemsOnEachPrintedPage-boolean-) | Anger om rubriker för pivot‑objekt i radområdet upprepas på varje utskriven sida för pivottfält i tabellform. |
| [setRowGrand(boolean value)](#setRowGrand-boolean-) | Anger om totalsummor för rader i denna pivottabell ska visas. |
| [setRowHeaderCaption(String value)](#setRowHeaderCaption-java.lang.String-) | Ställer in anpassad rubrik för radhuvudet i denna pivottabell. |
| [setSaveData(boolean value)](#setSaveData-boolean-) | Anger om data för PivotTable-rapporten sparas med arbetsboken. |
| [setSelected(boolean value)](#setSelected-boolean-) | Anger om denna pivottabell är markerad. |
| [setShowColumnGrandTotals(boolean value)](#setShowColumnGrandTotals-boolean-) | Anger om sammanlagda totaler för kolumnerna i denna pivottabell ska visas. |
| [setShowDataTips(boolean value)](#setShowDataTips-boolean-) | Anger om verktygstips ska visas för pivottabellens dataceller. |
| [setShowDrill(boolean value)](#setShowDrill-boolean-) | Anger om expandera-/kollapsa-knappar ska visas. |
| [setShowEmptyCol(boolean value)](#setShowEmptyCol-boolean-) | Anger om tomma kolumner ska inkluderas i tabellen. |
| [setShowEmptyRow(boolean value)](#setShowEmptyRow-boolean-) | Anger om tomma rader ska inkluderas i tabellen. |
| [setShowHeaders(boolean value)](#setShowHeaders-boolean-) | Om datafältetiketter och pivottfältetiketter ska visas på radaxeln och kolumnaxeln i pivottabellsvyn. |
| [setShowMemberPropertyTips(boolean value)](#setShowMemberPropertyTips-boolean-) | Specificerar ett booleskt värde som anger om medlemsegenskapsinformation ska utelämnas från pivottabellens verktygstips. |
| [setShowPivotStyleColumnHeader(boolean value)](#setShowPivotStyleColumnHeader-boolean-) | Anger om kolumnrubriken i pivottabellen ska ha stilen tillämpad. |
| [setShowPivotStyleColumnStripes(boolean value)](#setShowPivotStyleColumnStripes-boolean-) | Anger om ränderformatering tillämpas för kolumnen. |
| [setShowPivotStyleLastColumn(boolean value)](#setShowPivotStyleLastColumn-boolean-) | Anger om kolumnformatering har tillämpats. |
| [setShowPivotStyleRowHeader(boolean value)](#setShowPivotStyleRowHeader-boolean-) | Anger om radrubriken i pivottabellen ska ha stilen tillämpad. |
| [setShowPivotStyleRowStripes(boolean value)](#setShowPivotStyleRowStripes-boolean-) | Anger om radränderformatering tillämpas. |
| [setShowRowGrandTotals(boolean value)](#setShowRowGrandTotals-boolean-) | Anger om sammanlagda totaler för raderna i pivottabellen ska visas. |
| [setShowRowHeaderCaption(boolean value)](#setShowRowHeaderCaption-boolean-) | Anger om radrubrikens rubrik visas i pivottabellrapporten Anger om fältetiketter och filterrullgardiner visas. |
| [setShowValuesRow(boolean value)](#setShowValuesRow-boolean-) | Anger om värderad rad visas. |
| [setSubtotalHiddenPageItems(boolean value)](#setSubtotalHiddenPageItems-boolean-) | Anger om dolda sidfältsposter i pivottabellrapporten inkluderas i rad- och kolumnsubtotals, blocktotaler och sammanlagda totaler. |
| [setTag(String value)](#setTag-java.lang.String-) | Ställer in en användardefinierad sträng som är associerad med denna pivottabellvy. |
| [showDetail(int rowOffset, int columnOffset, boolean newSheet, int destRow, int destColumn)](#showDetail-int-int-boolean-int-int-) | Visa detaljerna för ett objekt i dataområdet i en ny tabell. |
| [showInCompactForm()](#showInCompactForm--) | Formaterar PivotTable-vyn i kompakt form. |
| [showInOutlineForm()](#showInOutlineForm--) | Formaterar PivotTable i konturform. |
| [showInTabularForm()](#showInTabularForm--) | Formaterar PivotTable i tabellform. |
| [showReportFilterPage(PivotField pageField)](#showReportFilterPage-com.aspose.cells.PivotField-) | Visa alla rapportsfilter‑sidor enligt PivotField, PivotField måste vara placerad i PageFields. |
| [showReportFilterPageByIndex(int posIndex)](#showReportFilterPageByIndex-int-) | Visa alla rapportsfilter‑sidor enligt positionsindexet i PageFields. |
| [showReportFilterPageByName(String fieldName)](#showReportFilterPageByName-java.lang.String-) | Visa alla rapportsfilter‑sidor enligt PivotFields namn, PivotField måste vara placerad i PageFields. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addCalculatedField(String name, String formula) {#addCalculatedField-java.lang.String-java.lang.String-}
```
public void addCalculatedField(String name, String formula)
```


Lägger till ett beräknat fält i pivotfältet och drar det till dataområdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Namnet på det beräknade fältet |
| formula | java.lang.String | Formeln för det beräknade fältet. |

### addCalculatedField(String name, String formula, boolean dragToDataArea) {#addCalculatedField-java.lang.String-java.lang.String-boolean-}
```
public void addCalculatedField(String name, String formula, boolean dragToDataArea)
```


Lägger till ett beräknat fält i pivotfältet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Namnet på det beräknade fältet |
| formula | java.lang.String | Formeln för det beräknade fältet. |
| dragToDataArea | boolean | Sant, dra detta fält till dataområdet omedelbart |

### addFieldToArea(int fieldType, PivotField pivotField) {#addFieldToArea-int-com.aspose.cells.PivotField-}
```
public int addFieldToArea(int fieldType, PivotField pivotField)
```


Lägger till fältet i det specifika området.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). fältområdestypen. |
| pivotField | [PivotField](../../com.aspose.cells/pivotfield) | fältet i basfälten. |

**Returns:**
int - fältets position i de specifika fälten.
### addFieldToArea(int fieldType, int baseFieldIndex) {#addFieldToArea-int-int-}
```
public int addFieldToArea(int fieldType, int baseFieldIndex)
```


Lägger till fältet i det specifika området.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Fältområdestypen. |
| baseFieldIndex | int | Indexet i basfälten. |

**Returns:**
int - Fältets position i de specifika fälten.
### addFieldToArea(int fieldType, String fieldName) {#addFieldToArea-int-java.lang.String-}
```
public int addFieldToArea(int fieldType, String fieldName)
```


Lägger till fältet i det specifika området.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Fältområdestypen. |
| fieldName | java.lang.String | Namnet i basfälten. |

**Returns:**
int - Fältets position i de specifika fälten. Om det inte finns något fält med detta namn, returnera -1.
### calculateData() {#calculateData--}
```
public void calculateData()
```


Beräknar data från pivottabellen till celler.

**Remarks**

Denna metod beräknar endast data med den cachade datan i [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--). Så om du vill beräkna med den senaste datakällan, använd metoden [PivotCache.refresh()](../../com.aspose.cells/pivotcache\#refresh--) . Om endast pivottabellens inställningar har ändrats, räcker [calculateData()](../../com.aspose.cells/pivottable\#calculateData--) .

### calculateData(PivotTableCalculateOption option) {#calculateData-com.aspose.cells.PivotTableCalculateOption-}
```
public PivotTable[] calculateData(PivotTableCalculateOption option)
```


Beräknar pivottabell med alternativ.

**Remarks**

Om [PivotTableCalculateOption.getRefreshData()](../../com.aspose.cells/pivottablecalculateoption\#getRefreshData--) är sant, kommer denna metod att uppdatera pivotcachen från datakällan, och sedan beräkna alla pivottabeller baserade på samma pivotcache. Annars beräknas endast med den cachade datan i pivotcachen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| option | [PivotTableCalculateOption](../../com.aspose.cells/pivottablecalculateoption) | Alternativen för att beräkna pivottabellen |

**Returns:**
com.aspose.cells.PivotTable[] - Returnerar alla pivottabeller som har beräknats. Om [PivotTableCalculateOption.getRefreshData()](../../com.aspose.cells/pivottablecalculateoption\#getRefreshData--) är sant, kommer alla pivottabeller baserade på samma pivotcache att beräknas tillsammans.
### calculateRange() {#calculateRange--}
```
public void calculateRange()
```


Beräknar pivottabellens område.

**Remarks**

Om denna metod inte har anropats, kan pivottabellens område vara felaktigt.

### changeDataSource(String[] source) {#changeDataSource-java.lang.String---}
```
public void changeDataSource(String[] source)
```


Ändra datakälla för pivottabellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| källa | java.lang.String[] |  |

### clearAll() {#clearAll--}
```
public void clearAll()
```


Ta bort alla fält från regioner.

### clearData() {#clearData--}
```
public void clearData()
```


Rensa data och formatering i PivotTable-vyn.

**Remarks**

Om den här metoden inte anropas innan du lägger till eller tar bort PivotField, kan PivotTable‑data vara felaktiga

### clearFilters() {#clearFilters--}
```
public void clearFilters()
```


Rensar alla filter i denna pivottabell.

### copyStyle(PivotTable pivotTable) {#copyStyle-com.aspose.cells.PivotTable-}
```
public void copyStyle(PivotTable pivotTable)
```


Kopierar namngiven stil från en annan pivottabell.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | Källpivot-tabell. |

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
### exportViewToJson(PivotViewToJsonOptions options) {#exportViewToJson-com.aspose.cells.PivotViewToJsonOptions-}
```
public String exportViewToJson(PivotViewToJsonOptions options)
```


Exporterar pivottvyn som JSON.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| options | [PivotViewToJsonOptions](../../com.aspose.cells/pivotviewtojsonoptions) |  |

**Returns:**
java.lang.String -
### fields(int fieldType) {#fields-int-}
```
public PivotFieldCollection fields(int fieldType)
```


Hämtar de specifika fälten efter fälttypen.

**Remarks**

OBS: Den här metoden är nu föråldrad. Använd i stället PivotField.GetFields(PivotFieldType)-metoden. Denna metod kommer att tas bort 12 månader senare från och med maj 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). fälttypen. |

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) - the specific field collection
### format(CellArea ca, Style style) {#format-com.aspose.cells.CellArea-com.aspose.cells.Style-}
```
public void format(CellArea ca, Style style)
```


Formaterar markerat område i pivottabellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Cellernas område. |
| style | [Style](../../com.aspose.cells/style) | Stilen |

### format(PivotArea pivotArea, Style style) {#format-com.aspose.cells.PivotArea-com.aspose.cells.Style-}
```
public void format(PivotArea pivotArea, Style style)
```


Formaterar markerat område i pivottabellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivotArea | [PivotArea](../../com.aspose.cells/pivotarea) | Det valda pivot‑vyområdet. |
| style | [Style](../../com.aspose.cells/style) | Den formaterade inställningen. |

### format(int row, int column, Style style) {#format-int-int-com.aspose.cells.Style-}
```
public void format(int row, int column, Style style)
```


Formaterar cellen i pivottabellområdet

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindex för cellen |
| kolumn | int | Kolumnindex för cellen |
| style | [Style](../../com.aspose.cells/style) | Stil som ska formatera cellen |

### formatAll(Style style) {#formatAll-com.aspose.cells.Style-}
```
public void formatAll(Style style)
```


Formatera alla celler i pivottabellområdet

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Stil som ska formatera |

### formatRow(int row, Style style) {#formatRow-int-com.aspose.cells.Style-}
```
public void formatRow(int row, Style style)
```


Formatera raddata i pivottabellområdet

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindex för radobjektet |
| style | [Style](../../com.aspose.cells/style) | Stil som ska formatera |

### getAllowMultipleFiltersPerField() {#getAllowMultipleFiltersPerField--}
```
public boolean getAllowMultipleFiltersPerField()
```


Anger ett booleskt värde som indikerar om fälten i en pivottabell kan ha flera filter inställda på dem.

**Returns:**
boolean
### getAltTextDescription() {#getAltTextDescription--}
```
public String getAltTextDescription()
```


Hämtar beskrivningen av alternativtexten.

**Returns:**
java.lang.String
### getAltTextTitle() {#getAltTextTitle--}
```
public String getAltTextTitle()
```


Hämtar titeln på alternativtexten.

**Returns:**
java.lang.String
### getAutoFormatType() {#getAutoFormatType--}
```
public int getAutoFormatType()
```


Hämtar den automatiska formattypen för pivottabellen.

Se [PivotTableAutoFormatType](../../com.aspose.cells/pivottableautoformattype).

**Returns:**
int
### getAutofitColumnWidthOnUpdate() {#getAutofitColumnWidthOnUpdate--}
```
public boolean getAutofitColumnWidthOnUpdate()
```


Anger om kolumnbredden ska anpassas automatiskt vid uppdatering

**Returns:**
boolean
### getBaseFields() {#getBaseFields--}
```
public PivotFieldCollection getBaseFields()
```


Returnerar alla grundläggande pivotfält i pivottabellen.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getButtonArea(int axisType) {#getButtonArea-int-}
```
public CellArea getButtonArea(int axisType)
```


Hämtar området som innehåller fältknappen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Regionstypen. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - 
### getCellByDisplayName(String displayName) {#getCellByDisplayName-java.lang.String-}
```
public Cell getCellByDisplayName(String displayName)
```


Hämtar [Cell](../../com.aspose.cells/cell)-objektet efter visningsnamnet för PivotField.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| displayName | java.lang.String | DisplayName för PivotField |

**Returns:**
[Cell](../../com.aspose.cells/cell) - the Cell object
### getChildren() {#getChildren--}
```
public PivotTable[] getChildren()
```


Hämtar de underordnade pivottabellerna som använder denna pivottabells data som datakälla.

**Remarks**

OBS: Den här metoden är nu föråldrad. Använd i stället PivotTable.GetDependentPivotTables()-metoden. Denna metod kommer att tas bort 12 månader senare från och med april 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
com.aspose.cells.PivotTable[] - PivotTable‑arrayobjektet
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnFields() {#getColumnFields--}
```
public PivotFieldCollection getColumnFields()
```


Returnerar ett PivotFields-objekt som för närvarande visas som kolumnfält.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getColumnGrand() {#getColumnGrand--}
```
public boolean getColumnGrand()
```


Anger om pivottabellsrapporten visar totalsummor för kolumner.

**Remarks**

OBS: Den här egenskapen är nu föråldrad. Använd i stället PivotTable.ShowColumnGrandTotals‑metoden. Denna metod kommer att tas bort 12 månader senare från och med december 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
boolean
### getColumnHeaderCaption() {#getColumnHeaderCaption--}
```
public String getColumnHeaderCaption()
```


Hämtar den anpassade rubriken för kolumnrubriken i pivottabellen.

**Returns:**
java.lang.String
### getColumnRange() {#getColumnRange--}
```
public CellArea getColumnRange()
```


Returnerar ett CellArea‑objekt som representerar området som innehåller kolumnområdet i PivotTable‑rapporten. Endast läs.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getConditionalFormats() {#getConditionalFormats--}
```
public PivotConditionalFormatCollection getConditionalFormats()
```


Hämtar de villkorliga formaten för pivottabellen.

**Returns:**
[PivotConditionalFormatCollection](../../com.aspose.cells/pivotconditionalformatcollection)
### getCustomListSort() {#getCustomListSort--}
```
public boolean getCustomListSort()
```


Anger om inbyggda anpassade listor ska beaktas vid sortering av data.

**Returns:**
boolean
### getDataBodyRange() {#getDataBodyRange--}
```
public CellArea getDataBodyRange()
```


Returnerar ett [CellArea](../../com.aspose.cells/cellarea)-objekt som representerar området som innehåller dataområdet i listan mellan rubrikraden och infogningsraden. Endast läs.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getDataField() {#getDataField--}
```
public PivotField getDataField()
```


Hämtar ett [PivotField](../../com.aspose.cells/pivotfield)-objekt som representerar alla datafält i en PivotTable. Endast läs. Det skapas endast när det finns två eller fler datafält i datatområdet. Som standard är det i radområdet. Du kan dra det till rad‑/kolumnområdet med metoden PivotTable.AddFieldToArea().

**Remarks**

OBS: Den här metoden är nu föråldrad. Använd i stället PivotTable.ValuesField‑egenskapen. Denna metod kommer att tas bort 12 månader senare från och med oktober 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
[PivotField](../../com.aspose.cells/pivotfield)
### getDataFieldHeaderName() {#getDataFieldHeaderName--}
```
public String getDataFieldHeaderName()
```


Hämtar namnet på fältets rubrik i värdeområdet i PivotTable.

**Returns:**
java.lang.String
### getDataFields() {#getDataFields--}
```
public PivotFieldCollection getDataFields()
```


Hämtar en [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) som representerar alla datafält i en PivotTable.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getDataSource() {#getDataSource--}
```
public String[] getDataSource()
```


Hämtar datakällan för pivottabellen.

**Returns:**
java.lang.String[]
### getDependentPivotTables() {#getDependentPivotTables--}
```
public PivotTable[] getDependentPivotTables()
```


Hämtar alla [PivotTable](../../com.aspose.cells/pivottable)s som använder denna PivotTable som sin datakälla.

**Remarks**

Eftersom pivottabeller kan bero på varandras data måste de uppdateras i rätt ordning för att säkerställa datakonsistens.

**Returns:**
com.aspose.cells.PivotTable[] -
### getDisplayErrorString() {#getDisplayErrorString--}
```
public boolean getDisplayErrorString()
```


Anger om PivotTable-rapporten visar en anpassad sträng i celler som innehåller fel.

**Returns:**
boolean
### getDisplayImmediateItems() {#getDisplayImmediateItems--}
```
public boolean getDisplayImmediateItems()
```


Anger om objekt i rad- och kolumnområdena är synliga när dataområdet i pivottabellen är tomt. Standardvärdet är true.

**Returns:**
boolean
### getDisplayNullString() {#getDisplayNullString--}
```
public boolean getDisplayNullString()
```


Anger om PivotTable-rapporten visar en anpassad sträng om värdet är null.

**Returns:**
boolean
### getEnableDataValueEditing() {#getEnableDataValueEditing--}
```
public boolean getEnableDataValueEditing()
```


Anger ett booleskt värde som visar om användaren får redigera cellerna i dataområdet i pivottabellen. Standardvärdet är false.

**Returns:**
boolean
### getEnableDrilldown() {#getEnableDrilldown--}
```
public boolean getEnableDrilldown()
```


Anger om drilldown är aktiverat.

**Returns:**
boolean
### getEnableFieldDialog() {#getEnableFieldDialog--}
```
public boolean getEnableFieldDialog()
```


Anger om dialogrutan PivotTable Field är tillgänglig när användaren dubbelklickar på PivotTable-fältet.

**Returns:**
boolean
### getEnableFieldList() {#getEnableFieldList--}
```
public boolean getEnableFieldList()
```


Anger om fältlistan för PivotTable är tillgänglig i Excel-vyn.

**Returns:**
boolean
### getEnableWizard() {#getEnableWizard--}
```
public boolean getEnableWizard()
```


Anger om PivotTable-guiden är tillgänglig.

**Returns:**
boolean
### getErrorString() {#getErrorString--}
```
public String getErrorString()
```


Hämtar strängen som visas i celler som innehåller fel när egenskapen DisplayErrorString är sann. Standardvärdet är en tom sträng.

**Returns:**
java.lang.String
### getExternalConnectionDataSource() {#getExternalConnectionDataSource--}
```
public ExternalConnection getExternalConnectionDataSource()
```


Hämtar den externa anslutningsdatakällan.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället PivotTable.GetSourceDataConnections()‑metoden. Denna metod kommer att tas bort 12 månader senare från och med oktober 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
[ExternalConnection](../../com.aspose.cells/externalconnection)
### getFieldListSortAscending() {#getFieldListSortAscending--}
```
public boolean getFieldListSortAscending()
```


Anger om fält i PivotTable är sorterade i icke‑standardordning i fältlistan.

**Returns:**
boolean
### getFields(int fieldType) {#getFields-int-}
```
public PivotFieldCollection getFields(int fieldType)
```


Hämtar den specifika pivotfältlistan efter region.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). regionstypen. |

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) - the specific pivot field collection
### getFilterArea() {#getFilterArea--}
```
public CellArea getFilterArea()
```


Hämtar området för filterregionen.

**Remarks**

Endast giltig om filtrerings-pivotfält finns. Ett tomt område kommer att returneras om denna pivottabell inte innehåller filtrerings-pivotfält.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getGrandTotalName() {#getGrandTotalName--}
```
public String getGrandTotalName()
```


Returnerar etiketten som visas i rubriken för totalkolumnen eller -raden. Standardvärdet är strängen "Grand Total".

**Returns:**
java.lang.String
### getHorizontalBreaks() {#getHorizontalBreaks--}
```
public ArrayList getHorizontalBreaks()
```


Hämtar pivottabellens radindexlista för horisontella sidbrytningar.

**Remarks**

OBS: Denna metod är nu föråldrad. Använd istället PivotTable.GetHorizontalPageBreaks()‑metoden. Denna metod kommer att tas bort 12 månader senare från och med december 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
java.util.ArrayList -
### getHorizontalPageBreaks() {#getHorizontalPageBreaks--}
```
public int[] getHorizontalPageBreaks()
```


Hämtar horisontella sidbrytningar för denna pivottabell.

**Returns:**
int[] -
### getIndent() {#getIndent--}
```
public int getIndent()
```


Specificerar indenteringsökningen för kompakt axel och kan användas för att ställa in rapportlayouten till kompakt form.

**Returns:**
int
### getItemPrintTitles() {#getItemPrintTitles--}
```
public boolean getItemPrintTitles()
```


Anger om PivotItem-namn ska upprepas högst upp på varje utskriven sida.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället PivotTable.RepeatItemsOnEachPrintedPage‑egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med oktober 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
boolean
### getManualUpdate() {#getManualUpdate--}
```
public boolean getManualUpdate()
```


Anger om PivotTable-rapporten endast beräknas om användaren begär det.

**Returns:**
boolean
### getMergeLabels() {#getMergeLabels--}
```
public boolean getMergeLabels()
```


Hämtar om rad-/kolumnfältetiketter som sträcker sig över flera celler ska slås ihop.

**Returns:**
boolean
### getMissingItemsLimit() {#getMissingItemsLimit--}
```
public int getMissingItemsLimit()
```


Anger ett booleskt värde som indikerar om fälten i en pivottabell kan ha flera filter inställda på dem.

Se [PivotMissingItemLimitType](../../com.aspose.cells/pivotmissingitemlimittype).

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället PivotCache.MissingItemsLimit‑egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Hämtar namnet på PivotTable.

**Returns:**
java.lang.String
### getNamesOfSourceDataConnections() {#getNamesOfSourceDataConnections--}
```
public String[] getNamesOfSourceDataConnections()
```


Hämtar namnen på externa källdatakopplingar.

**Returns:**
java.lang.String[]
### getNullString() {#getNullString--}
```
public String getNullString()
```


Hämtar strängen som visas i celler som innehåller null‑värden när egenskapen DisplayNullString är sann. Standardvärdet är en tom sträng.

**Returns:**
java.lang.String
### getPageFieldOrder() {#getPageFieldOrder--}
```
public int getPageFieldOrder()
```


Hämtar den ordning i vilken sidfält läggs till i PivotTable‑rapportens layout.

Se [PrintOrderType](../../com.aspose.cells/printordertype).

**Returns:**
int
### getPageFieldWrapCount() {#getPageFieldWrapCount--}
```
public int getPageFieldWrapCount()
```


Hämtar antalet sidfält i varje kolumn eller rad i PivotTable‑rapporten.

**Returns:**
int
### getPageFields() {#getPageFields--}
```
public PivotFieldCollection getPageFields()
```


Returnerar en [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) som för närvarande visas som sidfält.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getPivotCache() {#getPivotCache--}
```
public PivotCache getPivotCache()
```


Hämtar datakällan.

**Returns:**
[PivotCache](../../com.aspose.cells/pivotcache)
### getPivotFilters() {#getPivotFilters--}
```
public PivotFilterCollection getPivotFilters()
```


Returnerar alla filter i pivottabellen.

**Returns:**
[PivotFilterCollection](../../com.aspose.cells/pivotfiltercollection)
### getPivotFormatConditions() {#getPivotFormatConditions--}
```
public PivotFormatConditionCollection getPivotFormatConditions()
```


Hämtar formatvillkoren för pivottabellen.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället PivotTable.ConditionalFormats‑egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med december 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
[PivotFormatConditionCollection](../../com.aspose.cells/pivotformatconditioncollection)
### getPivotFormats() {#getPivotFormats--}
```
public PivotTableFormatCollection getPivotFormats()
```


Hämtar alla cellformat som tillämpas på denna pivottabell.

**Returns:**
[PivotTableFormatCollection](../../com.aspose.cells/pivottableformatcollection)
### getPivotTableStyle() {#getPivotTableStyle--}
```
public TableStyle getPivotTableStyle()
```


Hämtar [TableStyle](../../com.aspose.cells/tablestyle)-inställningarna för denna pivottabell.

**Returns:**
[TableStyle](../../com.aspose.cells/tablestyle)
### getPivotTableStyleName() {#getPivotTableStyleName--}
```
public String getPivotTableStyleName()
```


Hämtar stilnamnet för pivottabellen.

**Returns:**
java.lang.String
### getPivotTableStyleType() {#getPivotTableStyleType--}
```
public int getPivotTableStyleType()
```


Hämtar den inbyggda pivottabellstilen.

Se [PivotTableStyleType](../../com.aspose.cells/pivottablestyletype).

**Returns:**
int
### getPivotTablesWithSamePivotCache() {#getPivotTablesWithSamePivotCache--}
```
public PivotTable[] getPivotTablesWithSamePivotCache()
```


Hämtar alla pivottabeller med samma pivot‑cache.

**Returns:**
com.aspose.cells.PivotTable[] -
### getPreserveCellFormattingOnUpdate() {#getPreserveCellFormattingOnUpdate--}
```
public boolean getPreserveCellFormattingOnUpdate()
```


Anger om cellformatering ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) ska bevaras när pivottabellen uppdateras eller beräknas om.

**Returns:**
boolean
### getPreserveFormatting() {#getPreserveFormatting--}
```
public boolean getPreserveFormatting()
```


Anger om cellformatering ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) bevaras när pivottabellen uppdateras eller beräknas om.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället PivotTable.PreserveCellFormattingOnUpdate‑egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med juli 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
boolean
### getPrintDrill() {#getPrintDrill--}
```
public boolean getPrintDrill()
```


Anger ett booleskt värde som visar om drill‑indikatorer ska skrivas ut. Skriv ut expandera/kollapsa‑knappar när de visas i pivottabellen.

**Returns:**
boolean
### getPrintTitles() {#getPrintTitles--}
```
public boolean getPrintTitles()
```


Anger om utskriftstitlarna för kalkylbladet sätts baserat på pivottabellrapporten. Standardvärdet är false.

**Returns:**
boolean
### getRefreshDataOnOpeningFile() {#getRefreshDataOnOpeningFile--}
```
public boolean getRefreshDataOnOpeningFile()
```


Anger om data ska uppdateras när filen öppnas.

**Returns:**
boolean
### getRefreshDate() {#getRefreshDate--}
```
public DateTime getRefreshDate()
```


Hämtar det senaste datumet och tiden då pivottabellen uppdaterades.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getRefreshedByWho() {#getRefreshedByWho--}
```
public String getRefreshedByWho()
```


Hämtar namnet på den senaste användaren som uppdaterade denna pivottabell.

**Returns:**
java.lang.String
### getRepeatItemsOnEachPrintedPage() {#getRepeatItemsOnEachPrintedPage--}
```
public boolean getRepeatItemsOnEachPrintedPage()
```


Anger om rubriker för pivot‑objekt i radområdet upprepas på varje utskriven sida för pivottfält i tabellform.

**Returns:**
boolean
### getRowFields() {#getRowFields--}
```
public PivotFieldCollection getRowFields()
```


Returnerar en [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) som för närvarande visas som radfält.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getRowGrand() {#getRowGrand--}
```
public boolean getRowGrand()
```


Anger om totalsummor för rader i denna pivottabell ska visas.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället PivotTable.ShowRowGrandTotals‑metoden. Denna metod kommer att tas bort 12 månader senare från och med december 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
boolean
### getRowHeaderCaption() {#getRowHeaderCaption--}
```
public String getRowHeaderCaption()
```


Hämtar anpassad rubrik för radhuvudet i denna pivottabell.

**Returns:**
java.lang.String
### getRowRange() {#getRowRange--}
```
public CellArea getRowRange()
```


Returnerar ett CellArea‑objekt som representerar området som innehåller radområdet i pivottabellrapporten. Skrivskyddad.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getSaveData() {#getSaveData--}
```
public boolean getSaveData()
```


Anger om data för PivotTable-rapporten sparas med arbetsboken.

**Returns:**
boolean
### getShowColumnGrandTotals() {#getShowColumnGrandTotals--}
```
public boolean getShowColumnGrandTotals()
```


Anger om sammanlagda totaler för kolumnerna i denna pivottabell ska visas.

**Returns:**
boolean
### getShowDataTips() {#getShowDataTips--}
```
public boolean getShowDataTips()
```


Anger om verktygstips ska visas för pivottabellens dataceller.

**Returns:**
boolean
### getShowDrill() {#getShowDrill--}
```
public boolean getShowDrill()
```


Hämtar om expandera/kollapsa-knappar visas.

**Returns:**
boolean
### getShowEmptyCol() {#getShowEmptyCol--}
```
public boolean getShowEmptyCol()
```


Anger om tomma kolumner ska inkluderas i tabellen.

**Returns:**
boolean
### getShowEmptyRow() {#getShowEmptyRow--}
```
public boolean getShowEmptyRow()
```


Anger om tomma rader ska inkluderas i tabellen.

**Returns:**
boolean
### getShowHeaders() {#getShowHeaders--}
```
public boolean getShowHeaders()
```


Om datafältetiketter och pivottfältetiketter ska visas på radaxeln och kolumnaxeln i pivottabellsvyn.

**Returns:**
boolean
### getShowMemberPropertyTips() {#getShowMemberPropertyTips--}
```
public boolean getShowMemberPropertyTips()
```


Specificerar ett booleskt värde som anger om medlemsegenskapsinformation ska utelämnas från pivottabellens verktygstips.

**Returns:**
boolean
### getShowPivotStyleColumnHeader() {#getShowPivotStyleColumnHeader--}
```
public boolean getShowPivotStyleColumnHeader()
```


Anger om kolumnrubriken i pivottabellen ska ha stilen tillämpad.

**Returns:**
boolean
### getShowPivotStyleColumnStripes() {#getShowPivotStyleColumnStripes--}
```
public boolean getShowPivotStyleColumnStripes()
```


Anger om ränderformatering tillämpas för kolumnen.

**Returns:**
boolean
### getShowPivotStyleLastColumn() {#getShowPivotStyleLastColumn--}
```
public boolean getShowPivotStyleLastColumn()
```


Anger om kolumnformatering har tillämpats.

**Returns:**
boolean
### getShowPivotStyleRowHeader() {#getShowPivotStyleRowHeader--}
```
public boolean getShowPivotStyleRowHeader()
```


Anger om radrubriken i pivottabellen ska ha stilen tillämpad.

**Returns:**
boolean
### getShowPivotStyleRowStripes() {#getShowPivotStyleRowStripes--}
```
public boolean getShowPivotStyleRowStripes()
```


Anger om radränderformatering tillämpas.

**Returns:**
boolean
### getShowRowGrandTotals() {#getShowRowGrandTotals--}
```
public boolean getShowRowGrandTotals()
```


Anger om sammanlagda totaler för raderna i pivottabellen ska visas.

**Remarks**

**Returns:**
boolean
### getShowRowHeaderCaption() {#getShowRowHeaderCaption--}
```
public boolean getShowRowHeaderCaption()
```


Anger om radrubrikens rubrik visas i pivottabellrapporten Anger om fältetiketter och filterrullgardiner visas.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället PivotTable.ShowHeaders‑egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med april 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
boolean
### getShowValuesRow() {#getShowValuesRow--}
```
public boolean getShowValuesRow()
```


Anger om värderad rad visas.

**Returns:**
boolean
### getSource() {#getSource--}
```
public String[] getSource()
```


Hämta datakällan för denna pivottabell.

**Returns:**
java.lang.String[]
### getSource(boolean isOriginal) {#getSource-boolean-}
```
public String[] getSource(boolean isOriginal)
```


Hämta datakällan för denna pivottabell.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isOriginal | boolean | Anger om original‑ eller visningsdatakällan ska returneras. |

**Returns:**
java.lang.String[] -
### getSourceDataConnections() {#getSourceDataConnections--}
```
public ExternalConnection[] getSourceDataConnections()
```


Hämtar de externa anslutningsdatakällorna.

**Returns:**
com.aspose.cells.ExternalConnection[]
### getSourceType() {#getSourceType--}
```
public byte getSourceType()
```


Hämtar datakälltyp för pivottabellen.

Se [PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype).

**Returns:**
byte
### getSubtotalHiddenPageItems() {#getSubtotalHiddenPageItems--}
```
public boolean getSubtotalHiddenPageItems()
```


Indikerar om dolda sidfältsposter i PivotTable-rapporten inkluderas i rad- och kolumnsubtotaler, blocktotaler och totaler. Standardvärdet är False.

**Returns:**
boolean
### getTableRange1() {#getTableRange1--}
```
public CellArea getTableRange1()
```


Returnerar ett CellArea-objekt som representerar området som innehåller hela PivotTable-rapporten, men inkluderar inte sidfält. Skrivskyddad.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getTableRange2() {#getTableRange2--}
```
public CellArea getTableRange2()
```


Returnerar ett CellArea-objekt som representerar området som innehåller hela PivotTable-rapporten, inkluderar sidfält. Skrivskyddad.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getTag() {#getTag--}
```
public String getTag()
```


Hämtar en användardefinierad sträng som är associerad med denna pivottabellsvy.

**Returns:**
java.lang.String
### getTopRightArea() {#getTopRightArea--}
```
public CellArea getTopRightArea()
```


Representerar det tomma området högst upp till höger i pivottabellen (uppe till vänster för RTL-ark).

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getValuesField() {#getValuesField--}
```
public PivotField getValuesField()
```


Hämtar ett [PivotField](../../com.aspose.cells/pivotfield)-objekt som representerar alla datafält i en PivotTable. Endast läs. Det skapas endast när det finns två eller fler datafält i datatområdet. Som standard är det i radområdet. Du kan dra det till rad‑/kolumnområdet med metoden PivotTable.AddFieldToArea().

**Returns:**
[PivotField](../../com.aspose.cells/pivotfield)
### hasBlankRows() {#hasBlankRows--}
```
public boolean hasBlankRows()
```


Indikerar om tomma rader ska läggas till. Denna egenskap gäller endast för PivotTable‑autoformattyper som behöver lägga till tomma rader.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd i stället egenskapen PivotField.InsertBlankRow. Denna metod kommer att tas bort 12 månader senare från och med april 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoFormat() {#isAutoFormat--}
```
public boolean isAutoFormat()
```


Indikerar om PivotTable‑rapporten är automatiskt formaterad. Kryssrutan \"autoformat table\" som finns i pivottable‑alternativet för Excel 2003

**Returns:**
boolean
### isExcel2003Compatible() {#isExcel2003Compatible--}
```
public boolean isExcel2003Compatible()
```


Anger om PivotTable är kompatibel med Excel2003 vid uppdatering av PivotTable; om true måste en sträng vara högst 255 tecken, så om strängen är längre än 255 tecken kommer den att trunkeras. Om false har en sträng ingen sådan begränsning. Standardvärdet är true.

**Returns:**
boolean
### isGridDropZones() {#isGridDropZones--}
```
public boolean isGridDropZones()
```


Indikerar om PivotTable‑rapporten visar klassisk pivottable‑layout. (möjliggör dragning av fält i rutnätet)

**Returns:**
boolean
### isMultipleFieldFilters() {#isMultipleFieldFilters--}
```
public boolean isMultipleFieldFilters()
```


Anger ett booleskt värde som indikerar om fälten i en pivottabell kan ha flera filter inställda på dem.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd i stället egenskapen PivotTable.AllowMultipleFiltersPerField. Denna metod kommer att tas bort 12 månader senare från och med december 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
boolean
### isSelected() {#isSelected--}
```
public boolean isSelected()
```


Anger om denna pivottabell är markerad.

**Returns:**
boolean
### move(int row, int column) {#move-int-int-}
```
public void move(int row, int column)
```


Flyttar pivottabellen till en annan plats i kalkylbladet.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd i stället metoden PivotTable.MoveTo(). Denna metod kommer att tas bort 12 månader senare från och med december 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | radindex. |
| kolumn | int | kolumnindex. |

### move(String destCellName) {#move-java.lang.String-}
```
public void move(String destCellName)
```


Flyttar pivottabellen till en annan plats i kalkylbladet.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd i stället metoden PivotTable.MoveTo(). Denna metod kommer att tas bort 12 månader senare från och med december 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| destCellName | java.lang.String | destinationscellens namn. |

### moveItem(int region, String[] nodes, boolean absolute, int offset) {#moveItem-int-java.lang.String---boolean-int-}
```
public void moveItem(int region, String[] nodes, boolean absolute, int offset)
```


Flytta ett objekt upp eller ner.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| region | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Regionen. Endast för rad eller kolumn. |
| noder | java.lang.String[] | Objektet. |
| absolut | boolean | Indikerar om förskjutning är en absolut position. |
| förskjutning | int | Om absolut är true: 0 flyttar till början, -1 flyttar till slutet, andra betyder absolut position; annars är förskjutning en relativ position. |

### moveTo(int row, int column) {#moveTo-int-int-}
```
public void moveTo(int row, int column)
```


Flyttar pivottabellen till en annan plats i kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | radindex. |
| kolumn | int | kolumnindex. |

### moveTo(int sheetIndex, int row, int column) {#moveTo-int-int-int-}
```
public void moveTo(int sheetIndex, int row, int column)
```


Flyttar pivottabellen till en annan plats i kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetIndex | int | indexet för målarbetsbladet |
| rad | int | radindex. |
| kolumn | int | kolumnindex. |

### moveTo(String destCellName) {#moveTo-java.lang.String-}
```
public void moveTo(String destCellName)
```


Flyttar pivottabellen till en annan plats i kalkylbladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| destCellName | java.lang.String | destinationscellens namn. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refresh() {#refresh--}
```
public int refresh()
```


Uppdatera [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) från datakällan och beräkna data och stil för pivotsyn.

**Remarks**

Alla pivottabeller som beror på samma PivotCache kommer att beräknas om.

**Returns:**
int - [PivotRefreshState](../../com.aspose.cells/pivotrefreshstate).
### refresh(PivotTableRefreshOption option) {#refresh-com.aspose.cells.PivotTableRefreshOption-}
```
public int refresh(PivotTableRefreshOption option)
```


Uppdatera [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) från datakällan och beräkna data och stil för pivotsyn.

**Remarks**

Alla pivottabeller som beror på samma PivotCache kommer att beräknas om.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) |  |

**Returns:**
int - [PivotRefreshState](../../com.aspose.cells/pivotrefreshstate).
### refreshData() {#refreshData--}
```
public int refreshData()
```


Uppdaterar data från dess datakälla till pivottcachen.

**Remarks**

Vi kommer att samla data från datakällan till en pivottcache, sedan beräkna data i cachen till cellerna. Och det är bättre att du helt enkelt kan anropa [Workbook.refreshAll()](../../com.aspose.cells/workbook\#refreshAll--) för att uppdatera och beräkna alla pivottabeller i filen, istället för att uppdatera en efter en. OBS: Denna metod är nu föråldrad. Använd i stället metoden [PivotCache.refresh()](../../com.aspose.cells/pivotcache\#refresh--) och ta bort den efterföljande [calculateData()](../../com.aspose.cells/pivottable\#calculateData--) eftersom denna pivottabell kommer att beräknas när [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) uppdateras. Denna metod kommer att tas bort 12 månader senare från och med juni 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### refreshData(PivotTableRefreshOption option) {#refreshData-com.aspose.cells.PivotTableRefreshOption-}
```
public int refreshData(PivotTableRefreshOption option)
```


Uppdaterar pivottabellens data och inställningar från dess datakälla med alternativ.

**Remarks**

Vi kommer att samla data från datakällan till en pivottcache, sedan beräkna datan i cachen till cellerna. Och det är bättre att du enkelt kan anropa [Workbook.refreshAll()](../../com.aspose.cells/workbook\\#refreshAll--) för att uppdatera och beräkna alla pivottabeller i filen, inte att uppdatera en efter en. OBS: Denna metod är nu föråldrad. Använd i stället [PivotCache.refresh()](../../com.aspose.cells/pivotcache\\#refresh--) metoden och ta bort den efterföljande [calculateData()](../../com.aspose.cells/pivottable\\#calculateData--) eftersom denna pivottabell kommer att beräknas när du uppdaterar [getPivotCache()](../../com.aspose.cells/pivottable\\#getPivotCache--). Denna metod kommer att tas bort 12 månader senare sedan juni 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) | Alternativen för att uppdatera datakällan för pivottabellen. |

**Returns:**
int
### removeField(int fieldType, PivotField pivotField) {#removeField-int-com.aspose.cells.PivotField-}
```
public void removeField(int fieldType, PivotField pivotField)
```


Ta bort fält från specifikt fältområde

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). fältområdestypen. |
| pivotField | [PivotField](../../com.aspose.cells/pivotfield) | fältet i basfälten. |

### removeField(int fieldType, int baseFieldIndex) {#removeField-int-int-}
```
public void removeField(int fieldType, int baseFieldIndex)
```


Tar bort ett fält från ett specifikt pivottabellområde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Fältområdestypen. |
| baseFieldIndex | int | Fältindexet i basfälten. |

### removeField(int fieldType, String fieldName) {#removeField-int-java.lang.String-}
```
public void removeField(int fieldType, String fieldName)
```


Tar bort ett fält från specifikt fältområde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Fältområdestypen. |
| fieldName | java.lang.String | Namnet i basfälten. |

### selectArea(CellArea ca) {#selectArea-com.aspose.cells.CellArea-}
```
public PivotAreaCollection selectArea(CellArea ca)
```


Välj ett område i pivottabellvyn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Cellområdet. |

**Returns:**
[PivotAreaCollection](../../com.aspose.cells/pivotareacollection) - 
### setAllowMultipleFiltersPerField(boolean value) {#setAllowMultipleFiltersPerField-boolean-}
```
public void setAllowMultipleFiltersPerField(boolean value)
```


Anger ett booleskt värde som indikerar om fälten i en pivottabell kan ha flera filter inställda på dem.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAltTextDescription(String value) {#setAltTextDescription-java.lang.String-}
```
public void setAltTextDescription(String value)
```


Hämtar beskrivningen av alternativtexten.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setAltTextTitle(String value) {#setAltTextTitle-java.lang.String-}
```
public void setAltTextTitle(String value)
```


Ställer in titeln för alternativ text.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setAutoFormat(boolean value) {#setAutoFormat-boolean-}
```
public void setAutoFormat(boolean value)
```


Indikerar om PivotTable‑rapporten är automatiskt formaterad. Kryssrutan \"autoformat table\" som finns i pivottable‑alternativet för Excel 2003

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAutoFormatType(int value) {#setAutoFormatType-int-}
```
public void setAutoFormatType(int value)
```


Ställer in den automatiska formateringstypen för pivottabellen.

Se [PivotTableAutoFormatType](../../com.aspose.cells/pivottableautoformattype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setAutofitColumnWidthOnUpdate(boolean value) {#setAutofitColumnWidthOnUpdate-boolean-}
```
public void setAutofitColumnWidthOnUpdate(boolean value)
```


Anger om kolumnbredden ska anpassas automatiskt vid uppdatering

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setColumnGrand(boolean value) {#setColumnGrand-boolean-}
```
public void setColumnGrand(boolean value)
```


Anger om pivottabellsrapporten visar totalsummor för kolumner.

**Remarks**

OBS: Den här egenskapen är nu föråldrad. Använd i stället PivotTable.ShowColumnGrandTotals‑metoden. Denna metod kommer att tas bort 12 månader senare från och med december 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setColumnHeaderCaption(String value) {#setColumnHeaderCaption-java.lang.String-}
```
public void setColumnHeaderCaption(String value)
```


Ställer in den anpassade rubriken för kolumnhuvudet i pivottabellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setCustomListSort(boolean value) {#setCustomListSort-boolean-}
```
public void setCustomListSort(boolean value)
```


Anger om inbyggda anpassade listor ska beaktas vid sortering av data.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setDataFieldHeaderName(String value) {#setDataFieldHeaderName-java.lang.String-}
```
public void setDataFieldHeaderName(String value)
```


Ställer in namnet på värdeområdets fälthuvud i pivottabellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setDataSource(String[] value) {#setDataSource-java.lang.String---}
```
public void setDataSource(String[] value)
```


Ställer in datakällan för pivottabellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String[] |  |

### setDisplayErrorString(boolean value) {#setDisplayErrorString-boolean-}
```
public void setDisplayErrorString(boolean value)
```


Anger om PivotTable-rapporten visar en anpassad sträng i celler som innehåller fel.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setDisplayImmediateItems(boolean value) {#setDisplayImmediateItems-boolean-}
```
public void setDisplayImmediateItems(boolean value)
```


Anger om objekt i rad- och kolumnområdena är synliga när dataområdet i pivottabellen är tomt. Standardvärdet är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setDisplayNullString(boolean value) {#setDisplayNullString-boolean-}
```
public void setDisplayNullString(boolean value)
```


Anger om PivotTable-rapporten visar en anpassad sträng om värdet är null.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEnableDataValueEditing(boolean value) {#setEnableDataValueEditing-boolean-}
```
public void setEnableDataValueEditing(boolean value)
```


Anger ett booleskt värde som visar om användaren får redigera cellerna i dataområdet i pivottabellen. Standardvärdet är false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEnableDrilldown(boolean value) {#setEnableDrilldown-boolean-}
```
public void setEnableDrilldown(boolean value)
```


Anger om drilldown är aktiverat.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEnableFieldDialog(boolean value) {#setEnableFieldDialog-boolean-}
```
public void setEnableFieldDialog(boolean value)
```


Anger om dialogrutan PivotTable Field är tillgänglig när användaren dubbelklickar på PivotTable-fältet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEnableFieldList(boolean value) {#setEnableFieldList-boolean-}
```
public void setEnableFieldList(boolean value)
```


Anger om fältlistan för PivotTable är tillgänglig i Excel-vyn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEnableWizard(boolean value) {#setEnableWizard-boolean-}
```
public void setEnableWizard(boolean value)
```


Anger om PivotTable-guiden är tillgänglig.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setErrorString(String value) {#setErrorString-java.lang.String-}
```
public void setErrorString(String value)
```


Hämtar strängen som visas i celler som innehåller fel när egenskapen DisplayErrorString är sann. Standardvärdet är en tom sträng.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setExcel2003Compatible(boolean value) {#setExcel2003Compatible-boolean-}
```
public void setExcel2003Compatible(boolean value)
```


Anger om PivotTable är kompatibel med Excel2003 vid uppdatering av PivotTable; om true måste en sträng vara högst 255 tecken, så om strängen är längre än 255 tecken kommer den att trunkeras. Om false har en sträng ingen sådan begränsning. Standardvärdet är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setFieldListSortAscending(boolean value) {#setFieldListSortAscending-boolean-}
```
public void setFieldListSortAscending(boolean value)
```


Anger om fält i PivotTable är sorterade i icke‑standardordning i fältlistan.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setGrandTotalName(String value) {#setGrandTotalName-java.lang.String-}
```
public void setGrandTotalName(String value)
```


Returnerar etiketten som visas i rubriken för totalkolumnen eller -raden. Standardvärdet är strängen "Grand Total".

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setGridDropZones(boolean value) {#setGridDropZones-boolean-}
```
public void setGridDropZones(boolean value)
```


Indikerar om PivotTable‑rapporten visar klassisk pivottable‑layout. (möjliggör dragning av fält i rutnätet)

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHasBlankRows(boolean value) {#setHasBlankRows-boolean-}
```
public void setHasBlankRows(boolean value)
```


Indikerar om tomma rader ska läggas till. Denna egenskap gäller endast för PivotTable‑autoformattyper som behöver lägga till tomma rader.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd i stället egenskapen PivotField.InsertBlankRow. Denna metod kommer att tas bort 12 månader senare från och med april 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setIndent(int value) {#setIndent-int-}
```
public void setIndent(int value)
```


Specificerar indenteringsökningen för kompakt axel och kan användas för att ställa in rapportlayouten till kompakt form.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setItemPrintTitles(boolean value) {#setItemPrintTitles-boolean-}
```
public void setItemPrintTitles(boolean value)
```


Anger om PivotItem-namn ska upprepas högst upp på varje utskriven sida.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället PivotTable.RepeatItemsOnEachPrintedPage‑egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med oktober 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setManualUpdate(boolean value) {#setManualUpdate-boolean-}
```
public void setManualUpdate(boolean value)
```


Anger om PivotTable-rapporten endast beräknas om användaren begär det.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setMergeLabels(boolean value) {#setMergeLabels-boolean-}
```
public void setMergeLabels(boolean value)
```


Anger om rad-/kolumnfältetiketter som sträcker sig över flera celler ska slås ihop.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setMissingItemsLimit(int value) {#setMissingItemsLimit-int-}
```
public void setMissingItemsLimit(int value)
```


Anger ett booleskt värde som indikerar om fälten i en pivottabell kan ha flera filter inställda på dem.

Se [PivotMissingItemLimitType](../../com.aspose.cells/pivotmissingitemlimittype).

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället PivotCache.MissingItemsLimit‑egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setMultipleFieldFilters(boolean value) {#setMultipleFieldFilters-boolean-}
```
public void setMultipleFieldFilters(boolean value)
```


Anger ett booleskt värde som indikerar om fälten i en pivottabell kan ha flera filter inställda på dem.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd i stället egenskapen PivotTable.AllowMultipleFiltersPerField. Denna metod kommer att tas bort 12 månader senare från och med december 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Hämtar namnet på PivotTable.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setNullString(String value) {#setNullString-java.lang.String-}
```
public void setNullString(String value)
```


Hämtar strängen som visas i celler som innehåller null‑värden när egenskapen DisplayNullString är sann. Standardvärdet är en tom sträng.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setPageFieldOrder(int value) {#setPageFieldOrder-int-}
```
public void setPageFieldOrder(int value)
```


Anger den ordning i vilken sidfält läggs till i pivottabellrapportens layout.

Se [PrintOrderType](../../com.aspose.cells/printordertype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setPageFieldWrapCount(int value) {#setPageFieldWrapCount-int-}
```
public void setPageFieldWrapCount(int value)
```


Hämtar antalet sidfält i varje kolumn eller rad i PivotTable‑rapporten.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setPivotTableStyle(TableStyle value) {#setPivotTableStyle-com.aspose.cells.TableStyle-}
```
public void setPivotTableStyle(TableStyle value)
```


Hämtar [TableStyle](../../com.aspose.cells/tablestyle)-inställningarna för denna pivottabell.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [TableStyle](../../com.aspose.cells/tablestyle) |  |

### setPivotTableStyleName(String value) {#setPivotTableStyleName-java.lang.String-}
```
public void setPivotTableStyleName(String value)
```


Ställer in stilnamnet för pivottabellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setPivotTableStyleType(int value) {#setPivotTableStyleType-int-}
```
public void setPivotTableStyleType(int value)
```


Ställer in den inbyggda pivottabellstilen.

Se [PivotTableStyleType](../../com.aspose.cells/pivottablestyletype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setPreserveCellFormattingOnUpdate(boolean value) {#setPreserveCellFormattingOnUpdate-boolean-}
```
public void setPreserveCellFormattingOnUpdate(boolean value)
```


Anger om cellformatering ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) ska bevaras när pivottabellen uppdateras eller beräknas om.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setPreserveFormatting(boolean value) {#setPreserveFormatting-boolean-}
```
public void setPreserveFormatting(boolean value)
```


Anger om cellformatering ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) bevaras när pivottabellen uppdateras eller beräknas om.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället PivotTable.PreserveCellFormattingOnUpdate‑egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med juli 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setPrintDrill(boolean value) {#setPrintDrill-boolean-}
```
public void setPrintDrill(boolean value)
```


Anger ett booleskt värde som visar om drill‑indikatorer ska skrivas ut. Skriv ut expandera/kollapsa‑knappar när de visas i pivottabellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setPrintTitles(boolean value) {#setPrintTitles-boolean-}
```
public void setPrintTitles(boolean value)
```


Anger om utskriftstitlarna för kalkylbladet sätts baserat på pivottabellrapporten. Standardvärdet är false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setRefreshDataOnOpeningFile(boolean value) {#setRefreshDataOnOpeningFile-boolean-}
```
public void setRefreshDataOnOpeningFile(boolean value)
```


Anger om data ska uppdateras när filen öppnas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setRepeatItemsOnEachPrintedPage(boolean value) {#setRepeatItemsOnEachPrintedPage-boolean-}
```
public void setRepeatItemsOnEachPrintedPage(boolean value)
```


Anger om rubriker för pivot‑objekt i radområdet upprepas på varje utskriven sida för pivottfält i tabellform.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setRowGrand(boolean value) {#setRowGrand-boolean-}
```
public void setRowGrand(boolean value)
```


Anger om totalsummor för rader i denna pivottabell ska visas.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället PivotTable.ShowRowGrandTotals‑metoden. Denna metod kommer att tas bort 12 månader senare från och med december 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setRowHeaderCaption(String value) {#setRowHeaderCaption-java.lang.String-}
```
public void setRowHeaderCaption(String value)
```


Ställer in anpassad rubrik för radhuvudet i denna pivottabell.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setSaveData(boolean value) {#setSaveData-boolean-}
```
public void setSaveData(boolean value)
```


Anger om data för PivotTable-rapporten sparas med arbetsboken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSelected(boolean value) {#setSelected-boolean-}
```
public void setSelected(boolean value)
```


Anger om denna pivottabell är markerad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowColumnGrandTotals(boolean value) {#setShowColumnGrandTotals-boolean-}
```
public void setShowColumnGrandTotals(boolean value)
```


Anger om sammanlagda totaler för kolumnerna i denna pivottabell ska visas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowDataTips(boolean value) {#setShowDataTips-boolean-}
```
public void setShowDataTips(boolean value)
```


Anger om verktygstips ska visas för pivottabellens dataceller.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowDrill(boolean value) {#setShowDrill-boolean-}
```
public void setShowDrill(boolean value)
```


Anger om expandera-/kollapsa-knappar ska visas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowEmptyCol(boolean value) {#setShowEmptyCol-boolean-}
```
public void setShowEmptyCol(boolean value)
```


Anger om tomma kolumner ska inkluderas i tabellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowEmptyRow(boolean value) {#setShowEmptyRow-boolean-}
```
public void setShowEmptyRow(boolean value)
```


Anger om tomma rader ska inkluderas i tabellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowHeaders(boolean value) {#setShowHeaders-boolean-}
```
public void setShowHeaders(boolean value)
```


Om datafältetiketter och pivottfältetiketter ska visas på radaxeln och kolumnaxeln i pivottabellsvyn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowMemberPropertyTips(boolean value) {#setShowMemberPropertyTips-boolean-}
```
public void setShowMemberPropertyTips(boolean value)
```


Specificerar ett booleskt värde som anger om medlemsegenskapsinformation ska utelämnas från pivottabellens verktygstips.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowPivotStyleColumnHeader(boolean value) {#setShowPivotStyleColumnHeader-boolean-}
```
public void setShowPivotStyleColumnHeader(boolean value)
```


Anger om kolumnrubriken i pivottabellen ska ha stilen tillämpad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowPivotStyleColumnStripes(boolean value) {#setShowPivotStyleColumnStripes-boolean-}
```
public void setShowPivotStyleColumnStripes(boolean value)
```


Anger om ränderformatering tillämpas för kolumnen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowPivotStyleLastColumn(boolean value) {#setShowPivotStyleLastColumn-boolean-}
```
public void setShowPivotStyleLastColumn(boolean value)
```


Anger om kolumnformatering har tillämpats.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowPivotStyleRowHeader(boolean value) {#setShowPivotStyleRowHeader-boolean-}
```
public void setShowPivotStyleRowHeader(boolean value)
```


Anger om radrubriken i pivottabellen ska ha stilen tillämpad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowPivotStyleRowStripes(boolean value) {#setShowPivotStyleRowStripes-boolean-}
```
public void setShowPivotStyleRowStripes(boolean value)
```


Anger om radränderformatering tillämpas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowRowGrandTotals(boolean value) {#setShowRowGrandTotals-boolean-}
```
public void setShowRowGrandTotals(boolean value)
```


Anger om sammanlagda totaler för raderna i pivottabellen ska visas.

**Remarks**

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowRowHeaderCaption(boolean value) {#setShowRowHeaderCaption-boolean-}
```
public void setShowRowHeaderCaption(boolean value)
```


Anger om radrubrikens rubrik visas i pivottabellrapporten Anger om fältetiketter och filterrullgardiner visas.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället PivotTable.ShowHeaders‑egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med april 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowValuesRow(boolean value) {#setShowValuesRow-boolean-}
```
public void setShowValuesRow(boolean value)
```


Anger om värderad rad visas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSubtotalHiddenPageItems(boolean value) {#setSubtotalHiddenPageItems-boolean-}
```
public void setSubtotalHiddenPageItems(boolean value)
```


Indikerar om dolda sidfältsposter i PivotTable-rapporten inkluderas i rad- och kolumnsubtotaler, blocktotaler och totaler. Standardvärdet är False.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setTag(String value) {#setTag-java.lang.String-}
```
public void setTag(String value)
```


Ställer in en användardefinierad sträng som är associerad med denna pivottabellvy.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### showDetail(int rowOffset, int columnOffset, boolean newSheet, int destRow, int destColumn) {#showDetail-int-int-boolean-int-int-}
```
public void showDetail(int rowOffset, int columnOffset, boolean newSheet, int destRow, int destColumn)
```


Visa detaljerna för ett objekt i dataområdet i en ny tabell.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowOffset | int | Offset till den första dataraden i dataområdet. |
| columnOffset | int | Offset till den första datakolumnen i dataområdet. |
| newSheet | boolean | Visa detaljen i ett nytt kalkylblad. |
| destRow | int | Målraden. |
| destColumn | int | Målkolumnen. |

### showInCompactForm() {#showInCompactForm--}
```
public void showInCompactForm()
```


Formaterar PivotTable-vyn i kompakt form.

### showInOutlineForm() {#showInOutlineForm--}
```
public void showInOutlineForm()
```


Formaterar PivotTable i konturform.

### showInTabularForm() {#showInTabularForm--}
```
public void showInTabularForm()
```


Formaterar PivotTable i tabellform.

### showReportFilterPage(PivotField pageField) {#showReportFilterPage-com.aspose.cells.PivotField-}
```
public void showReportFilterPage(PivotField pageField)
```


Visa alla rapportsfilter‑sidor enligt PivotField, PivotField måste vara placerad i PageFields.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageField | [PivotField](../../com.aspose.cells/pivotfield) | PivotField-objektet |

### showReportFilterPageByIndex(int posIndex) {#showReportFilterPageByIndex-int-}
```
public void showReportFilterPageByIndex(int posIndex)
```


Visa alla rapportsfilter‑sidor enligt positionsindexet i PageFields.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| posIndex | int | Positionsindexet i PageFields |

### showReportFilterPageByName(String fieldName) {#showReportFilterPageByName-java.lang.String-}
```
public void showReportFilterPageByName(String fieldName)
```


Visa alla rapportsfilter‑sidor enligt PivotFields namn, PivotField måste vara placerad i PageFields.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldName | java.lang.String | Namnet på PivotField |

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

