##Aspose::Cells::AbstractFormulaChangeMonitor class
'Aspose::Cells::AbstractFormulaChangeMonitor class. Monitor for user to track the change of formulas during certain operations in C++.'
## AbstractFormulaChangeMonitor class
Monitor for user to track the change of formulas during certain operations.
```cpp
class AbstractFormulaChangeMonitor
```
## Methods
| Method | Description |
| --- | --- |
| virtual [OnCellFormulaChanged(int32_t sheetIndex, int32_t rowIndex, int32_t columnIndex)](./oncellformulachanged/) | The event that will be triggered when the formula in a cell is changed. |
| virtual [OnFormatConditionFormulaChanged(FormatCondition\& fc)](./onformatconditionformulachanged/) | The event that will be triggered when the formula of [FormatCondition](../formatcondition/) is changed. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Remarks
For example, while deleting/inserting range of cells, formulas of other cells may be changed because of the shift of references. Please note, methods in the monitor may be invoked multiple times for one object which contains the formula.
## Examples
```cpp
Aspose::Cells::Startup();
class MyFormulaChangeMonitor : public AbstractFormulaChangeMonitor
{
private:
WorksheetCollection* mWorksheets;
public:
MyFormulaChangeMonitor(WorksheetCollection& worksheets)
{
mWorksheets = &worksheets;
}
void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
{
int i = rowIndex;
std::cout << "Cell " << mWorksheets->Get(sheetIndex).GetName().ToUtf8() << "!"
}
};
Workbook wb(u"template.xlsx");
WorksheetCollection wc = wb.GetWorksheets();
MyFormulaChangeMonitor my(wc);
InsertOptions options;
options.SetFormulaChangeMonitor(&my);
wb.GetWorksheets().Get(0).GetCells().InsertRows(0, 2, options);
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
