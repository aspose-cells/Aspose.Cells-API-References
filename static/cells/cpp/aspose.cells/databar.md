##Aspose::Cells::DataBar class
'Aspose::Cells::DataBar class. Describe the DataBar conditional formatting rule. This conditional formatting rule displays a gradated data bar in the range of cells in C++.'
## DataBar class
Describe the [DataBar](./) conditional formatting rule. This conditional formatting rule displays a gradated data bar in the range of cells.
```cpp
class DataBar
```
## Methods
| Method | Description |
| --- | --- |
| [DataBar(DataBar_Impl* impl)](./databar/) | Constructs from an implementation object. |
| [DataBar(const DataBar\& src)](./databar/) | Copy constructor. |
| [GetAxisColor()](./getaxiscolor/) | Gets the color of the axis for cells with conditional formatting as data bars. |
| [GetAxisPosition()](./getaxisposition/) | Gets or sets the position of the axis of the data bars specified by a conditional formatting rule. |
| [GetBarBorder()](./getbarborder/) | Gets an object that specifies the border of a data bar. |
| [GetBarFillType()](./getbarfilltype/) | Gets or sets how a data bar is filled with color. |
| [GetColor()](./getcolor/) | Get or set this [DataBar](./)'s [Color](../color/). |
| [GetDirection()](./getdirection/) | Gets or sets the direction the databar is displayed. |
| [GetMaxCfvo()](./getmaxcfvo/) | Get or set this [DataBar](./)'s max value object. Cannot set null or CFValueObject with type [FormatConditionValueType.Min](../formatconditionvaluetype/) to it. |
| [GetMaxLength()](./getmaxlength/) | Represents the max length of data bar . |
| [GetMinCfvo()](./getmincfvo/) | Get or set this [DataBar](./)'s min value object. Cannot set null or CFValueObject with type [FormatConditionValueType.Max](../formatconditionvaluetype/) to it. |
| [GetMinLength()](./getminlength/) | Represents the min length of data bar . |
| [GetNegativeBarFormat()](./getnegativebarformat/) | Gets the [NegativeBarFormat](../negativebarformat/) object associated with a data bar conditional formatting rule. |
| [GetShowValue()](./getshowvalue/) | Get or set the flag indicating whether to show the values of the cells on which this data bar is applied. Default value is true. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const DataBar\& src)](./operator_asm/) | operator= |
| [SetAxisColor(const Aspose::Cells::Color\& value)](./setaxiscolor/) | Gets the color of the axis for cells with conditional formatting as data bars. |
| [SetAxisPosition(DataBarAxisPosition value)](./setaxisposition/) | Gets or sets the position of the axis of the data bars specified by a conditional formatting rule. |
| [SetBarFillType(DataBarFillType value)](./setbarfilltype/) | Gets or sets how a data bar is filled with color. |
| [SetColor(const Aspose::Cells::Color\& value)](./setcolor/) | Get or set this [DataBar](./)'s [Color](../color/). |
| [SetDirection(TextDirectionType value)](./setdirection/) | Gets or sets the direction the databar is displayed. |
| [SetMaxLength(int32_t value)](./setmaxlength/) | Represents the max length of data bar . |
| [SetMinLength(int32_t value)](./setminlength/) | Represents the min length of data bar . |
| [SetShowValue(bool value)](./setshowvalue/) | Get or set the flag indicating whether to show the values of the cells on which this data bar is applied. Default value is true. |
| [ToImage(const Cell\& cell, const ImageOrPrintOptions\& imgOpts)](./toimage/) | Render data bar in cell to image byte array. |
| [~DataBar()](./~databar/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
//Instantiating a Workbook object
Workbook workbook;
Worksheet sheet = workbook.GetWorksheets().Get(0);
//Adds an empty conditional formatting
int index = sheet.GetConditionalFormattings().Add();
FormatConditionCollection fcs = sheet.GetConditionalFormattings().Get(index);
//Sets the conditional format range.
CellArea ca;
ca.StartRow = 0;
ca.EndRow = 2;
ca.StartColumn = 0;
ca.EndColumn = 0;
fcs.AddArea(ca);
//Adds condition.
int idx = fcs.AddCondition(FormatConditionType::DataBar);
fcs.AddArea(ca);
FormatCondition cond = fcs.Get(idx);
//Get Databar
DataBar dataBar = cond.GetDataBar();
dataBar.SetColor(Color{ 0xff, 0xff, 0xa5, 0 });
//Set Databar properties
dataBar.GetMinCfvo().SetType(FormatConditionValueType::Percentile);
dataBar.SetShowValue(false);
dataBar.GetBarBorder().SetType(DataBarBorderType::Solid);
dataBar.GetBarBorder().SetColor(Color{ 0xff, 0xdd, 0xa0, 0xdd });//Plum
dataBar.SetBarFillType(DataBarFillType::Solid);
dataBar.SetAxisColor(Color{ 0xff, 0xff, 0, 0 });//Red
dataBar.SetAxisPosition(DataBarAxisPosition::Midpoint);
dataBar.GetNegativeBarFormat().SetColorType(DataBarNegativeColorType::Color);
dataBar.GetNegativeBarFormat().SetColor(Color{ 0xff, 0xff, 0xff, 0xff });//White
dataBar.GetNegativeBarFormat().SetBorderColorType(DataBarNegativeColorType::Color);
dataBar.GetNegativeBarFormat().SetBorderColor(Color{ 0xff, 0xff, 0xff, 0 });//Yellow
//Put Cell Values
Cell cell1 = sheet.GetCells().Get(u"A1");
cell1.PutValue(10);
Cell cell2 = sheet.GetCells().Get(u"A2");
cell2.PutValue(120);
Cell cell3 = sheet.GetCells().Get(u"A3");
cell3.PutValue(260);
//Saving the Excel file
workbook.Save(u"book1.xlsx");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
