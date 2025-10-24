##Aspose::Cells::Cell::SetFormula method
'Aspose::Cells::Cell::SetFormula method. Gets or sets a formula of the Cell in C++.'
## Cell::SetFormula(const U16String\&) method
Gets or sets a formula of the [Cell](../).
```cpp
void Aspose::Cells::Cell::SetFormula(const U16String &value)
```
## Remarks
A formula string always begins with an equal sign (=). And please always use comma(,) as parameters delimiter, such as "=SUM(A1, E1, H2)".
## Examples
```cpp
Aspose::Cells::Startup();
Workbook excel;
Cells cells = excel.GetWorksheets().Get(0).GetCells();
U16String f = u"=SUM(B2:B5, E1) + sheet1!A1";
cells.Get(u"B6").SetFormula(f);
Aspose::Cells::Cleanup();
```
## See Also
* Class [U16String](../../u16string/)
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cell::SetFormula(const char16_t*) method
Gets or sets a formula of the [Cell](../).
```cpp
void Aspose::Cells::Cell::SetFormula(const char16_t *value)
```
## Remarks
A formula string always begins with an equal sign (=). And please always use comma(,) as parameters delimiter, such as "=SUM(A1, E1, H2)".
## Examples
```cpp
Aspose::Cells::Startup();
Workbook excel;
Cells cells = excel.GetWorksheets().Get(0).GetCells();
cells.Get(u"B6").SetFormula(u"=SUM(B2:B5, E1) + sheet1!A1");
Aspose::Cells::Cleanup();
```
## See Also
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cell::SetFormula(const U16String\&, const Aspose::Cells::Object\&) method
Set the formula and the value(calculated result) of the formula.
```cpp
void Aspose::Cells::Cell::SetFormula(const U16String &formula, const Aspose::Cells::Object &value)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formula | const U16String\& | The formula. |
| value | const Aspose::Cells::Object\& | The value(calculated result) of the formula. |
## See Also
* Class [U16String](../../u16string/)
* Class [Object](../../object/)
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cell::SetFormula(const char16_t*, const Aspose::Cells::Object\&) method
Set the formula and the value(calculated result) of the formula.
```cpp
void Aspose::Cells::Cell::SetFormula(const char16_t *formula, const Aspose::Cells::Object &value)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formula | const char16_t* | The formula. |
| value | const Aspose::Cells::Object\& | The value(calculated result) of the formula. |
## See Also
* Class [Object](../../object/)
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cell::SetFormula(const U16String\&, const FormulaParseOptions\&) method
Set the formula and the value(calculated result) of the formula.
```cpp
void Aspose::Cells::Cell::SetFormula(const U16String &formula, const FormulaParseOptions &options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formula | const U16String\& | The formula. |
| options | const FormulaParseOptions\& | Options for parsing the formula. |
## See Also
* Class [U16String](../../u16string/)
* Class [FormulaParseOptions](../../formulaparseoptions/)
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cell::SetFormula(const char16_t*, const FormulaParseOptions\&) method
Set the formula and the value(calculated result) of the formula.
```cpp
void Aspose::Cells::Cell::SetFormula(const char16_t *formula, const FormulaParseOptions &options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formula | const char16_t* | The formula. |
| options | const FormulaParseOptions\& | Options for parsing the formula. |
## See Also
* Class [FormulaParseOptions](../../formulaparseoptions/)
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cell::SetFormula(const U16String\&, const FormulaParseOptions\&, const Aspose::Cells::Object\&) method
Set the formula and the value(calculated result) of the formula.
```cpp
void Aspose::Cells::Cell::SetFormula(const U16String &formula, const FormulaParseOptions &options, const Aspose::Cells::Object &value)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formula | const U16String\& | The formula. |
| options | const FormulaParseOptions\& | Options for parsing the formula. |
| value | const Aspose::Cells::Object\& | The value(calculated result) of the formula. |
## See Also
* Class [U16String](../../u16string/)
* Class [FormulaParseOptions](../../formulaparseoptions/)
* Class [Object](../../object/)
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cell::SetFormula(const char16_t*, const FormulaParseOptions\&, const Aspose::Cells::Object\&) method
Set the formula and the value(calculated result) of the formula.
```cpp
void Aspose::Cells::Cell::SetFormula(const char16_t *formula, const FormulaParseOptions &options, const Aspose::Cells::Object &value)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formula | const char16_t* | The formula. |
| options | const FormulaParseOptions\& | Options for parsing the formula. |
| value | const Aspose::Cells::Object\& | The value(calculated result) of the formula. |
## See Also
* Class [FormulaParseOptions](../../formulaparseoptions/)
* Class [Object](../../object/)
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
