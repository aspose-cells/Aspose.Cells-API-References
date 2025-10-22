##Aspose::Cells::Name class
'Aspose::Cells::Name class. Represents a defined name for a range of cells in C++.'
## Name class
Represents a defined name for a range of cells.
```cpp
class Name
```
## Methods
| Method | Description |
| --- | --- |
| [GetComment()](./getcomment/) | Gets and sets the comment of the name. Only applies for Excel 2007 or higher versions. |
| [GetFullText()](./getfulltext/) | Gets the name full text of the object with the scope setting. |
| [GetR1C1RefersTo()](./getr1c1refersto/) | Gets or sets a R1C1 reference of the [Name](./). |
| [GetRange()](./getrange/) | Gets the range if this name refers to a range. |
| [GetRange(bool recalculate)](./getrange/) | Gets the range if this name refers to a range. |
| [GetRange(int32_t sheetIndex, int32_t row, int32_t column)](./getrange/) | Gets the range if this name refers to a range. If the reference of this name is not absolute, the range may be different for different cell. |
| [GetRanges()](./getranges/) | Gets all ranges referred by this name. |
| [GetRanges(bool recalculate)](./getranges/) | Gets all ranges referred by this name. |
| [GetReferredAreas(bool recalculate)](./getreferredareas/) | Gets all references referred by this name. |
| [GetRefersTo()](./getrefersto/) | Returns or sets the formula that the name is defined to refer to, beginning with an equal sign. |
| [GetRefersTo(bool isR1C1, bool isLocal)](./getrefersto/) | Get the reference of this [Name](./). |
| [GetRefersTo(bool isR1C1, bool isLocal, int32_t row, int32_t column)](./getrefersto/) | Get the reference of this [Name](./) based on specified cell. |
| [GetSheetIndex()](./getsheetindex/) | Indicates this name belongs to [Workbook](../workbook/) or [Worksheet](../worksheet/). 0 = Global name, otherwise index to sheet (one-based) |
| [GetText()](./gettext/) | Gets the name text of the object. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsReferred()](./isreferred/) | Indicates whether this name is referred by other formulas. |
| [IsVisible()](./isvisible/) | Indicates whether the name is visible. |
| [Name(Name_Impl* impl)](./name/) | Constructs from an implementation object. |
| [Name(const Name\& src)](./name/) | Copy constructor. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const Name\& src)](./operator_asm/) | operator= |
| [SetComment(const U16String\& value)](./setcomment/) | Gets and sets the comment of the name. Only applies for Excel 2007 or higher versions. |
| [SetComment(const char16_t* value)](./setcomment/) | Gets and sets the comment of the name. Only applies for Excel 2007 or higher versions. |
| [SetIsVisible(bool value)](./setisvisible/) | Indicates whether the name is visible. |
| [SetR1C1RefersTo(const U16String\& value)](./setr1c1refersto/) | Gets or sets a R1C1 reference of the [Name](./). |
| [SetR1C1RefersTo(const char16_t* value)](./setr1c1refersto/) | Gets or sets a R1C1 reference of the [Name](./). |
| [SetRefersTo(const U16String\& value)](./setrefersto/) | Returns or sets the formula that the name is defined to refer to, beginning with an equal sign. |
| [SetRefersTo(const char16_t* value)](./setrefersto/) | Returns or sets the formula that the name is defined to refer to, beginning with an equal sign. |
| [SetRefersTo(const U16String\& refersTo, bool isR1C1, bool isLocal)](./setrefersto/) | Set the reference of this [Name](./). |
| [SetRefersTo(const char16_t* refersTo, bool isR1C1, bool isLocal)](./setrefersto/) | Set the reference of this [Name](./). |
| [SetSheetIndex(int32_t value)](./setsheetindex/) | Indicates this name belongs to [Workbook](../workbook/) or [Worksheet](../worksheet/). 0 = Global name, otherwise index to sheet (one-based) |
| [SetText(const U16String\& value)](./settext/) | Gets the name text of the object. |
| [SetText(const char16_t* value)](./settext/) | Gets the name text of the object. |
| [ToString()](./tostring/) | Returns a string represents the current [Range](../range/) object. |
| [~Name()](./~name/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
//Instantiating a Workbook object
Workbook workbook;
//Accessing the first worksheet in the Excel file
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//Creating a named range
Range range = worksheet.GetCells().CreateRange(u"B4", u"G14");
//Setting the name of the named range
range.SetName(u"TestRange");
//Saving the modified Excel file in default (that is Excel 2000) format
workbook.Save(u"output.xls");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
