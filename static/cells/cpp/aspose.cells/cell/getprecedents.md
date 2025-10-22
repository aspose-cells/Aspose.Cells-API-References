##Aspose::Cells::Cell::GetPrecedents method
'Aspose::Cells::Cell::GetPrecedents method. Gets all references appearing in this cell''s formula in C++.'
## Cell::GetPrecedents method
Gets all references appearing in this cell's formula.
```cpp
ReferredAreaCollection Aspose::Cells::Cell::GetPrecedents()
```
## ReturnValue
Collection of all references appearing in this cell's formula.
## Remarks
* Returns null if this is not a formula cell.
* All references appearing in this cell's formula will be returned no matter they are referenced or not while calculating. For example, although cell A2 in formula "=IF(TRUE,A1,A2)" is not used while calculating, it is still taken as the formula's precedents.
* To get those references which influence the calculation only, please use [GetPrecedentsInCalculation()](../getprecedentsincalculation/).
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook;
Cells cells = workbook.GetWorksheets().Get(0).GetCells();
cells.Get(u"A1").SetFormula(u"=B1+SUM(B1:B10)+[Book1.xls]Sheet1!A1");
ReferredAreaCollection areas = cells.Get(u"A1").GetPrecedents();
for (int i = 0; i < areas.GetCount(); i++)
{
ReferredArea area = areas.Get(i);
U16String stringBuilder = "";
if (area.IsExternalLink())
{
stringBuilder += u"[";
stringBuilder += area.GetExternalFileName();
stringBuilder += u"]";
}
stringBuilder += area.GetSheetName();
stringBuilder += u"!";
stringBuilder += CellsHelper::CellIndexToName(area.GetStartRow(), area.GetStartColumn());
if (area.IsArea())
{
stringBuilder += u":";
stringBuilder += CellsHelper::CellIndexToName(area.GetEndRow(), area.GetEndColumn());
}
std::cout << stringBuilder.ToUtf8() << std::endl;
}
Aspose::Cells::Cleanup();
```
## See Also
* Class [ReferredAreaCollection](../../referredareacollection/)
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
