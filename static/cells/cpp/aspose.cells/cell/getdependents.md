##Aspose::Cells::Cell::GetDependents method
'Aspose::Cells::Cell::GetDependents method. Get all cells whose formula references to this cell directly in C++.'
## Cell::GetDependents method
Get all cells whose formula references to this cell directly.
```cpp
Vector<Cell> Aspose::Cells::Cell::GetDependents(bool isAll)
```
| Parameter | Type | Description |
| --- | --- | --- |
| isAll | bool | Indicates whether check formulas in other worksheets |
## Remarks
* If one reference containing this cell appears in one cell's formula, that cell will be taken as the dependent of this cell, no matter the reference or this cell is used or not while calculating. For example, although cell A2 in formula "=IF(TRUE,A1,A2)" is not used while calculating, this formula is still be taken as A2's dependent.
* To get those formulas whose calculated results depend on this cell, please use [GetDependentsInCalculation(bool)](../getdependentsincalculation/).
* When tracing dependents for one cell, all formulas in the workbook or worksheet will be analized and checked. So it is a time consumed process. If user need to trace dependents for lots of cells, using this method will cause poor performance. For performance consideration, user should use [GetDependentsInCalculation(bool)](../getdependentsincalculation/) instead. Or, user may gather precedents map of all cells by [GetPrecedents()](../getprecedents/) firstly, and then build the dependents map according to the precedents map.
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook;
Cells cells = workbook.GetWorksheets().Get(0).GetCells();
cells.Get(u"A1").SetFormula(u"=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2");
cells.Get(u"A2").SetFormula(u"=IF(TRUE,B2,B1)");
Vector<Cell> dependents = cells.Get(u"B1").GetDependents(true);
for (int i = 0; i < dependents.GetLength(); i++)
{
std::cout << dependents[i].GetName().ToUtf8() << std::endl;
}
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../vector/)
* Class [Cell](../)
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
