##WorkbookRender Class
'WorkbookRender class. Encapsulates the object that represents workbookrender in Go.'
## WorkbookRender class
Represents a Workbook render.The constructor of this class , must be used after modification of pagesetup, cell style.
```go
type WorkbookRender struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewWorkbookRender](./newworkbookrender/) | The construct of WorkbookRender |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetPageCount](./getpagecount/) | Gets the total page count of workbook. |
|[GetPageSizeInch](./getpagesizeinch/) | Get page size in inch of output image. |
|[ToImage](./toimage/) | Render whole workbook as Tiff Image to stream. |
|[ToImage_String](./toimage_string/) | Render whole workbook as Tiff Image to a file. |
|[ToImage_Int_String](./toimage_int_string/) | Render certain page to a file. |
|[ToImage_Int](./toimage_int/) | Render certain page to a stream. |
|[Dispose](./dispose/) | Releases resources created and used for rendering. |
