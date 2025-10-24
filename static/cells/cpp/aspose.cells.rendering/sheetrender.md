##Aspose::Cells::Rendering::SheetRender class
'Aspose::Cells::Rendering::SheetRender class. Represents a worksheet render which can render worksheet to various images such as (BMP, PNG, JPEG, TIFF..) The constructor of this class , must be used after modification of pagesetup, cell style in C++.'
## SheetRender class
Represents a worksheet render which can render worksheet to various images such as (BMP, PNG, JPEG, TIFF..) The constructor of this class , must be used after modification of pagesetup, cell style.
```cpp
class SheetRender
```
## Methods
| Method | Description |
| --- | --- |
| [Dispose()](./dispose/) | Releases resources created and used for rendering. |
| [GetPageCount()](./getpagecount/) | Gets the total page count of current worksheet. |
| [GetPageScale()](./getpagescale/) | Gets calculated page scale of the sheet. Returns the set scale if PageSetup.Zoom is set. Otherwise, returns the calculated scale according to PageSetup.FitToPagesWide and PageSetup.FitToPagesTall. |
| [GetPageSizeInch(int32_t pageIndex)](./getpagesizeinch/) | Get page size in inch of output image. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const SheetRender\& src)](./operator_asm/) | operator= |
| [SheetRender(const Worksheet\& worksheet, const ImageOrPrintOptions\& options)](./sheetrender/) | the construct of [SheetRender](./), need worksheet and [ImageOrPrintOptions](../imageorprintoptions/) as params |
| [SheetRender(SheetRender_Impl* impl)](./sheetrender/) | Constructs from an implementation object. |
| [SheetRender(const SheetRender\& src)](./sheetrender/) | Copy constructor. |
| [ToImage(int32_t pageIndex, const U16String\& fileName)](./toimage/) | Render certain page to a file. |
| [ToImage(int32_t pageIndex, const char16_t* fileName)](./toimage/) | Render certain page to a file. |
| [ToImage(int32_t pageIndex)](./toimage/) | Render certain page to a stream. |
| [ToTiff()](./totiff/) | Render whole worksheet as Tiff Image to stream. |
| [ToTiff(const U16String\& filename)](./totiff/) | Render whole worksheet as Tiff Image to a file. |
| [ToTiff(const char16_t* filename)](./totiff/) | Render whole worksheet as Tiff Image to a file. |
| [~SheetRender()](./~sheetrender/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Namespace [Aspose::Cells::Rendering](../)
* Library [Aspose.Cells for C++](../../)
