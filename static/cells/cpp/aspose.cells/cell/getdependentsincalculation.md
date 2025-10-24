##Aspose::Cells::Cell::GetDependentsInCalculation method
'Aspose::Cells::Cell::GetDependentsInCalculation method. Gets all cells whose calculated result depends on this cell in C++.'
## Cell::GetDependentsInCalculation method
Gets all cells whose calculated result depends on this cell.
```cpp
Enumerator<Cell> Aspose::Cells::Cell::GetDependentsInCalculation(bool recursive)
```
| Parameter | Type | Description |
| --- | --- | --- |
| recursive | bool | Whether returns those dependents which do not reference to this cell directly but reference to other leafs of this cell |
## ReturnValue
[Enumerator](../../enumerator/) to enumerate all dependents(Cell objects)
## Remarks
To use this method, please make sure the workbook has been set with true value for FormulaSettings.EnableCalculationChain and has been fully calculated with this setting. If there is no formula reference to this cell, null will be returned.
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook;
Cells cells = workbook.GetWorksheets().Get(0).GetCells();
cells.Get(u"A1").SetFormula(u"=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2");
cells.Get(u"A2").SetFormula(u"=IF(TRUE,B2,B1)");
workbook.GetSettings().GetFormulaSettings().SetEnableCalculationChain(true);
workbook.CalculateFormula();
Enumerator<Cell> en = cells.Get(u"B1").GetDependentsInCalculation(false);
std::cout << "B1's calculation dependents:" << std::endl;
while (en.MoveNext())
{
Cell c = (Cell)en.GetCurrent();
std::cout << c.GetName().ToUtf8() << std::endl;
}
en = cells.Get(u"B2").GetDependentsInCalculation(false);
std::cout << "B2's calculation dependents:" << std::endl;
while (en.MoveNext())
{
Cell c = (Cell)en.GetCurrent();
std::cout << c.GetName().ToUtf8() << std::endl;
}
Aspose::Cells::Cleanup();
```
## See Also
* Class [Enumerator](../../enumerator/)
* Class [Cell](../)
* Class [Vector](../../vector/)
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
