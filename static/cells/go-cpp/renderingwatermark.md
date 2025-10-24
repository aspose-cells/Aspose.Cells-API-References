##RenderingWatermark Class
'RenderingWatermark class. Encapsulates the object that represents renderingwatermark in Go.'
## RenderingWatermark class
Watermark for rendering.
```go
type RenderingWatermark struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewRenderingWatermark_String_RenderingFont](./newrenderingwatermark_string_renderingfont/) | Creates instance of text watermark. |
|[NewRenderingWatermark_Stream](./newrenderingwatermark_stream/) | Creates instance of image watermark. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetRotation](./getrotation/) | Gets or sets roation of the watermark in degrees. |
|[SetRotation](./setrotation/) | Gets or sets roation of the watermark in degrees. |
|[GetScaleToPagePercent](./getscaletopagepercent/) | Gets or sets scale relative to target page in percent. |
|[SetScaleToPagePercent](./setscaletopagepercent/) | Gets or sets scale relative to target page in percent. |
|[GetOpacity](./getopacity/) | Gets or sets opacity of the watermark in range [0, 1]. |
|[SetOpacity](./setopacity/) | Gets or sets opacity of the watermark in range [0, 1]. |
|[IsBackground](./isbackground/) | Indicates whether the watermark is placed behind page contents. |
|[SetIsBackground](./setisbackground/) | Indicates whether the watermark is placed behind page contents. |
|[GetText](./gettext/) | Gets text of the watermark. |
|[GetFont](./getfont/) | Gets font of the watermark. |
|[GetImage](./getimage/) | Gets image of the watermark. |
|[GetHAlignment](./gethalignment/) | Gets or sets horizontal alignment of the watermark to the page. |
|[SetHAlignment](./sethalignment/) | Gets or sets horizontal alignment of the watermark to the page. |
|[GetVAlignment](./getvalignment/) | Gets or sets vertical alignment of the watermark to the page. |
|[SetVAlignment](./setvalignment/) | Gets or sets vertical alignment of the watermark to the page. |
|[GetOffsetX](./getoffsetx/) | Gets or sets offset value to HAlignment |
|[SetOffsetX](./setoffsetx/) | Gets or sets offset value to HAlignment |
|[GetOffsetY](./getoffsety/) | Gets or sets offset value to VAlignment |
|[SetOffsetY](./setoffsety/) | Gets or sets offset value to VAlignment |
