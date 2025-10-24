##Aspose::Cells::Cell::GetFormula method
'Aspose::Cells::Cell::GetFormula method. Gets or sets a formula of the Cell in C++.'
## Cell::GetFormula() method
Gets or sets a formula of the [Cell](../).
```cpp
U16String Aspose::Cells::Cell::GetFormula()
```
## Remarks
A formula string always begins with an equal sign (=). And please always use comma(,) as parameters delimiter, such as "=SUM(A1, E1, H2)".
## Examples
```cpp
Aspose::Cells::Startup();
Workbook excel;
Cells cells = excel.GetWorksheets().Get(0).GetCells();
U16String f = cells.Get(u"B6").GetFormula();
Aspose::Cells::Cleanup();
```
## See Also
* Class [U16String](../../u16string/)
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cell::GetFormula(bool, bool) method
Get the formula of this cell.
```cpp
U16String Aspose::Cells::Cell::GetFormula(bool isR1C1, bool isLocal)
```
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | bool | Whether the formula needs to be formatted as R1C1. |
| isLocal | bool | Whether the formula needs to be formatted by locale. |
## ReturnValue
the formula of this cell.
## See Also
* Class [U16String](../../u16string/)
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
