##Cell
Encapsulates the object that represents a single Workbook cell.
**Inheritance:**
java.lang.Object
```
public class Cell
```
Encapsulates the object that represents a single Workbook cell.
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
## Methods
| Method | Description |
| --- | --- |
| [calculate(CalculationOptions options)](#calculate-com.aspose.cells.CalculationOptions-) | Calculates the formula of the cell. |
| [characters(int startIndex, int length)](#characters-int-int-) | Returns a Characters object that represents a range of characters within the cell text. |
| [containsExternalLink()](#containsExternalLink--) | Indicates whether this cell contains an external link. |
| [copy(Cell cell)](#copy-com.aspose.cells.Cell-) | Copies data from a source cell. |
| [equals(Cell cell)](#equals-com.aspose.cells.Cell-) | Checks whether this object refers to the same cell with another cell object. |
| [equals(Object obj)](#equals-java.lang.Object-) | Checks whether this object refers to the same cell with another. |
| [getArrayRange()](#getArrayRange--) | Gets the array range if the cell's formula is an array formula. |
| [getBoolValue()](#getBoolValue--) | Gets the boolean value contained in the cell. |
| [getCharacters()](#getCharacters--) | Returns all Characters objects that represents a range of characters within the cell text. |
| [getCharacters(boolean flag)](#getCharacters-boolean-) | Returns all Characters objects that represents a range of characters within the cell text. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Gets column number (zero based) of the cell. |
| [getComment()](#getComment--) | Gets the comment of this cell. |
| [getConditionalFormattingResult()](#getConditionalFormattingResult--) | Get the result of the conditional formatting. |
| [getDateTimeValue()](#getDateTimeValue--) | Gets the DateTime value contained in the cell. |
| [getDependents(boolean isAll)](#getDependents-boolean-) | Get all cells whose formula references to this cell directly. |
| [getDependentsInCalculation(boolean recursive)](#getDependentsInCalculation-boolean-) | Gets all cells whose calculated result depends on this cell. |
| [getDisplayStringValue()](#getDisplayStringValue--) | Gets the formatted string value of this cell by cell's display style. |
| [getDisplayStyle()](#getDisplayStyle--) | Gets the display style of this cell. |
| [getDisplayStyle(boolean includeMergedBorders)](#getDisplayStyle-boolean-) | Gets the display style of this cell. |
| [getDisplayStyle(int adjacentBorders)](#getDisplayStyle-int-) | Gets the display style of this cell. |
| [getDoubleValue()](#getDoubleValue--) | Gets the double value contained in the cell. |
| [getEmbeddedImage()](#getEmbeddedImage--) | Gets the embeddedn image in the cell. |
| [getFloatValue()](#getFloatValue--) | Gets the float value contained in the cell. |
| [getFormatConditions()](#getFormatConditions--) | Gets format conditions which applies to this cell. |
| [getFormula()](#getFormula--) | Gets a formula of the [Cell](../../com.aspose.cells/cell). |
| [getFormula(boolean isR1C1, boolean isLocal)](#getFormula-boolean-boolean-) | Get the formula of this cell. |
| [getFormulaLocal()](#getFormulaLocal--) | Get the locale formatted formula of the cell. |
| [getHeightOfValue()](#getHeightOfValue--) | Gets the height of the value in unit of pixels. |
| [getHtmlString()](#getHtmlString--) | Gets the html string which contains data and some formats in this cell. |
| [getHtmlString(boolean html5)](#getHtmlString-boolean-) | Gets the html string which contains data and some formats in this cell. |
| [getIntValue()](#getIntValue--) | Gets the integer value contained in the cell. |
| [getLeafs()](#getLeafs--) | Get all cells which reference to this cell directly and need to be updated when this cell is modified. |
| [getLeafs(boolean recursive)](#getLeafs-boolean-) | Get all cells which will be updated when this cell is modified. |
| [getMergedRange()](#getMergedRange--) | Returns a [Range](../../com.aspose.cells/range) object which represents a merged range. |
| [getName()](#getName--) | Gets the name of the cell. |
| [getNumberCategoryType()](#getNumberCategoryType--) | Represents the category type of this cell's number formatting. |
| [getPrecedents()](#getPrecedents--) | Gets all references appearing in this cell's formula. |
| [getPrecedentsInCalculation()](#getPrecedentsInCalculation--) | Gets all precedents(reference to cells in current workbook) used by this cell's formula while calculating it. |
| [getR1C1Formula()](#getR1C1Formula--) | Gets a R1C1 formula of the [Cell](../../com.aspose.cells/cell). |
| [getRichValue()](#getRichValue--) | Gets rich value of the cell. |
| [getRow()](#getRow--) | Gets row number (zero based) of the cell. |
| [getSharedStyleIndex()](#getSharedStyleIndex--) | Gets cell's shared style index in the style pool. |
| [getStringValue()](#getStringValue--) | Gets the string value contained in the cell. |
| [getStringValue(int formatStrategy)](#getStringValue-int-) | Gets the string value by specific formatted strategy. |
| [getStringValueWithoutFormat()](#getStringValueWithoutFormat--) | Gets cell's value as string without any format. |
| [getStyle()](#getStyle--) | Gets the cell style. |
| [getStyle(boolean checkBorders)](#getStyle-boolean-) | If checkBorders is true, check whether other cells' borders will effect the style of this cell. |
| [getTable()](#getTable--) | Gets the table which contains this cell. |
| [getType()](#getType--) | Represents cell value type. |
| [getValidation()](#getValidation--) | Gets the validation applied to this cell. |
| [getValidationValue()](#getValidationValue--) | Gets the value of validation which applied to this cell. |
| [getValue()](#getValue--) | Gets the value contained in this cell. |
| [getWidthOfValue()](#getWidthOfValue--) | Gets the width of the value in unit of pixels. |
| [getWorksheet()](#getWorksheet--) | Gets the parent worksheet. |
| [hasCustomFunction()](#hasCustomFunction--) | Checks whether there is custom function(unsupported function) in this cell's formula. |
| [hasCustomStyle()](#hasCustomStyle--) | Indicates whether this cell has custom style settings(different from the default one inherited from corresponding row, column, or workbook). |
| [hashCode()](#hashCode--) | Serves as a hash function for a particular type. |
| [insertText(int index, String text)](#insertText-int-java.lang.String-) | Insert some characters to the cell. |
| [isArrayFormula()](#isArrayFormula--) | Indicates whether the cell formula is an array formula. |
| [isArrayHeader()](#isArrayHeader--) | Indicates the cell's formula is an array formula and it is the first cell of the array. |
| [isCheckBoxStyle()](#isCheckBoxStyle--) | Indicates whether setting this cell as a check box. |
| [isDynamicArrayFormula()](#isDynamicArrayFormula--) | Indicates whether the cell's formula is dynamic array formula(true) or legacy array formula(false). |
| [isErrorValue()](#isErrorValue--) | Checks if the value of this cell is an error. |
| [isFormula()](#isFormula--) | Represents if the specified cell contains formula. |
| [isInArray()](#isInArray--) | Indicates whether the cell formula is an array formula. |
| [isInTable()](#isInTable--) | Indicates whether this cell is part of table formula. |
| [isMerged()](#isMerged--) | Checks if a cell is part of a merged range or not. |
| [isNumericValue()](#isNumericValue--) | Indicates whether the value of this cell is numeric(int, double and datetime) |
| [isRichText()](#isRichText--) | Indicates whether the string value of this cell is a rich formatted text. |
| [isSharedFormula()](#isSharedFormula--) | Indicates whether the cell formula is part of shared formula. |
| [isStyleSet()](#isStyleSet--) | Indicates if the cell's style is set. |
| [isTableFormula()](#isTableFormula--) | Indicates whether this cell is part of table formula. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(boolean boolValue)](#putValue-boolean-) | Puts a boolean value into the cell. |
| [putValue(DateTime dateTime)](#putValue-com.aspose.cells.DateTime-) | Puts a DateTime value into the cell. |
| [putValue(double doubleValue)](#putValue-double-) | Puts a double value into the cell. |
| [putValue(int intValue)](#putValue-int-) | Puts an integer value into the cell. |
| [putValue(Object objectValue)](#putValue-java.lang.Object-) | Puts an object value into the cell. |
| [putValue(String stringValue)](#putValue-java.lang.String-) | Puts a string value into the cell. |
| [putValue(String stringValue, boolean isConverted)](#putValue-java.lang.String-boolean-) | Puts a string value into the cell and converts the value to other data type if appropriate. |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | Puts a value into the cell, if appropriate the value will be converted to other data type and cell's number format will be reset. |
| [removeArrayFormula(boolean leaveNormalFormula)](#removeArrayFormula-boolean-) | Remove array formula. |
| [replace(String placeHolder, String newValue, ReplaceOptions options)](#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-) | Replace text of the cell with options. |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber)](#setArrayFormula-java.lang.String-int-int-) | Sets an array formula(legacy array formula entered via CTRL+SHIFT+ENTER in ms excel) to a range of cells. |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)](#setArrayFormula-java.lang.String-int-int-boolean-boolean-) | Sets an array formula to a range of cells. |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options)](#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-) | Sets an array formula to a range of cells. |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)](#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----) | Sets an array formula to a range of cells. |
| [setCharacters(FontSetting[] characters)](#setCharacters-com.aspose.cells.FontSetting---) | Sets rich text format of the cell. |
| [setCheckBoxStyle(boolean value)](#setCheckBoxStyle-boolean-) | Indicates whether setting this cell as a check box. |
| [setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, boolean calculateValue)](#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-boolean-) | Sets dynamic array formula and make the formula spill into neighboring cells if possible. |
| [setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue)](#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-) | Sets dynamic array formula and make the formula spill into neighboring cells if possible. |
| [setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue, CalculationOptions copts)](#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-com.aspose.cells.CalculationOptions-) | Sets dynamic array formula and make the formula spill into neighboring cells if possible. |
| [setEmbeddedImage(byte[] value)](#setEmbeddedImage-byte---) | Sets the embeddedn image in the cell. |
| [setFormula(String value)](#setFormula-java.lang.String-) | Sets a formula of the [Cell](../../com.aspose.cells/cell). |
| [setFormula(String formula, boolean isR1C1, boolean isLocal, Object value)](#setFormula-java.lang.String-boolean-boolean-java.lang.Object-) | Set the formula and the value of the formula. |
| [setFormula(String formula, FormulaParseOptions options)](#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-) | Set the formula and the value(calculated result) of the formula. |
| [setFormula(String formula, FormulaParseOptions options, Object value)](#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-) | Set the formula and the value(calculated result) of the formula. |
| [setFormula(String formula, Object value)](#setFormula-java.lang.String-java.lang.Object-) | Set the formula and the value(calculated result) of the formula. |
| [setFormulaLocal(String value)](#setFormulaLocal-java.lang.String-) | Get the locale formatted formula of the cell. |
| [setHtmlString(String value)](#setHtmlString-java.lang.String-) | Sets the html string which contains data and some formats in this cell. |
| [setR1C1Formula(String value)](#setR1C1Formula-java.lang.String-) | Sets a R1C1 formula of the [Cell](../../com.aspose.cells/cell). |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber)](#setSharedFormula-java.lang.String-int-int-) | Sets shared formulas to a range of cells. |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)](#setSharedFormula-java.lang.String-int-int-boolean-boolean-) | Sets a formula to a range of cells. |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options)](#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-) | Sets shared formulas to a range of cells. |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)](#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----) | Sets shared formulas to a range of cells. |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Sets the cell style. |
| [setStyle(Style style, boolean explicitFlag)](#setStyle-com.aspose.cells.Style-boolean-) | Apply the changed property of style to the cell. |
| [setStyle(Style style, StyleFlag flag)](#setStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Apply the cell style based on flags. |
| [setTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, int columnIndexOfInputCell, boolean isRowInput, Object[][] values)](#setTableFormula-int-int-int-int-boolean-java.lang.Object-----) | Create one-variable data table for given range starting from this cell. |
| [setTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, Object[][] values)](#setTableFormula-int-int-int-int-int-int-java.lang.Object-----) | Create two-variable data table for given range starting from this cell. |
| [setTableFormula(int rowNumber, int columnNumber, String inputCell, boolean isRowInput, Object[][] values)](#setTableFormula-int-int-java.lang.String-boolean-java.lang.Object-----) | Create one-variable data table for given range starting from this cell. |
| [setTableFormula(int rowNumber, int columnNumber, String rowInputCell, String columnInputCell, Object[][] values)](#setTableFormula-int-int-java.lang.String-java.lang.String-java.lang.Object-----) | Create two-variable data table for given range starting from this cell. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Sets the value contained in this cell. |
| [toJson()](#toJson--) | Convert [Cell](../../com.aspose.cells/cell) to JSON struct data. |
| [toString()](#toString--) | Returns a string represents the current Cell object. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### calculate(CalculationOptions options) {#calculate-com.aspose.cells.CalculationOptions-}
```
public void calculate(CalculationOptions options)
```
Calculates the formula of the cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Options for calculation |
### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```
Returns a Characters object that represents a range of characters within the cell text.
**Remarks**
This method only works on cell with string value.
**Example**
```
Workbook excel = new Workbook();
Cells cells = excel.getWorksheets().get(0).getCells();
cells.get("A1").putValue("Helloworld");
cells.get("A1").characters(5, 5).getFont().setBold(true);
cells.get("A1").characters(5, 5).getFont().setColor(Color.getBlue());
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | int | The index of the start of the character. |
| length | int | The number of characters. |
**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - Characters object.
### containsExternalLink() {#containsExternalLink--}
```
public boolean containsExternalLink()
```
Indicates whether this cell contains an external link. Only applies when the cell is a formula cell.
**Returns:**
boolean
### copy(Cell cell) {#copy-com.aspose.cells.Cell-}
```
public void copy(Cell cell)
```
Copies data from a source cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | Source [Cell](../../com.aspose.cells/cell) object. |
### equals(Cell cell) {#equals-com.aspose.cells.Cell-}
```
public boolean equals(Cell cell)
```
Checks whether this object refers to the same cell with another cell object.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | another cell object |
**Returns:**
boolean - true if two cell objects refers to the same cell.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```
Checks whether this object refers to the same cell with another.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | another object |
**Returns:**
boolean - true if two objects refers to the same cell.
### getArrayRange() {#getArrayRange--}
```
public CellArea getArrayRange()
```
Gets the array range if the cell's formula is an array formula.
**Remarks**
Only applies when the cell's formula is an array formula
**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - The array range.
### getBoolValue() {#getBoolValue--}
```
public boolean getBoolValue()
```
Gets the boolean value contained in the cell.
**Returns:**
boolean
### getCharacters() {#getCharacters--}
```
public FontSetting[] getCharacters()
```
Returns all Characters objects that represents a range of characters within the cell text.
**Returns:**
com.aspose.cells.FontSetting[] - All Characters objects
### getCharacters(boolean flag) {#getCharacters-boolean-}
```
public FontSetting[] getCharacters(boolean flag)
```
Returns all Characters objects that represents a range of characters within the cell text.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| flag | boolean | Indicates whether applying table style to the cell if the cell is in the table. |
**Returns:**
com.aspose.cells.FontSetting[] - All Characters objects
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
Gets column number (zero based) of the cell.
**Returns:**
int
### getComment() {#getComment--}
```
public Comment getComment()
```
Gets the comment of this cell.
**Remarks**
If there is no comment applies to the cell, returns null.
**Returns:**
[Comment](../../com.aspose.cells/comment)
### getConditionalFormattingResult() {#getConditionalFormattingResult--}
```
public ConditionalFormattingResult getConditionalFormattingResult()
```
Get the result of the conditional formatting.
**Remarks**
Returns null if no conditional formatting is applied to this cell,
**Returns:**
[ConditionalFormattingResult](../../com.aspose.cells/conditionalformattingresult)
### getDateTimeValue() {#getDateTimeValue--}
```
public DateTime getDateTimeValue()
```
Gets the DateTime value contained in the cell.
**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getDependents(boolean isAll) {#getDependents-boolean-}
```
public Cell[] getDependents(boolean isAll)
```
Get all cells whose formula references to this cell directly.
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
| Parameter | Type | Description |
| --- | --- | --- |
| isAll | boolean | Indicates whether check formulas in other worksheets |
**Returns:**
com.aspose.cells.Cell[]
### getDependentsInCalculation(boolean recursive) {#getDependentsInCalculation-boolean-}
```
public Iterator getDependentsInCalculation(boolean recursive)
```
Gets all cells whose calculated result depends on this cell.
**Remarks**
To use this method, please make sure the workbook has been set with true value for [FormulaSettings.getEnableCalculationChain()](../../com.aspose.cells/formulasettings\#getEnableCalculationChain--) and has been fully calculated with this setting. If there is no formula reference to this cell, null will be returned.
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
| Parameter | Type | Description |
| --- | --- | --- |
| recursive | boolean | Whether returns those dependents which do not reference to this cell directly but reference to other leafs of this cell |
**Returns:**
java.util.Iterator - Enumerator to enumerate all dependents(Cell objects)
### getDisplayStringValue() {#getDisplayStringValue--}
```
public String getDisplayStringValue()
```
Gets the formatted string value of this cell by cell's display style.
**Returns:**
java.lang.String
### getDisplayStyle() {#getDisplayStyle--}
```
public Style getDisplayStyle()
```
Gets the display style of this cell.
**Remarks**
Same with using [BorderType.SIDE\_BORDERS](../../com.aspose.cells/bordertype\#SIDE-BORDERS) for [getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-). That is, this method will check and adjust top/bottom/left/right borders of this cell according to the style([getStyle()](../../com.aspose.cells/cell\#getStyle--)) of its adjacent cells, but do not check the merged cells, and do not check the display style of adjacent cells.
**Returns:**
[Style](../../com.aspose.cells/style) - display style of this cell
### getDisplayStyle(boolean includeMergedBorders) {#getDisplayStyle-boolean-}
```
public Style getDisplayStyle(boolean includeMergedBorders)
```
Gets the display style of this cell.
**Remarks**
If the specified flag is false, then it is same with [getDisplayStyle()](../../com.aspose.cells/cell\#getDisplayStyle--). Otherwise it is same with using [BorderType.SIDE\_BORDERS](../../com.aspose.cells/bordertype\#SIDE-BORDERS)\|[BorderType.DYNAMIC\_STYLE\_BORDERS](../../com.aspose.cells/bordertype\#DYNAMIC-STYLE-BORDERS) for [getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| includeMergedBorders | boolean | Indicates whether checking borders of merged cells. |
**Returns:**
[Style](../../com.aspose.cells/style) - display style of this cell
### getDisplayStyle(int adjacentBorders) {#getDisplayStyle-int-}
```
public Style getDisplayStyle(int adjacentBorders)
```
Gets the display style of this cell.
**Remarks**
If this cell is also affected by other settings such as conditional formatting, list objects, etc., then the display style may be different from [getStyle()](../../com.aspose.cells/cell\#getStyle--).
For flags of adjusting borders according to adjacent cells, [BorderType.TOP\_BORDER](../../com.aspose.cells/bordertype\#TOP-BORDER)/[BorderType.BOTTOM\_BORDER](../../com.aspose.cells/bordertype\#BOTTOM-BORDER) /[BorderType.LEFT\_BORDER](../../com.aspose.cells/bordertype\#LEFT-BORDER)/[BorderType.RIGHT\_BORDER](../../com.aspose.cells/bordertype\#RIGHT-BORDER) denote whether check and combine the bottom/top/right/left borders of the left/right/top/bottom cells adjacent to this one.
For performance and compatibility consideration, some enums are used to denote some special operations:
[BorderType.HORIZONTAL](../../com.aspose.cells/bordertype\#HORIZONTAL)/[BorderType.VERTICAL](../../com.aspose.cells/bordertype\#VERTICAL) denote whether check and combine the bottom/right border of merged cells to this one.
[BorderType.DIAGONAL](../../com.aspose.cells/bordertype\#DIAGONAL)(that is, both [StyleModifyFlag.DIAGONAL\_UP\_BORDER](../../com.aspose.cells/stylemodifyflag\#DIAGONAL-UP-BORDER) and [StyleModifyFlag.DIAGONAL\_DOWN\_BORDER](../../com.aspose.cells/stylemodifyflag\#DIAGONAL-DOWN-BORDER) have been set) denotes check and combine borders from the display style of adjacent cells.
Please note, checking borders/styles of adjacent cells, especially the display styles, is time-consumed process. If there is no need to get the borders for the returned style, using [BorderType.NONE](../../com.aspose.cells/bordertype\#NONE) to disable the process of adjacent cells will give better performance. When getting borders of adjacent cells from styles defined on those cells only(without setting [BorderType.DIAGONAL](../../com.aspose.cells/bordertype\#DIAGONAL)), the performance also may be better because checking the display style of one cell is time-consumed too.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| adjacentBorders | int | [BorderType](../../com.aspose.cells/bordertype). Indicates which borders need to be checked and adjusted according to the borders of adjacent cells. |
**Returns:**
[Style](../../com.aspose.cells/style) - display style of this cell
### getDoubleValue() {#getDoubleValue--}
```
public double getDoubleValue()
```
Gets the double value contained in the cell.
**Returns:**
double
### getEmbeddedImage() {#getEmbeddedImage--}
```
public byte[] getEmbeddedImage()
```
Gets the embeddedn image in the cell.
**Returns:**
byte[]
### getFloatValue() {#getFloatValue--}
```
public float getFloatValue()
```
Gets the float value contained in the cell.
**Returns:**
float
### getFormatConditions() {#getFormatConditions--}
```
public FormatConditionCollection[] getFormatConditions()
```
Gets format conditions which applies to this cell.
**Returns:**
com.aspose.cells.FormatConditionCollection[] - Returns [FormatConditionCollection](../../com.aspose.cells/formatconditioncollection) object
### getFormula() {#getFormula--}
```
public String getFormula()
```
Gets a formula of the [Cell](../../com.aspose.cells/cell).
**Remarks**
A formula string always begins with an equal sign (=). And please always use comma(,) as parameters delimiter, such as "=SUM(A1, E1, H2)".
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
Get the formula of this cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |
**Returns:**
java.lang.String - the formula of this cell.
### getFormulaLocal() {#getFormulaLocal--}
```
public String getFormulaLocal()
```
Get the locale formatted formula of the cell.
**Returns:**
java.lang.String
### getHeightOfValue() {#getHeightOfValue--}
```
public int getHeightOfValue()
```
Gets the height of the value in unit of pixels.
**Returns:**
int -
### getHtmlString() {#getHtmlString--}
```
public String getHtmlString()
```
Gets the html string which contains data and some formats in this cell.
**Returns:**
java.lang.String
### getHtmlString(boolean html5) {#getHtmlString-boolean-}
```
public String getHtmlString(boolean html5)
```
Gets the html string which contains data and some formats in this cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| html5 | boolean | Indicates whether the value is compatible for html5 |
**Returns:**
java.lang.String -
### getIntValue() {#getIntValue--}
```
public int getIntValue()
```
Gets the integer value contained in the cell.
**Returns:**
int
### getLeafs() {#getLeafs--}
```
public Iterator getLeafs()
```
Get all cells which reference to this cell directly and need to be updated when this cell is modified.
**Remarks**
NOTE: This class is now obsolete. Instead, please use Cell.GetDependentsInCalculation(bool) to get all dependents in calculation chain. This property will be removed 12 months later since May 2022. Aspose apologizes for any inconvenience you may have experienced.
**Returns:**
java.util.Iterator - Enumerator to enumerate all dependents(Cell)
### getLeafs(boolean recursive) {#getLeafs-boolean-}
```
public Iterator getLeafs(boolean recursive)
```
Get all cells which will be updated when this cell is modified.
**Remarks**
NOTE: This class is now obsolete. Instead, please use Cell.GetDependentsInCalculation(bool) to get all dependents in calculation chain. This property will be removed 12 months later since May 2022. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| recursive | boolean | Whether returns those leafs that do not reference to this cell directly but reference to other leafs of this cell |
**Returns:**
java.util.Iterator - Enumerator to enumerate all dependents(Cell)
### getMergedRange() {#getMergedRange--}
```
public Range getMergedRange()
```
Returns a [Range](../../com.aspose.cells/range) object which represents a merged range.
**Returns:**
[Range](../../com.aspose.cells/range) - [Range](../../com.aspose.cells/range) object. Null if this cell is not merged.
### getName() {#getName--}
```
public String getName()
```
Gets the name of the cell.
**Remarks**
A cell name includes its column letter and row number. For example, the name of a cell in row 0 and column 0 is A1.
**Returns:**
java.lang.String
### getNumberCategoryType() {#getNumberCategoryType--}
```
public int getNumberCategoryType()
```
Represents the category type of this cell's number formatting.
See [NumberCategoryType](../../com.aspose.cells/numbercategorytype).
**Remarks**
When cell's formatting pattern is combined with conditional formatting patterns, then the returned type is corresponding to the part which is used for current value of this cell. For example, if the formatting pattern for this cell is "\#,\#\#0;(\#,\#\#0);"-";@", then when cell's value is numeric and not 0, the returned type is [NumberCategoryType.NUMBER](../../com.aspose.cells/numbercategorytype\#NUMBER); When cell's value is 0 or not numeric value, the returned type is [NumberCategoryType.TEXT](../../com.aspose.cells/numbercategorytype\#TEXT).
**Returns:**
int
### getPrecedents() {#getPrecedents--}
```
public ReferredAreaCollection getPrecedents()
```
Gets all references appearing in this cell's formula.
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
Gets all precedents(reference to cells in current workbook) used by this cell's formula while calculating it.
**Remarks**
This method can only work with the situation that [FormulaSettings.getEnableCalculationChain()](../../com.aspose.cells/formulasettings\#getEnableCalculationChain--) is true for the workbook and the workbook has been fully calculated. If this cell is not a formula or it does not reference to any other cells, null will be returned.
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
java.util.Iterator - Enumerator to enumerate all references(ReferredArea)
### getR1C1Formula() {#getR1C1Formula--}
```
public String getR1C1Formula()
```
Gets a R1C1 formula of the [Cell](../../com.aspose.cells/cell).
**Returns:**
java.lang.String
### getRichValue() {#getRichValue--}
```
public CellRichValue getRichValue()
```
Gets rich value of the cell.
**Returns:**
[CellRichValue](../../com.aspose.cells/cellrichvalue)
### getRow() {#getRow--}
```
public int getRow()
```
Gets row number (zero based) of the cell.
**Returns:**
int
### getSharedStyleIndex() {#getSharedStyleIndex--}
```
public int getSharedStyleIndex()
```
Gets cell's shared style index in the style pool.
**Returns:**
int
### getStringValue() {#getStringValue--}
```
public String getStringValue()
```
Gets the string value contained in the cell. If the type of this cell is string, then return the string value itself. For other cell types, the formatted string value (formatted with the specified style of this cell) will be returned. The formatted cell value is same with what you can get from excel when copying a cell as text(such as copying cell to text editor or exporting to csv).
**Returns:**
java.lang.String
### getStringValue(int formatStrategy) {#getStringValue-int-}
```
public String getStringValue(int formatStrategy)
```
Gets the string value by specific formatted strategy.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formatStrategy | int | [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy). The formatted strategy. |
**Returns:**
java.lang.String -
### getStringValueWithoutFormat() {#getStringValueWithoutFormat--}
```
public String getStringValueWithoutFormat()
```
Gets cell's value as string without any format.
**Remarks**
NOTE: This method is now obsolete. Instead, User should get the value object and format it according to the value type and the specific requirement. This property will be removed 12 months later since December 2020. Aspose apologizes for any inconvenience you may have experienced.
**Returns:**
java.lang.String
### getStyle() {#getStyle--}
```
public Style getStyle()
```
Gets the cell style.
**Remarks**
To change the style of the cell, please call Cell.SetStyle() method after modifying the returned style object. This method is same with [getStyle(boolean)](../../com.aspose.cells/cell\#getStyle-boolean-) with true value for the parameter.
**Returns:**
[Style](../../com.aspose.cells/style) - Style object.
### getStyle(boolean checkBorders) {#getStyle-boolean-}
```
public Style getStyle(boolean checkBorders)
```
If checkBorders is true, check whether other cells' borders will effect the style of this cell.
**Remarks**
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| checkBorders | boolean | Check other cells' borders |
**Returns:**
[Style](../../com.aspose.cells/style) - Style object.
### getTable() {#getTable--}
```
public ListObject getTable()
```
Gets the table which contains this cell.
**Returns:**
[ListObject](../../com.aspose.cells/listobject) -
### getType() {#getType--}
```
public int getType()
```
Represents cell value type.
See [CellValueType](../../com.aspose.cells/cellvaluetype).
**Returns:**
int
### getValidation() {#getValidation--}
```
public Validation getValidation()
```
Gets the validation applied to this cell.
**Returns:**
[Validation](../../com.aspose.cells/validation) -
### getValidationValue() {#getValidationValue--}
```
public boolean getValidationValue()
```
Gets the value of validation which applied to this cell.
**Returns:**
boolean -
### getValue() {#getValue--}
```
public Object getValue()
```
Gets the value contained in this cell.
**Remarks**
Possible type:
null,
Boolean,
DateTime,
Double,
Integer
String.
For int value, it may be returned as an Integer object or a Double object. And there is no guarantee that the returned value will be kept as the same type of object always.
**Returns:**
java.lang.Object
### getWidthOfValue() {#getWidthOfValue--}
```
public int getWidthOfValue()
```
Gets the width of the value in unit of pixels.
**Returns:**
int -
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```
Gets the parent worksheet.
**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hasCustomFunction() {#hasCustomFunction--}
```
public boolean hasCustomFunction()
```
Checks whether there is custom function(unsupported function) in this cell's formula.
**Returns:**
boolean
### hasCustomStyle() {#hasCustomStyle--}
```
public boolean hasCustomStyle()
```
Indicates whether this cell has custom style settings(different from the default one inherited from corresponding row, column, or workbook).
**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```
Serves as a hash function for a particular type.
**Returns:**
int - A hash code for current Cell object.
### insertText(int index, String text) {#insertText-int-java.lang.String-}
```
public void insertText(int index, String text)
```
Insert some characters to the cell. If the cell is rich formatted, this method could keep the original formatting.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The index. |
| text | java.lang.String | Inserted text. |
### isArrayFormula() {#isArrayFormula--}
```
public boolean isArrayFormula()
```
Indicates whether the cell formula is an array formula.
**Returns:**
boolean
### isArrayHeader() {#isArrayHeader--}
```
public boolean isArrayHeader()
```
Indicates the cell's formula is an array formula and it is the first cell of the array.
**Returns:**
boolean
### isCheckBoxStyle() {#isCheckBoxStyle--}
```
public boolean isCheckBoxStyle()
```
Indicates whether setting this cell as a check box.
**Returns:**
boolean
### isDynamicArrayFormula() {#isDynamicArrayFormula--}
```
public boolean isDynamicArrayFormula()
```
Indicates whether the cell's formula is dynamic array formula(true) or legacy array formula(false).
**Returns:**
boolean
### isErrorValue() {#isErrorValue--}
```
public boolean isErrorValue()
```
Checks if the value of this cell is an error.
**Remarks**
Also applies to formula cell to check whether the calculated result is an error.
**Returns:**
boolean
### isFormula() {#isFormula--}
```
public boolean isFormula()
```
Represents if the specified cell contains formula.
**Returns:**
boolean
### isInArray() {#isInArray--}
```
public boolean isInArray()
```
Indicates whether the cell formula is an array formula.
**Remarks**
NOTE: This class is now obsolete. Instead, please use Cell.IsArrayFormula to check whether the cell formula is an array formula. This property will be removed 12 months later since May 2018. Aspose apologizes for any inconvenience you may have experienced.
**Returns:**
boolean
### isInTable() {#isInTable--}
```
public boolean isInTable()
```
Indicates whether this cell is part of table formula.
**Remarks**
NOTE: This class is now obsolete. Instead, please use Cell.IsTableFormula to check whether the cell formula is part of table formula. This property will be removed 12 months later since May 2018. Aspose apologizes for any inconvenience you may have experienced.
**Returns:**
boolean
### isMerged() {#isMerged--}
```
public boolean isMerged()
```
Checks if a cell is part of a merged range or not.
**Returns:**
boolean
### isNumericValue() {#isNumericValue--}
```
public boolean isNumericValue()
```
Indicates whether the value of this cell is numeric(int, double and datetime)
**Remarks**
Also applies to formula cell to check the calculated result
**Returns:**
boolean
### isRichText() {#isRichText--}
```
public boolean isRichText()
```
Indicates whether the string value of this cell is a rich formatted text.
**Returns:**
boolean
### isSharedFormula() {#isSharedFormula--}
```
public boolean isSharedFormula()
```
Indicates whether the cell formula is part of shared formula.
**Returns:**
boolean
### isStyleSet() {#isStyleSet--}
```
public boolean isStyleSet()
```
Indicates if the cell's style is set. If return false, it means this cell has a default cell format.
**Returns:**
boolean
### isTableFormula() {#isTableFormula--}
```
public boolean isTableFormula()
```
Indicates whether this cell is part of table formula.
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
Puts a boolean value into the cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| boolValue | boolean |  |
### putValue(DateTime dateTime) {#putValue-com.aspose.cells.DateTime-}
```
public void putValue(DateTime dateTime)
```
Puts a DateTime value into the cell.
**Remarks**
Setting a DateTime value for a cell dose not means the cell will be formatted as date time automatically. DateTime value was maintained as numeric value in the data model of both ms excel and Aspose.Cells. Whether the numeric value will be taken as the numeric value itself or date time depends on the number format applied on this cell. If this cell has not been formatted as date time, it will be displayed as a numeric value even though what you input is DateTime.
**Example**
This example shows how to set DateTime value to a cell and make it be displayed as date time.
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
| Parameter | Type | Description |
| --- | --- | --- |
| dateTime | [DateTime](../../com.aspose.cells/datetime) | Input value |
### putValue(double doubleValue) {#putValue-double-}
```
public void putValue(double doubleValue)
```
Puts a double value into the cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| doubleValue | double | Input value |
### putValue(int intValue) {#putValue-int-}
```
public void putValue(int intValue)
```
Puts an integer value into the cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| intValue | int | Input value |
### putValue(Object objectValue) {#putValue-java.lang.Object-}
```
public void putValue(Object objectValue)
```
Puts an object value into the cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| objectValue | java.lang.Object | input value |
### putValue(String stringValue) {#putValue-java.lang.String-}
```
public void putValue(String stringValue)
```
Puts a string value into the cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stringValue | java.lang.String | Input value |
### putValue(String stringValue, boolean isConverted) {#putValue-java.lang.String-boolean-}
```
public void putValue(String stringValue, boolean isConverted)
```
Puts a string value into the cell and converts the value to other data type if appropriate.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stringValue | java.lang.String | Input value |
| isConverted | boolean | True: converted to other data type if appropriate. |
### putValue(String stringValue, boolean isConverted, boolean setStyle) {#putValue-java.lang.String-boolean-boolean-}
```
public void putValue(String stringValue, boolean isConverted, boolean setStyle)
```
Puts a value into the cell, if appropriate the value will be converted to other data type and cell's number format will be reset.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stringValue | java.lang.String | Input value |
| isConverted | boolean | True: converted to other data type if appropriate. |
| setStyle | boolean | True: set the number format to cell's style when converting to other data type |
### removeArrayFormula(boolean leaveNormalFormula) {#removeArrayFormula-boolean-}
```
public void removeArrayFormula(boolean leaveNormalFormula)
```
Remove array formula.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| leaveNormalFormula | boolean | True represents converting the array formula to normal formula. |
### replace(String placeHolder, String newValue, ReplaceOptions options) {#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-}
```
public void replace(String placeHolder, String newValue, ReplaceOptions options)
```
Replace text of the cell with options.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | java.lang.String | Cell placeholder |
| newValue | java.lang.String | String value to replace |
| options | [ReplaceOptions](../../com.aspose.cells/replaceoptions) | The replace options |
### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber) {#setArrayFormula-java.lang.String-int-int-}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber)
```
Sets an array formula(legacy array formula entered via CTRL+SHIFT+ENTER in ms excel) to a range of cells.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | java.lang.String | Array formula. |
| rowNumber | int | Number of rows to populate result of the array formula. |
| columnNumber | int | Number of columns to populate result of the array formula. |
### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal) {#setArrayFormula-java.lang.String-int-int-boolean-boolean-}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)
```
Sets an array formula to a range of cells.
**Remarks**
NOTE: This class is now obsolete. Instead, please use Cell.SetArrayFormula(string,int,int,FormulaParseOptions). This property will be removed 12 months later since December 2019. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | java.lang.String | Array formula. |
| rowNumber | int | Number of rows to populate result of the array formula. |
| columnNumber | int | Number of columns to populate result of the array formula. |
| isR1C1 | boolean | whether the formula is R1C1 formula |
| isLocal | boolean | whether the formula is locale formatted |
### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options) {#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options)
```
Sets an array formula to a range of cells.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | java.lang.String | Array formula. |
| rowNumber | int | Number of rows to populate result of the array formula. |
| columnNumber | int | Number of columns to populate result of the array formula. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Options for parsing the formula. |
### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values) {#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)
```
Sets an array formula to a range of cells.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | java.lang.String | Array formula. |
| rowNumber | int | Number of rows to populate result of the array formula. |
| columnNumber | int | Number of columns to populate result of the array formula. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Options for parsing the formula. |
| values | java.lang.Object[][] | values for those cells with given array formula |
### setCharacters(FontSetting[] characters) {#setCharacters-com.aspose.cells.FontSetting---}
```
public void setCharacters(FontSetting[] characters)
```
Sets rich text format of the cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| characters | [FontSetting\[\]](../../com.aspose.cells/fontsetting) | All Characters objects. |
### setCheckBoxStyle(boolean value) {#setCheckBoxStyle-boolean-}
```
public void setCheckBoxStyle(boolean value)
```
Indicates whether setting this cell as a check box.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, boolean calculateValue) {#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-boolean-}
```
public CellArea setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, boolean calculateValue)
```
Sets dynamic array formula and make the formula spill into neighboring cells if possible.
**Remarks**
the returned range may be not same with the actual one that this dynamic array formula spills into. If there are non-empty cells in the range, the formula will be set for current cell only and marked as "\#SPILL!". But for such kind of situation we still return the whole range that this formula should spill into.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | java.lang.String | the formula expression |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | options to parse formula. "Parse" option will be ignored and the formula will always be parsed immediately |
| calculateValue | boolean | whether calculate this dynamic array formula for those cells in the spilled range. |
**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the range that the formula should spill into.
### setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue) {#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-}
```
public CellArea setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue)
```
Sets dynamic array formula and make the formula spill into neighboring cells if possible.
**Remarks**
the returned range may be not same with the actual one that this dynamic array formula spills into. If there are non-empty cells in the range, the formula will be set for current cell only and marked as "\#SPILL!". But for such kind of situation we still return the whole range that this formula should spill into.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | java.lang.String | the formula expression |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | options to parse formula. "Parse" option will be ignored and the formula will always be parsed immediately |
| values | java.lang.Object[][] | values(calculated results) for those cells with given dynamic array formula |
| calculateRange | boolean | Whether calculate the spilled range for this dynamic array formula. If the "values" parameter is not null and this flag is false, then the spilled range's height will be values.Length and width will be values[0].Length. |
| calculateValue | boolean | whether calculate this dynamic array formula for those cells in the spilled range when "values" is null or corresponding item in "values" for one cell is null. |
**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the range that the formula should spill into.
### setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue, CalculationOptions copts) {#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-com.aspose.cells.CalculationOptions-}
```
public CellArea setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue, CalculationOptions copts)
```
Sets dynamic array formula and make the formula spill into neighboring cells if possible.
**Remarks**
the returned range may be not same with the actual one that this dynamic array formula spills into. If there are non-empty cells in the range, the formula will be set for current cell only and marked as "\#SPILL!". But for such kind of situation we still return the whole range that this formula should spill into.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | java.lang.String | the formula expression |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | options to parse formula. "Parse" option will be ignored and the formula will always be parsed immediately |
| values | java.lang.Object[][] | values(calculated results) for those cells with given dynamic array formula |
| calculateRange | boolean | Whether calculate the spilled range for this dynamic array formula. If the "values" parameter is not null and this flag is false, then the spilled range's height will be values.Length and width will be values[0].Length. |
| calculateValue | boolean | whether calculate this dynamic array formula for those cells in the spilled range when "values" is null or corresponding item in "values" for one cell is null. |
| copts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | The options for calculating formula. Commonly, for performance consideration, the [CalculationOptions.getRecursive()](../../com.aspose.cells/calculationoptions\#getRecursive--) property should be false. |
**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the range that the formula should spill into.
### setEmbeddedImage(byte[] value) {#setEmbeddedImage-byte---}
```
public void setEmbeddedImage(byte[] value)
```
Sets the embeddedn image in the cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte[] |  |
### setFormula(String value) {#setFormula-java.lang.String-}
```
public void setFormula(String value)
```
Sets a formula of the [Cell](../../com.aspose.cells/cell).
**Remarks**
A formula string always begins with an equal sign (=). And please always use comma(,) as parameters delimiter, such as "=SUM(A1, E1, H2)".
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setFormula(String formula, boolean isR1C1, boolean isLocal, Object value) {#setFormula-java.lang.String-boolean-boolean-java.lang.Object-}
```
public void setFormula(String formula, boolean isR1C1, boolean isLocal, Object value)
```
Set the formula and the value of the formula.
**Remarks**
NOTE: This class is now obsolete. Instead, please use Cell.SetFormula(string,FormulaParseOptions,object). This property will be removed 12 months later since December 2019. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | java.lang.String | The formula. |
| isR1C1 | boolean | Whether the formula is R1C1 formula. |
| isLocal | boolean | Whether the formula is locale formatted. |
| value | java.lang.Object | The value of the formula. |
### setFormula(String formula, FormulaParseOptions options) {#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-}
```
public void setFormula(String formula, FormulaParseOptions options)
```
Set the formula and the value(calculated result) of the formula.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | java.lang.String | The formula. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Options for parsing the formula. |
### setFormula(String formula, FormulaParseOptions options, Object value) {#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-}
```
public void setFormula(String formula, FormulaParseOptions options, Object value)
```
Set the formula and the value(calculated result) of the formula.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | java.lang.String | The formula. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Options for parsing the formula. |
| value | java.lang.Object | The value(calculated result) of the formula. |
### setFormula(String formula, Object value) {#setFormula-java.lang.String-java.lang.Object-}
```
public void setFormula(String formula, Object value)
```
Set the formula and the value(calculated result) of the formula.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | java.lang.String | The formula. |
| value | java.lang.Object | The value(calculated result) of the formula. |
### setFormulaLocal(String value) {#setFormulaLocal-java.lang.String-}
```
public void setFormulaLocal(String value)
```
Get the locale formatted formula of the cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setHtmlString(String value) {#setHtmlString-java.lang.String-}
```
public void setHtmlString(String value)
```
Sets the html string which contains data and some formats in this cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setR1C1Formula(String value) {#setR1C1Formula-java.lang.String-}
```
public void setR1C1Formula(String value)
```
Sets a R1C1 formula of the [Cell](../../com.aspose.cells/cell).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber) {#setSharedFormula-java.lang.String-int-int-}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber)
```
Sets shared formulas to a range of cells.
**Remarks**
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sharedFormula | java.lang.String | Shared formula. |
| rowNumber | int | Number of rows to populate the formula. |
| columnNumber | int | Number of columns to populate the formula. |
### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal) {#setSharedFormula-java.lang.String-int-int-boolean-boolean-}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)
```
Sets a formula to a range of cells.
**Remarks**
NOTE: This class is now obsolete. Instead, please use Cell.SetSharedFormula(string,int,int,FormulaParseOptions). This property will be removed 12 months later since December 2019. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sharedFormula | java.lang.String | Shared formula. |
| rowNumber | int | Number of rows to populate the formula. |
| columnNumber | int | Number of columns to populate the formula. |
| isR1C1 | boolean | whether the formula is R1C1 formula |
| isLocal | boolean | whether the formula is locale formatted |
### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options) {#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options)
```
Sets shared formulas to a range of cells.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sharedFormula | java.lang.String | Shared formula. |
| rowNumber | int | Number of rows to populate the formula. |
| columnNumber | int | Number of columns to populate the formula. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Options for parsing the formula. |
### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values) {#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)
```
Sets shared formulas to a range of cells.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sharedFormula | java.lang.String | Shared formula. |
| rowNumber | int | Number of rows to populate the formula. |
| columnNumber | int | Number of columns to populate the formula. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Options for parsing the formula. |
| values | java.lang.Object[][] | values for those cells with given shared formula |
### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```
Sets the cell style.
**Remarks**
If the border settings are changed, the border of adjust cells will be updated too.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | The cell style. |
### setStyle(Style style, boolean explicitFlag) {#setStyle-com.aspose.cells.Style-boolean-}
```
public void setStyle(Style style, boolean explicitFlag)
```
Apply the changed property of style to the cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | The cell style. |
| explicitFlag | boolean | True, only overwriting formatting which is explicitly set. |
### setStyle(Style style, StyleFlag flag) {#setStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void setStyle(Style style, StyleFlag flag)
```
Apply the cell style based on flags.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | The cell style. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | The style flag. |
### setTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, int columnIndexOfInputCell, boolean isRowInput, Object[][] values) {#setTableFormula-int-int-int-int-boolean-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, int columnIndexOfInputCell, boolean isRowInput, Object[][] values)
```
Create one-variable data table for given range starting from this cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowNumber | int | Number of rows to populate the formula. |
| columnNumber | int | Number of columns to populate the formula. |
| rowIndexOfInputCell | int | row index of the input cell |
| columnIndexOfInputCell | int | column index of the input cell |
| isRowInput | boolean | Indicates whether the input cell is a row input cell(true) or a column input cell(false). |
| values | java.lang.Object[][] | values for cells in table formula range |
### setTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, Object[][] values) {#setTableFormula-int-int-int-int-int-int-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, Object[][] values)
```
Create two-variable data table for given range starting from this cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowNumber | int | Number of rows to populate the formula. |
| columnNumber | int | Number of columns to populate the formula. |
| rowIndexOfRowInputCell | int | row index of the row input cell |
| columnIndexOfRowInputCell | int | column index of the row input cell |
| rowIndexOfColumnInputCell | int | row index of the column input cell |
| columnIndexOfColumnInputCell | int | column index of the column input cell |
| values | java.lang.Object[][] | values for cells in table formula range |
### setTableFormula(int rowNumber, int columnNumber, String inputCell, boolean isRowInput, Object[][] values) {#setTableFormula-int-int-java.lang.String-boolean-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, String inputCell, boolean isRowInput, Object[][] values)
```
Create one-variable data table for given range starting from this cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowNumber | int | Number of rows to populate the formula. |
| columnNumber | int | Number of columns to populate the formula. |
| inputCell | java.lang.String | the input cell |
| isRowInput | boolean | Indicates whether the input cell is a row input cell(true) or a column input cell(false). |
| values | java.lang.Object[][] | values for cells in table formula range |
### setTableFormula(int rowNumber, int columnNumber, String rowInputCell, String columnInputCell, Object[][] values) {#setTableFormula-int-int-java.lang.String-java.lang.String-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, String rowInputCell, String columnInputCell, Object[][] values)
```
Create two-variable data table for given range starting from this cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowNumber | int | Number of rows to populate the formula. |
| columnNumber | int | Number of columns to populate the formula. |
| rowInputCell | java.lang.String | the row input cell |
| columnInputCell | java.lang.String | the column input cell |
| values | java.lang.Object[][] | values for cells in table formula range |
### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```
Sets the value contained in this cell.
**Remarks**
Possible type:
null,
Boolean,
DateTime,
Double,
Integer
String.
For int value, it may be returned as an Integer object or a Double object. And there is no guarantee that the returned value will be kept as the same type of object always.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.Object |  |
### toJson() {#toJson--}
```
public String toJson()
```
Convert [Cell](../../com.aspose.cells/cell) to JSON struct data.
**Returns:**
java.lang.String -
### toString() {#toString--}
```
public String toString()
```
Returns a string represents the current Cell object.
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
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |
