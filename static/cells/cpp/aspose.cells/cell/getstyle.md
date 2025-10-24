##Aspose::Cells::Cell::GetStyle method
'Aspose::Cells::Cell::GetStyle method. Gets the cell style in C++.'
## Cell::GetStyle() method
Gets the cell style.
```cpp
Style Aspose::Cells::Cell::GetStyle()
```
## ReturnValue
[Style](../../style/) object.
## Remarks
To change the style of the cell, please call [Cell.SetStyle()](../setstyle/) method after modifying the returned style object. This method is same with [GetStyle(bool)](./) with true value for the parameter.
## See Also
* Class [Style](../../style/)
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cell::GetStyle(bool) method
If checkBorders is true, check whether other cells' borders will effect the style of this cell.
```cpp
Style Aspose::Cells::Cell::GetStyle(bool checkBorders)
```
| Parameter | Type | Description |
| --- | --- | --- |
| checkBorders | bool | Check other cells' borders |
## ReturnValue
[Style](../../style/) object.
## See Also
* Class [Style](../../style/)
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
