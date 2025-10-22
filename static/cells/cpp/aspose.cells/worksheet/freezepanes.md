##Aspose::Cells::Worksheet::FreezePanes method
'Aspose::Cells::Worksheet::FreezePanes method. Freezes panes at the specified cell in the worksheet in C++.'
## Worksheet::FreezePanes(int32_t, int32_t, int32_t, int32_t) method
Freezes panes at the specified cell in the worksheet.
```cpp
void Aspose::Cells::Worksheet::FreezePanes(int32_t row, int32_t column, int32_t freezedRows, int32_t freezedColumns)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | int32_t | [Row](../../row/) index. |
| column | int32_t | [Column](../../column/) index. |
| freezedRows | int32_t | Number of visible rows in top pane, no more than row index. |
| freezedColumns | int32_t | Number of visible columns in left pane, no more than column index. |
## Remarks
[Row](../../row/) index and column index cannot all be zero. Number of rows and number of columns also cannot all be zero.
The first two parameters specify the froze position and the last two parameters specify the area frozen on the left top pane.
## See Also
* Class [Vector](../../vector/)
* Class [Worksheet](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Worksheet::FreezePanes(const U16String\&, int32_t, int32_t) method
Freezes panes at the specified cell in the worksheet.
```cpp
void Aspose::Cells::Worksheet::FreezePanes(const U16String &cellName, int32_t freezedRows, int32_t freezedColumns)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | const U16String\& | [Cell](../../cell/) name. |
| freezedRows | int32_t | Number of visible rows in top pane, no more than row index. |
| freezedColumns | int32_t | Number of visible columns in left pane, no more than column index. |
## Remarks
[Row](../../row/) index and column index cannot all be zero. Number of rows and number of columns also cannot all be zero.
## See Also
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [Worksheet](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Worksheet::FreezePanes(const char16_t*, int32_t, int32_t) method
Freezes panes at the specified cell in the worksheet.
```cpp
void Aspose::Cells::Worksheet::FreezePanes(const char16_t *cellName, int32_t freezedRows, int32_t freezedColumns)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | const char16_t* | [Cell](../../cell/) name. |
| freezedRows | int32_t | Number of visible rows in top pane, no more than row index. |
| freezedColumns | int32_t | Number of visible columns in left pane, no more than column index. |
## Remarks
[Row](../../row/) index and column index cannot all be zero. Number of rows and number of columns also cannot all be zero.
## See Also
* Class [Vector](../../vector/)
* Class [Worksheet](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
