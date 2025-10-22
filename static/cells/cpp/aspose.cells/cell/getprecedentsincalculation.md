##Aspose::Cells::Cell::GetPrecedentsInCalculation method
'Aspose::Cells::Cell::GetPrecedentsInCalculation method. Gets all precedents(reference to cells in current workbook) used by this cell''s formula while calculating it in C++.'
## Cell::GetPrecedentsInCalculation method
Gets all precedents(reference to cells in current workbook) used by this cell's formula while calculating it.
```cpp
Enumerator<ReferredArea> Aspose::Cells::Cell::GetPrecedentsInCalculation()
```
## ReturnValue
[Enumerator](../../enumerator/) to enumerate all references(ReferredArea)
## Remarks
This method can only work with the situation that FormulaSettings.EnableCalculationChain is true for the workbook and the workbook has been fully calculated. If this cell is not a formula or it does not reference to any other cells, null will be returned.
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook;
Cells cells = workbook.GetWorksheets().Get(0).GetCells();
cells.Get(u"A2").SetFormula(u"=IF(TRUE,B2,B1)");
workbook.GetSettings().GetFormulaSettings().SetEnableCalculationChain(true);
workbook.CalculateFormula();
Enumerator<ReferredArea> en = cells.Get(u"A2").GetPrecedentsInCalculation();
std::cout << "A2's calculation precedents:" << std::endl;
while (en.MoveNext())
{
ReferredArea r = (ReferredArea)en.GetCurrent();
std::cout << r.ToString().ToUtf8() << std::endl;
}
Aspose::Cells::Cleanup();
```
## See Also
* Class [Enumerator](../../enumerator/)
* Class [ReferredArea](../../referredarea/)
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
