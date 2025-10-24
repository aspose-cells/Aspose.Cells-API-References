##Aspose::Cells::Cells::Get method
'Aspose::Cells::Cells::Get method. Gets the Cell element at the specified cell row index and column index in C++.'
## Cells::Get(int32_t, int32_t) method
Gets the [Cell](../../cell/) element at the specified cell row index and column index.
```cpp
Cell Aspose::Cells::Cells::Get(int32_t row, int32_t column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | int32_t | [Row](../../row/) index. |
| column | int32_t | [Column](../../column/) index. |
## ReturnValue
The [Cell](../../cell/) object.
## Examples
```cpp
Aspose::Cells::Startup();
Workbook excel;
Cells cells = excel.GetWorksheets().Get(0).GetCells();
Cell cell = cells.Get(0, 0);//Gets the cell at "A1"
Aspose::Cells::Cleanup();
```
## See Also
* Class [Cell](../../cell/)
* Class [Vector](../../vector/)
* Class [Cells](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cells::Get(const U16String\&) method
Gets the [Cell](../../cell/) element at the specified cell name.
```cpp
Cell Aspose::Cells::Cells::Get(const U16String &cellName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | const U16String\& | [Cell](../../cell/) name,including its column letter and row number, for example A5. |
## ReturnValue
A [Cell](../../cell/) object
## Examples
```cpp
Aspose::Cells::Startup();
Workbook excel;
Cells cells = excel.GetWorksheets().Get(0).GetCells();
U16String val = u"A1";
Cell cell = cells.Get(val);//Gets the cell at "A1"
Aspose::Cells::Cleanup();
```
## See Also
* Class [Cell](../../cell/)
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [Cells](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cells::Get(const char16_t*) method
Gets the [Cell](../../cell/) element at the specified cell name.
```cpp
Cell Aspose::Cells::Cells::Get(const char16_t *cellName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | const char16_t* | [Cell](../../cell/) name,including its column letter and row number, for example A5. |
## ReturnValue
A [Cell](../../cell/) object
## Examples
```cpp
Aspose::Cells::Startup();
Workbook excel;
Cells cells = excel.GetWorksheets().Get(0).GetCells();
Cell cell = cells.Get(u"A1");//Gets the cell at "A1"
Aspose::Cells::Cleanup();
```
## See Also
* Class [Cell](../../cell/)
* Class [Vector](../../vector/)
* Class [Cells](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
