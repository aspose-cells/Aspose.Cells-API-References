---
title: "Cell"
second_title: "Aspose.Cells för Java API-referens"
description: "Inkapslar objektet som representerar en enskild Workbook-cell."
type: docs
url: /sv/java/com.aspose.cells/cell/
---

**Inheritance:**
java.lang.Object
```
public class Cell
```

Inkapslar objektet som representerar en enskild Workbook-cell.

**Example**

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
 
         //Put a string into a cell
         Cell cell = cells.get(0, 0);
         cell.putValue("Hello");
 
         String first = cell.getStringValue();
 
         //Put an integer into a cell
         cell = cells.get("B1");
         cell.putValue(12);
 
         int second = cell.getIntValue();
 
         //Put a double into a cell
         cell = cells.get(0, 2);
         cell.putValue(-1.234);
 
         double third = cell.getDoubleValue();
 
         //Put a formula into a cell
         cell = cells.get("D1");
         cell.setFormula("=B1 + C1");
 
         //Put a combined formula: "sum(average(b1,c1), b1)" to cell at b2
         cell = cells.get("b2");
         cell.setFormula("=sum(average(b1,c1), b1)");
 
         //Set style of a cell
         Style style = cell.getStyle();
         //Set background color
         style.setBackgroundColor(Color.getYellow());
         //Set format of a cell
         style.getFont().setName("Courier New");
         style.setVerticalAlignment(TextAlignmentType.TOP);
          cell.setStyle(style);
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [calculate(CalculationOptions options)](#calculate-com.aspose.cells.CalculationOptions-) | Beräknar cellens formel. |
| [characters(int startIndex, int length)](#characters-int-int-) | Returnerar ett Characters-objekt som representerar ett teckensegment inom cellens text. |
| [containsExternalLink()](#containsExternalLink--) | Anger om den här cellen innehåller en extern länk. |
| [copy(Cell cell)](#copy-com.aspose.cells.Cell-) | Kopierar data från en källcell. |
| [equals(Cell cell)](#equals-com.aspose.cells.Cell-) | Kontrollerar om detta objekt refererar till samma cell som ett annat cellobjekt. |
| [equals(Object obj)](#equals-java.lang.Object-) | Kontrollerar om detta objekt refererar till samma cell som ett annat. |
| [getArrayRange()](#getArrayRange--) | Hämtar array-intervallet om cellens formel är en arrayformel. |
| [getBoolValue()](#getBoolValue--) | Hämtar det booleska värdet som finns i cellen. |
| [getCharacters()](#getCharacters--) | Returnerar alla Characters-objekt som representerar ett teckensegment inom cellens text. |
| [getCharacters(boolean flag)](#getCharacters-boolean-) | Returnerar alla Characters-objekt som representerar ett teckensegment inom cellens text. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Hämtar kolumnnumret (nollbaserat) för cellen. |
| [getComment()](#getComment--) | Hämtar kommentaren för den här cellen. |
| [getConditionalFormattingResult()](#getConditionalFormattingResult--) | Hämta resultatet av den villkorliga formateringen. |
| [getDateTimeValue()](#getDateTimeValue--) | Hämtar DateTime‑värdet som finns i cellen. |
| [getDependents(boolean isAll)](#getDependents-boolean-) | Hämta alla celler vars formel refererar direkt till den här cellen. |
| [getDependentsInCalculation(boolean recursive)](#getDependentsInCalculation-boolean-) | Hämtar alla celler vars beräknade resultat beror på den här cellen. |
| [getDisplayStringValue()](#getDisplayStringValue--) | Hämtar det formaterade strängvärdet för den här cellen enligt cellens visningsstil. |
| [getDisplayStyle()](#getDisplayStyle--) | Hämtar cellens visningsstil. |
| [getDisplayStyle(boolean includeMergedBorders)](#getDisplayStyle-boolean-) | Hämtar cellens visningsstil. |
| [getDisplayStyle(int adjacentBorders)](#getDisplayStyle-int-) | Hämtar cellens visningsstil. |
| [getDoubleValue()](#getDoubleValue--) | Hämtar det dubbelvärde som finns i cellen. |
| [getEmbeddedImage()](#getEmbeddedImage--) | Hämtar den inbäddade bilden i cellen. |
| [getFloatValue()](#getFloatValue--) | Hämtar flyttalsvärdet som finns i cellen. |
| [getFormatConditions()](#getFormatConditions--) | Hämtar formatvillkor som gäller för den här cellen. |
| [getFormula()](#getFormula--) | Hämtar en formel för [Cell](../../com.aspose.cells/cell). |
| [getFormula(boolean isR1C1, boolean isLocal)](#getFormula-boolean-boolean-) | Hämta formeln för den här cellen. |
| [getFormulaLocal()](#getFormulaLocal--) | Hämta den lokaliserade formaterade formeln för cellen. |
| [getHeightOfValue()](#getHeightOfValue--) | Hämtar höjden på värdet i enheten pixlar. |
| [getHtmlString()](#getHtmlString--) | Hämtar HTML-strängen som innehåller data och vissa format i den här cellen. |
| [getHtmlString(boolean html5)](#getHtmlString-boolean-) | Hämtar HTML-strängen som innehåller data och vissa format i den här cellen. |
| [getIntValue()](#getIntValue--) | Hämtar heltalsvärdet som finns i cellen. |
| [getLeafs()](#getLeafs--) | Hämta alla celler som refererar till den här cellen direkt och som behöver uppdateras när den här cellen ändras. |
| [getLeafs(boolean recursive)](#getLeafs-boolean-) | Hämta alla celler som kommer att uppdateras när den här cellen ändras. |
| [getMergedRange()](#getMergedRange--) | Returnerar ett [Range](../../com.aspose.cells/range)-objekt som representerar ett sammanslaget område. |
| [getName()](#getName--) | Hämtar namnet på cellen. |
| [getNumberCategoryType()](#getNumberCategoryType--) | Representerar kategoritypen för den här cellens talformatering. |
| [getPicture()](#getPicture--) | Hämtar en [Picture](../../com.aspose.cells/picture)-instans som representerar den inbäddade bilden i den här cellen eller null om det inte finns någon inbäddad bild för den här cellen. |
| [getPrecedents()](#getPrecedents--) | Hämtar alla referenser som förekommer i den här cellens formel. |
| [getPrecedentsInCalculation()](#getPrecedentsInCalculation--) | Hämtar alla föregångare (referenser till celler i aktuell arbetsbok) som används av den här cellens formel vid beräkning. |
| [getR1C1Formula()](#getR1C1Formula--) | Hämtar en R1C1-formel för [Cell](../../com.aspose.cells/cell). |
| [getRichValue()](#getRichValue--) | Hämtar det rika värdet för cellen. |
| [getRow()](#getRow--) | Hämtar radnumret (nollbaserat) för cellen. |
| [getSharedStyleIndex()](#getSharedStyleIndex--) | Hämtar cellens delade stilindex i stilpoolen. |
| [getStringValue()](#getStringValue--) | Hämtar strängvärdet som finns i cellen. |
| [getStringValue(int formatStrategy)](#getStringValue-int-) | Hämtar strängvärdet enligt en specifik formateringsstrategi. |
| [getStringValueWithoutFormat()](#getStringValueWithoutFormat--) | Hämtar cellens värde som sträng utan någon formatering. |
| [getStyle()](#getStyle--) | Hämtar cellstilen. |
| [getStyle(boolean checkBorders)](#getStyle-boolean-) | Om checkBorders är true, kontrollera om andra cellers kanter kommer att påverka stilen för den här cellen. |
| [getTable()](#getTable--) | Hämtar tabellen som innehåller den här cellen. |
| [getType()](#getType--) | Representerar cellvärdestyp. |
| [getValidation()](#getValidation--) | Hämtar valideringen som tillämpas på den här cellen. |
| [getValidationValue()](#getValidationValue--) | Hämtar värdet för valideringen som tillämpas på den här cellen. |
| [getValue()](#getValue--) | Hämtar värdet som finns i den här cellen. |
| [getWidthOfValue()](#getWidthOfValue--) | Hämtar bredden på värdet i enheten pixlar. |
| [getWorksheet()](#getWorksheet--) | Hämtar det överordnade kalkylbladet. |
| [hasCustomFunction()](#hasCustomFunction--) | Kontrollerar om det finns en anpassad funktion (ej stödd funktion) i den här cellens formel. |
| [hasCustomStyle()](#hasCustomStyle--) | Anger om den här cellen har anpassade stilinställningar (annorlunda än standardinställningen som ärvs från motsvarande rad, kolumn eller arbetsbok). |
| [hashCode()](#hashCode--) | Fungerar som en hash-funktion för en specifik typ. |
| [insertText(int index, String text)](#insertText-int-java.lang.String-) | Infoga några tecken i cellen. |
| [isArrayFormula()](#isArrayFormula--) | Anger om cellens formel är en matrisformel. |
| [isArrayHeader()](#isArrayHeader--) | Anger att cellens formel är en matrisformel och att den är den första cellen i matrisen. |
| [isCheckBoxStyle()](#isCheckBoxStyle--) | Anger om den här cellen är inställd som en kryssruta. |
| [isDynamicArrayFormula()](#isDynamicArrayFormula--) | Anger om cellens formel är en dynamisk matrisformel (true) eller en äldre matrisformel (false). |
| [isErrorValue()](#isErrorValue--) | Kontrollerar om värdet i den här cellen är ett fel. |
| [isFormula()](#isFormula--) | Representerar om den angivna cellen innehåller en formel. |
| [isInArray()](#isInArray--) | Anger om cellens formel är en matrisformel. |
| [isInTable()](#isInTable--) | Anger om den här cellen är en del av en tabellformel. |
| [isMerged()](#isMerged--) | Kontrollerar om en cell är en del av ett sammanslaget område eller inte. |
| [isNumericValue()](#isNumericValue--) | Anger om värdet i den här cellen är numeriskt (int, double och datetime). |
| [isRichText()](#isRichText--) | Anger om strängvärdet i den här cellen är rik formaterad text. |
| [isSharedFormula()](#isSharedFormula--) | Anger om cellens formel är en del av en delad formel. |
| [isStyleSet()](#isStyleSet--) | Anger om cellens stil är inställd. |
| [isTableFormula()](#isTableFormula--) | Anger om den här cellen är en del av en tabellformel. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(boolean boolValue)](#putValue-boolean-) | Sätter ett booleskt värde i cellen. |
| [putValue(DateTime dateTime)](#putValue-com.aspose.cells.DateTime-) | Sätter ett DateTime‑värde i cellen. |
| [putValue(double doubleValue)](#putValue-double-) | Lägger in ett dubbelvärde i cellen. |
| [putValue(int intValue)](#putValue-int-) | Lägger in ett heltalsvärde i cellen. |
| [putValue(Object objectValue)](#putValue-java.lang.Object-) | Lägger in ett objektvärde i cellen. |
| [putValue(String stringValue)](#putValue-java.lang.String-) | Lägger in ett strängvärde i cellen. |
| [putValue(String stringValue, boolean isConverted)](#putValue-java.lang.String-boolean-) | Lägger in ett strängvärde i cellen och konverterar värdet till en annan datatyp om det är lämpligt. |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | Lägger in ett värde i cellen, om det är lämpligt konverteras värdet till en annan datatyp och cellens talformat återställs. |
| [removeArrayFormula(boolean leaveNormalFormula)](#removeArrayFormula-boolean-) | Ta bort matrisformel. |
| [replace(String placeHolder, String newValue, ReplaceOptions options)](#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-) | Ersätt cellens text med alternativ. |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber)](#setArrayFormula-java.lang.String-int-int-) | Ställer in en matrisformel (legacy-matrisformel som matas in via CTRL+SHIFT+ENTER i MS Excel) för ett cellområde. |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)](#setArrayFormula-java.lang.String-int-int-boolean-boolean-) | Ställer in en matrisformel för ett cellområde. |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options)](#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-) | Ställer in en matrisformel för ett cellområde. |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)](#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----) | Ställer in en matrisformel för ett cellområde. |
| [setCharacters(FontSetting[] characters)](#setCharacters-com.aspose.cells.FontSetting---) | Ställer in rik textformat för cellen. |
| [setCheckBoxStyle(boolean value)](#setCheckBoxStyle-boolean-) | Anger om den här cellen är inställd som en kryssruta. |
| [setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, boolean calculateValue)](#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-boolean-) | Ställer in dynamisk matrisformel och låter formeln spilla över till angränsande celler om möjligt. |
| [setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue)](#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-) | Ställer in dynamisk matrisformel och låter formeln spilla över till angränsande celler om möjligt. |
| [setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue, CalculationOptions copts)](#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-com.aspose.cells.CalculationOptions-) | Ställer in dynamisk matrisformel och låter formeln spilla över till angränsande celler om möjligt. |
| [setEmbeddedImage(byte[] value)](#setEmbeddedImage-byte---) | Ställer in den inbäddade bilden i cellen. |
| [setFormula(String value)](#setFormula-java.lang.String-) | Ställer in en formel för [Cell](../../com.aspose.cells/cell). |
| [setFormula(String formula, boolean isR1C1, boolean isLocal, Object value)](#setFormula-java.lang.String-boolean-boolean-java.lang.Object-) | Ställ in formeln och formelns värde. |
| [setFormula(String formula, FormulaParseOptions options)](#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-) | Ställ in formeln och värdet (beräknat resultat) för formeln. |
| [setFormula(String formula, FormulaParseOptions options, Object value)](#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-) | Ställ in formeln och värdet (beräknat resultat) för formeln. |
| [setFormula(String formula, Object value)](#setFormula-java.lang.String-java.lang.Object-) | Ställ in formeln och värdet (beräknat resultat) för formeln. |
| [setFormulaLocal(String value)](#setFormulaLocal-java.lang.String-) | Hämta den lokaliserade formaterade formeln för cellen. |
| [setHtmlString(String value)](#setHtmlString-java.lang.String-) | Ställer in HTML-strängen som innehåller data och vissa format i den här cellen. |
| [setR1C1Formula(String value)](#setR1C1Formula-java.lang.String-) | Ställer in en R1C1-formel för [Cell](../../com.aspose.cells/cell). |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber)](#setSharedFormula-java.lang.String-int-int-) | Ställer in delade formler för ett cellområde. |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)](#setSharedFormula-java.lang.String-int-int-boolean-boolean-) | Ställer in en formel för ett cellområde. |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options)](#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-) | Ställer in delade formler för ett cellområde. |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)](#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----) | Ställer in delade formler för ett cellområde. |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Ställer in cellstilen. |
| [setStyle(Style style, boolean explicitFlag)](#setStyle-com.aspose.cells.Style-boolean-) | Tillämpa den ändrade egenskapen för stilen på cellen. |
| [setStyle(Style style, StyleFlag flag)](#setStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Tillämpa cellstilen baserat på flaggor. |
| [setTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, int columnIndexOfInputCell, boolean isRowInput, Object[][] values)](#setTableFormula-int-int-int-int-boolean-java.lang.Object-----) | Skapa en envariabels datatabell för det angivna området med början från den här cellen. |
| [setTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, Object[][] values)](#setTableFormula-int-int-int-int-int-int-java.lang.Object-----) | Skapa en tvåvariabels datatabell för det angivna området med början från den här cellen. |
| [setTableFormula(int rowNumber, int columnNumber, String inputCell, boolean isRowInput, Object[][] values)](#setTableFormula-int-int-java.lang.String-boolean-java.lang.Object-----) | Skapa en envariabels datatabell för det angivna området med början från den här cellen. |
| [setTableFormula(int rowNumber, int columnNumber, String rowInputCell, String columnInputCell, Object[][] values)](#setTableFormula-int-int-java.lang.String-java.lang.String-java.lang.Object-----) | Skapa en tvåvariabels datatabell för det angivna området med början från den här cellen. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Ställer in värdet som finns i den här cellen. |
| [toJson()](#toJson--) | Konvertera [Cell](../../com.aspose.cells/cell) till JSON‑strukturdata. |
| [toString()](#toString--) | Returnerar en sträng som representerar det aktuella Cell‑objektet. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### calculate(CalculationOptions options) {#calculate-com.aspose.cells.CalculationOptions-}
```
public void calculate(CalculationOptions options)
```


Beräknar cellens formel.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| options | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Alternativ för beräkning |

### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```


Returnerar ett Characters-objekt som representerar ett teckensegment inom cellens text.

**Remarks**

Denna metod fungerar endast på celler med strängvärde.

**Example**

```
         Workbook excel = new Workbook();
         	Cells cells = excel.getWorksheets().get(0).getCells();
         cells.get("A1").putValue("Helloworld");
         cells.get("A1").characters(5, 5).getFont().setBold(true);
         cells.get("A1").characters(5, 5).getFont().setColor(Color.getBlue());
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startIndex | int | Indexet för tecknets början. |
| length | int | Antalet tecken. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - Characters object.
### containsExternalLink() {#containsExternalLink--}
```
public boolean containsExternalLink()
```


Anger om den här cellen innehåller en extern länk. Gäller endast när cellen är en formelcell.

**Returns:**
boolean
### copy(Cell cell) {#copy-com.aspose.cells.Cell-}
```
public void copy(Cell cell)
```


Kopierar data från en källcell.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | Käll‑[Cell](../../com.aspose.cells/cell)‑objekt. |

### equals(Cell cell) {#equals-com.aspose.cells.Cell-}
```
public boolean equals(Cell cell)
```


Kontrollerar om detta objekt refererar till samma cell som ett annat cellobjekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | ett annat cellobjekt |

**Returns:**
boolesk – true om två cellobjekt refererar till samma cell.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Kontrollerar om detta objekt refererar till samma cell som ett annat.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | java.lang.Object | ett annat objekt |

**Returns:**
boolesk – true om två objekt refererar till samma cell.
### getArrayRange() {#getArrayRange--}
```
public CellArea getArrayRange()
```


Hämtar array-intervallet om cellens formel är en arrayformel.

**Remarks**

Gäller endast när cellens formel är en matrisformel

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - The array range.
### getBoolValue() {#getBoolValue--}
```
public boolean getBoolValue()
```


Hämtar det booleska värdet som finns i cellen.

**Returns:**
boolean
### getCharacters() {#getCharacters--}
```
public FontSetting[] getCharacters()
```


Returnerar alla Characters-objekt som representerar ett teckensegment inom cellens text.

**Returns:**
com.aspose.cells.FontSetting[] - Alla tecken‑objekt
### getCharacters(boolean flag) {#getCharacters-boolean-}
```
public FontSetting[] getCharacters(boolean flag)
```


Returnerar alla Characters-objekt som representerar ett teckensegment inom cellens text.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| flagga | boolean | Anger om tabellstil ska tillämpas på cellen när cellen är i tabellen. |

**Returns:**
com.aspose.cells.FontSetting[] - Alla tecken‑objekt
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumn() {#getColumn--}
```
public int getColumn()
```


Hämtar kolumnnumret (nollbaserat) för cellen.

**Returns:**
int
### getComment() {#getComment--}
```
public Comment getComment()
```


Hämtar kommentaren för den här cellen.

**Remarks**

Om det inte finns någon kommentar som gäller för cellen returneras null.

**Returns:**
[Comment](../../com.aspose.cells/comment)
### getConditionalFormattingResult() {#getConditionalFormattingResult--}
```
public ConditionalFormattingResult getConditionalFormattingResult()
```


Hämta resultatet av den villkorliga formateringen.

**Remarks**

Returnerar null om ingen villkorsstyrd formatering har tillämpats på den här cellen,

**Returns:**
[ConditionalFormattingResult](../../com.aspose.cells/conditionalformattingresult)
### getDateTimeValue() {#getDateTimeValue--}
```
public DateTime getDateTimeValue()
```


Hämtar DateTime‑värdet som finns i cellen.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getDependents(boolean isAll) {#getDependents-boolean-}
```
public Cell[] getDependents(boolean isAll)
```


Hämta alla celler vars formel refererar direkt till den här cellen.

**Remarks**

 *  If one reference containing this cell appears in one cell's formula, that cell will be taken as the dependent of this cell, no matter the reference or this cell is used or not while calculating. For example, although cell A2 in formula "=IF(TRUE,A1,A2)" is not used while calculating, this formula is still be taken as A2's dependent.
 *  To get those formulas whose calculated results depend on this cell, please use .
 *  When tracing dependents for one cell, all formulas in the workbook or worksheet will be analized and checked. So it is a time consumed process. If user need to trace dependents for lots of cells, using this method will cause poor performance. For performance consideration, user should use  instead. Or, user may gather precedents map of all cells by  firstly, and then build the dependents map according to the precedents map.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("A1").setFormula("=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2");
         cells.get("A2").setFormula("=IF(TRUE,B2,B1)");
         Cell[] dependents = cells.get("B1").getDependents(true);
         for (int i = 0; i <dependents.length; i++)
         {
              System.out.println(dependents[i].getName());
         }
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isAll | boolean | Anger om formler i andra arbetsblad ska kontrolleras |

**Returns:**
com.aspose.cells.Cell[]
### getDependentsInCalculation(boolean recursive) {#getDependentsInCalculation-boolean-}
```
public Iterator getDependentsInCalculation(boolean recursive)
```


Hämtar alla celler vars beräknade resultat beror på den här cellen.

**Remarks**

För att använda den här metoden, se till att arbetsboken har satts till true för [FormulaSettings.getEnableCalculationChain()](../../com.aspose.cells/formulasettings\#getEnableCalculationChain--) och har beräknats helt med den här inställningen. Om det inte finns någon formelreferens till den här cellen returneras null.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("A1").setFormula("=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2");
         cells.get("A2").setFormula("=IF(TRUE,B2,B1)");
         workbook.getSettings().getFormulaSettings().setEnableCalculationChain(true);
         workbook.calculateFormula();
         Iterator en = cells.get("B1").getDependentsInCalculation(false);
         System.out.println("B1's calculation dependents:");
         while(en.hasNext())
         {
             Cell c = (Cell)en.next();
             System.out.println(c.getName());
         }
         en = cells.get("B2").getDependentsInCalculation(false);
         System.out.println("B2's calculation dependents:");
         while(en.hasNext())
         {
             Cell c = (Cell)en.next();
             System.out.println(c.getName());
         }
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rekursiv | boolean | Anger om de beroenden som returneras inte refererar direkt till den här cellen utan refererar till andra löv för denna cell. |

**Returns:**
java.util.Iterator – Enumerator för att enumerera alla beroenden (Cell‑objekt)
### getDisplayStringValue() {#getDisplayStringValue--}
```
public String getDisplayStringValue()
```


Hämtar det formaterade strängvärdet för den här cellen enligt cellens visningsstil.

**Returns:**
java.lang.String
### getDisplayStyle() {#getDisplayStyle--}
```
public Style getDisplayStyle()
```


Hämtar cellens visningsstil.

**Remarks**

Samma som att använda [BorderType.SIDE\_BORDERS](../../com.aspose.cells/bordertype\#SIDE-BORDERS) för [getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-). Det vill säga, den här metoden kommer att kontrollera och justera övre/nedre/vänstra/högra kanter för denna cell enligt stilen ([getStyle()](../../com.aspose.cells/cell\#getStyle--)) för dess intilliggande celler, men kontrollerar inte sammanslagna celler och kontrollerar inte visningsstilen för intilliggande celler.

**Returns:**
[Style](../../com.aspose.cells/style) - display style of this cell
### getDisplayStyle(boolean includeMergedBorders) {#getDisplayStyle-boolean-}
```
public Style getDisplayStyle(boolean includeMergedBorders)
```


Hämtar cellens visningsstil.

**Remarks**

Om den angivna flaggan är false, är den samma som [getDisplayStyle()](../../com.aspose.cells/cell\#getDisplayStyle--). Annars är den samma som att använda [BorderType.SIDE\_BORDERS](../../com.aspose.cells/bordertype\#SIDE-BORDERS)\|[BorderType.DYNAMIC\_STYLE\_BORDERS](../../com.aspose.cells/bordertype\#DYNAMIC-STYLE-BORDERS) för [getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| includeMergedBorders | boolean | Anger om kanter för sammanslagna celler ska kontrolleras. |

**Returns:**
[Style](../../com.aspose.cells/style) - display style of this cell
### getDisplayStyle(int adjacentBorders) {#getDisplayStyle-int-}
```
public Style getDisplayStyle(int adjacentBorders)
```


Hämtar cellens visningsstil.

**Remarks**

Om den här cellen också påverkas av andra inställningar såsom villkorsstyrd formatering, listobjekt osv., kan visningsstilen vara annorlunda än [getStyle()](../../com.aspose.cells/cell\#getStyle--).

För flaggor som justerar kanter enligt intilliggande celler, [BorderType.TOP\_BORDER](../../com.aspose.cells/bordertype\#TOP-BORDER)/[BorderType.BOTTOM\_BORDER](../../com.aspose.cells/bordertype\#BOTTOM-BORDER)/[BorderType.LEFT\_BORDER](../../com.aspose.cells/bordertype\#LEFT-BORDER)/[BorderType.RIGHT\_BORDER](../../com.aspose.cells/bordertype\#RIGHT-BORDER) anger om man ska kontrollera och kombinera den nedre/övre/höger/vänstra kanten av de vänstra/höger/övre/nedre cellerna som är intilliggande denna.

Av prestanda- och kompatibilitetsskäl används vissa uppräkningar för att ange vissa speciella operationer:

[BorderType.HORIZONTAL](../../com.aspose.cells/bordertype\#HORIZONTAL)/[BorderType.VERTICAL](../../com.aspose.cells/bordertype\#VERTICAL) denote whether check and combine the bottom/right border of merged cells to this one.

[BorderType.DIAGONAL](../../com.aspose.cells/bordertype\#DIAGONAL)(that is, both [StyleModifyFlag.DIAGONAL\_UP\_BORDER](../../com.aspose.cells/stylemodifyflag\#DIAGONAL-UP-BORDER) and [StyleModifyFlag.DIAGONAL\_DOWN\_BORDER](../../com.aspose.cells/stylemodifyflag\#DIAGONAL-DOWN-BORDER) have been set) denotes check and combine borders from the display style of adjacent cells.

Observera att kontroll av kanter/stilar för intilliggande celler, särskilt visningsstilarna, är en tidskrävande process. Om det inte behövs att hämta kanterna för den returnerade stilen, ger användning av [BorderType.NONE](../../com.aspose.cells/bordertype\#NONE) för att inaktivera processen för intilliggande celler bättre prestanda. När kanter för intilliggande celler hämtas från stilar som endast är definierade på dessa celler (utan att ange [BorderType.DIAGONAL](../../com.aspose.cells/bordertype\#DIAGONAL)), kan prestandan också bli bättre eftersom kontroll av en cells visningsstil också är tidskrävande.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| adjacentBorders | int | [BorderType](../../com.aspose.cells/bordertype). Anger vilka kanter som måste kontrolleras och justeras enligt kanterna för intilliggande celler. |

**Returns:**
[Style](../../com.aspose.cells/style) - display style of this cell
### getDoubleValue() {#getDoubleValue--}
```
public double getDoubleValue()
```


Hämtar det dubbelvärde som finns i cellen.

**Returns:**
double
### getEmbeddedImage() {#getEmbeddedImage--}
```
public byte[] getEmbeddedImage()
```


Hämtar den inbäddade bilden i cellen.

**Returns:**
byte[]
### getFloatValue() {#getFloatValue--}
```
public float getFloatValue()
```


Hämtar flyttalsvärdet som finns i cellen.

**Returns:**
float
### getFormatConditions() {#getFormatConditions--}
```
public FormatConditionCollection[] getFormatConditions()
```


Hämtar formatvillkor som gäller för den här cellen.

**Returns:**
com.aspose.cells.FormatConditionCollection[] - Returnerar [FormatConditionCollection](../../com.aspose.cells/formatconditioncollection)-objekt
### getFormula() {#getFormula--}
```
public String getFormula()
```


Hämtar en formel för [Cell](../../com.aspose.cells/cell).

**Remarks**

En formelsträng börjar alltid med ett likhetstecken (=). Och vänligen använd alltid kommatecken (,) som parameteravgränsare, till exempel \"=SUM(A1, E1, H2)\".

**Example**

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
         cells.get("B6").setFormula("=SUM(B2:B5, E1) + sheet1!A1");
```

**Returns:**
java.lang.String
### getFormula(boolean isR1C1, boolean isLocal) {#getFormula-boolean-boolean-}
```
public String getFormula(boolean isR1C1, boolean isLocal)
```


Hämta formeln för den här cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isR1C1 | boolean | Om formeln behöver formateras som R1C1. |
| isLocal | boolean | Om formeln behöver formateras enligt lokala inställningar. |

**Returns:**
java.lang.String - formeln för denna cell.
### getFormulaLocal() {#getFormulaLocal--}
```
public String getFormulaLocal()
```


Hämta den lokaliserade formaterade formeln för cellen.

**Returns:**
java.lang.String
### getHeightOfValue() {#getHeightOfValue--}
```
public int getHeightOfValue()
```


Hämtar höjden på värdet i enheten pixlar.

**Returns:**
int -
### getHtmlString() {#getHtmlString--}
```
public String getHtmlString()
```


Hämtar HTML-strängen som innehåller data och vissa format i den här cellen.

**Returns:**
java.lang.String
### getHtmlString(boolean html5) {#getHtmlString-boolean-}
```
public String getHtmlString(boolean html5)
```


Hämtar HTML-strängen som innehåller data och vissa format i den här cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| html5 | boolean | Anger om värdet är kompatibelt med html5 |

**Returns:**
java.lang.String -
### getIntValue() {#getIntValue--}
```
public int getIntValue()
```


Hämtar heltalsvärdet som finns i cellen.

**Returns:**
int
### getLeafs() {#getLeafs--}
```
public Iterator getLeafs()
```


Hämta alla celler som refererar till den här cellen direkt och som behöver uppdateras när den här cellen ändras.

**Remarks**

OBS: Denna klass är nu föråldrad. Använd istället Cell.GetDependentsInCalculation(bool) för att hämta alla beroenden i beräkningskedjan. Denna egenskap kommer att tas bort 12 månader senare från och med maj 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
java.util.Iterator - Enumerator för att enumerera alla beroenden (Cell)
### getLeafs(boolean recursive) {#getLeafs-boolean-}
```
public Iterator getLeafs(boolean recursive)
```


Hämta alla celler som kommer att uppdateras när den här cellen ändras.

**Remarks**

OBS: Denna klass är nu föråldrad. Använd istället Cell.GetDependentsInCalculation(bool) för att hämta alla beroenden i beräkningskedjan. Denna egenskap kommer att tas bort 12 månader senare från och med maj 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rekursiv | boolean | Anger om den returnerar de löv som inte refererar direkt till denna cell men refererar till andra löv för denna cell |

**Returns:**
java.util.Iterator - Enumerator för att enumerera alla beroenden (Cell)
### getMergedRange() {#getMergedRange--}
```
public Range getMergedRange()
```


Returnerar ett [Range](../../com.aspose.cells/range)-objekt som representerar ett sammanslaget område.

**Returns:**
[Range](../../com.aspose.cells/range) - [Range](../../com.aspose.cells/range) object. Null if this cell is not merged.
### getName() {#getName--}
```
public String getName()
```


Hämtar namnet på cellen.

**Remarks**

Ett cellnamn innehåller dess kolumnbokstav och radnummer. Till exempel är namnet på en cell i rad 0 och kolumn 0 A1.

**Returns:**
java.lang.String
### getNumberCategoryType() {#getNumberCategoryType--}
```
public int getNumberCategoryType()
```


Representerar kategoritypen för den här cellens talformatering.

Se [NumberCategoryType](../../com.aspose.cells/numbercategorytype).

**Remarks**

När en cells formateringsmönster kombineras med villkorsformateringsmönster, motsvarar den returnerade typen den del som används för cellens aktuella värde. Till exempel, om formateringsmönstret för denna cell är \"\#,\#\#0;(\#,\#\#0);\"-\";@\", så är den returnerade typen [NumberCategoryType.NUMBER](../../com.aspose.cells/numbercategorytype\#NUMBER) när cellens värde är numeriskt och inte 0; när cellens värde är 0 eller inte är numeriskt, är den returnerade typen [NumberCategoryType.TEXT](../../com.aspose.cells/numbercategorytype\#TEXT).

**Returns:**
int
### getPicture() {#getPicture--}
```
public Picture getPicture()
```


Hämtar en [Picture](../../com.aspose.cells/picture)-instans som representerar den inbäddade bilden i den här cellen eller null om det inte finns någon inbäddad bild för den här cellen.

**Returns:**
[Picture](../../com.aspose.cells/picture)
### getPrecedents() {#getPrecedents--}
```
public ReferredAreaCollection getPrecedents()
```


Hämtar alla referenser som förekommer i den här cellens formel.

**Remarks**

 *  Returns null if this is not a formula cell.
 *  All references appearing in this cell's formula will be returned no matter they are referenced or not while calculating. For example, although cell A2 in formula "=IF(TRUE,A1,A2)" is not used while calculating, it is still taken as the formula's precedents.
 *  To get those references which influence the calculation only, please use .

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("A1").setFormula("=B1+SUM(B1:B10)+[Book1.xls]Sheet1!A1");
         ReferredAreaCollection areas = cells.get("A1").getPrecedents();
         for (int i = 0; i <areas.getCount(); i++)
         {
              ReferredArea area = areas.get(i);
              StringBuilder stringBuilder = new StringBuilder();
              if (area.isExternalLink())
              {
                  stringBuilder.append("[");
                  stringBuilder.append(area.getExternalFileName());
                  stringBuilder.append("]");
              }
              stringBuilder.append(area.getSheetName());
              stringBuilder.append("!");
              stringBuilder.append(CellsHelper.cellIndexToName(area.getStartRow(), area.getStartColumn()));
              if (area.isArea())
              {
                  stringBuilder.append(":");
                  stringBuilder.append(CellsHelper.cellIndexToName(area.getEndRow(), area.getEndColumn()));
              }
              System.out.println(stringBuilder.toString());
         }
```

**Returns:**
[ReferredAreaCollection](../../com.aspose.cells/referredareacollection) - Collection of all references appearing in this cell's formula.
### getPrecedentsInCalculation() {#getPrecedentsInCalculation--}
```
public Iterator getPrecedentsInCalculation()
```


Hämtar alla föregångare (referenser till celler i aktuell arbetsbok) som används av den här cellens formel vid beräkning.

**Remarks**

Denna metod kan endast fungera när [FormulaSettings.getEnableCalculationChain()](../../com.aspose.cells/formulasettings\#getEnableCalculationChain--) är true för arbetsboken och arbetsboken har beräknats fullt ut. Om denna cell inte är en formel eller den inte refererar till några andra celler, returneras null.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("A2").setFormula("=IF(TRUE,B2,B1)");
         workbook.getSettings().getFormulaSettings().setEnableCalculationChain(true);
         workbook.calculateFormula();
         Iterator en = cells.get("A2").getPrecedentsInCalculation();
         System.out.println("A2's calculation precedents:");
         while(en.hasNext())
         {
             ReferredArea r = (ReferredArea)en.next();
             System.out.println(r);
         }
```

**Returns:**
java.util.Iterator - Uppräkning för att lista alla referenser (ReferredArea)
### getR1C1Formula() {#getR1C1Formula--}
```
public String getR1C1Formula()
```


Hämtar en R1C1-formel för [Cell](../../com.aspose.cells/cell).

**Returns:**
java.lang.String
### getRichValue() {#getRichValue--}
```
public CellRichValue getRichValue()
```


Hämtar det rika värdet för cellen.

**Returns:**
[CellRichValue](../../com.aspose.cells/cellrichvalue)
### getRow() {#getRow--}
```
public int getRow()
```


Hämtar radnumret (nollbaserat) för cellen.

**Returns:**
int
### getSharedStyleIndex() {#getSharedStyleIndex--}
```
public int getSharedStyleIndex()
```


Hämtar cellens delade stilindex i stilpoolen.

**Returns:**
int
### getStringValue() {#getStringValue--}
```
public String getStringValue()
```


Hämtar strängvärdet som finns i cellen. Om cellens typ är sträng returneras själva strängvärdet. För andra celltyper returneras det formaterade strängvärdet (formaterat med den angivna stilen för denna cell). Det formaterade cellvärdet är detsamma som vad du kan få från Excel när du kopierar en cell som text (t.ex. kopierar cellen till en textredigerare eller exporterar till CSV).

**Returns:**
java.lang.String
### getStringValue(int formatStrategy) {#getStringValue-int-}
```
public String getStringValue(int formatStrategy)
```


Hämtar strängvärdet enligt en specifik formateringsstrategi.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formatStrategy | int | [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy). Den formaterade strategin. |

**Returns:**
java.lang.String -
### getStringValueWithoutFormat() {#getStringValueWithoutFormat--}
```
public String getStringValueWithoutFormat()
```


Hämtar cellens värde som sträng utan någon formatering.

**Remarks**

OBS: Denna metod är nu föråldrad. Istället bör användaren hämta värdeobjektet och formatera det enligt värdetypen och de specifika kraven. Denna egenskap kommer att tas bort 12 månader senare, sedan december 2020. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
java.lang.String
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Hämtar cellstilen.

**Remarks**

För att ändra cellens stil, anropa metoden Cell.SetStyle() efter att du har modifierat det returnerade stilobjektet. Denna metod är densamma som [getStyle(boolean)](../../com.aspose.cells/cell\#getStyle-boolean-) med true som parametervärde.

**Returns:**
[Style](../../com.aspose.cells/style) - Style object.
### getStyle(boolean checkBorders) {#getStyle-boolean-}
```
public Style getStyle(boolean checkBorders)
```


Om checkBorders är true, kontrollera om andra cellers kanter kommer att påverka stilen för den här cellen.

**Remarks**

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| checkBorders | boolean | Kontrollera andra cellers kanter |

**Returns:**
[Style](../../com.aspose.cells/style) - Style object.
### getTable() {#getTable--}
```
public ListObject getTable()
```


Hämtar tabellen som innehåller den här cellen.

**Returns:**
[ListObject](../../com.aspose.cells/listobject) - 
### getType() {#getType--}
```
public int getType()
```


Representerar cellvärdestyp.

Se [CellValueType](../../com.aspose.cells/cellvaluetype).

**Returns:**
int
### getValidation() {#getValidation--}
```
public Validation getValidation()
```


Hämtar valideringen som tillämpas på den här cellen.

**Returns:**
[Validation](../../com.aspose.cells/validation) - 
### getValidationValue() {#getValidationValue--}
```
public boolean getValidationValue()
```


Hämtar värdet för valideringen som tillämpas på den här cellen.

**Returns:**
boolean -
### getValue() {#getValue--}
```
public Object getValue()
```


Hämtar värdet som finns i den här cellen.

**Remarks**

Möjlig typ:

null,

Boolean,

DateTime,

Double,

Integer

String.

För int‑värden kan de returneras som ett Integer‑objekt eller ett Double‑objekt. Det finns ingen garanti för att det returnerade värdet alltid behålls som samma objekttyp.

**Returns:**
java.lang.Object
### getWidthOfValue() {#getWidthOfValue--}
```
public int getWidthOfValue()
```


Hämtar bredden på värdet i enheten pixlar.

**Returns:**
int -
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Hämtar det överordnade kalkylbladet.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hasCustomFunction() {#hasCustomFunction--}
```
public boolean hasCustomFunction()
```


Kontrollerar om det finns en anpassad funktion (ej stödd funktion) i den här cellens formel.

**Returns:**
boolean
### hasCustomStyle() {#hasCustomStyle--}
```
public boolean hasCustomStyle()
```


Anger om den här cellen har anpassade stilinställningar (annorlunda än standardinställningen som ärvs från motsvarande rad, kolumn eller arbetsbok).

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```


Fungerar som en hash-funktion för en specifik typ.

**Returns:**
int – En hashkod för det aktuella Cell‑objektet.
### insertText(int index, String text) {#insertText-int-java.lang.String-}
```
public void insertText(int index, String text)
```


Infoga några tecken i cellen. Om cellen är rikformatterad kan denna metod behålla den ursprungliga formateringen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Indexet. |
| text | java.lang.String | Infogad text. |

### isArrayFormula() {#isArrayFormula--}
```
public boolean isArrayFormula()
```


Anger om cellens formel är en matrisformel.

**Returns:**
boolean
### isArrayHeader() {#isArrayHeader--}
```
public boolean isArrayHeader()
```


Anger att cellens formel är en matrisformel och att den är den första cellen i matrisen.

**Returns:**
boolean
### isCheckBoxStyle() {#isCheckBoxStyle--}
```
public boolean isCheckBoxStyle()
```


Anger om den här cellen är inställd som en kryssruta.

**Returns:**
boolean
### isDynamicArrayFormula() {#isDynamicArrayFormula--}
```
public boolean isDynamicArrayFormula()
```


Anger om cellens formel är en dynamisk matrisformel (true) eller en äldre matrisformel (false).

**Returns:**
boolean
### isErrorValue() {#isErrorValue--}
```
public boolean isErrorValue()
```


Kontrollerar om värdet i den här cellen är ett fel.

**Remarks**

Gäller också för formelceller för att kontrollera om det beräknade resultatet är ett fel.

**Returns:**
boolean
### isFormula() {#isFormula--}
```
public boolean isFormula()
```


Representerar om den angivna cellen innehåller en formel.

**Returns:**
boolean
### isInArray() {#isInArray--}
```
public boolean isInArray()
```


Anger om cellens formel är en matrisformel.

**Remarks**

OBS: Denna klass är nu föråldrad. Använd istället Cell.IsArrayFormula för att kontrollera om cellens formel är en matrisformel. Denna egenskap kommer att tas bort 12 månader senare, sedan maj 2018. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
boolean
### isInTable() {#isInTable--}
```
public boolean isInTable()
```


Anger om den här cellen är en del av en tabellformel.

**Remarks**

OBS: Denna klass är nu föråldrad. Använd istället Cell.IsTableFormula för att kontrollera om cellens formel är en del av en tabellformel. Denna egenskap kommer att tas bort 12 månader senare, sedan maj 2018. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
boolean
### isMerged() {#isMerged--}
```
public boolean isMerged()
```


Kontrollerar om en cell är en del av ett sammanslaget område eller inte.

**Returns:**
boolean
### isNumericValue() {#isNumericValue--}
```
public boolean isNumericValue()
```


Anger om värdet i den här cellen är numeriskt (int, double och datetime).

**Remarks**

Gäller också för formelceller för att kontrollera det beräknade resultatet

**Returns:**
boolean
### isRichText() {#isRichText--}
```
public boolean isRichText()
```


Anger om strängvärdet i den här cellen är rik formaterad text.

**Returns:**
boolean
### isSharedFormula() {#isSharedFormula--}
```
public boolean isSharedFormula()
```


Anger om cellens formel är en del av en delad formel.

**Returns:**
boolean
### isStyleSet() {#isStyleSet--}
```
public boolean isStyleSet()
```


Indikerar om cellens stil är inställd. Om den returnerar false betyder det att cellen har ett standardcellformat.

**Returns:**
boolean
### isTableFormula() {#isTableFormula--}
```
public boolean isTableFormula()
```


Anger om den här cellen är en del av en tabellformel.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### putValue(boolean boolValue) {#putValue-boolean-}
```
public void putValue(boolean boolValue)
```


Sätter ett booleskt värde i cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| boolValue | boolean |  |

### putValue(DateTime dateTime) {#putValue-com.aspose.cells.DateTime-}
```
public void putValue(DateTime dateTime)
```


Sätter ett DateTime‑värde i cellen.

**Remarks**

Att sätta ett DateTime‑värde för en cell betyder inte att cellen automatiskt formateras som datum/tid. DateTime‑värdet lagras som ett numeriskt värde i datamodellen för både MS Excel och Aspose.Cells. Huruvida det numeriska värdet tolkas som ett tal eller som datum/tid beror på det talformat som tillämpas på cellen. Om cellen inte har formaterats som datum/tid kommer den att visas som ett numeriskt värde även om du har angett ett DateTime‑värde.

**Example**

Detta exempel visar hur man sätter ett DateTime‑värde i en cell och får det att visas som datum/tid.

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
 
         //Put date time into a cell
         Cell cell = cells.get(0, 0);
         cell.putValue(new DateTime(2023, 5, 15));
         Style style = cell.getStyle(false);
         style.setNumber(14);
         cell.setStyle(style);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dateTime | [DateTime](../../com.aspose.cells/datetime) | Indatavärde |

### putValue(double doubleValue) {#putValue-double-}
```
public void putValue(double doubleValue)
```


Lägger in ett dubbelvärde i cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| doubleValue | double | Indatavärde |

### putValue(int intValue) {#putValue-int-}
```
public void putValue(int intValue)
```


Lägger in ett heltalsvärde i cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| intValue | int | Indatavärde |

### putValue(Object objectValue) {#putValue-java.lang.Object-}
```
public void putValue(Object objectValue)
```


Lägger in ett objektvärde i cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| objectValue | java.lang.Object | indatavärde |

### putValue(String stringValue) {#putValue-java.lang.String-}
```
public void putValue(String stringValue)
```


Lägger in ett strängvärde i cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stringValue | java.lang.String | Indatavärde |

### putValue(String stringValue, boolean isConverted) {#putValue-java.lang.String-boolean-}
```
public void putValue(String stringValue, boolean isConverted)
```


Lägger in ett strängvärde i cellen och konverterar värdet till en annan datatyp om det är lämpligt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stringValue | java.lang.String | Indatavärde |
| isConverted | boolean | True: konverterad till annan datatyp om lämpligt. |

### putValue(String stringValue, boolean isConverted, boolean setStyle) {#putValue-java.lang.String-boolean-boolean-}
```
public void putValue(String stringValue, boolean isConverted, boolean setStyle)
```


Lägger in ett värde i cellen, om det är lämpligt konverteras värdet till en annan datatyp och cellens talformat återställs.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stringValue | java.lang.String | Indatavärde |
| isConverted | boolean | True: konverterad till annan datatyp om lämpligt. |
| setStyle | boolean | True: sätt talformatet till cellens stil när du konverterar till annan datatyp |

### removeArrayFormula(boolean leaveNormalFormula) {#removeArrayFormula-boolean-}
```
public void removeArrayFormula(boolean leaveNormalFormula)
```


Ta bort matrisformel.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| leaveNormalFormula | boolean | True representerar konvertering av matrisformeln till en normal formel. |

### replace(String placeHolder, String newValue, ReplaceOptions options) {#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-}
```
public void replace(String placeHolder, String newValue, ReplaceOptions options)
```


Ersätt cellens text med alternativ.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| platshållare | java.lang.String | Cellplatshållare |
| newValue | java.lang.String | Strängvärde att ersätta |
| options | [ReplaceOptions](../../com.aspose.cells/replaceoptions) | Ersättningsalternativen |

### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber) {#setArrayFormula-java.lang.String-int-int-}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber)
```


Ställer in en matrisformel (legacy-matrisformel som matas in via CTRL+SHIFT+ENTER i MS Excel) för ett cellområde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arrayFormula | java.lang.String | Matrisformel. |
| rowNumber | int | Antal rader för att fylla resultatet av matrisformeln. |
| columnNumber | int | Antal kolumner för att fylla resultatet av matrisformeln. |

### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal) {#setArrayFormula-java.lang.String-int-int-boolean-boolean-}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)
```


Ställer in en matrisformel för ett cellområde.

**Remarks**

OBS: Denna klass är nu föråldrad. Använd istället Cell.SetArrayFormula(string,int,int,FormulaParseOptions). Denna egenskap kommer att tas bort 12 månader senare sedan december 2019. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arrayFormula | java.lang.String | Matrisformel. |
| rowNumber | int | Antal rader för att fylla resultatet av matrisformeln. |
| columnNumber | int | Antal kolumner för att fylla resultatet av matrisformeln. |
| isR1C1 | boolean | om formeln är en R1C1-formel |
| isLocal | boolean | om formeln är lokalanpassad |

### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options) {#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options)
```


Ställer in en matrisformel för ett cellområde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arrayFormula | java.lang.String | Matrisformel. |
| rowNumber | int | Antal rader för att fylla resultatet av matrisformeln. |
| columnNumber | int | Antal kolumner för att fylla resultatet av matrisformeln. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Alternativ för att tolka formeln. |

### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values) {#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)
```


Ställer in en matrisformel för ett cellområde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arrayFormula | java.lang.String | Matrisformel. |
| rowNumber | int | Antal rader för att fylla resultatet av matrisformeln. |
| columnNumber | int | Antal kolumner för att fylla resultatet av matrisformeln. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Alternativ för att tolka formeln. |
| värden | java.lang.Object[][] | värden för de celler som har given matrisformel |

### setCharacters(FontSetting[] characters) {#setCharacters-com.aspose.cells.FontSetting---}
```
public void setCharacters(FontSetting[] characters)
```


Ställer in rik textformat för cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| characters | [FontSetting\[\]](../../com.aspose.cells/fontsetting) | Alla teckenobjekt. |

### setCheckBoxStyle(boolean value) {#setCheckBoxStyle-boolean-}
```
public void setCheckBoxStyle(boolean value)
```


Anger om den här cellen är inställd som en kryssruta.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, boolean calculateValue) {#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-boolean-}
```
public CellArea setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, boolean calculateValue)
```


Ställer in dynamisk matrisformel och låter formeln spilla över till angränsande celler om möjligt.

**Remarks**

Det returnerade området kan skilja sig från det faktiska område som denna dynamiska matrisformel spillar in i. Om det finns icke-tomma celler i området kommer formeln endast att sättas för den aktuella cellen och markeras som "\\#SPILL!". Men i sådana situationer returnerar vi fortfarande hela området som formeln bör spilla in i.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arrayFormula | java.lang.String | formeluttrycket |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | alternativ för att tolka formeln. Alternativet "Parse" kommer att ignoreras och formeln kommer alltid att tolkas omedelbart |
| calculateValue | boolean | om denna dynamiska arrayformel ska beräknas för de cellerna i det spillade området. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the range that the formula should spill into.
### setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue) {#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-}
```
public CellArea setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue)
```


Ställer in dynamisk matrisformel och låter formeln spilla över till angränsande celler om möjligt.

**Remarks**

Det returnerade området kan skilja sig från det faktiska område som denna dynamiska matrisformel spillar in i. Om det finns icke-tomma celler i området kommer formeln endast att sättas för den aktuella cellen och markeras som "\\#SPILL!". Men i sådana situationer returnerar vi fortfarande hela området som formeln bör spilla in i.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arrayFormula | java.lang.String | formeluttrycket |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | alternativ för att tolka formeln. Alternativet "Parse" kommer att ignoreras och formeln kommer alltid att tolkas omedelbart |
| värden | java.lang.Object[][] | values(kalkylerade resultat) för de celler med given dynamisk arrayformel |
| calculateRange | boolean | Om beräkna det spillade området för denna dynamiska arrayformel. Om parametern "values" inte är null och denna flagga är falsk, kommer det spillade områdets höjd att vara values.Length och bredden att vara values[0].Length. |
| calculateValue | boolean | om beräkna denna dynamiska arrayformel för de celler i det spillade området när "values" är null eller motsvarande element i "values" för en cell är null. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the range that the formula should spill into.
### setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue, CalculationOptions copts) {#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-com.aspose.cells.CalculationOptions-}
```
public CellArea setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue, CalculationOptions copts)
```


Ställer in dynamisk matrisformel och låter formeln spilla över till angränsande celler om möjligt.

**Remarks**

Det returnerade området kan skilja sig från det faktiska område som denna dynamiska matrisformel spillar in i. Om det finns icke-tomma celler i området kommer formeln endast att sättas för den aktuella cellen och markeras som "\\#SPILL!". Men i sådana situationer returnerar vi fortfarande hela området som formeln bör spilla in i.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arrayFormula | java.lang.String | formeluttrycket |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | alternativ för att tolka formeln. Alternativet "Parse" kommer att ignoreras och formeln kommer alltid att tolkas omedelbart |
| värden | java.lang.Object[][] | values(kalkylerade resultat) för de celler med given dynamisk arrayformel |
| calculateRange | boolean | Om beräkna det spillade området för denna dynamiska arrayformel. Om parametern "values" inte är null och denna flagga är falsk, kommer det spillade områdets höjd att vara values.Length och bredden att vara values[0].Length. |
| calculateValue | boolean | om beräkna denna dynamiska arrayformel för de celler i det spillade området när "values" är null eller motsvarande element i "values" för en cell är null. |
| copts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Alternativen för att beräkna formeln. Vanligtvis, av prestandaskäl, bör egenskapen [CalculationOptions.getRecursive()](../../com.aspose.cells/calculationoptions\#getRecursive--) vara falsk. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the range that the formula should spill into.
### setEmbeddedImage(byte[] value) {#setEmbeddedImage-byte---}
```
public void setEmbeddedImage(byte[] value)
```


Ställer in den inbäddade bilden i cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | byte[] |  |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public void setFormula(String value)
```


Ställer in en formel för [Cell](../../com.aspose.cells/cell).

**Remarks**

En formelsträng börjar alltid med ett likhetstecken (=). Och vänligen använd alltid kommatecken (,) som parameteravgränsare, till exempel \"=SUM(A1, E1, H2)\".

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setFormula(String formula, boolean isR1C1, boolean isLocal, Object value) {#setFormula-java.lang.String-boolean-boolean-java.lang.Object-}
```
public void setFormula(String formula, boolean isR1C1, boolean isLocal, Object value)
```


Ställ in formeln och formelns värde.

**Remarks**

OBS: Denna klass är nu föråldrad. Använd istället Cell.SetFormula(string,FormulaParseOptions,object). Denna egenskap kommer att tas bort 12 månader senare sedan december 2019. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formula | java.lang.String | Formeln. |
| isR1C1 | boolean | Om formeln är en R1C1-formel. |
| isLocal | boolean | Om formeln är lokalanpassad. |
| värde | java.lang.Object | Formelns värde. |

### setFormula(String formula, FormulaParseOptions options) {#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-}
```
public void setFormula(String formula, FormulaParseOptions options)
```


Ställ in formeln och värdet (beräknat resultat) för formeln.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formula | java.lang.String | Formeln. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Alternativ för att tolka formeln. |

### setFormula(String formula, FormulaParseOptions options, Object value) {#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-}
```
public void setFormula(String formula, FormulaParseOptions options, Object value)
```


Ställ in formeln och värdet (beräknat resultat) för formeln.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formula | java.lang.String | Formeln. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Alternativ för att tolka formeln. |
| värde | java.lang.Object | Formelns värde(kalkylerat resultat) |

### setFormula(String formula, Object value) {#setFormula-java.lang.String-java.lang.Object-}
```
public void setFormula(String formula, Object value)
```


Ställ in formeln och värdet (beräknat resultat) för formeln.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formula | java.lang.String | Formeln. |
| värde | java.lang.Object | Formelns värde(kalkylerat resultat) |

### setFormulaLocal(String value) {#setFormulaLocal-java.lang.String-}
```
public void setFormulaLocal(String value)
```


Hämta den lokaliserade formaterade formeln för cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setHtmlString(String value) {#setHtmlString-java.lang.String-}
```
public void setHtmlString(String value)
```


Ställer in HTML-strängen som innehåller data och vissa format i den här cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setR1C1Formula(String value) {#setR1C1Formula-java.lang.String-}
```
public void setR1C1Formula(String value)
```


Ställer in en R1C1-formel för [Cell](../../com.aspose.cells/cell).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber) {#setSharedFormula-java.lang.String-int-int-}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber)
```


Ställer in delade formler för ett cellområde.

**Remarks**

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sharedFormula | java.lang.String | Delad formel. |
| rowNumber | int | Antal rader att fylla i formeln. |
| columnNumber | int | Antal kolumner att fylla i formeln. |

### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal) {#setSharedFormula-java.lang.String-int-int-boolean-boolean-}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)
```


Ställer in en formel för ett cellområde.

**Remarks**

OBS: Denna klass är nu föråldrad. Använd istället Cell.SetSharedFormula(string,int,int,FormulaParseOptions). Denna egenskap kommer att tas bort 12 månader senare sedan december 2019. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sharedFormula | java.lang.String | Delad formel. |
| rowNumber | int | Antal rader att fylla i formeln. |
| columnNumber | int | Antal kolumner att fylla i formeln. |
| isR1C1 | boolean | om formeln är en R1C1-formel |
| isLocal | boolean | om formeln är lokalanpassad |

### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options) {#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options)
```


Ställer in delade formler för ett cellområde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sharedFormula | java.lang.String | Delad formel. |
| rowNumber | int | Antal rader att fylla i formeln. |
| columnNumber | int | Antal kolumner att fylla i formeln. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Alternativ för att tolka formeln. |

### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values) {#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)
```


Ställer in delade formler för ett cellområde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sharedFormula | java.lang.String | Delad formel. |
| rowNumber | int | Antal rader att fylla i formeln. |
| columnNumber | int | Antal kolumner att fylla i formeln. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Alternativ för att tolka formeln. |
| värden | java.lang.Object[][] | values för de celler med given delad formel |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


Ställer in cellstilen.

**Remarks**

Om kantinställningarna ändras, kommer kanten på justeringscellerna också att uppdateras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Cellstilen. |

### setStyle(Style style, boolean explicitFlag) {#setStyle-com.aspose.cells.Style-boolean-}
```
public void setStyle(Style style, boolean explicitFlag)
```


Tillämpa den ändrade egenskapen för stilen på cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Cellstilen. |
| explicitFlag | boolean | Sant, endast skriva över formatering som är explicit angiven. |

### setStyle(Style style, StyleFlag flag) {#setStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void setStyle(Style style, StyleFlag flag)
```


Tillämpa cellstilen baserat på flaggor.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Cellstilen. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Stilflaggan. |

### setTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, int columnIndexOfInputCell, boolean isRowInput, Object[][] values) {#setTableFormula-int-int-int-int-boolean-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, int columnIndexOfInputCell, boolean isRowInput, Object[][] values)
```


Skapa en envariabels datatabell för det angivna området med början från den här cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowNumber | int | Antal rader att fylla i formeln. |
| columnNumber | int | Antal kolumner att fylla i formeln. |
| rowIndexOfInputCell | int | radindex för inmatningscellen |
| columnIndexOfInputCell | int | kolumnindex för inmatningscellen |
| isRowInput | boolean | Anger om inmatningscellen är en radinmatningscell (true) eller en kolumninmatningscell (false). |
| värden | java.lang.Object[][] | värden för celler i tabellens formelintervall |

### setTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, Object[][] values) {#setTableFormula-int-int-int-int-int-int-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, Object[][] values)
```


Skapa en tvåvariabels datatabell för det angivna området med början från den här cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowNumber | int | Antal rader att fylla i formeln. |
| columnNumber | int | Antal kolumner att fylla i formeln. |
| rowIndexOfRowInputCell | int | radindex för radinmatningscellen |
| columnIndexOfRowInputCell | int | kolumnindex för radinmatningscellen |
| rowIndexOfColumnInputCell | int | radindex för kolumninmatningscellen |
| columnIndexOfColumnInputCell | int | kolumnindex för kolumninmatningscellen |
| värden | java.lang.Object[][] | värden för celler i tabellens formelintervall |

### setTableFormula(int rowNumber, int columnNumber, String inputCell, boolean isRowInput, Object[][] values) {#setTableFormula-int-int-java.lang.String-boolean-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, String inputCell, boolean isRowInput, Object[][] values)
```


Skapa en envariabels datatabell för det angivna området med början från den här cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowNumber | int | Antal rader att fylla i formeln. |
| columnNumber | int | Antal kolumner att fylla i formeln. |
| inputCell | java.lang.String | inmatningscellen |
| isRowInput | boolean | Anger om inmatningscellen är en radinmatningscell (true) eller en kolumninmatningscell (false). |
| värden | java.lang.Object[][] | värden för celler i tabellens formelintervall |

### setTableFormula(int rowNumber, int columnNumber, String rowInputCell, String columnInputCell, Object[][] values) {#setTableFormula-int-int-java.lang.String-java.lang.String-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, String rowInputCell, String columnInputCell, Object[][] values)
```


Skapa en tvåvariabels datatabell för det angivna området med början från den här cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowNumber | int | Antal rader att fylla i formeln. |
| columnNumber | int | Antal kolumner att fylla i formeln. |
| rowInputCell | java.lang.String | radinmatningscellen |
| columnInputCell | java.lang.String | kolumninmatningscellen |
| värden | java.lang.Object[][] | värden för celler i tabellens formelintervall |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Ställer in värdet som finns i den här cellen.

**Remarks**

Möjlig typ:

null,

Boolean,

DateTime,

Double,

Integer

String.

För int‑värden kan de returneras som ett Integer‑objekt eller ett Double‑objekt. Det finns ingen garanti för att det returnerade värdet alltid behålls som samma objekttyp.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.Object |  |

### toJson() {#toJson--}
```
public String toJson()
```


Konvertera [Cell](../../com.aspose.cells/cell) till JSON‑strukturdata.

**Returns:**
java.lang.String -
### toString() {#toString--}
```
public String toString()
```


Returnerar en sträng som representerar det aktuella Cell‑objektet.

**Returns:**
java.lang.String -
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

