##Aspose::Cells::PageSetup::GetPicture method
'Aspose::Cells::PageSetup::GetPicture method. Gets the Picture object of the header / footer in C++.'
## PageSetup::GetPicture(bool, int32_t) method
Gets the Picture object of the header / footer.
```cpp
Aspose::Cells::Drawing::Picture Aspose::Cells::PageSetup::GetPicture(bool isHeader, int32_t section)
```
| Parameter | Type | Description |
| --- | --- | --- |
| isHeader | bool | Indicates whether it is in the header or footer. |
| section | int32_t | 0: Left Section, 1: Center Section, 2: Right Section. |
## ReturnValue
Returns Picture object. Returns null if there is no picture.
## See Also
* Class [Picture](../../../aspose.cells.drawing/picture/)
* Class [Vector](../../vector/)
* Class [PageSetup](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## PageSetup::GetPicture(bool, bool, bool, int32_t) method
Gets the Picture object of the header / footer.
```cpp
Aspose::Cells::Drawing::Picture Aspose::Cells::PageSetup::GetPicture(bool isFirst, bool isEven, bool isHeader, int32_t section)
```
| Parameter | Type | Description |
| --- | --- | --- |
| isFirst | bool | Indicates whether getting the picture of first page header/footer. |
| isEven | bool | Indicates whether getting the picture of even page header/footer. |
| isHeader | bool | Indicates whether getting the picture of header/footer. |
| section | int32_t | 0: Left Section, 1: Center Section, 2: Right Section. |
## ReturnValue
Returns Picture object.
## See Also
* Class [Picture](../../../aspose.cells.drawing/picture/)
* Class [Vector](../../vector/)
* Class [PageSetup](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
