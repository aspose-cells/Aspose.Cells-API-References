##Aspose::Cells::Tables::ListColumn class
'Aspose::Cells::Tables::ListColumn class. Represents a column in a Table in C++.'
## ListColumn class
Represents a column in a Table.
```cpp
class ListColumn
```
## Methods
| Method | Description |
| --- | --- |
| [GetCustomCalculatedFormula(bool isR1C1, bool isLocal)](./getcustomcalculatedformula/) | Gets the formula of this list column. |
| [GetCustomTotalsRowFormula(bool isR1C1, bool isLocal)](./getcustomtotalsrowformula/) | Gets the formula of totals row of this list column. |
| [GetDataStyle()](./getdatastyle/) | Gets the style of the data in this column of the table. |
| [GetFormula()](./getformula/) | Gets and sets the formula of the list column. |
| [GetName()](./getname/) | Gets and sets the name of the column. |
| [GetRange()](./getrange/) | Gets the range of this list column. |
| [GetTotalsCalculation()](./gettotalscalculation/) | Gets and sets the type of calculation in the Totals row of the list column. |
| [GetTotalsRowLabel()](./gettotalsrowlabel/) | Gets and sets the display labels of total row. |
| [IsArrayFormula()](./isarrayformula/) | Indicates whether the fomula is array formula. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [ListColumn(ListColumn_Impl* impl)](./listcolumn/) | Constructs from an implementation object. |
| [ListColumn(const ListColumn\& src)](./listcolumn/) | Copy constructor. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ListColumn\& src)](./operator_asm/) | operator= |
| [SetCustomCalculatedFormula(const U16String\& formula, bool isR1C1, bool isLocal)](./setcustomcalculatedformula/) | Sets the formula for this list column. |
| [SetCustomCalculatedFormula(const char16_t* formula, bool isR1C1, bool isLocal)](./setcustomcalculatedformula/) | Sets the formula for this list column. |
| [SetCustomTotalsRowFormula(const U16String\& formula, bool isR1C1, bool isLocal)](./setcustomtotalsrowformula/) | Gets the formula of totals row of this list column. |
| [SetCustomTotalsRowFormula(const char16_t* formula, bool isR1C1, bool isLocal)](./setcustomtotalsrowformula/) | Gets the formula of totals row of this list column. |
| [SetDataStyle(const Style\& style)](./setdatastyle/) | Sets the style of the data in this column of the table. |
| [SetFormula(const U16String\& value)](./setformula/) | Gets and sets the formula of the list column. |
| [SetFormula(const char16_t* value)](./setformula/) | Gets and sets the formula of the list column. |
| [SetName(const U16String\& value)](./setname/) | Gets and sets the name of the column. |
| [SetName(const char16_t* value)](./setname/) | Gets and sets the name of the column. |
| [SetTotalsCalculation(TotalsCalculation value)](./settotalscalculation/) | Gets and sets the type of calculation in the Totals row of the list column. |
| [SetTotalsRowLabel(const U16String\& value)](./settotalsrowlabel/) | Gets and sets the display labels of total row. |
| [SetTotalsRowLabel(const char16_t* value)](./settotalsrowlabel/) | Gets and sets the display labels of total row. |
| [~ListColumn()](./~listcolumn/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook;
Cells cells = workbook.GetWorksheets().Get(0).GetCells();
for (int i = 0; i < 5; i++)
{
cells.Get(0, i).PutValue(CellsHelper::ColumnIndexToName(i));
}
for (int row = 1; row < 10; row++)
{
for (int column = 0; column < 4; column++)
{
cells.Get(row, column).PutValue(row * column);
}
}
ListObjectCollection tables = workbook.GetWorksheets().Get(0).GetListObjects();
int index = tables.Add(0, 0, 9, 4, true);
ListObject table = tables.Get(0);
table.SetShowTotals(true);
ListColumn listColumn = table.GetListColumns().Get(4);
listColumn.SetTotalsCalculation(TotalsCalculation::Sum);
listColumn.SetFormula(u"=[A]");
workbook.Save(u"Book1.xlsx");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells::Tables](../)
* Library [Aspose.Cells for C++](../../)
