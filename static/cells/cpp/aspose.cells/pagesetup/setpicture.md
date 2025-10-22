##Aspose::Cells::PageSetup::SetPicture method
'Aspose::Cells::PageSetup::SetPicture method. Sets an image in the header/footer of a worksheet in C++.'
## PageSetup::SetPicture method
Sets an image in the header/footer of a worksheet.
```cpp
Aspose::Cells::Drawing::Picture Aspose::Cells::PageSetup::SetPicture(bool isFirst, bool isEven, bool isHeader, int32_t section, const Vector<uint8_t> &imageData)
```
| Parameter | Type | Description |
| --- | --- | --- |
| isFirst | bool | Indicates whether setting the picture of first page header/footer. |
| isEven | bool | Indicates whether setting the picture of even page header/footer. |
| isHeader | bool | Indicates whether setting the picture of header/footer. |
| section | int32_t | 0: Left Section, 1: Center Section, 2: Right Section. |
| imageData | const Vector \<uint8_t\>\& | Image data. |
## ReturnValue
Returns Picture object.
## See Also
* Class [Picture](../../../aspose.cells.drawing/picture/)
* Class [Vector](../../vector/)
* Class [PageSetup](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
