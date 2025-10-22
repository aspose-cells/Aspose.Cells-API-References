##Cell Class
'Cell class. Encapsulates the object that represents cell in Go.'
## Cell class
Encapsulates the object that represents a single Workbook cell.
```go
type Cell struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[Calculate](./calculate/) | Calculates the formula of the cell. |
|[GetWorksheet](./getworksheet/) | Gets the parent worksheet. |
|[PutValue_Bool](./putvalue_bool/) | Puts a boolean value into the cell. |
|[PutValue_Int](./putvalue_int/) | Puts an integer value into the cell. |
|[PutValue_Double](./putvalue_double/) | Puts a double value into the cell. |
|[PutValue_String_Bool_Bool](./putvalue_string_bool_bool/) | Puts a value into the cell, if appropriate the value will be converted to other data type and cell's number format will be reset. |
|[PutValue_String_Bool](./putvalue_string_bool/) | Puts a string value into the cell and converts the value to other data type if appropriate. |
|[PutValue_String](./putvalue_string/) | Puts a string value into the cell. |
|[PutValue_Date](./putvalue_date/) | Puts a DateTime value into the cell. |
|[GetDateTimeValue](./getdatetimevalue/) | Gets the DateTime value contained in the cell. |
|[PutValue_Object](./putvalue_object/) | Puts an object value into the cell. |
|[GetRow](./getrow/) | Gets row number (zero based) of the cell. |
|[GetColumn](./getcolumn/) | Gets column number (zero based) of the cell. |
|[IsFormula](./isformula/) | Represents if the specified cell contains formula. |
|[GetHasCustomFunction](./gethascustomfunction/) | Checks whether there is custom function(unsupported function) in this cell's formula. |
|[GetType](./gettype/) | Represents cell value type. |
|[GetName](./getname/) | Gets the name of the cell. |
|[IsErrorValue](./iserrorvalue/) | Checks if the value of this cell is an error. |
|[IsNumericValue](./isnumericvalue/) | Indicates whether the value of this cell is numeric(int, double and datetime) |
|[GetStringValue_CellValueFormatStrategy](./getstringvalue_cellvalueformatstrategy/) | Gets the string value by specific formatted strategy. |
|[GetStringValue](./getstringvalue/) | Gets the string value contained in the cell. If the type of this cell is string, then return the string value itself.For other cell types, the formatted string value (formatted with the specified style of this cell) will be returned.The formatted cell value is same with what you can get from excel when copying a cell as text(such ascopying cell to text editor or exporting to csv). |
|[GetNumberCategoryType](./getnumbercategorytype/) | Represents the category type of this cell's number formatting. |
|[GetDisplayStringValue](./getdisplaystringvalue/) | Gets the formatted string value of this cell by cell's display style. |
|[GetIntValue](./getintvalue/) | Gets the integer value contained in the cell. |
|[GetDoubleValue](./getdoublevalue/) | Gets the double value contained in the cell. |
|[GetFloatValue](./getfloatvalue/) | Gets the float value contained in the cell. |
|[GetBoolValue](./getboolvalue/) | Gets the boolean value contained in the cell. |
|[GetWidthOfValue](./getwidthofvalue/) | Gets the width of the value in unit of pixels. |
|[GetHeightOfValue](./getheightofvalue/) | Gets the height of the value in unit of pixels. |
|[GetDisplayStyle](./getdisplaystyle/) | Gets the display style of this cell. |
|[GetDisplayStyle_Bool](./getdisplaystyle_bool/) | Gets the display style of this cell. |
|[GetDisplayStyle_BorderType](./getdisplaystyle_bordertype/) | Gets the display style of this cell. |
|[GetFormatConditions](./getformatconditions/) | Gets format conditions which applies to this cell. |
|[GetStyle](./getstyle/) | Gets the cell style. |
|[GetStyle_Bool](./getstyle_bool/) | If checkBorders is true, check whether other cells' borders will effect the style of this cell. |
|[SetStyle_Style](./setstyle_style/) | Sets the cell style. |
|[SetStyle_Style_Bool](./setstyle_style_bool/) | Apply the changed property of style to the cell. |
|[SetStyle_Style_StyleFlag](./setstyle_style_styleflag/) | Apply the cell style based on flags. |
|[GetHasCustomStyle](./gethascustomstyle/) | Indicates whether this cell has custom style settings(different from the default one inheritedfrom corresponding row, column, or workbook). |
|[GetSharedStyleIndex](./getsharedstyleindex/) | Gets cell's shared style index in the style pool. |
|[GetFormula](./getformula/) | Gets or sets a formula of the Cell. |
|[SetFormula_String](./setformula_string/) | Gets or sets a formula of the Cell. |
|[GetFormulaLocal](./getformulalocal/) | Get the locale formatted formula of the cell. |
|[SetFormulaLocal](./setformulalocal/) | Get the locale formatted formula of the cell. |
|[GetR1C1Formula](./getr1c1formula/) | Gets or sets a R1C1 formula of the Cell. |
|[SetR1C1Formula](./setr1c1formula/) | Gets or sets a R1C1 formula of the Cell. |
|[SetFormula_String_Object](./setformula_string_object/) | Set the formula and the value(calculated result) of the formula. |
|[SetFormula_String_FormulaParseOptions](./setformula_string_formulaparseoptions/) | Set the formula and the value(calculated result) of the formula. |
|[GetFormula_Bool_Bool](./getformula_bool_bool/) | Get the formula of this cell. |
|[SetFormula_String_FormulaParseOptions_Object](./setformula_string_formulaparseoptions_object/) | Set the formula and the value(calculated result) of the formula. |
|[SetArrayFormula_String_Int_Int](./setarrayformula_string_int_int/) | Sets an array formula(legacy array formula entered via CTRL+SHIFT+ENTER in ms excel) to a range of cells. |
|[SetArrayFormula_String_Int_Int_FormulaParseOptions](./setarrayformula_string_int_int_formulaparseoptions/) | Sets an array formula to a range of cells. |
|[SetArrayFormula_String_Int_Int_FormulaParseOptions_Object2Array](./setarrayformula_string_int_int_formulaparseoptions_object2array/) | Sets an array formula to a range of cells. |
|[SetSharedFormula_String_Int_Int](./setsharedformula_string_int_int/) | Sets shared formulas to a range of cells. |
|[SetSharedFormula_String_Int_Int_FormulaParseOptions](./setsharedformula_string_int_int_formulaparseoptions/) | Sets shared formulas to a range of cells. |
|[SetSharedFormula_String_Int_Int_FormulaParseOptions_Object2Array](./setsharedformula_string_int_int_formulaparseoptions_object2array/) | Sets shared formulas to a range of cells. |
|[GetContainsExternalLink](./getcontainsexternallink/) | Indicates whether this cell contains an external link.Only applies when the cell is a formula cell. |
|[GetPrecedents](./getprecedents/) | Gets all references appearing in this cell's formula. |
|[GetDependents](./getdependents/) | Get all cells whose formula references to this cell directly. |
|[GetPrecedentsInCalculation](./getprecedentsincalculation/) | Gets all precedents(reference to cells in current workbook) used by this cell's formula while calculating it. |
|[GetDependentsInCalculation](./getdependentsincalculation/) | Gets all cells whose calculated result depends on this cell. |
|[IsArrayHeader](./isarrayheader/) | Indicates the cell's formula is an array formulaand it is the first cell of the array. |
|[IsDynamicArrayFormula](./isdynamicarrayformula/) | Indicates whether the cell's formula is dynamic array formula(true) or legacy array formula(false). |
|[GetArrayRange](./getarrayrange/) | Gets the array range if the cell's formula is an array formula. |
|[IsArrayFormula](./isarrayformula/) | Indicates whether the cell formula is an array formula. |
|[IsSharedFormula](./issharedformula/) | Indicates whether the cell formula is part of shared formula. |
|[IsTableFormula](./istableformula/) | Indicates whether this cell is part of table formula. |
|[SetDynamicArrayFormula_String_FormulaParseOptions_Bool](./setdynamicarrayformula_string_formulaparseoptions_bool/) | Sets dynamic array formula and make the formula spill into neighboring cells if possible. |
|[SetDynamicArrayFormula_String_FormulaParseOptions_Object2Array_Bool_Bool](./setdynamicarrayformula_string_formulaparseoptions_object2array_bool_bool/) | Sets dynamic array formula and make the formula spill into neighboring cells if possible. |
|[SetDynamicArrayFormula_String_FormulaParseOptions_Object2Array_Bool_Bool_CalculationOptions](./setdynamicarrayformula_string_formulaparseoptions_object2array_bool_bool_calculationoptions/) | Sets dynamic array formula and make the formula spill into neighboring cells if possible. |
|[SetTableFormula_Int_Int_String_String_Object2Array](./settableformula_int_int_string_string_object2array/) | Create two-variable data table for given range starting from this cell. |
|[SetTableFormula_Int_Int_String_Bool_Object2Array](./settableformula_int_int_string_bool_object2array/) | Create one-variable data table for given range starting from this cell. |
|[SetTableFormula_Int_Int_Int_Int_Int_Int_Object2Array](./settableformula_int_int_int_int_int_int_object2array/) | Create two-variable data table for given range starting from this cell. |
|[SetTableFormula_Int_Int_Int_Int_Bool_Object2Array](./settableformula_int_int_int_int_bool_object2array/) | Create one-variable data table for given range starting from this cell. |
|[RemoveArrayFormula](./removearrayformula/) | Remove array formula. |
|[Copy](./copy/) | Copies data from a source cell. |
|[GetValue](./getvalue/) | Gets/sets the value contained in this cell. |
|[SetValue](./setvalue/) | Gets/sets the value contained in this cell. |
|[IsStyleSet](./isstyleset/) | Indicates if the cell's style is set. If return false, it means this cell has a default cell format. |
|[Characters](./characters/) | Returns a Characters object that represents a range of characters within the cell text. |
|[Replace](./replace/) | Replace text of the cell with options. |
|[InsertText](./inserttext/) | Insert some characters to the cell.If the cell is rich formatted, this method could keep the original formatting. |
|[IsRichText](./isrichtext/) | Indicates whether the string value of this cell is a rich formatted text. |
|[GetCharacters](./getcharacters/) | Returns all Characters objectsthat represents a range of characters within the cell text. |
|[GetCharacters_Bool](./getcharacters_bool/) | Returns all Characters objectsthat represents a range of characters within the cell text. |
|[SetCharacters](./setcharacters/) | Sets rich text format of the cell. |
|[IsMerged](./ismerged/) | Checks if a cell is part of a merged range or not. |
|[GetMergedRange](./getmergedrange/) | Returns a Range object which represents a merged range. |
|[GetComment](./getcomment/) | Gets the comment of this cell. |
|[GetHtmlString](./gethtmlstring/) | Gets and sets the html string which contains data and some formats in this cell. |
|[SetHtmlString](./sethtmlstring/) | Gets and sets the html string which contains data and some formats in this cell. |
|[GetHtmlString_Bool](./gethtmlstring_bool/) | Gets the html string which contains data and some formats in this cell. |
|[ToString](./tostring/) | Returns a string represents the current Cell object. |
|[ToJson](./tojson/) | Convert Cell to JSON struct data. |
|[Equals_Object](./equals_object/) | Checks whether this object refers to the same cell with another. |
|[GetHashCode](./gethashcode/) | Serves as a hash function for a particular type. |
|[Equals_Cell](./equals_cell/) | Checks whether this object refers to the same cell with another cell object. |
|[GetConditionalFormattingResult](./getconditionalformattingresult/) | Get the result of the conditional formatting. |
|[GetValidation](./getvalidation/) | Gets the validation applied to this cell. |
|[GetValidationValue](./getvalidationvalue/) | Gets the value of validation which applied to this cell. |
|[GetTable](./gettable/) | Gets the table which contains this cell. |
|[IsCheckBoxStyle](./ischeckboxstyle/) | Indicates whether setting this cell as a check box. |
|[SetIsCheckBoxStyle](./setischeckboxstyle/) | Indicates whether setting this cell as a check box. |
|[GetRichValue](./getrichvalue/) | Gets rich value of the cell. |
|[GetEmbeddedImage](./getembeddedimage/) | Gets and sets the embeddedn image in the cell. |
|[SetEmbeddedImage](./setembeddedimage/) | Gets and sets the embeddedn image in the cell. |
|[Dispose](./dispose/) |  |
