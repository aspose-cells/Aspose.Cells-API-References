##Aspose::Cells::Rendering::WorkbookRender class
'Aspose::Cells::Rendering::WorkbookRender class. Represents a Workbook render. The constructor of this class , must be used after modification of pagesetup, cell style in C++.'
## WorkbookRender class
Represents a [Workbook](../../aspose.cells/workbook/) render. The constructor of this class , must be used after modification of pagesetup, cell style.
```cpp
class WorkbookRender
```
## Methods
| Method | Description |
| --- | --- |
| [Dispose()](./dispose/) | Releases resources created and used for rendering. |
| [GetPageCount()](./getpagecount/) | Gets the total page count of workbook. |
| [GetPageSizeInch(int32_t pageIndex)](./getpagesizeinch/) | Get page size in inch of output image. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const WorkbookRender\& src)](./operator_asm/) | operator= |
| [ToImage()](./toimage/) | Render whole workbook as Tiff Image to stream. |
| [ToImage(const U16String\& filename)](./toimage/) | Render whole workbook as Tiff Image to a file. |
| [ToImage(const char16_t* filename)](./toimage/) | Render whole workbook as Tiff Image to a file. |
| [ToImage(int32_t pageIndex, const U16String\& fileName)](./toimage/) | Render certain page to a file. |
| [ToImage(int32_t pageIndex, const char16_t* fileName)](./toimage/) | Render certain page to a file. |
| [ToImage(int32_t pageIndex)](./toimage/) | Render certain page to a stream. |
| [WorkbookRender(const Workbook\& workbook, const ImageOrPrintOptions\& options)](./workbookrender/) | The construct of [WorkbookRender](./). |
| [WorkbookRender(WorkbookRender_Impl* impl)](./workbookrender/) | Constructs from an implementation object. |
| [WorkbookRender(const WorkbookRender\& src)](./workbookrender/) | Copy constructor. |
| [~WorkbookRender()](./~workbookrender/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Namespace [Aspose::Cells::Rendering](../)
* Library [Aspose.Cells for C++](../../)
