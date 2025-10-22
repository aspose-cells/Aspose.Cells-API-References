##Aspose::Cells::Rendering::ImageOrPrintOptions::GetTiffColorDepth method
'Aspose::Cells::Rendering::ImageOrPrintOptions::GetTiffColorDepth method. Gets or sets bit depth to apply only when saving pages to the Tiff format in C++.'
## ImageOrPrintOptions::GetTiffColorDepth method
Gets or sets bit depth to apply only when saving pages to the **Tiff** format.
```cpp
ColorDepth Aspose::Cells::Rendering::ImageOrPrintOptions::GetTiffColorDepth()
```
## Remarks
Has effect only when saving to TIFF. If TiffCompression is set to CCITT3, CCITT4, this will not take effect, the bit depth of the generated tiff image will be always 1.
## See Also
* Enum [ColorDepth](../../colordepth/)
* Class [ImageOrPrintOptions](../)
* Namespace [Aspose::Cells::Rendering](../../)
* Library [Aspose.Cells for C++](../../../)
