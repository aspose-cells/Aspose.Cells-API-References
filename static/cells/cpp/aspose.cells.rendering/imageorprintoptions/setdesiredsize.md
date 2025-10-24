##Aspose::Cells::Rendering::ImageOrPrintOptions::SetDesiredSize method
'Aspose::Cells::Rendering::ImageOrPrintOptions::SetDesiredSize method. Sets desired width and height of image in C++.'
## ImageOrPrintOptions::SetDesiredSize method
Sets desired width and height of image.
```cpp
void Aspose::Cells::Rendering::ImageOrPrintOptions::SetDesiredSize(int32_t desiredWidth, int32_t desiredHeight, bool keepAspectRatio)
```
| Parameter | Type | Description |
| --- | --- | --- |
| desiredWidth | int32_t | desired width in pixels |
| desiredHeight | int32_t | desired height in pixels |
| keepAspectRatio | bool | whether to keep aspect ratio of origin image |
## Remarks
The width and height of the output image in pixels will be only based on the set desired width and height.
The HorizontalResolution and VerticalResolution will not effect the width and height of the output image in this case.
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [ImageOrPrintOptions](../)
* Namespace [Aspose::Cells::Rendering](../../)
* Library [Aspose.Cells for C++](../../../)
