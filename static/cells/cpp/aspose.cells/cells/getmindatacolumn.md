##Aspose::Cells::Cells::GetMinDataColumn method
'Aspose::Cells::Cells::GetMinDataColumn method. Minimum column index of cell which contains data in C++.'
## Cells::GetMinDataColumn method
Minimum column index of cell which contains data.
```cpp
int32_t Aspose::Cells::Cells::GetMinDataColumn()
```
## Remarks
-1 will be returned if there is no cell which contains data. This property needs to iterate and check all cells in a worksheet dynamically, so it is a time-consumed progress and should not be invoked repeatedly, such as using it directly as condition in a loop.
## See Also
* Class [Vector](../../vector/)
* Class [Cells](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
