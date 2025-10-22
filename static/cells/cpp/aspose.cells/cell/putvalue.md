##Aspose::Cells::Cell::PutValue method
'Aspose::Cells::Cell::PutValue method. Puts a boolean value into the cell in C++.'
## Cell::PutValue(bool) method
Puts a boolean value into the cell.
```cpp
void Aspose::Cells::Cell::PutValue(bool boolValue)
```
| Parameter | Type | Description |
| --- | --- | --- |
| boolValue | bool |  |
## See Also
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cell::PutValue(int32_t) method
Puts an integer value into the cell.
```cpp
void Aspose::Cells::Cell::PutValue(int32_t intValue)
```
| Parameter | Type | Description |
| --- | --- | --- |
| intValue | int32_t | Input value |
## See Also
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cell::PutValue(double) method
Puts a double value into the cell.
```cpp
void Aspose::Cells::Cell::PutValue(double doubleValue)
```
| Parameter | Type | Description |
| --- | --- | --- |
| doubleValue | double | Input value |
## See Also
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cell::PutValue(const U16String\&, bool, bool) method
Puts a value into the cell, if appropriate the value will be converted to other data type and cell's number format will be reset.
```cpp
void Aspose::Cells::Cell::PutValue(const U16String &stringValue, bool isConverted, bool setStyle)
```
| Parameter | Type | Description |
| --- | --- | --- |
| stringValue | const U16String\& | Input value |
| isConverted | bool | True: converted to other data type if appropriate. |
| setStyle | bool | True: set the number format to cell's style when converting to other data type |
## See Also
* Class [U16String](../../u16string/)
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cell::PutValue(const char16_t*, bool, bool) method
Puts a value into the cell, if appropriate the value will be converted to other data type and cell's number format will be reset.
```cpp
void Aspose::Cells::Cell::PutValue(const char16_t *stringValue, bool isConverted, bool setStyle)
```
| Parameter | Type | Description |
| --- | --- | --- |
| stringValue | const char16_t* | Input value |
| isConverted | bool | True: converted to other data type if appropriate. |
| setStyle | bool | True: set the number format to cell's style when converting to other data type |
## See Also
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cell::PutValue(const U16String\&, bool) method
Puts a string value into the cell and converts the value to other data type if appropriate.
```cpp
void Aspose::Cells::Cell::PutValue(const U16String &stringValue, bool isConverted)
```
| Parameter | Type | Description |
| --- | --- | --- |
| stringValue | const U16String\& | Input value |
| isConverted | bool | True: converted to other data type if appropriate. |
## See Also
* Class [U16String](../../u16string/)
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cell::PutValue(const char16_t*, bool) method
Puts a string value into the cell and converts the value to other data type if appropriate.
```cpp
void Aspose::Cells::Cell::PutValue(const char16_t *stringValue, bool isConverted)
```
| Parameter | Type | Description |
| --- | --- | --- |
| stringValue | const char16_t* | Input value |
| isConverted | bool | True: converted to other data type if appropriate. |
## See Also
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cell::PutValue(const U16String\&) method
Puts a string value into the cell.
```cpp
void Aspose::Cells::Cell::PutValue(const U16String &stringValue)
```
| Parameter | Type | Description |
| --- | --- | --- |
| stringValue | const U16String\& | Input value |
## See Also
* Class [U16String](../../u16string/)
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cell::PutValue(const char16_t*) method
Puts a string value into the cell.
```cpp
void Aspose::Cells::Cell::PutValue(const char16_t *stringValue)
```
| Parameter | Type | Description |
| --- | --- | --- |
| stringValue | const char16_t* | Input value |
## See Also
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cell::PutValue(const Date\&) method
Puts a DateTime value into the cell.
```cpp
void Aspose::Cells::Cell::PutValue(const Date &dateTime)
```
| Parameter | Type | Description |
| --- | --- | --- |
| dateTime | const Date\& | Input value |
## Remarks
Setting a DateTime value for a cell dose not means the cell will be formatted as date time automatically. DateTime value was maintained as numeric value in the data model of both ms excel and [Aspose.Cells](../../). Whether the numeric value will be taken as the numeric value itself or date time depends on the number format applied on this cell. If this cell has not been formatted as date time, it will be displayed as a numeric value even though what you input is DateTime.
## Examples
```cpp
Aspose::Cells::Startup();
Workbook excel;
Cells cells = excel.GetWorksheets().Get(0).GetCells();
//Put date time into a cell
Cell cell = cells.Get(0, 0);
cell.PutValue(Date{ 2023, 5, 15 });
Style style = cell.GetStyle(false);
style.SetNumber(14);
cell.SetStyle(style);
Aspose::Cells::Cleanup();
```
## See Also
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cell::PutValue(const Aspose::Cells::Object\&) method
Puts an object value into the cell.
```cpp
void Aspose::Cells::Cell::PutValue(const Aspose::Cells::Object &objectValue)
```
| Parameter | Type | Description |
| --- | --- | --- |
| objectValue | const Aspose::Cells::Object\& | input value |
## See Also
* Class [Object](../../object/)
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
