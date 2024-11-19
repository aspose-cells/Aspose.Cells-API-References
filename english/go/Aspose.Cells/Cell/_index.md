---
title: Cell Class 
linktitle: Cell
second_title: Aspose.Cells for Go API Reference
description: 'Cell class. Encapsulates the object that represents cell in Go.'
type: docs
weight: 200
url: /go/aspose.cells/cell/
---

## Cell class

Encapsulates the object that represents a single Workbook cell.

```go

type Cell struct 

cell, _ := asposecells.NewCell()

```
## Constructors

| Method | Description |
| --- | --- |
|[NewCell](./newcell/) | Constructs from an implementation object. | 

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[Calculate](./calculate/) | Calculates the formula of the cell. | 
|[GetWorksheet](./getworksheet/) | Gets the parent worksheet. | 
|[PutValue](./putvalue/) | Puts a boolean value into the cell. | 
|[PutValue](./putvalue/) | Puts an integer value into the cell. | 
|[PutValue](./putvalue/) | Puts a double value into the cell. | 
|[PutValue](./putvalue/) | Puts a value into the cell, if appropriate the value will be converted to other data type and cell's number format will be reset. | 
|[PutValue](./putvalue/) | Puts a string value into the cell and converts the value to other data type if appropriate. | 
|[PutValue](./putvalue/) | Puts a string value into the cell. | 
|[PutValue](./putvalue/) | Puts a DateTime value into the cell. | 
|[GetDateTimeValue](./getdatetimevalue/) | Gets the DateTime value contained in the cell. | 
|[PutValue](./putvalue/) | Puts an object value into the cell. | 
|[GetRow](./getrow/) | Gets row number (zero based) of the cell. | 
|[GetColumn](./getcolumn/) | Gets column number (zero based) of the cell. | 
|[IsFormula](./isformula/) | Represents if the specified cell contains formula. | 
|[GetType](./gettype/) | Represents cell value type. | 
|[GetName](./getname/) | Gets the name of the cell. | 
|[IsErrorValue](./iserrorvalue/) | Checks if the value of this cell is an error. | 
|[IsNumericValue](./isnumericvalue/) | Indicates whether the value of this cell is numeric(int, double and datetime) | 
|[GetStringValue](./getstringvalue/) | Gets the string value by specific formatted strategy. | 
|[GetStringValue](./getstringvalue/) | Gets the string value contained in the cell. If the type of this cell is string, then return the string value itself.For other cell types, the formatted string value (formatted with the specified style of this cell) will be returned.The formatted cell value is same with what you can get from excel when copying a cell as text(such ascopying cell to text editor or exporting to csv). | 
|[GetNumberCategoryType](./getnumbercategorytype/) | Represents the category type of this cell's number formatting. | 
|[GetDisplayStringValue](./getdisplaystringvalue/) | Gets the formatted string value of this cell by cell's display style. | 
|[GetIntValue](./getintvalue/) | Gets the integer value contained in the cell. | 
|[GetDoubleValue](./getdoublevalue/) | Gets the double value contained in the cell. | 
|[GetFloatValue](./getfloatvalue/) | Gets the float value contained in the cell. | 
|[GetBoolValue](./getboolvalue/) | Gets the boolean value contained in the cell. | 
|[GetWidthOfValue](./getwidthofvalue/) | Gets the width of the value in unit of pixels. | 
|[GetHeightOfValue](./getheightofvalue/) | Gets the height of the value in unit of pixels. | 
|[GetDisplayStyle](./getdisplaystyle/) | Gets the display style of the cell.If this cell is also affected by other settings such as conditional formatting, list objects, etc.,then the display style may be different from cell.GetStyle(). | 
|[GetDisplayStyle](./getdisplaystyle/) | Gets the display style of the cell.If the cell is conditional formatted, the display style is not same as the cell.GetStyle(). | 
|[GetStyle](./getstyle/) | Gets the cell style. | 
|[GetStyle](./getstyle/) | If checkBorders is true, check whether other cells' borders will effect the style of this cell. | 
|[SetStyle](./setstyle/) | Sets the cell style. | 
|[SetStyle](./setstyle/) | Apply the changed property of style to the cell. | 
|[SetStyle](./setstyle/) | Apply the cell style based on flags. | 
|[GetHasCustomStyle](./gethascustomstyle/) | Indicates whether this cell has custom style settings(different from the default one inheritedfrom corresponding row, column, or workbook). | 
|[GetSharedStyleIndex](./getsharedstyleindex/) | Gets cell's shared style index in the style pool. | 
|[GetFormula](./getformula/) | Gets or sets a formula of the <see cref="Cell"/>. | 
|[SetFormula](./setformula/) | Gets or sets a formula of the <see cref="Cell"/>. | 
|[GetFormulaLocal](./getformulalocal/) | Get the locale formatted formula of the cell. | 
|[SetFormulaLocal](./setformulalocal/) | Get the locale formatted formula of the cell. | 
|[GetR1C1Formula](./getr1c1formula/) | Gets or sets a R1C1 formula of the <see cref="Cell"/>. | 
|[SetR1C1Formula](./setr1c1formula/) | Gets or sets a R1C1 formula of the <see cref="Cell"/>. | 
|[SetFormula](./setformula/) | Set the formula and the value(calculated result) of the formula. | 
|[SetFormula](./setformula/) | Set the formula and the value(calculated result) of the formula. | 
|[GetFormula](./getformula/) | Get the formula of this cell. | 
|[SetFormula](./setformula/) | Set the formula and the value(calculated result) of the formula. | 
|[SetArrayFormula](./setarrayformula/) | Sets an array formula(legacy array formula entered via CTRL+SHIFT+ENTER in ms excel) to a range of cells. | 
|[SetArrayFormula](./setarrayformula/) | Sets an array formula to a range of cells. | 
|[SetSharedFormula](./setsharedformula/) | Sets shared formulas to a range of cells. | 
|[SetSharedFormula](./setsharedformula/) | Sets shared formulas to a range of cells. | 
|[GetContainsExternalLink](./getcontainsexternallink/) | Indicates whether this cell contains an external link.Only applies when the cell is a formula cell. | 
|[GetPrecedents](./getprecedents/) | Gets all references appearing in this cell's formula. | 
|[IsArrayHeader](./isarrayheader/) | Indicates the cell's formula is an array formulaand it is the first cell of the array. | 
|[IsDynamicArrayFormula](./isdynamicarrayformula/) | Indicates whether the cell's formula is dynamic array formula(true) or legacy array formula(false). | 
|[GetArrayRange](./getarrayrange/) | Gets the array range if the cell's formula is an array formula. | 
|[IsArrayFormula](./isarrayformula/) | Indicates whether the cell formula is an array formula. | 
|[IsSharedFormula](./issharedformula/) | Indicates whether the cell formula is part of shared formula. | 
|[IsTableFormula](./istableformula/) | Indicates whether this cell is part of table formula. | 
|[SetDynamicArrayFormula](./setdynamicarrayformula/) | Sets dynamic array formula and make the formula spill into neighboring cells if possible. | 
|[RemoveArrayFormula](./removearrayformula/) | Remove array formula. | 
|[Copy](./copy/) | Copies data from a source cell. | 
|[GetValue](./getvalue/) | Gets/sets the value contained in this cell. | 
|[SetValue](./setvalue/) | Gets/sets the value contained in this cell. | 
|[IsStyleSet](./isstyleset/) | Indicates if the cell's style is set. If return false, it means this cell has a default cell format. | 
|[Characters](./characters/) | Returns a Characters object that represents a range of characters within the cell text. | 
|[Replace](./replace/) | Replace text of the cell with options. | 
|[InsertText](./inserttext/) | Insert some characters to the cell.If the cell is rich formatted, this method could keep the original formatting. | 
|[IsRichText](./isrichtext/) | Indicates whether the string value of this cell is a rich formatted text. | 
|[IsMerged](./ismerged/) | Checks if a cell is part of a merged range or not. | 
|[GetMergedRange](./getmergedrange/) | Returns a <see cref="Range"/> object which represents a merged range. | 
|[GetComment](./getcomment/) | Gets the comment of this cell. | 
|[GetHtmlString](./gethtmlstring/) | Gets and sets the html string which contains data and some formats in this cell. | 
|[SetHtmlString](./sethtmlstring/) | Gets and sets the html string which contains data and some formats in this cell. | 
|[GetHtmlString](./gethtmlstring/) | Gets the html string which contains data and some formats in this cell. | 
|[ToString](./tostring/) | Returns a string represents the current Cell object. | 
|[ToJson](./tojson/) | Convert <see cref="Cell"/> to JSON struct data. | 
|[Equals](./equals/) | Checks whether this object refers to the same cell with another. | 
|[GetHashCode](./gethashcode/) | Serves as a hash function for a particular type. | 
|[Equals](./equals/) | Checks whether this object refers to the same cell with another cell object. | 
|[GetConditionalFormattingResult](./getconditionalformattingresult/) | Get the result of the conditional formatting. | 
|[GetValidation](./getvalidation/) | Gets the validation applied to this cell. | 
|[GetValidationValue](./getvalidationvalue/) | Gets the value of validation which applied to this cell. | 
|[GetTable](./gettable/) | Gets the table which contains this cell. | 
|[IsCheckBoxStyle](./ischeckboxstyle/) | Indicates whether setting this cell as a check box. | 
|[SetIsCheckBoxStyle](./setischeckboxstyle/) | Indicates whether setting this cell as a check box. | 
|[GetRichValue](./getrichvalue/) | Gets rich value of the cell. | 
|[Dispose](./dispose/) |  | 
