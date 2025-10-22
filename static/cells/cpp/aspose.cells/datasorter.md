##Aspose::Cells::DataSorter class
'Aspose::Cells::DataSorter class. Summary description for DataSorter in C++.'
## DataSorter class
Summary description for [DataSorter](./).
```cpp
class DataSorter
```
## Methods
| Method | Description |
| --- | --- |
| [AddColorKey(int32_t key, SortOnType type, SortOrder order, const Aspose::Cells::Color\& color)](./addcolorkey/) | Adds color sort key. |
| [AddKey(int32_t key, SortOrder order)](./addkey/) | Adds sorted column index and sort order. |
| [AddKey(int32_t key, SortOrder order, const U16String\& customList)](./addkey/) | Adds sorted column index and sort order with custom sort list. |
| [AddKey(int32_t key, SortOrder order, const char16_t* customList)](./addkey/) | Adds sorted column index and sort order with custom sort list. |
| [AddKey(int32_t key, SortOnType type, SortOrder order, const Aspose::Cells::Object\& customList)](./addkey/) | Adds sorted column index and sort order with custom sort list. |
| [AddKey(int32_t key, SortOrder order, const Vector \<U16String\>\& customList)](./addkey/) | Adds sorted column index and sort order with custom sort list. |
| [Clear()](./clear/) | Clear all settings. |
| [DataSorter(DataSorter_Impl* impl)](./datasorter/) | Constructs from an implementation object. |
| [DataSorter(const DataSorter\& src)](./datasorter/) | Copy constructor. |
| [GetCaseSensitive()](./getcasesensitive/) | Gets and sets whether case sensitive when comparing string. |
| [GetHasHeaders()](./gethasheaders/) | Represents whether the range has headers. |
| [GetKey1()](./getkey1/) | Represents first sorted column index(absolute position, column A is 0, B is 1, ...). |
| [GetKey2()](./getkey2/) | Represents second sorted column index(absolute position, column A is 0, B is 1, ...). |
| [GetKey3()](./getkey3/) | Represents third sorted column index(absolute position, column A is 0, B is 1, ...). |
| [GetKeys()](./getkeys/) | Gets the key list of data sorter. |
| [GetOrder1()](./getorder1/) | Represents sort order of the first key. |
| [GetOrder2()](./getorder2/) | Represents sort order of the second key. |
| [GetOrder3()](./getorder3/) | Represents sort order of the third key. |
| [GetSortAsNumber()](./getsortasnumber/) | Indicates whether sorting anything that looks like a number. |
| [GetSortLeftToRight()](./getsortlefttoright/) | True means that sorting orientation is from left to right. False means that sorting orientation is from top to bottom. The default value is false. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const DataSorter\& src)](./operator_asm/) | operator= |
| [SetCaseSensitive(bool value)](./setcasesensitive/) | Gets and sets whether case sensitive when comparing string. |
| [SetHasHeaders(bool value)](./sethasheaders/) | Represents whether the range has headers. |
| [SetKey1(int32_t value)](./setkey1/) | Represents first sorted column index(absolute position, column A is 0, B is 1, ...). |
| [SetKey2(int32_t value)](./setkey2/) | Represents second sorted column index(absolute position, column A is 0, B is 1, ...). |
| [SetKey3(int32_t value)](./setkey3/) | Represents third sorted column index(absolute position, column A is 0, B is 1, ...). |
| [SetOrder1(SortOrder value)](./setorder1/) | Represents sort order of the first key. |
| [SetOrder2(SortOrder value)](./setorder2/) | Represents sort order of the second key. |
| [SetOrder3(SortOrder value)](./setorder3/) | Represents sort order of the third key. |
| [SetSortAsNumber(bool value)](./setsortasnumber/) | Indicates whether sorting anything that looks like a number. |
| [SetSortLeftToRight(bool value)](./setsortlefttoright/) | True means that sorting orientation is from left to right. False means that sorting orientation is from top to bottom. The default value is false. |
| [Sort(const Cells\& cells, int32_t startRow, int32_t startColumn, int32_t endRow, int32_t endColumn)](./sort/) | Sorts the data of the area. |
| [Sort(const Cells\& cells, const CellArea\& area)](./sort/) | Sort the data of the area. |
| [Sort()](./sort/) | Sort the data in the range. |
| [~DataSorter()](./~datasorter/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
//Instantiate a new Workbook object.
Workbook workbook(u"Book1.xls");
//Get the workbook datasorter object.
DataSorter sorter = workbook.GetDataSorter();
//Set the first order for datasorter object.
sorter.SetOrder1(SortOrder::Descending);
//Define the first key.
sorter.SetKey1(0);
//Set the second order for datasorter object.
sorter.SetOrder2(SortOrder::Ascending);
//Define the second key.
sorter.SetKey2(1);
//Create a cells area (range).
CellArea ca;
//Specify the start row index.
ca.StartRow = 0;
//Specify the start column index.
ca.StartColumn = 0;
//Specify the last row index.
ca.EndRow = 13;
//Specify the last column index.
ca.EndColumn = 1;
//Sort data in the specified data range (A1:B14)
sorter.Sort(workbook.GetWorksheets().Get(0).GetCells(), ca);
//Save the excel file.
workbook.Save(u"outBook.xls");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
