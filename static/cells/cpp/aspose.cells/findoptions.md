##Aspose::Cells::FindOptions class
'Aspose::Cells::FindOptions class. Represents find options in C++.'
## FindOptions class
Represents find options.
```cpp
class FindOptions
```
## Methods
| Method | Description |
| --- | --- |
| [FindOptions()](./findoptions/) | Default constructor. |
| [FindOptions(FindOptions_Impl* impl)](./findoptions/) | Constructs from an implementation object. |
| [FindOptions(const FindOptions\& src)](./findoptions/) | Copy constructor. |
| [GetCaseSensitive()](./getcasesensitive/) | Indicates if the searched string is case sensitive. |
| [GetConvertNumericData()](./getconvertnumericdata/) | Gets or sets a value that indicates whether converting the searched string value to numeric data. |
| [GetLookAtType()](./getlookattype/) | Look at type. |
| [GetLookInType()](./getlookintype/) | Look in type. |
| [GetRange()](./getrange/) | Gets and sets the searched range. |
| [GetRegexKey()](./getregexkey/) | Indicates whether the searched key is regex. If true the searched key will be taken as regex and parsed. Otherwise the key will be parsed according to the rules in ms excel. |
| [GetSearchBackward()](./getsearchbackward/) | Whether search backward for cells. |
| [GetSearchOrderByRows()](./getsearchorderbyrows/) | Indicates whether search order by rows or columns. |
| [GetStyle()](./getstyle/) | The format to search for. |
| [GetValueTypeSensitive()](./getvaluetypesensitive/) | Indicates whether searched cell value type should be same with the searched key. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsRangeSet()](./israngeset/) | Indicates whether the searched range is set. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const FindOptions\& src)](./operator_asm/) | operator= |
| [SetCaseSensitive(bool value)](./setcasesensitive/) | Indicates if the searched string is case sensitive. |
| [SetConvertNumericData(bool value)](./setconvertnumericdata/) | Gets or sets a value that indicates whether converting the searched string value to numeric data. |
| [SetLookAtType(LookAtType value)](./setlookattype/) | Look at type. |
| [SetLookInType(LookInType value)](./setlookintype/) | Look in type. |
| [SetRange(const CellArea\& ca)](./setrange/) | Sets the searched range. |
| [SetRegexKey(bool value)](./setregexkey/) | Indicates whether the searched key is regex. If true the searched key will be taken as regex and parsed. Otherwise the key will be parsed according to the rules in ms excel. |
| [SetSearchBackward(bool value)](./setsearchbackward/) | Whether search backward for cells. |
| [SetSearchOrderByRows(bool value)](./setsearchorderbyrows/) | Indicates whether search order by rows or columns. |
| [SetStyle(const Style\& value)](./setstyle/) | The format to search for. |
| [SetValueTypeSensitive(bool value)](./setvaluetypesensitive/) | Indicates whether searched cell value type should be same with the searched key. |
| [~FindOptions()](./~findoptions/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
