##AutoFitterOptions Class
'AutoFitterOptions class. Encapsulates the object that represents autofitteroptions in Go.'
## AutoFitterOptions class
Represents all auto fitter options.
```go
type AutoFitterOptions struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewAutoFitterOptions](./newautofitteroptions/) | Default constructor. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetDefaultEditLanguage](./getdefaulteditlanguage/) | Gets or sets default edit language. |
|[SetDefaultEditLanguage](./setdefaulteditlanguage/) | Gets or sets default edit language. |
|[GetAutoFitMergedCellsType](./getautofitmergedcellstype/) | Gets and set the type of auto fitting row height of merged cells. |
|[SetAutoFitMergedCellsType](./setautofitmergedcellstype/) | Gets and set the type of auto fitting row height of merged cells. |
|[GetOnlyAuto](./getonlyauto/) | Indicates whether only fit the rows which height are not customed. |
|[SetOnlyAuto](./setonlyauto/) | Indicates whether only fit the rows which height are not customed. |
|[GetIgnoreHidden](./getignorehidden/) | Ignores the hidden rows/columns. |
|[SetIgnoreHidden](./setignorehidden/) | Ignores the hidden rows/columns. |
|[GetMaxRowHeight](./getmaxrowheight/) | Gets and sets the max row height(in unit of Point) when autofitting rows. |
|[SetMaxRowHeight](./setmaxrowheight/) | Gets and sets the max row height(in unit of Point) when autofitting rows. |
|[GetAutoFitWrappedTextType](./getautofitwrappedtexttype/) | Gets and sets the type of auto fitting wrapped text. |
|[SetAutoFitWrappedTextType](./setautofitwrappedtexttype/) | Gets and sets the type of auto fitting wrapped text. |
|[GetFormatStrategy](./getformatstrategy/) | Gets and sets the formatted strategy. |
|[SetFormatStrategy](./setformatstrategy/) | Gets and sets the formatted strategy. |
|[GetForRendering](./getforrendering/) | Indicates whether fit for rendering purpose. |
|[SetForRendering](./setforrendering/) | Indicates whether fit for rendering purpose. |
