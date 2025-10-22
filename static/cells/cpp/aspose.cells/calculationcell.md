##Aspose::Cells::CalculationCell class
'Aspose::Cells::CalculationCell class. Represents the calculation relevant data about one cell which is being calculated in C++.'
## CalculationCell class
Represents the calculation relevant data about one cell which is being calculated.
```cpp
class CalculationCell
```
## Methods
| Method | Description |
| --- | --- |
| [CalculationCell(CalculationCell_Impl* impl)](./calculationcell/) | Constructs from an implementation object. |
| [CalculationCell(const CalculationCell\& src)](./calculationcell/) | Copy constructor. |
| [GetCell()](./getcell/) | Gets the [Cell](../cell/) object which is being calculated. |
| [GetCellColumn()](./getcellcolumn/) | Gets the column index of the cell. |
| [GetCellRow()](./getcellrow/) | Gets the row index of the cell. |
| [GetWorkbook()](./getworkbook/) | Gets the [Workbook](../workbook/) object. |
| [GetWorksheet()](./getworksheet/) | Gets the [Worksheet](../worksheet/) object where the cell is in. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const CalculationCell\& src)](./operator_asm/) | operator= |
| [SetCalculatedValue(const Aspose::Cells::Object\& v)](./setcalculatedvalue/) | Sets the calculated value for the cell. |
| [~CalculationCell()](./~calculationcell/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Remarks
All objects provided by this class are for "read" purpose only. User should not change any data in the [Workbook](../workbook/) during the formula calculation process, Otherwise unexpected result or Exception may be caused.
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
